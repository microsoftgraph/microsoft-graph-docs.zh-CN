---
title: 在 Microsoft Graph 中使用 Dynamics 365 Business Central API
description: 与 Microsoft Graph 集成的 API 文档
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: conceptualPageType
ms.openlocfilehash: 97031294aa27ef18e2043f8250c6c6c893e3539d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42503906"
---
# <a name="working-with-the-dynamics-365-business-central-api-in-microsoft-graph"></a><span data-ttu-id="ae857-103">在 Microsoft Graph 中使用 Dynamics 365 Business Central API</span><span class="sxs-lookup"><span data-stu-id="ae857-103">Working with the Dynamics 365 Business Central API in Microsoft Graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae857-104">您可以使用 Microsoft Graph 连接 web 服务或 SaaS 解决方案并将其与 Microsoft Dynamics 365 Business Central 相集成。</span><span class="sxs-lookup"><span data-stu-id="ae857-104">You can use Microsoft Graph to connect and integrate your web service or SaaS solution with Microsoft Dynamics 365 Business Central.</span></span> <span data-ttu-id="ae857-105">通过 Microsoft Graph，你可以构建可获得授权访问和与 Microsoft Dynamics 365 业务中心数据无缝集成的应用程序。</span><span class="sxs-lookup"><span data-stu-id="ae857-105">With Microsoft Graph, you can build apps that get authorized access to and integrate seamlessly with Microsoft Dynamics 365 Business Central data.</span></span>

## <a name="authorization"></a><span data-ttu-id="ae857-106">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae857-106">Authorization</span></span>
<span data-ttu-id="ae857-107">使用 Azure AD v2.0 终结点对 Dynamics 365 Business Central Api 进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="ae857-107">Use the Azure AD v2.0 endpoint to authenticate Dynamics 365 Business Central APIs.</span></span> <span data-ttu-id="ae857-108">所有 Api 都需要`Authorization: Bearer {access-token}`请求标头。</span><span class="sxs-lookup"><span data-stu-id="ae857-108">All APIs require the `Authorization: Bearer {access-token}` request header.</span></span> <span data-ttu-id="ae857-109">有关授权的详细信息，请参阅[获取访问令牌以调用 Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview)。</span><span class="sxs-lookup"><span data-stu-id="ae857-109">For more information about authorization, see [Get access tokens to call Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span></span>

## <a name="common-dynamics-365-business-central-scenarios"></a><span data-ttu-id="ae857-110">公共 Dynamics 365 业务中心方案</span><span class="sxs-lookup"><span data-stu-id="ae857-110">Common Dynamics 365 Business Central scenarios</span></span>
<span data-ttu-id="ae857-111">Dynamics 365 Business Central API 允许您通过通过单个终结点连接并集成的应用程序读取和修改业务数据。</span><span class="sxs-lookup"><span data-stu-id="ae857-111">The Dynamics 365 Business Central API allows you to read and modify business data through apps that are connected and integrated through a single endpoint.</span></span> <span data-ttu-id="ae857-112">例如，使用 API 获取对[客户](../resources/dynamics-customer.md)和[供应商](../resources/dynamics-vendor.md)信息的访问权限，或[查看逾期付款](../resources/dynamics-agedaccountspayable.md)。</span><span class="sxs-lookup"><span data-stu-id="ae857-112">Use the API to, for example, get access to [customer](../resources/dynamics-customer.md) and [vendor](../resources/dynamics-vendor.md) information, or [view overdue payments](../resources/dynamics-agedaccountspayable.md).</span></span>

## <a name="next-steps"></a><span data-ttu-id="ae857-113">后续步骤</span><span class="sxs-lookup"><span data-stu-id="ae857-113">Next steps</span></span>
<span data-ttu-id="ae857-114">Dynamics 365 Business Central API 可为你与用户接洽的新方式开放。</span><span class="sxs-lookup"><span data-stu-id="ae857-114">The Dynamics 365 Business Central API can open up new ways for you to engage with users.</span></span> <span data-ttu-id="ae857-115">要了解更多信息，请参阅以下内容：</span><span class="sxs-lookup"><span data-stu-id="ae857-115">To learn more, see the following:</span></span>

+ [<span data-ttu-id="ae857-116">Dynamics 365 Business Central 概述</span><span class="sxs-lookup"><span data-stu-id="ae857-116">Dynamics 365 Business Central Overview</span></span>](/graph/dynamics-business-central-concept-overview)
+ <span data-ttu-id="ae857-117">请尝试[Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)。</span><span class="sxs-lookup"><span data-stu-id="ae857-117">Try [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>

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
