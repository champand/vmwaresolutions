---

copyright:

  years:  2019, 2020

lastupdated: "2020-08-10"

keywords: vRealize, vRealize info, tech specs vRealize

subcollection: vmwaresolutions


---

{:shortdesc: .shortdesc}
{:external: target="_blank" .external}
{:tip: .tip}
{:note: .note}
{:important: .important}

# vRealize Operations and Log Insight overview
{: #vrops_overview}

The vRealize Operations and Log Insight service deploys the VMware vRealize Operations (vROps) and VMware vRealize Log Insight (vRLI) tools. These tools help you operate and monitor the performance, health, and capacity of your {{site.data.keyword.IBM}}-hosted, dedicated VMware environment. The service also includes vRLI to help you troubleshoot issues by using log files more quickly.
{: shortdesc}

These tools are deployed by using the IBM advanced automation and are based on a consistent highly available design. vROps includes preinstalled and configured Management Packs to provide deeper visibility into the core VMware Software Defined Data Center components like VMware NSX, vSAN, and HCX. The automation provides optimized dashboards out of the box so that you can monitor the full VMware stack more easily.

Like the other VMware components in the stack, you have the flexibility to bring your enterprise licenses to the cloud (per CPU or OSI) or to rent VMware licenses from {{site.data.keyword.cloud_notm}}.

{{site.data.keyword.vmwaresolutions_full}} offers promotions for some add-on services. Promotional pricing offers a number of months free of charge for a service’s licenses, if the service has license charges. For more information, see [Promotions for VMware Solutions add-on services](/docs/vmwaresolutions?topic=vmwaresolutions-vc_addingremovingservices#vc_addingremovingservices-service-promotions).

The current versions that are installed are vROps 7.5 and vRLI 4.8.
{:note}

## Technical specifications for vRealize Operations and Log Insight
{: #vrops_overview-specs}

For information about resource requirements and capacity checking for some services, see [Resource requirements for add-on services](/docs/vmwaresolutions?topic=vmwaresolutions-vc_addingremovingservices#vc_addingremovingservices-resource-requirements).

The following components are ordered and included in the vRealize Operations and Log Insight service:
* VMware vRealize Operations (vROps) 7.5
* VMware vRealize Log Insight (vRLI) 4.8

For information about the design, requirements, and preconfigured management packs, see [Operations management architecture overview](/docs/vmwaresolutions?topic=vmwaresolutions-opsmgmt-arch).

## Considerations when you delete vRealize Operations and Log Insight
{: #vrops_overview-remove}

Review the following considerations before you delete the service:
* Only the virtual machines (VMs) that were deployed during the initial installation of vRealize Operations and Log Insight are deleted. Any node that is deployed after the installation will not be cleaned up.
* The VXLAN, DLR, and the Edge Gateway that were created during the initial deployment of vRealize Operations and Log Insight will be deleted. The VMs that you deployed on VXLAN will lose connectivity after starting the deletion of vRealize Operations and Log Insight.
* If you delete vRealize Operations and Log Insight, you need to remove the Syslog Server from the NSX Manager and the NSX Controller manually.

### Removing the Syslog Server from the NSX Manager
{: #vrops_overview-remove-nsx-manager}

1. Log in to the console of the NSX Manager Appliance.
2. Select **Manage Appliance Settings**.
3. Under the **General** tab, remove the Syslog Server configuration.

### Removing the Syslog Server from the NSX Controller nodes
{: #vrops_overview-remove-nsx-controller}

1. Log in to the VMware vSphere Web Client.
2. Go to **Networking & Security > Installation and Upgrade > Management > NSX Controller Nodes**.
3. Select the NSX Manager that manages the NSX Controller nodes that you want to modify.
4. Click the Common Controller Attributes EDIT link.
5. Remove any Syslog Servers as needed.

## Related links
{: #vrops_overview-related}

* [Ordering vRealize Operations and Log Insight](/docs/vmwaresolutions?topic=vmwaresolutions-vrops_ordering)
* [Managing vRealize Operations and Log Insight](/docs/vmwaresolutions?topic=vmwaresolutions-managing_vrops)
