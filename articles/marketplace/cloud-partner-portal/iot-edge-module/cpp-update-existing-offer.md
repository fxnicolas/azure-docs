---
title: Update an existing Azure IoT Edge module offer | Azure Marketplace
description: How to update an existing IoT Edge module offer on Azure Marketplace.
author: dsindona
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
ms.date: 04/06/2020
ms.author: dsindona
---

# Update an existing IoT Edge module offer

>[!Important]
>Starting March 30th, 2020, we'll begin moving management of your IoT Edge module offers to Partner Center. After the migration, you'll create and manage your offers in Partner Center. Follow the instructions in [Create an IoT Edge module offer](https://aka.ms/AzureCreateIoT) to manage your migrated offers.

This article steps through the different aspects of updating your IoT Edge module offer in the [Cloud Partner Portal](https://cloudpartner.azure.com/) and then republishing the offer.

There are several reasons why you might want to update your offer, such as:

-  Adding a new IoT Edge module image version to existing SKUs.
-  Adding new SKUs.
-  Updating the marketplace metadata for the offer or individual SKUs.

To assist you in these modifications, the portal offers the **Compare** and **History** features.  


## Unpermitted changes to IoT Edge module offer or SKU

There are attributes of an IoT Edge module offer or SKU that can't be changed after the  offer is live on the Azure Marketplace. You can't change the following settings:

-  **Offer ID** and **Publisher ID** of the offer
-  **SKU ID** of existing SKUs
-  Version tags, for example: `1.0.1`
-  Billing/license model changes to existing SKUs

## Common update operations

The following update operations are common.

### Update the IoT Edge module image version for a SKU

It's common for an IoT Edge module image to be periodically updated with security patches, additional features, and so on. In this scenario, you want to update the IoT Edge module image that your SKU references by using the following steps:

1.  Sign into the [Cloud Partner Portal](https://cloudpartner.azure.com/).

2.  Under **All offers**, find the offer you want to update.

3.  In the **SKUs** tab, select the SKU associated with the IoT Edge module image to update.

4.  Under **Edge module image**, select **+ New Image Version** to add a new IoT Edge module image.

5.  Provide the new IoT Edge module **image versions**. The image version needs to follow the same tags guidelines as previous versions. Version tags should be of the form X.Y.Z, where X, Y, and Z are integers. Verify that the new version you provide is greater than all previous versions.

6.  Select **Publish** to start the workflow to publish your new IoT Edge module version to the Azure Marketplace.

### Add a new SKU

Use the following steps to make a new SKU available for your offer: 

1.  Sign into the [Cloud Partner Portal](https://cloudpartner.azure.com/).

2.  Under **All offers**, find the offer you want to update.

3.  Under the **SKUs** tab, select **Add new SKU** and provide a **SKU ID** in the pop-up window.

4.  Republish the IoT Edge module using the steps described in [Publish an IoT Edge module to Azure Marketplace](./cpp-publish-offer.md).

5.  Select **Publish** to start the workflow to publish your new SKU.


### Update offer marketplace metadata

Use the following steps to update the marketplace metadata associated with your offer. (For example: company name, logos, etc.)

1.  Sign into the [Cloud Partner Portal](https://cloudpartner.azure.com/).

2.  Under **All offers**, find the offer you would like to update.

3.  Go to the **Marketplace** tab. Use the  instructions in the [Publish an IoT Edge module to Azure Marketplace](./cpp-publish-offer.md) article to make metadata changes.

4.  Select **Publish** to start the workflow to publish your changes.

## Compare Feature

When you make changes on a published offer, you can use the **Compare** feature to audit the changes that you've made. 

**To use the Compare feature:**

1.  At any point in the editing process, select **Compare** for your offer.

    ![Compare feature button](./media/iot-edge-module-compare.png)


2.  Look at side-by-side versions of marketing assets and metadata.


## History of Publishing Actions

To see historical publishing activity, select the **History** tab on the left navigation menu bar of Cloud Partner Portal. You can see the timestamped actions taken during the lifetime of your Azure Marketplace offers.  <!-- Need to find correct link here:  legal time windowsFor more information, see [History page](cpp-history-page.md) -->
