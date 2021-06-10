---
title: 获取 printUsageByPrinter
description: 检索特定时间段的打印机使用情况摘要。
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
ms.date: 2/4/2020
doc_type: apiPageType
ms.openlocfilehash: 2789109eeab11a00cd49d9c03163b6b224725e80
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869875"
---
# <a name="get-printusagebyprinter"></a><span data-ttu-id="e2f48-103">获取 printUsageByPrinter</span><span class="sxs-lookup"><span data-stu-id="e2f48-103">Get printUsageByPrinter</span></span>

<span data-ttu-id="e2f48-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2f48-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2f48-105">检索 [特定](../resources/printer.md)时间段的打印机使用情况摘要。</span><span class="sxs-lookup"><span data-stu-id="e2f48-105">Retrieve a [printer](../resources/printer.md)'s usage summary for a particular time period.</span></span>

<span data-ttu-id="e2f48-106">有关每个终结点的说明，请参阅 [printUsageByPrinter](../resources/printUsageByPrinter.md)。</span><span class="sxs-lookup"><span data-stu-id="e2f48-106">For descriptions of each of the endpoints, see [printUsageByPrinter](../resources/printUsageByPrinter.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e2f48-107">权限</span><span class="sxs-lookup"><span data-stu-id="e2f48-107">Permissions</span></span>
<span data-ttu-id="e2f48-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e2f48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="e2f48-110">若要使用通用打印服务，除了下表中列出的权限之外，用户或应用的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="e2f48-110">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span>

|<span data-ttu-id="e2f48-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e2f48-111">Permission type</span></span> | <span data-ttu-id="e2f48-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e2f48-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="e2f48-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e2f48-113">Delegated (work or school account)</span></span>| <span data-ttu-id="e2f48-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2f48-114">Reports.Read.All</span></span> |
|<span data-ttu-id="e2f48-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e2f48-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2f48-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e2f48-116">Not Supported.</span></span>|
|<span data-ttu-id="e2f48-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e2f48-117">Application</span></span>|<span data-ttu-id="e2f48-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e2f48-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2f48-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e2f48-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /reports/dailyPrintUsageByPrinter/{id}
GET /reports/monthlyPrintUsageByPrinter/{id}
GET /print/reports/dailyPrintUsageByPrinter/{id}
GET /print/reports/monthlyPrintUsageByPrinter/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e2f48-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e2f48-120">Optional query parameters</span></span>
<span data-ttu-id="e2f48-121">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e2f48-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="e2f48-122">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="e2f48-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e2f48-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="e2f48-123">Request headers</span></span>
| <span data-ttu-id="e2f48-124">名称</span><span class="sxs-lookup"><span data-stu-id="e2f48-124">Name</span></span>      |<span data-ttu-id="e2f48-125">说明</span><span class="sxs-lookup"><span data-stu-id="e2f48-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e2f48-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2f48-126">Authorization</span></span> | <span data-ttu-id="e2f48-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e2f48-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e2f48-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="e2f48-129">Request body</span></span>
<span data-ttu-id="e2f48-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e2f48-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="e2f48-131">响应</span><span class="sxs-lookup"><span data-stu-id="e2f48-131">Response</span></span>
<span data-ttu-id="e2f48-132">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [printUsageByPrinter](../resources/printUsageByPrinter.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e2f48-132">If successful, this method returns a `200 OK` response code and a [printUsageByPrinter](../resources/printUsageByPrinter.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e2f48-133">示例</span><span class="sxs-lookup"><span data-stu-id="e2f48-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="e2f48-134">请求</span><span class="sxs-lookup"><span data-stu-id="e2f48-134">Request</span></span>
<span data-ttu-id="e2f48-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e2f48-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e2f48-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="e2f48-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printUsageByPrinter",
  "sampleKeys": ["016b5565-3bbf-4067-b9ff-4d68167eb1a6"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/reports/dailyPrintUsageByPrinter/016b5565-3bbf-4067-b9ff-4d68167eb1a6
```
# <a name="c"></a>[<span data-ttu-id="e2f48-137">C#</span><span class="sxs-lookup"><span data-stu-id="e2f48-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printusagebyprinter-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e2f48-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e2f48-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printusagebyprinter-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e2f48-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e2f48-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printusagebyprinter-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e2f48-140">Java</span><span class="sxs-lookup"><span data-stu-id="e2f48-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printusagebyprinter-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="e2f48-141">响应</span><span class="sxs-lookup"><span data-stu-id="e2f48-141">Response</span></span>
<span data-ttu-id="e2f48-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e2f48-142">The following is an example of the response.</span></span>
><span data-ttu-id="e2f48-143">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e2f48-143">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printUsageByPrinter"
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
  "description": "Get printUsageByPrinter",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

