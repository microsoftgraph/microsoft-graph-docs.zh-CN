---
title: 在 Microsoft Graph 中使用 Dynamics 365 Business Central API
description: 与 Microsoft Graph 集成的 API 文档
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: conceptualPageType
ms.openlocfilehash: 5173bdba342b6774ffc931ae0b769b1d1228894d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972934"
---
# <a name="working-with-the-dynamics-365-business-central-api-in-microsoft-graph"></a>在 Microsoft Graph 中使用 Dynamics 365 Business Central API
您可以使用 Microsoft Graph 连接 web 服务或 SaaS 解决方案并将其与 Microsoft Dynamics 365 Business Central 相集成。 通过 Microsoft Graph, 你可以构建可获得授权访问和与 Microsoft Dynamics 365 业务中心数据无缝集成的应用程序。

## <a name="authorization"></a>Authorization
使用 Azure AD v2.0 终结点对 Dynamics 365 Business Central Api 进行身份验证。 所有 Api 都需要`Authorization: Bearer {access-token}`请求标头。 有关授权的详细信息, 请参阅[获取访问令牌以调用 Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview)。

## <a name="common-dynamics-365-business-central-scenarios"></a>公共 Dynamics 365 业务中心方案
Dynamics 365 Business Central API 允许您通过通过单个终结点连接并集成的应用程序读取和修改业务数据。 例如, 使用 API 获取对[客户](../resources/dynamics-customer.md)和[供应商](../resources/dynamics-vendor.md)信息的访问权限, 或[查看逾期付款](../resources/dynamics-agedaccountspayable.md)。

## <a name="next-steps"></a>后续步骤
Dynamics 365 Business Central API 可为你与用户接洽的新方式开放。 要了解更多信息，请参阅以下内容：

+ [Dynamics 365 Business Central 概述](/graph/dynamics-business-central-concept-overview)
+ 请尝试[Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)。

<!--
|For Resource Type |See                                                 |
|:-----------------|:---------------------------------------------------|
|account resource type|[account](../resources/dynamics-account.md)|
|aged accounts receivable resource type|[agedAccountsReceivable](../resources/dynamics-agedaccountsreceivable.md)|
|aged accounts payable resource type|[agedAccountsPayable](../resources/dynamics-agedaccountspayable.md)|
|balance sheet resource type|[balanceSheet](../resources/dynamics-balancesheet.md)|
|companies resource type|[companies](../resources/dynamics-companies.md)|
|companyInformation resource type|[companyInformation](../resources/dynamics-companyinformation.md)|
|countriesRegions resource type|[countriesRegions](../resources/dynamics-countriesregions.md)|
|currencies resource type|[currencies](../resources/dynamics-currencies.md)|
|customer resource type|[customer](../resources/dynamics-customer.md)|
|customerPaymentJournal resource type|[customerPaymentsJournal](../resources/dynamics-customerpaymentsjournal.md)|
|customerPayment resource type|[customerPayment](../resources/dynamics-customerpayment.md)|
|dimension resource type|[dimension](../resources/dynamics-dimension.md)|
|dimensionValue resource type|[dimensionValue](../resources/dynamics-dimensionvalue.md)
|employee resource type|[employee](../resources/dynamics-employee.md)|
|generalLedgerEntries resource type|[generalLedgerEntries](../resources/dynamics-generalledgerentries.md)|
|item resource type|[item](../resources/dynamics-item.md)|
|itemCategories resource type|[itemCategories](../resources/dynamics-itemcategories.md)|
|income statement resource type|[incomeStatement](../resources/dynamics-incomestatement.md)|
|IRS1099 resource type|[irs1099](../resources/dynamics-irs1099.md)|
|journal resource type|[journal](../resources/dynamics-journal.md)|
|journalLine resource type|[journalLine](../resources/dynamics-journalline.md)|
|paymentMethods resource type|[paymentMethods](../resources/dynamics-paymentmethods.md)|
|paymentTerms resource type|[paymentTerms](../resources/dynamics-paymentterms.md)|
|retained earnings statement resource type|[retainedEarningsStatement](../resources/dynamics-retainedearningsstatement.md)|
|shipmentMethods resource type|[shipmentMethods](../resources/dynamics-shipmentmethods.md)|
|taxGroups resource type|[taxGroups](../resources/dynamics-taxgroups.md)|
|taxArea resource type|[taxAreas](..resources/dynamics-taxarea.md)|
|trial balance resource type|[trialBalance](../resources/dynamics-trialbalance.md)|
|unitsOfMeasure resource type|[unitsOfMeasure](../resources/dynamics-unitsofmeasure.md)|
|vendor resource type|[vendor](../resources/dynamics-vendor.md)|
-->
