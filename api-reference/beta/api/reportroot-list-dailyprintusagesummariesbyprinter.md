---
title: 列出 dailyPrintUsageSummariesByPrinter
description: 检索按打印机分组的每日打印使用情况摘要列表。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: a7ba73373ee0c575ca32ab9a1e594089ae9cc93e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054922"
---
# <a name="list-dailyprintusagesummariesbyprinter"></a><span data-ttu-id="ccc03-103">列出 dailyPrintUsageSummariesByPrinter</span><span class="sxs-lookup"><span data-stu-id="ccc03-103">List dailyPrintUsageSummariesByPrinter</span></span>

<span data-ttu-id="ccc03-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ccc03-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ccc03-105">检索按打印机分组的每日打印使用情况摘要 [列表](../resources/printer.md)。</span><span class="sxs-lookup"><span data-stu-id="ccc03-105">Retrieve a list of daily print usage summaries, grouped by [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ccc03-106">权限</span><span class="sxs-lookup"><span data-stu-id="ccc03-106">Permissions</span></span>
<span data-ttu-id="ccc03-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ccc03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="ccc03-109">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="ccc03-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="ccc03-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ccc03-110">Permission type</span></span> | <span data-ttu-id="ccc03-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ccc03-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="ccc03-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ccc03-112">Delegated (work or school account)</span></span>| <span data-ttu-id="ccc03-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ccc03-113">Reports.Read.All</span></span> |
|<span data-ttu-id="ccc03-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ccc03-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ccc03-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ccc03-115">Not Supported.</span></span>|
|<span data-ttu-id="ccc03-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ccc03-116">Application</span></span>|<span data-ttu-id="ccc03-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ccc03-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ccc03-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ccc03-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /reports/dailyPrintUsageSummariesByPrinter
GET /print/reports/dailyPrintUsageSummariesByPrinter
```

## <a name="request-headers"></a><span data-ttu-id="ccc03-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ccc03-119">Request headers</span></span>
| <span data-ttu-id="ccc03-120">名称</span><span class="sxs-lookup"><span data-stu-id="ccc03-120">Name</span></span>      |<span data-ttu-id="ccc03-121">说明</span><span class="sxs-lookup"><span data-stu-id="ccc03-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ccc03-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ccc03-122">Authorization</span></span> | <span data-ttu-id="ccc03-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ccc03-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ccc03-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="ccc03-125">Request body</span></span>
<span data-ttu-id="ccc03-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ccc03-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="ccc03-127">响应</span><span class="sxs-lookup"><span data-stu-id="ccc03-127">Response</span></span>
<span data-ttu-id="ccc03-128">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [printUsageSummaryByPrinter](../resources/printusagesummarybyprinter.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ccc03-128">If successful, this method returns a `200 OK` response code and a collection of [printUsageSummaryByPrinter](../resources/printusagesummarybyprinter.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ccc03-129">示例</span><span class="sxs-lookup"><span data-stu-id="ccc03-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ccc03-130">请求</span><span class="sxs-lookup"><span data-stu-id="ccc03-130">Request</span></span>
<span data-ttu-id="ccc03-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ccc03-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ccc03-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="ccc03-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_endpoints_3"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/reports/dailyPrintUsageSummariesByPrinter
```
# <a name="c"></a>[<span data-ttu-id="ccc03-133">C#</span><span class="sxs-lookup"><span data-stu-id="ccc03-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-endpoints-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ccc03-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ccc03-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-endpoints-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ccc03-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ccc03-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-endpoints-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ccc03-136">Java</span><span class="sxs-lookup"><span data-stu-id="ccc03-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-endpoints-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ccc03-137">响应</span><span class="sxs-lookup"><span data-stu-id="ccc03-137">Response</span></span>
<span data-ttu-id="ccc03-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ccc03-138">The following is an example of the response.</span></span>
><span data-ttu-id="ccc03-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ccc03-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printUsageSummaryByPrinter",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 314

{
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "printerId": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "usageDate": "2020-02-04T00:00:00.0000000Z",
      "completedBlackAndWhiteJobCount": 42,
      "completedColorJobCount": 0,
      "incompleteJobCount": 6
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List dailyPrintUsageSummariesByPrinter",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


