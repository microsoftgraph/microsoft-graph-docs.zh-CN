---
title: 在 Microsoft Graph 中处理 Dynamics 365 商业中心 API
description: 与 Microsoft Graph 集成的 API 文档
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: conceptualPageType
ms.openlocfilehash: b1fdc91d884c4c0869b97f2068d005407158d6a5
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473574"
---
# <a name="working-with-the-dynamics-365-business-central-api-in-microsoft-graph"></a><span data-ttu-id="4b53f-103">在 Microsoft Graph 中处理 Dynamics 365 商业中心 API</span><span class="sxs-lookup"><span data-stu-id="4b53f-103">Working with the Dynamics 365 Business Central API in Microsoft Graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b53f-104">可以使用 Microsoft Graph 将 Web 服务或 SaaS 解决方案与 Microsoft Dynamics 365 Business Central 连接和集成。</span><span class="sxs-lookup"><span data-stu-id="4b53f-104">You can use Microsoft Graph to connect and integrate your web service or SaaS solution with Microsoft Dynamics 365 Business Central.</span></span> <span data-ttu-id="4b53f-105">借助 Microsoft Graph，你可以构建获得 Microsoft Dynamics 365 Business Central 数据的授权访问权限并无缝集成的应用。</span><span class="sxs-lookup"><span data-stu-id="4b53f-105">With Microsoft Graph, you can build apps that get authorized access to and integrate seamlessly with Microsoft Dynamics 365 Business Central data.</span></span>

## <a name="authorization"></a><span data-ttu-id="4b53f-106">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b53f-106">Authorization</span></span>
<span data-ttu-id="4b53f-107">使用 Azure AD v2.0 终结点对 Dynamics 365 商业中心 API 进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="4b53f-107">Use the Azure AD v2.0 endpoint to authenticate Dynamics 365 Business Central APIs.</span></span> <span data-ttu-id="4b53f-108">所有 API 都需要请求 `Authorization: Bearer {access-token}` 标头。</span><span class="sxs-lookup"><span data-stu-id="4b53f-108">All APIs require the `Authorization: Bearer {access-token}` request header.</span></span> <span data-ttu-id="4b53f-109">有关授权的信息，请参阅[获取访问令牌以调用 Microsoft Graph。](/graph/auth/)</span><span class="sxs-lookup"><span data-stu-id="4b53f-109">For more information about authorization, see [Get access tokens to call Microsoft Graph](/graph/auth/).</span></span>

## <a name="common-dynamics-365-business-central-scenarios"></a><span data-ttu-id="4b53f-110">常见 Dynamics 365 Business Central 方案</span><span class="sxs-lookup"><span data-stu-id="4b53f-110">Common Dynamics 365 Business Central scenarios</span></span>
<span data-ttu-id="4b53f-111">Dynamics 365 Business Central API 允许你通过通过单个终结点连接和集成的应用读取和修改业务数据。</span><span class="sxs-lookup"><span data-stu-id="4b53f-111">The Dynamics 365 Business Central API allows you to read and modify business data through apps that are connected and integrated through a single endpoint.</span></span> <span data-ttu-id="4b53f-112">例如，使用 API 获取客户和供应商信息的访问权限[](../resources/dynamics-customer.md)，或[](../resources/dynamics-vendor.md)[查看过期付款](../resources/dynamics-agedaccountspayable.md)。</span><span class="sxs-lookup"><span data-stu-id="4b53f-112">Use the API to, for example, get access to [customer](../resources/dynamics-customer.md) and [vendor](../resources/dynamics-vendor.md) information, or [view overdue payments](../resources/dynamics-agedaccountspayable.md).</span></span>

## <a name="whats-new"></a><span data-ttu-id="4b53f-113">最近更新</span><span class="sxs-lookup"><span data-stu-id="4b53f-113">What's new</span></span>
<span data-ttu-id="4b53f-114">了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。</span><span class="sxs-lookup"><span data-stu-id="4b53f-114">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>

## <a name="next-steps"></a><span data-ttu-id="4b53f-115">后续步骤</span><span class="sxs-lookup"><span data-stu-id="4b53f-115">Next steps</span></span>
<span data-ttu-id="4b53f-116">Dynamics 365 商业中心 API 可以打开与用户互动的新方式。</span><span class="sxs-lookup"><span data-stu-id="4b53f-116">The Dynamics 365 Business Central API can open up new ways for you to engage with users.</span></span> <span data-ttu-id="4b53f-117">要了解更多信息，请参阅以下内容：</span><span class="sxs-lookup"><span data-stu-id="4b53f-117">To learn more, see the following:</span></span>

+ [<span data-ttu-id="4b53f-118">Dynamics 365 Business Central Overview</span><span class="sxs-lookup"><span data-stu-id="4b53f-118">Dynamics 365 Business Central Overview</span></span>](/graph/dynamics-business-central-concept-overview)
+ <span data-ttu-id="4b53f-119">尝试 [Graph 资源管理器](https://developer.microsoft.com/graph/graph-explorer)。</span><span class="sxs-lookup"><span data-stu-id="4b53f-119">Try [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>

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
|unitsOfMeasure resource type|[unitsOfMeasure](../resources/dynamics-unitsofmeasure.md)|
|vendor resource type|[vendor](../resources/dynamics-vendor.md)|
-->