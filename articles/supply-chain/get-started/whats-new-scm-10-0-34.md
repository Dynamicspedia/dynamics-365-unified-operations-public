---
title: What's new or changed in Dynamics 365 Supply Chain Management 10.0.34 (June 2023)
description: This article describes features that are either new or changed in Microsoft Dynamics 365 Supply Chain Management 10.0.34. 
author: kamaybac
ms.author: kamaybac
ms.reviewer: kamaybac
ms.search.form:
ms.topic: conceptual
ms.date: 06/19/2023
audience: Application User
ms.search.region: Global
ms.custom: bap-template
---

# What's new or changed in Dynamics 365 Supply Chain Management 10.0.34 (June 2023)

[!include [banner](../includes/banner.md)]

This article lists features that are either new or changed in Microsoft Dynamics 365 Supply Chain Management version 10.0.34. This version has a build number of 10.0.1591 and is available on the following schedule:

- **Preview of release:** April 2023
- **General availability of release (self-update):** June 2023
- **General availability of release (auto-update):** July 2023

## Features included in this release

The following table lists the features that are included in this release. We might update this article to include features that were added to the build after this article was originally published.

| Feature area | Feature | More information | Enabled by |
|---|---|---|---|
| Copilot and AI innovation | [Summarize purchase order changes for better decision making](/dynamics365/release-plan/2023wave1/finance-operations/dynamics365-supply-chain-management/summarize-purchase-order-changes-better-decision-making) | [Review and accept changes to confirmed purchase orders](../procurement/purchase-order-changes-after-confirmation.md) | Feature management:<br>*Review changes to confirmed purchase orders based on downstream impact*  |
| Inventory and logistics | [Add efficiency in prospect-to-cash integration with Sales](/dynamics365/release-plan/2023wave1/finance-operations/dynamics365-supply-chain-management/gain-added-efficiency-prospect-to-cash-integration-dynamics-365-sales) | [Add efficiency in quote-to-cash with Dynamics 365 Sales](../../fin-ops-core/dev-itpro/data-entities/dual-write/add-efficiency-in-quote-to-cash-concept.md) | One or more features must be enabled in feature management, depending on which functionality you require. See [Enable extra efficiency in quote-to-cash with Dynamics 365 Sales](../../fin-ops-core/dev-itpro/data-entities/dual-write/add-efficiency-in-quote-to-cash-enable.md) for details. |
| Inventory and logistics | [Apply right tax with minimal effort in order entry for product variants](/dynamics365/release-plan/2023wave1/finance-operations/dynamics365-supply-chain-management/apply-right-taxation-minimal-effort-order-entry-product-variants) | [Predefined product variants](../pim/tasks/create-predefined-product-variants.md) | Feature management:<br>*Apply sales tax group for product variants in sales and procurement* |
| Inventory and logistics | [Archive sales orders](/dynamics365/release-plan/2023wave1/finance-operations/dynamics365-supply-chain-management/archive-sales-orders) | [Archive sales orders](../../fin-ops-core/dev-itpro/sysadmin/archive-sales-orders.md) | Feature management:<ul><li>*(Preview) Archive*</li><li>*(Preview) Archive sales orders to history tables*</li><li>*(Preview) Archive sales orders to history tables using archive service*</li></ul> |
| Manufacturing and asset management | [Check material availability for scheduled operations](/dynamics365/release-plan/2023wave1/finance-operations/dynamics365-supply-chain-management/check-material-availability-scheduled-operations) | This feature makes it possible for organizations that use the scheduling type *Schedule operations* to check for material availability. Previously, it was only possible to check for material availability when using the *Schedule jobs* scheduling type. Before releasing a production order to the shop floor, production supervisors can check the material availability of each order by going to the **Production floor management** workspace and selecting the **Production orders to release** tile. The **Production orders to release** page now lists and indicates material availability both for orders that use the *Schedule operations* scheduling type and for orders that use the *Schedule jobs* scheduling type. | Feature management:<br>*Material availability check for operations scheduled production orders* |
| Warehouse management | Print labels using an external service<br><br>(Part of [Optimize warehouse management implementation and maintenance](/dynamics365/release-plan/2023wave1/finance-operations/dynamics365-supply-chain-management/optimize-warehouse-management-implementation-maintenance).) | <p>[Print labels using an external service](../warehousing/label-printing-using-external-label-service.md)</p><p>[Print labels using the Loftware NiceLabel label service solution](../warehousing/label-printing-using-nicelabel.md)</p><p>[Print labels using the Seagull Scientific BarTender label service solution](../warehousing/label-printing-using-bartender.md)</p> | Enabled by default |
| Warehouse management | [Run the Warehouse Management mobile app on iOS devices](/dynamics365/release-plan/2023wave1/finance-operations/dynamics365-supply-chain-management/run-warehouse-management-mobile-app-ios-devices) | [Install and connect the Warehouse Management mobile app](../warehousing/install-configure-warehouse-management-app.md) | Enabled by default |

