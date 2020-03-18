---

copyright:
  years: 2019, 2020

lastupdated: "2020-03-06"

keywords: faq, virtual server, network bandwidth, private network setup, multi-tenant environment, delete service, supported operating systems, hardware specifications, software maps, affinity

subcollection: power-iaas

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen: .screen}
{:codeblock: .codeblock}
{:pre: .pre}
{:tip: .tip}
{:note: .note}
{:important: .important}
{:deprecated: .deprecated}
{:external: target="_blank" .external}
{:faq: data-hd-content-type='faq'}
{:support: data-reuse='support'}

# FAQ
{: #power-iaas-faqs}

## Where can I learn how to use a Power Systems Virtual Server?
{: #training}
{: faq}
{: support}

To learn more about how to use a {{site.data.keyword.powerSys_notm}}, see the [AIX & IBM i in IBM (Public) Cloud](https://www.youtube.com/watch?v=y5QaNdGJ6R0&feature=youtu.be){: new_window}{: external} video.

This video does not capture the latest updates to the {{site.data.keyword.powerSys_notm}} offering. You might notice differences in functionality between what's shown in the video and the current offering.
{: note}

## What versions of AIX and IBM i operating systems (OS) are supported?
{: #os_versions}
{: faq}
{: support}

The supported AIX and IBM i operating system versions depend on the IBM Power Systems hardware that you select for the {{site.data.keyword.powerSys_notm}}: S922 (9009-22A), E880 (9119-MHE), or E980 (9080-M9S - Frankfurt only). To view a list of the supported AIX and IBM i operating system technology levels, see the following system software maps:

The {{site.data.keyword.powerSys_notm}} offering does not support AIX 6.1. When viewing the system software maps, refer to only the AIX 7.1 and AIX 7.2 information. If you use an unsupported version, it will be subject to outages during planned maintenance windows with no advanced notification given.
{: important}

**AIX**

* [S922 (9009-22A) AIX software map](https://www-01.ibm.com/support/docview.wss?uid=ssm1platformaix9009-22A-vios-only){: new_window}{: external}
* [E880 (9119-MHE) AIX software map](https://www-01.ibm.com/support/docview.wss?uid=ssm1platformaix9119-MHE-vios-only){: new_window}{: external}
* [E980 (9080-M9S) AIX software map](http://www-01.ibm.com/support/docview.wss?uid=ssm1platformaix9080-M9S-vios-only){: new_window}{: external}

**IBM i**

* [S922 (9009-22A), E880 (9119-MHE), and E980 (9080-M9S) software maps](https://www-01.ibm.com/support/docview.wss?uid=ssm1platformibmi){: new_window}{: external}

## Can I use my own AIX or IBM i image?
{: #image}
{: faq}
{: support}

Yes. This function is known as **bring your own image**. For more information, see [Deploying a custom image within a Power Systems Virtual Server](/docs/power-iaas?topic=power-iaas-deploy-custom-image).

## What formats should I use when uploading a custom image?
{: #custom-image}
{: faq}

Currently, you can import a custom image in the following formats: _.ova_, _.ova.gz_, _.tar_, _.tar.gz_ and _.tgz_.

## What are the available storage types in the Storage Area Network (SAN)?
{: #storage}
{: faq}
{: support}

The storage types vary by region and cannot be changed once the volume is created. A VM cannot have disks from both storage types.

* The **us-east (WDC)** region uses **Standard** or **SSD** storage types.
* The **us-south (DAL)** and **eu-de (FRA04 and FRA05)** regions uses **Tier 1 (NVMe-based flash storage)** or **Tier 3 (SSD flash storage)** storage types. The **Tier 1** storage type is best for customers who require higher throughput. Customers who do not require exceptionally high throughput and are looking to minimize costs want to select **Tier 3**.

The boot image storage type is predefined and cannot be chosen.
{: note}

## What's the difference between capped and uncapped shared processor performance? How does each one compare to dedicated processor performance?
{: #processor}
{: faq}

For more information, see the [How Does Shared Processor Performance Compare to Dedicated Processors](https://www.ibm.com/developerworks/community/wikis/home?lang=en#!/wiki/Power%20Systems/page/How%20does%20Shared%20Processor%20Performance%20Compare%20to%20Dedicated%20Processors){: new_window}{: external} wiki.

## How does my current environment compare to what's available through the Power Systems Virtual Server offering?
{: #performance}
{: faq}

If you'd like to compare your current environment's performance to what's available through the {{site.data.keyword.powerSys_notm}} offering, see the [IBM Power Systems Performance Report](https://www.ibm.com/downloads/cas/K90RQOW8){: new_window}{: external}. For a more condensed comparison, see [IBM Power Systems CPW performance data comparison](https://www.itechsol.com/wp-content/uploads/2018/07/IBM-Power-Systems-CPW-Performance-Data-Comparison-P7-vs-P8-vs-P9-rev3-July-2018.pdf){: new_window}{: external}.

## How do I migrate my VM from one colo to another (WDC04 to DAl13)?
{: #vm-migration}
{: faq}

To migrate your VM from one colo to another, you must capture and export your VM to Cloud Object Storage (COS). After you successfully capture and export your VM, copy it to the COS in the destination region, then perform an import followed by a deploy.

## What does it mean to set an affinity or anti-affinity rule?
{: #affinity}
{: faq}

You can apply affinity and anti-affinity policies to both VMs and volumes. VM affinity and anti-affinity rules allow you to spread a group of VMs across different hosts or keep them on a specific host.

You can control the placement of a new volume in a particular storage provider based on an existing volume by using volume affinity. When you set an affinity policy for a new storage volume, the volume is created within the same storage provider as an existing volume. With an anti-affinity policy, the new volume is created in a different storage provider as an existing volume.

## Does IBM provide maintenance for the AIX or IBM i operating systems?
{: #licensing_os}
{: faq}

No. It is the customer's responsibility to maintain, update, and manage the AIX or IBM i operating system.

## How does licensing work for the AIX and IBM i operating systems?
{: #os_support}
{: faq}

The license for the operating system is part of the overall cost for the service. You cannot use an existing license that you already purchased.

## How does third-party licensing work?
{: #thridparty}
{: faq}

Clients are responsible for third-party licensing.

## What are the hardware specifications?
{: #hardwarespecs}
{: faq}
{: support}

For more information, see [Hardware specifications](/docs/power-iaas?topic=power-iaas-about-virtual-server#hardware-specifications).

## Do Power Systems Virtual Servers run in a multi-tenant environment?
{: #multi}
{: faq}

Yes, {{site.data.keyword.powerSys_notm}} run in a multi-tenant environment.

## Are there bare-metal options?
{: #bare}
{: faq}

There are no bare-metal options. The {{site.data.keyword.powerSys_notm}} offering focuses on virtual instances.

## How do you set up private networks between Intel&reg; Virtual Servers (x86) and Power System Virtual Servers?
{: #connecting}
{: faq}
{: support}

For more information, see [Ordering IBM Cloud Direct Link Connect for Power Systems Virtual Servers](/docs/power-iaas?topic=power-iaas-ordering-direct-link-connect).

## How do you set up customer site access to a private network by using VPN?
{: #configuring}
{: faq}
{: support}

For more information, see [Configuring IBM Power Systems Virtual Servers](/docs/power-iaas?topic=power-iaas-configuring-power).

## What firewall options are there around VPN connectivity?
{: #firewall}
{: faq}

You must set your own firewall in your IBM Cloud account.

## How do you connect a server instance between two colocations (DAL to WDC)?
{: #gts-cloud-connect}
{: faq}
{: support}

You can use IBM Cloud Connect to connect two colocations. IBM Cloud Connect is a software-defined network interconnect service that brings secure public cloud and SaaS solution connectivity to client locations around the world. For more information, see [Connecting Power Systems Virtual Server instances and networks](/docs/power-iaas?topic=power-iaas-connecting-networks).

## How is network bandwidth billed?
{: #billing}
{: faq}
{: support}

**IBM Cloud Classic environment:** Inbound bandwidth is unlimited and not charged. Outbound bandwidth is charged per GB tier with bandwidth offered as an allotment for each month. As an example, for your compute instances, 250 GB is included with each monthly virtual server and 20 TB is included with each monthly bare metal server. Extra bandwidth can also be purchased per packages. For more information, see [Bandwidth packages](https://www.ibm.com/cloud/bandwidth){: new_window}{: external}.

**IBM Cloud Power environment:** Inbound bandwidth is unlimited and not charged. Outbound bandwidth is charged per gigabyte (GB) when you use a public network. If you are using a private network with DirectLink Connect, you are charged **IBM Cloud Classic environment** rates.

## What monitoring services are available?
{: #monitoring}
{: faq}

IBM does not provide status and performance monitoring for the IBM Cloud. Clients must use their own on-premises tools.

## What performance and capacity planning services do you provide for IBM i on IBM Cloud?
{: #ibmi-performance}
{: faq}

IBM uses the same tools that are on an on-premises system.

## IBM i and solution certification
{: #ibmi-certification}
{: faq}

You can find self-certification and listing information on the [IBM Global Solutions Directory](https://www.ibm.com/partnerworld/public/find-partner-solution){: new_window}{: external}.

## How do I delete the service or a specific instance?
{: #delete-service}
{: faq}

You can delete the service by clicking the overflow menu in the **Virtual server instances** page and selecting **Delete service**. To delete an instance, click the trash icon after you select the wanted instance.
