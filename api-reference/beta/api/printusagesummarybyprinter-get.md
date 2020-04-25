---
title: 获取 printUsageSummaryByPrinter
description: 检索打印机在特定时间段内的使用率摘要。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
ms.date: 2/4/2020
doc_type: apiPageType
ms.openlocfilehash: ceccd866e4ba8e19f2c4e93ff8e06e9da700cc47
ms.sourcegitcommit: d2536f56e3a424219660bc0495ec8632932b4fb8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/25/2020
ms.locfileid: "43812560"
---
# <a name="get-printusagesummarybyprinter"></a><span data-ttu-id="d4ca4-103">获取 printUsageSummaryByPrinter</span><span class="sxs-lookup"><span data-stu-id="d4ca4-103">Get printUsageSummaryByPrinter</span></span>

<span data-ttu-id="d4ca4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4ca4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4ca4-105">检索[打印机](../resources/printer.md)在特定时间段内的使用率摘要。</span><span class="sxs-lookup"><span data-stu-id="d4ca4-105">Retrieve a [printer](../resources/printer.md)'s usage summary for a particular time period.</span></span> <span data-ttu-id="d4ca4-106">有关每个终结点的说明，请参阅[printUsageSummaryByPrinter](../resources/printUsageSummaryByPrinter.md)。</span><span class="sxs-lookup"><span data-stu-id="d4ca4-106">For descriptions of each of the endpoints, see [printUsageSummaryByPrinter](../resources/printUsageSummaryByPrinter.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d4ca4-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="d4ca4-107">Permissions</span></span>
<span data-ttu-id="d4ca4-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d4ca4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="d4ca4-110">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="d4ca4-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="d4ca4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d4ca4-111">Permission type</span></span> | <span data-ttu-id="d4ca4-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d4ca4-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="d4ca4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d4ca4-113">Delegated (work or school account)</span></span>| <span data-ttu-id="d4ca4-114">已阅读的用户。所有</span><span class="sxs-lookup"><span data-stu-id="d4ca4-114">Users.Read.All</span></span> |
|<span data-ttu-id="d4ca4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d4ca4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4ca4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d4ca4-116">Not Supported.</span></span>|
|<span data-ttu-id="d4ca4-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d4ca4-117">Application</span></span>|<span data-ttu-id="d4ca4-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="d4ca4-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4ca4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d4ca4-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /reports/dailyPrintUsageSummariesByPrinter/{id}
GET /reports/monhtlyPrintUsageSummariesByPrinter/{id}
GET /print/reports/dailyPrintUsageSummariesByPrinter/{id}
GET /print/reports/monthlyPrintUsageSummariesByPrinter/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d4ca4-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d4ca4-120">Optional query parameters</span></span>
<span data-ttu-id="d4ca4-121">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d4ca4-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="d4ca4-122">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="d4ca4-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d4ca4-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="d4ca4-123">Request headers</span></span>
| <span data-ttu-id="d4ca4-124">名称</span><span class="sxs-lookup"><span data-stu-id="d4ca4-124">Name</span></span>      |<span data-ttu-id="d4ca4-125">说明</span><span class="sxs-lookup"><span data-stu-id="d4ca4-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d4ca4-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4ca4-126">Authorization</span></span> | <span data-ttu-id="d4ca4-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d4ca4-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d4ca4-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="d4ca4-129">Request body</span></span>
<span data-ttu-id="d4ca4-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d4ca4-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d4ca4-131">响应</span><span class="sxs-lookup"><span data-stu-id="d4ca4-131">Response</span></span>
<span data-ttu-id="d4ca4-132">如果成功，此方法在响应`200 OK`正文中返回响应代码和[printUsageSummaryByPrinter](../resources/printusagesummarybyprinter.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d4ca4-132">If successful, this method returns a `200 OK` response code and a [printUsageSummaryByPrinter](../resources/printusagesummarybyprinter.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d4ca4-133">示例</span><span class="sxs-lookup"><span data-stu-id="d4ca4-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d4ca4-134">请求</span><span class="sxs-lookup"><span data-stu-id="d4ca4-134">Request</span></span>
<span data-ttu-id="d4ca4-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d4ca4-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_printUsageSummaryByPrinter"
}-->
```http
GET https://graph.microsoft.com/beta/print/reports/dailyPrintUsageSummariesByPrinter/{id}
```
##### <a name="response"></a><span data-ttu-id="d4ca4-136">响应</span><span class="sxs-lookup"><span data-stu-id="d4ca4-136">Response</span></span>
<span data-ttu-id="d4ca4-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d4ca4-137">The following is an example of the response.</span></span>
><span data-ttu-id="d4ca4-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d4ca4-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printUsageSummaryByPrinter"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 269

{
    "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
    "printerId": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
    "usageDate": "2020-02-04T00:00:00.0000000Z",
    "completedBlackAndWhiteJobCount": 42,
    "completedColorJobCount": 0,
    "incompleteJobCount": 6
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get printUsageSummaryByPrinter",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->