---

copyright:

  years:  2016, 2018

lastupdated: "2018-10-01"

subcollection: vmwaresolutions


---

{:external: target="_blank" .external}
{:tip: .tip}
{:note: .note}
{:important: .important}
{:deprecated: .deprecated}

# Release notes for V2.6
{: #relnotes_v26}

This release includes new features, component updates, usability enhancements, and bug fixes.

## Spectre and Meltdown remediation
{: #relnotes_v26-spectre}

{{site.data.keyword.vmwaresolutions_short}} has released patches from VMware in response to vulnerabilities related to Spectre and Meltdown (CVE-2017-5753, CVE-2017-5715, and CVE-2017-5754).

* CVEID: [CVE-2017-5753](http://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2017-5753)
* CVEID: [CVE-2017-5715](http://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2017-5715)
* CVEID: [CVE-2017-5754](http://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2017-5754)

## High Performance with Intel Optane option
{: #relnotes_v26-optane}

This release provides the option to add high-performance cache for vSAN storage when you are ordering a new instance or when you add a vSAN cluster after initial deployment.

With this option, you can increase the number of storage capacity disks from eight to a maximum of ten.

The High Performance with Intel Optane option is available only for customized configurations with Dual Intel Xeon Gold 5120 and Dual Intel Xeon Gold 6140 processors.

For more information, see the appropriate ordering topic for your instance or cluster type.

## Enabling a public or private network
{: #relnotes_v26-pub-private-network}

You can now deploy vCenter Server and vCenter Server with Hybridity Bundle instances, as well as VMware vSphere clusters, with public and private network interface cards (NICs) enabled or private only NICs enabled. This option is also available when you add a cluster to your vCenter Server and vCenter Server with Hybridity Bundle instance.

Some add-on services require public NICs and are not available if you select to enable a private only network.

## Deleting ESXi servers
{: #relnotes_v26-delete-esxi}

You can now delete any ESXi server from your vCenter Server, vCenter Server with Hybridity Bundle, or Cloud Foundation instance if you meet the minimum requirements for your instance.

## Updates for VMware vCenter Server instances
{: #relnotes_v26-vcs}

This release applies the following upgrades and improvements:

* vSphere ESXi 6.5 Update 2c
* vCenter Server Appliance 6.5 Update 2c
* Platform Services Controller 6.5 Update 2c
* NSX for vSphere 6.4.1

## Updates for VMware vCenter Server with Hybridity Bundle
{: #relnotes_v26-vcs-hybrid}

### Removing the Hybridity Bundle from a vCenter Server instance
{: #relnotes_v26-remove-bundle}

You can now remove the Hybridity Bundle license from your vCenter Server instance. You are required to replace the VMware NSX and VMware vSAN rental license keys with Bring Your Own License (BYOL) keys. You are required to open a support ticket to cancel charges for the rental licenses.

### vCenter Server with Hybridity Bundle availability
{: #relnotes_v26-bundle-available}

Business Partners can now order a vCenter Server with Hybridity Bundle instance. Business Partners cannot upgrade an existing vCenter Server instance to a vCenter Server with Hybridity Bundle instance and cannot remove the Hybridity Bundle from a vCenter Server with Hybridity Bundle instance.

## Updates for VMware Cloud Foundation instances
{: #relnotes_v26-vcf}

This release applies the following upgrades and improvements:

* vSphere ESXi 6.5 Update 2c
* vCenter Server Appliance 6.5 Update 2c
* Platform Services Controller 6.5 Update 2c
* NSX for vSphere 6.4.1

## Updates for add-on services
{: #relnotes_v26-services}

### HyTrust KeyControl on IBM Cloud
{: #relnotes_v26-htkc}

The HyTrust KeyControl on {{site.data.keyword.cloud_notm}} service is now available to VMware Cloud Foundation instances and VMware vCenter Server instances that are running vSphere 6.5 and that are deployed in or upgraded to V2.5 and later releases. The service simplifies the management of encrypted workloads by automating and simplifying the lifecycle of encryption keys. The service can easily manage encryption keys at scale by using FIPS 140-2 compliant encryption. By using this service, you can manage the encryption keys for all your virtual machines and encrypted data stores, and scale it to support thousands of encrypted workloads in large deployments.

You can order instances with the service included when you order your instance, or add this service to your existing instances later.

### HyTrust CloudControl on IBM Cloud
{: #relnotes_v26-htcc}

The current release installs HyTrust CloudControl 5.4 on all newly deployed instances.

### HyTrust DataControl on IBM Cloud
{: #relnotes_v26-htdc}

The current release installs HyTrust DataControl 4.2 on all newly deployed instances.

### Veeam on IBM Cloud support for vSphere ESXi V6.5 update 2c
{: #relnotes_v26-veeam}

Beginning in V2.6, new instances and new hosts are provisioned by using the vSphere ESXi V6.5 Update 2c. If you are using Veeam Backup and Replication, Veeam recommends that you update your Veeam on {{site.data.keyword.cloud_notm}} instance to V9.5u3a or later. This update ensures the best compatibility with vSphere ESXi 6.5 Update 2c.

It is recommended that existing Cloud Foundation instances that have Veeam on {{site.data.keyword.cloud_notm}} installed also update to V9.5u3a or later.

### VMware HCX on IBM Cloud
{: #relnotes_v26-hcx}

The current release installs VMware HCX 3.5.1 on all newly deployed instances.

### Zerto on IBM Cloud support for vSphere ESXi V6.5 update 2c
{: #relnotes_v26-zerto}

If you update existing hosts to vSphere ESXi V6.5 update 2, and have previously installed Zerto on {{site.data.keyword.cloud_notm}}, the Zerto Virtual
Replication console might show the `Unsupported ESX Version` warning message under the Zerto Virtual Replication Appliances (VRAs) status.

## New and updated documentation
{: #relnotes_v26-new-docs}

### Reference architecture documentation
{: #relnotes_v26-ref-archi}

The {{site.data.keyword.vmwaresolutions_short}} architecture document is updated to include important considerations to understand your responsibilities for managing and operating your VMware instance.

## User interface updates and enhancements
{: #relnotes_v26-ui}

The user interface is updated and provides the following enhancements:

* Various error messages and tooltip enhancements are available to assist you in selecting the appropriate setting on the user interface.
