---

copyright:
  years: 2022

lastupdated: "2022-06-06"

keywords: virtual appliance, VTL, virtual tape, onboarding, ISV

subcollection: power-iaas

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
{:help: data-hd-content-type='help'}
{:support: data-reuse='support'}

# Managing virtual appliances
{: #virtual-appliances}

Virtual appliance is bring-your-own license model, where independent software vendors (ISV) can offer OVA (ISV software plus operating system of your choice) for quick deployment of Power Systems Virtual Server workloads. It is an appliance-as-a service that allows seamless management and metering of PowerVS. Software support is handled directly by the ISVs for virtual appliances. 
 
With virtual appliances, you can use additional services within Power Systems Virtual Server such as virtual tape libraries. For more information, see [Managing Virtual tape library](/docs/power-iaas?topic=power-iaas-managing-virtual-tape-library).
## Onboarding your virtual server images for Power Systems Virtual Servers
{: #onboard-vsi}

Independent software vendors can sell software on the IBM Cloud platform by enrolling their account in the Partner Center and by completing the onboarding process from the IBM Cloud catalog. If you are an ISV and want to sell your software, see [Selling on IBM Cloud](/docs/sell?topic=sell-selling-clouds){: external}.

As part of the onboarding process for selling Power Systems Virtual Server software, sellers must provide a public (shareable) virtual server image asset. To provide a public virtual server image for Power Systems Virtual Server, complete the following steps:

1.	Create your [Power Systems Virtual Server instance](/docs/power-iaas?topic=power-iaas-creating-power-virtual-server).
2.	Create an instance of [IBM Cloud Object Storage](/docs/cloud-object-storage?topic=cloud-object-storage-getting-started-cloud-object-storage) and upload your image to a bucket.
3.	Create your [HMAC credentials](/docs/cloud-object-storage?topic=cloud-object-storage-uhc-hmac-credentials-main).
4.	[Open a support case](/docs/power-iaas?topic=power-iaas-getting-help-and-support) so that the Power Systems Virtual Server product management team can convert your image into a stock image. Include your HMAC credentials and bucket details in the support case.
<!--
## Virtual tape libraries
{: #virtual-tape-libraries}

Virtual tape libraries are devices that are commonly used to backup IBM i data. The Power Systems Virtual Servers replicates the on-premises solution by providing a software-virtual tape library (VTL) appliance that can be dynamically provisioned in the IBM Cloud. FalconStor Restore provides a deduplicated, scalable backup solution and is the only IBM certified on-premises and PowerVS VTL solution for IBM i. For more information, see [Power Virtual Server VTL Overview](https://cloud.ibm.com/media/docs/downloads/power-iaas/PowerVS_VTL_Overview.pdf){: external}.-->