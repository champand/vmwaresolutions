---

copyright:

  years:  2016, 2017

lastupdated: "2017-03-30"

subcollection: vmwaresolutions


---

{:external: target="_blank" .external}
{:tip: .tip}
{:note: .note}
{:important: .important}
{:deprecated: .deprecated}

# Release notes for V1.5
{: #relnotes_v15}

This release includes new features, usability enhancements, and bug fixes.

## Virtual Routing and Forwarding versus classic SoftLayer account requirements
{: #relnotes_v15-vrf}

For classic SoftLayer® accounts, VLAN spanning is a setting that can be enabled at the account level. {{site.data.keyword.vmwaresolutions_short}} requires that VLAN spanning is enabled.

For Virtual Routing and Forwarding (VRF) SoftLayer accounts, the equivalent of VLAN spanning is a permanent setting that cannot be changed. No user configuration is required for VRF accounts.

Before you place an instance order, ensure that your SoftLayer account is either a VRF account or a classic (non-VRF) account with VLAN spanning enabled. Otherwise, the order might fail.

To confirm if your SoftLayer account is a VRF account, verify with IBM Bluemix Support. For classic accounts, you must enable VLAN spanning by following the instructions from [Enable or Disable VLAN Spanning](/docs/vlans?topic=vlans-vlan-spanning).

## Service charge model updates
{: #relnotes_v15-svc-charge}

For Cloud Foundation instances, a new _SDDC Manager_ license is introduced, which is a monthly fee that is applied to each node.

## Usability enhancements
{: #relnotes_v15-ui}

Improvements are made throughout the user interface:

* The availability of various {{site.data.keyword.cloud_notm}} data centers and whether they have sufficient inventory to fulfill the order is clearly indicated on the user interface. Use these details to make an informed decision about the {{site.data.keyword.cloud_notm}} data center to select when you order an instance.
* For Cloud Foundation instances, information such as the instance name, domain and subdomain name, and data center location, is automatically displayed in graphical format as you enter the required information in the input fields.
