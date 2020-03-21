---
title: 获取 printUsageSummaryByPrinter
description: 检索打印机在特定时间段内的使用率摘要。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
ms.date: 2/4/2020
doc_type: apiPageType
ms.openlocfilehash: 71bce2c90d9ade62f5d473e2d0e530767e8092fe
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895657"
---
# <a name="get-printusagesummarybyprinter"></a><span data-ttu-id="4e77b-103">获取 printUsageSummaryByPrinter</span><span class="sxs-lookup"><span data-stu-id="4e77b-103">Get printUsageSummaryByPrinter</span></span>

<span data-ttu-id="4e77b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e77b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e77b-105">检索[打印机](../resources/printer.md)在特定时间段内的使用率摘要。</span><span class="sxs-lookup"><span data-stu-id="4e77b-105">Retrieve a [printer](../resources/printer.md)'s usage summary for a particular time period.</span></span> <span data-ttu-id="4e77b-106">有关每个终结点的说明，请参阅[printUsageSummaryByPrinter](../resources/printUsageSummaryByPrinter.md)。</span><span class="sxs-lookup"><span data-stu-id="4e77b-106">For descriptions of each of the endpoints, see [printUsageSummaryByPrinter](../resources/printUsageSummaryByPrinter.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4e77b-107">权限</span><span class="sxs-lookup"><span data-stu-id="4e77b-107">Permissions</span></span>
<span data-ttu-id="4e77b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4e77b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="4e77b-110">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="4e77b-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="4e77b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4e77b-111">Permission type</span></span> | <span data-ttu-id="4e77b-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4e77b-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="4e77b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4e77b-113">Delegated (work or school account)</span></span>| <span data-ttu-id="4e77b-114">已阅读的用户。所有</span><span class="sxs-lookup"><span data-stu-id="4e77b-114">Users.Read.All</span></span> |
|<span data-ttu-id="4e77b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4e77b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e77b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4e77b-116">Not Supported.</span></span>|
|<span data-ttu-id="4e77b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="4e77b-117">Application</span></span>|<span data-ttu-id="4e77b-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="4e77b-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e77b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4e77b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /reports/dailyPrintUsageSummariesByPrinter/{id}
GET /reports/monhtlyPrintUsageSummariesByPrinter/{id}
GET /print/reports/dailyPrintUsageSummariesByPrinter/{id}
GET /print/reports/monthlyPrintUsageSummariesByPrinter/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4e77b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4e77b-120">Request headers</span></span>
| <span data-ttu-id="4e77b-121">名称</span><span class="sxs-lookup"><span data-stu-id="4e77b-121">Name</span></span>      |<span data-ttu-id="4e77b-122">说明</span><span class="sxs-lookup"><span data-stu-id="4e77b-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4e77b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e77b-123">Authorization</span></span> | <span data-ttu-id="4e77b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4e77b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4e77b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4e77b-126">Request body</span></span>
<span data-ttu-id="4e77b-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4e77b-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="4e77b-128">响应</span><span class="sxs-lookup"><span data-stu-id="4e77b-128">Response</span></span>
<span data-ttu-id="4e77b-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和[printUsageSummaryByPrinter](../resources/printusagesummarybyprinter.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4e77b-129">If successful, this method returns a `200 OK` response code and a [printUsageSummaryByPrinter](../resources/printusagesummarybyprinter.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4e77b-130">示例</span><span class="sxs-lookup"><span data-stu-id="4e77b-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4e77b-131">请求</span><span class="sxs-lookup"><span data-stu-id="4e77b-131">Request</span></span>
<span data-ttu-id="4e77b-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4e77b-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_printUsageSummaryByPrinter"
}-->
```http
GET https://graph.microsoft.com/beta/print/reports/dailyPrintUsageSummariesByPrinter/{id}
```
##### <a name="response"></a><span data-ttu-id="4e77b-133">响应</span><span class="sxs-lookup"><span data-stu-id="4e77b-133">Response</span></span>
<span data-ttu-id="4e77b-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4e77b-134">The following is an example of the response.</span></span>
><span data-ttu-id="4e77b-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4e77b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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