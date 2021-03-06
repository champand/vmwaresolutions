---

copyright:

  years:  2016, 2020

lastupdated: "2020-09-16"

keywords: vSphere order cluster, vSphere configuration, order vSphere cluster

subcollection: vmwaresolutions

---

{:tip: .tip}
{:note: .note}
{:important: .important}

# Ordering vSphere clusters based on existing configurations
{: #vs_orderingbasedonexistingconfig}

You can order a VMware vSphere cluster based on a configuration template that you saved. Use this procedure to define a new cluster configuration based on an existing cluster configuration.

## Requirements
{: #vs_orderingbasedonexistingconfig-req}

Ensure that you completed the following tasks:
* If this is the first time you order an instance, ensure that you completed the tasks in the **Before you begin** section on the ordering page. For more information, see [Setting up your environment for your first order](/docs/vmwaresolutions?topic=vmwaresolutions-completing_checklist).
*  You reviewed the requirements and considerations in [Requirements and planning for vSphere clusters](/docs/vmwaresolutions?topic=vmwaresolutions-vs_planning).
*  You created a configuration template to be reused.

## Procedure to order vSphere clusters based on existing configurations
{: #vs_orderingbasedonexistingconfig-procedure}

1. In the {{site.data.keyword.vmwaresolutions_short}} console, click the **VMware Solutions Dedicated** card in the **Start provisioning** section.
2. On the **VMware Solutions Dedicated** page, click the **VMware vSphere** card.
3. Ensure that you are on the **Create new** tab. Select a configuration template from the **Cluster configurations** list.
4. Enter a new cluster name.
5. Review the cluster settings that are automatically completed and update the settings according to your needs. For more information about the settings, see [Ordering new vSphere clusters](/docs/vmwaresolutions?topic=vmwaresolutions-vs_orderinginstances).
6. In the **Summary** pane, verify the instance configuration and the estimated price.
   * To save the configuration as a template without placing an order, click **Save configuration**.
   * To place the order, ensure that the account to be charged is correct, review and accept the terms, and then click **Create**.

   Only the {{site.data.keyword.cloud_notm}} bare metal server are installed. You're responsible for installing and configuring various components after cluster deployment, such as VMware vCenter, VMware NSX, VMware vSAN.
   {:note}

## Results
{: #vs_orderingbasedonexistingconfig-results}

If you saved the cluster configuration as a template, you get a console notification that the configuration was saved. You can then find the template in the **Cluster configurations** list.

If you placed an order, the deployment of the cluster starts automatically. You receive an email confirmation that the order is being processed. When the cluster is ready to use, you're also notified by email.

The vSphere clusters, unlike the vCenter Server instances, are not displayed on the **Resources** page.
{:note}

## Related links
{: #vs_orderingbasedonexistingconfig-related}

* [Ordering new vSphere clusters](/docs/vmwaresolutions?topic=vmwaresolutions-vs_orderinginstances)
* [Scaling existing vSphere clusters](/docs/vmwaresolutions?topic=vmwaresolutions-vs_scalingexistingclusters)
* [Scaling clusters created outside of the console](/docs/vmwaresolutions?topic=vmwaresolutions-vs_orderingforclustersoutside)