## Feature enhancements included in this release

The following table lists the feature enhancements that are included in this release. Each of these enhancements provides an incremental improvement to an existing feature. Because they're only enhancements, they aren't listed in the [release plan](/dynamics365-release-plan/2022wave1/finance-operations/dynamics365-supply-chain-management/planned-features). However, to ensure that these enhancements won't conflict with your existing customizations or preferences, each of them is turned off by default (unless otherwise noted).

If you want to turn any of these features on or off, you must do so in [feature management](../../fin-ops-core/fin-ops/get-started/feature-management/feature-management-overview.md).

| Module | Feature name in feature management | More information |
|---|---|---|
| Engineering change management | Release multiple BOMs/formulas for Engineering Change Management | Lets you release all BOMs or formulas that are active for a product when you release the product. This functionality can be relevant, for example, if you have multiple active formulas that apply for various from quantities. You'll be able to view the different BOMs or formulas and their respective routes on the BOM designer when releasing on the **Release product structure** page and when reviewing the release on **Open product releases** page. For more information, see [Release product structures](../engineering-change-management/release-product-structure.md). |
| Inventory and warehouse management | Inventory Visibility integration with inventory adjustment offset | Makes it possible to offset an inventory adjustment that was previously posted in Inventory Visibility. |
| Inventory and warehouse management | Inventory Visibility integration with inventory adjustment posting | Makes it possible to post inventory adjustments to inventory visibility by batch. |
| Product information management | User specific product name and description | Lets workers select the language in which product names and descriptions are shown for them in the user interface. |
| Production control | Faster Gantt charts | Enables Gantt charts to load more quickly throughout the system, making it faster for you to review orders, material availability, calendars, and more. |
| Sales and marketing | Adjusting reverse match for a settlement process | Improves the reverse-match functionality of the deduction workbench to ensure that the system correctly reinstates the previously matched amount for an open transaction. Without this feature, reversing a match for a deduction transaction against an open transaction correctly puts the deduction transaction back in status *Open* (if fully unmatched), but the amount for the open transactions won't be updated with the reverse-match value. |
| Sales and marketing | Calculate and push prices, discounts and totals for selective sales orders and sales quotations when integrated to Dynamics 365 Sales | This feature requires the *Integrate Sales Quotation lifecycle with Dynamics 365 Sales* feature. It enables Supply Chain Management to calculate and push line prices, discounts, charges, taxes, and totals for a single sales order and sales quotation to Sales. It adds a new menu item to sales orders and sales quotations that, when selected, will run the calculation and push the results to Sales. The feature also adds two new pages (**Calculate sales order totals for Sales** and **Calculate sales quotation totals for Sales**), which complement the existing **Calculate sales totals** page. The new pages make it possible to specify a range of sales orders or quotations to be considered in the calculation.<br><br>**Note:** This feature is a component of the [Add efficiency in prospect-to-cash integration with Sales](/dynamics365/release-plan/2023wave1/finance-operations/dynamics365-supply-chain-management/gain-added-efficiency-prospect-to-cash-integration-dynamics-365-sales) functionality, which requires Supply Chain Management version 10.0.34 and other prerequisites listed in [Enable extra efficiency in quote-to-cash with Dynamics 365 Sales](../../fin-ops-core/dev-itpro/data-entities/dual-write/add-efficiency-in-quote-to-cash-enable.md). Make sure that your system meets all of the listed prerequisites before you enable this feature. |
| Sales and marketing | Copy Supply Chain Management sales quotation data to sales orders synced from Dynamics 365 Sales | This feature requires the *Integrate Sales Quotation lifecycle with Dynamics 365 Sales* feature. It ensures data consistency between sales orders and related sales quotations in Supply Chain Management when sales orders are created from sales quotations in Sales and then synchronized over dual-write. As a result, sales orders in Supply Chain Management will include information copied from their related sales quotations. This feature adds a setting on the **Dynamics 365 Sales integration** tab of the **Accounts receivable parameters** page, which lets admins choose whether to copy quotation information on order creation or later through the message processor.<br><br>**Note:** This feature is a component of the [Add efficiency in prospect-to-cash integration with Sales](/dynamics365/release-plan/2023wave1/finance-operations/dynamics365-supply-chain-management/gain-added-efficiency-prospect-to-cash-integration-dynamics-365-sales) functionality, which requires Supply Chain Management version 10.0.34 and other prerequisites listed in [Enable extra efficiency in quote-to-cash with Dynamics 365 Sales](../../fin-ops-core/dev-itpro/data-entities/dual-write/add-efficiency-in-quote-to-cash-enable.md). Make sure that your system meets all of the listed prerequisites before you enable this feature. |
| Sales and marketing | Make Supply Chain Management price master when integrated with Dynamics 365 Sales | This feature requires the *Integrate Sales Quotation lifecycle with Dynamics 365 Sales* feature. When it's enabled, Sales won't perform calculations for extended amounts, summary amounts, subtotals, and totals for sales quotations and sales orders. When quotations or sales orders are created in Sales, and a price list exists in Sales, then that price will be used, but no other calculations will be made. All calculated monetary fields are calculated in and synchronized from Supply Chain Management. In Sales, this feature sets **Use system price calculation** to *No* and **Discount calculation method** to *Per unit*. The following changes are also made in the Sales user interface for sales quotation and sales order lines: the **Volume discount** field is hidden, the **Discount** field is expressed as per-unit discount amount, and the **Manual discount** field is made read-only and relabeled. Manual discounts can henceforth be entered in the **Line discount amount** field.<br><br>**Note:** This feature is a component of the [Add efficiency in prospect-to-cash integration with Sales](/dynamics365/release-plan/2023wave1/finance-operations/dynamics365-supply-chain-management/gain-added-efficiency-prospect-to-cash-integration-dynamics-365-sales) functionality, which requires Supply Chain Management version 10.0.34 and other prerequisites listed in [Enable extra efficiency in quote-to-cash with Dynamics 365 Sales](../../fin-ops-core/dev-itpro/data-entities/dual-write/add-efficiency-in-quote-to-cash-enable.md). Make sure that your system meets all of the listed prerequisites before you enable this feature. |
| Sales and marketing | Set default ownership for sales quotations when integrated with Dynamics 365 Sales | This feature requires the *Integrate Sales Quotation lifecycle with Dynamics 365 Sales* feature. It adds a setting to the **Accounts receivables parameters** page that lets you set the default ownership of new sales quotations. Default ownership can be set to *Based on origin*, *Dynamics 365 Sales*, or *Supply Chain Management*. When this feature is disabled, ownership is always *Based on origin*.<br><br>**Note:** This feature is a component of the [Add efficiency in prospect-to-cash integration with Sales](/dynamics365/release-plan/2023wave1/finance-operations/dynamics365-supply-chain-management/gain-added-efficiency-prospect-to-cash-integration-dynamics-365-sales) functionality, which requires Supply Chain Management version 10.0.34 and other prerequisites listed in [Enable extra efficiency in quote-to-cash with Dynamics 365 Sales](../../fin-ops-core/dev-itpro/data-entities/dual-write/add-efficiency-in-quote-to-cash-enable.md). Make sure that your system meets all of the listed prerequisites before you enable this feature. |
| Shared AP and AR | Rebate management sold-to customers posting | Lets you select sold-to customers as an option for the Rebate management posting account source. With the introduction of this new account source type, you can use *sold-to customers* as an extension type of a deal line account, and use this posting profile on any number of rebate lines. Once *sold-to customers* is set, date transactions will be split and grouped together per account when rebates are processed. Those transactions will also be posted to the same account. |
| Transportation management | (Preview) Source document and accounting distribution support for Landed Cost | Lets you include landed costs in the accounting distribution of purchased product receipts, which makes it easy to identify and track these costs. This feature lets you associate freight cost from Landed cost with their corresponding source documents, which provides a more accurate and comprehensive view of the total cost of goods received. With this functionality, you can gain greater visibility into the expenses associated with your purchases and transportation, allowing for better cost analysis and management. For more information, see [Show landed costs in the accounting distribution of product receipts](../landed-cost/manage-voyages.md#source-doc-post) |

## Additional resources

### Platform updates for Finance and Operations apps

Microsoft Dynamics 365 Supply Chain Management 10.0.34 includes platform updates. To learn more, see [Platform updates for version 10.0.34 of Finance and Operations apps (June 2023)](../../fin-ops-core/dev-itpro/get-started/whats-new-platform-updates-10-0-34.md).

### Bug fixes

For information about the bug fixes included in each of the updates that are part of version 10.0.34, sign in to Microsoft Dynamics Lifecycle Services and view the [KB article](https://fix.lcs.dynamics.com/Issue/Details?bugId=805875).

### Dynamics 365 and industry clouds: 2023 release wave 1 plan

Wondering about upcoming and recently released capabilities in any of our business apps or platform?

Check out the [Dynamics 365 and industry clouds: 2023 release wave 1 plan](/dynamics365/release-plan/2023wave1/). We've captured all the details, end to end, top to bottom, in a single document that you can use for planning.

### Removed and deprecated Supply Chain Management features

The [Removed or deprecated features in Dynamics 365 Supply Chain Management](removed-deprecated-features-scm-updates.md) article describes features that have been or are scheduled to be removed or deprecated for Supply Chain Management.

- A *removed* feature is no longer available in the product.
- A *deprecated* feature isn't in active development and may be removed in a future update.

Before any feature is removed from the product, the deprecation notice will be announced in the [Removed or deprecated features in Dynamics 365 Supply Chain Management](removed-deprecated-features-scm-updates.md) article 12 months prior to the removal.

For breaking changes that only affect compilation time, but are binary compatible with sandbox and production environments, the deprecation time will be less than 12 months. Typically, these are functional updates that need to be made to the compiler.

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
