---

copyright:
  years: 2019, 2023

lastupdated: "2023-03-23"

keywords: release notes, announcements, feature updates, changes, power systems virtual server

---

{:shortdesc: .shortdesc}
{:screen: .screen}
{:codeblock: .codeblock}
{:pre: .pre}
{:tip: .tip}
{:note: .note}
{:important: .important}
{:deprecated: .deprecated}
{:preview: .preview}
{:external: target="_blank" .external}

# Release notes
{: #release-notes}

Use these release notes to learn about the latest changes to the {{site.data.keyword.powerSysShort}}.
{: shortdesc}

## March 2023
{: #mar-2023}

- **Update on new SAP HANA large t-shirt profiles feature**:
  IBM supports SLES15 SP4 for SAP and RHEL8.6 for SAP OS images with all other features on all t-shirt profiles with less than 64 cores. These SLES15 SP4 for SAP and RHEL8.6 for SAP OS images are in the process of being updated to support the larger t-shirt profiles. Until further notice please use the larger t-shirt profiles with the SLES15 SP3 for SAP OS image or the RHEL8.4 for SAP OS image. For more information, see the SAP documentation on [OS for IBM Power Virtual Servers](/docs/sap?topic=sap-compute-os-design-considerations#os-power).

  The RHEL8.6 for SAP OS image is currently available in `DAL10`, `DAL12`, `FRA04`, `FRA05`, `LON04`, `LON05`, `MON01`, `SYD05`, `TOR01`, `WDC04` and `WDC06`. The image will be available in all data centers by 3/27/23.

- **{{site.data.keyword.powerSys_notm}} cost estimator**:
  Effective 3/23/23, two of the latest large SAP HANA t-shirt profiles `mh1-90x16200` and `mh1-100x18000` are available options in the [cost estimator](https://cloud.ibm.com/power/overview#estimator){: external}. In April 2023, the latest largest profile `mh1-125x22500` will also be available in the estimator.

- **Access your event logs and notifications**:
  You can now access your event logs and notification from the **Event logs** page on the Power System Virtual Server user interface. For more information, see [Managing events logs and notifications](/docs/power-iaas?topic=power-iaas-manage-event-logs)

## February 2023
{: #feb-2023}

- Added a new data center DAL10 in the exsisting list of Power Systems Virtual Server data centers. For more information, see [Creating a Power Systems Virtual Server workspace](/docs/power-iaas?topic=power-iaas-creating-power-virtual-server#creating-service).

## December 2022
{: #dec-2022}

- Get the list of internationally recognized {{site.data.keyword.powerSys_notm}} compliance certifications. For more information, see [Power Systems Virtual Server compliance certifications](/docs/power-iaas?topic=power-iaas-compliances-list).

- You can integrate Hyper Protect Crypto Services (HPCS) with {{site.data.keyword.powerSys_notm}} to securely store and protect encryption key information for AIX and Linux. For more information, see [Integrating {{site.data.keyword.powerSys_notm}} with HPCS](/docs/power-iaas?topic=power-iaas-integrate-hpcs).

## September 2022
{: #sept-2022}

- You can share a group of processors between multiple virtual machines that allows you to group your applications together using the shared processor pool. For more information, see [Managing shared processor pool](/docs/power-iaas?topic=power-iaas-manage-SPP).

- {{site.data.keyword.powerSys_notm}} allows you to automate the complete data recovery solution using the API and CLI interfaces of global replication service. For more information, see [Managing global replication service](/docs/power-iaas?topic=power-iaas-getting-started-GRS).

- You can choose to deploy Epic workloads on a VM for more cost savings. For more information, see [Configuring a VM for Epic workloads](/docs/power-iaas?topic=power-iaas-creating-power-virtual-server#configuring-a-vm-for-epic-workloads).

- Full Linux subscription on {{site.data.keyword.powerSys_notm}} now supports SLES 15 SP4 (General).

## August 2022
{: #aug-2022}

- You can use FalconStor VTL in {{site.data.keyword.powerSys_notm}} for data protection and cloud migration as a Service for IBM i. See [Managing Virtual tape library](/docs/power-iaas?topic=power-iaas-managing-virtual-tape-library).

## July 2022
{: #jul-2022}

- You can use IBM Transit Gateway to interconnect your {{site.data.keyword.powerSys_notm}} to the {{site.data.keyword.cloud_notm}} classic and Virtual Private Cloud (VPC). See [Creating IBM Cloud connections](/docs/power-iaas?topic=power-iaas-cloud-connections#create-cloud-connections).
- {{site.data.keyword.powerSys_notm}} now supports full Linux subscription on RHEL 8.6. See [Full Linux® subscription for Power Systems Virtual Servers](/docs/power-iaas?topic=power-iaas-set-full-Linux).

## June 2022
{: #jun-2022}

- {{site.data.keyword.powerSys_notm}} now supports Linux (RHEL and SLES) stock images for non-SAP applications by using full Linux subscription. See [Full Linux® subscription for Power Systems Virtual Servers](/docs/power-iaas?topic=power-iaas-set-full-Linux).
- IBM i 7.5 is supported on {{site.data.keyword.powerSys_notm}}s.
- With virtual appliances independent software vendors (ISV) can offer OVA (ISV software plus operating system of your choice) for quick deployment of {{site.data.keyword.powerSys_notm}} workloads. See [Managing virtual appliances](/docs/power-iaas?topic=power-iaas-virtual-appliances).
  
## April 2022
{: #apr-2022}

- Snapshots that are created is monitored hourly and priced depending on the disk space used. See [Metering and pricing of snapshot](/docs/power-iaas?topic=power-iaas-volume-snapshot-clone#metering-snapshot).

## March 2022
{: #march-2022}

- The Power Systems Virtual Server now supports [AIX 7.3](/docs/power-iaas?topic=power-iaas-deploy-custom-image#aix-details).
- You can view best practices and guidelines on [AIX backup performance on IBM Power Systems Virtual Server](/docs/power-iaas?topic=power-iaas-backup-strategies#backup-aix).

## December 2021
{: #dec-2021}

- You can now configure [Virtual private network (VPN)](/docs/power-iaas?topic=power-iaas-VPN-connections) by using the Power Systems Virtual Server GUI.
- You can now configure [Placement groups](/docs/power-iaas?topic=power-iaas-placement-groups) by using the Power Systems Virtual Server GUI.
- You can now set [10 Gbps speed for Cloud connection](/docs/power-iaas?topic=power-iaas-cloud-connections) by using the Power Systems Virtual Server GUI.
- You can now set [affinity policy for storage pools](/docs/power-iaas?topic=power-iaas-creating-power-virtual-server#configuring-instance) by using the Power Systems Virtual Server GUI.

## October 2021
{: #oct-2021}

- You can now use [Virtual private network (VPN)](/docs/power-iaas?topic=power-iaas-VPN-connections) to connect an on-premises VPN gateway to an IBM Cloud™ VPN gateway that is created within a Power Systems Virtual Server VPN service. 
- You can now use [Virtual tape libraries](/docs/power-iaas?topic=power-iaas-virtual-tape-libraries) to backup IBM i data. 

## September 2021
{: #sep-2021}

- You can now use [Capturing and exporting a virtual machine](/docs/power-iaas?topic=power-iaas-capturing-exporting-vm) to view the new Job feature and view restrictions for VM capture, image import, and image export.
- You can now use [Mixed storage](/docs/power-iaas?topic=power-iaas-power-iaas-faqs#mixed_storage) to attach storage volumes to a PVM instance from different storage tiers and pools.

## June 2021
{: #jun-2021}

- You can now use [Placement groups](/docs/power-iaas?topic=power-iaas-placement-groups) to add your servers into groups and apply affinity or anti-affinity policies.

## May 2021
{: #may-2021}

- You can now use [Cloud connections](/docs/power-iaas?topic=power-iaas-managing-cloud-connections) to automate the way you connect your Power Systems Virtual Server instances to the IBM Cloud resources.
- Power Systems Virtual Server now supports SAP HANA applications in IBM-provided RHEL stock images. For more information, see [Preparing Linux OS on IBM Power VS for SAP HANA](/docs/sap?topic=sap-power-vs-sles-hana).


## March 2021
{: #mar-2021}

- You can now deploy a Red Hat Enterprise Linux (RHEL) 8.1 and 8.2 virtual machine (VM) on a VM instance. For more information, see [Using RHEL within the Power Systems Virtual Server workspace](/docs/power-iaas?topic=power-iaas-linux-with-powervs).
- {{site.data.keyword.powerSys_notm}} provides a community-supported CentOS image under Linux operating system. However, IBM does not provide any support for this image. For more information, see [Configuring a Power Systems Virtual Server instance](/docs/power-iaas?topic=power-iaas-creating-power-virtual-server#configuring-instance ).
- You can now choose *OSA21* data center to deploy your {{site.data.keyword.powerSys_notm}}.

## February 2021
{: #feb-2021}

- You can now choose *MON01* data center to deploy your {{site.data.keyword.powerSys_notm}}.
- The Power Systems Virtual Server offering now supports IBM i 7.1. For more information, see [Minimium PTF levels for IBM i](/docs/power-iaas?topic=power-iaas-minimum-levels).
- You can clone a volume or multiple volumes to create a consistent full copy of the volume. For more information, see [Cloning a volume](/docs/power-iaas?topic=power-iaas-volume-snapshot-clone#cloning-volume).
- You can resize the memory and core counts to a maximum of 8 times of the specified values, and to a minimum of 1/8 times of the specified values when the VM was provisioned. For more information see [Resizing the virtual machine core count and memory](/docs/power-iaas?topic=power-iaas-modifying-server#resize-core-mem).
