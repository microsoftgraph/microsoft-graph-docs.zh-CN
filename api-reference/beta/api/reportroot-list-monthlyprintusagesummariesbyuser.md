---
title: 列出 monthlyPrintUsageSummariesByUser
description: 检索按用户分组的每月打印使用情况摘要列表。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: eeb9ca170a489da0882bf1782f850f802557d0f3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954238"
---
# <a name="list-monthlyprintusagesummariesbyuser"></a><span data-ttu-id="cf0f6-103">列出 monthlyPrintUsageSummariesByUser</span><span class="sxs-lookup"><span data-stu-id="cf0f6-103">List monthlyPrintUsageSummariesByUser</span></span>

<span data-ttu-id="cf0f6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf0f6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf0f6-105">检索按用户分组的每月打印使用情况摘要列表。</span><span class="sxs-lookup"><span data-stu-id="cf0f6-105">Retrieve a list of monthly print usage summaries, grouped by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="cf0f6-106">权限</span><span class="sxs-lookup"><span data-stu-id="cf0f6-106">Permissions</span></span>
<span data-ttu-id="cf0f6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cf0f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="cf0f6-109">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="cf0f6-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="cf0f6-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="cf0f6-110">Permission type</span></span> | <span data-ttu-id="cf0f6-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cf0f6-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="cf0f6-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cf0f6-112">Delegated (work or school account)</span></span>| <span data-ttu-id="cf0f6-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf0f6-113">Reports.Read.All</span></span> |
|<span data-ttu-id="cf0f6-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cf0f6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf0f6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cf0f6-115">Not Supported.</span></span>|
|<span data-ttu-id="cf0f6-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="cf0f6-116">Application</span></span>|<span data-ttu-id="cf0f6-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="cf0f6-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf0f6-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cf0f6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /reports/monthlyPrintUsageSummariesByUser
GET /print/reports/monthlyPrintUsageSummariesByUser
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cf0f6-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="cf0f6-119">Optional query parameters</span></span>
<span data-ttu-id="cf0f6-120">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="cf0f6-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="cf0f6-121">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="cf0f6-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="cf0f6-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="cf0f6-122">Request headers</span></span>
| <span data-ttu-id="cf0f6-123">名称</span><span class="sxs-lookup"><span data-stu-id="cf0f6-123">Name</span></span>      |<span data-ttu-id="cf0f6-124">说明</span><span class="sxs-lookup"><span data-stu-id="cf0f6-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cf0f6-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf0f6-125">Authorization</span></span> | <span data-ttu-id="cf0f6-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cf0f6-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cf0f6-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="cf0f6-128">Request body</span></span>
<span data-ttu-id="cf0f6-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cf0f6-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="cf0f6-130">响应</span><span class="sxs-lookup"><span data-stu-id="cf0f6-130">Response</span></span>
<span data-ttu-id="cf0f6-131">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [printUsageSummaryByUser](../resources/printusagesummarybyuser.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="cf0f6-131">If successful, this method returns a `200 OK` response code and a collection of [printUsageSummaryByUser](../resources/printusagesummarybyuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cf0f6-132">示例</span><span class="sxs-lookup"><span data-stu-id="cf0f6-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cf0f6-133">请求</span><span class="sxs-lookup"><span data-stu-id="cf0f6-133">Request</span></span>
<span data-ttu-id="cf0f6-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cf0f6-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cf0f6-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="cf0f6-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_endpoints_6"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/reports/monthlyPrintUsageSummariesByUser
```
# <a name="c"></a>[<span data-ttu-id="cf0f6-136">C#</span><span class="sxs-lookup"><span data-stu-id="cf0f6-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-endpoints-6-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cf0f6-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cf0f6-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-endpoints-6-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cf0f6-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cf0f6-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-endpoints-6-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cf0f6-139">Java</span><span class="sxs-lookup"><span data-stu-id="cf0f6-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-endpoints-6-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="cf0f6-140">响应</span><span class="sxs-lookup"><span data-stu-id="cf0f6-140">Response</span></span>
<span data-ttu-id="cf0f6-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cf0f6-141">The following is an example of the response.</span></span>
><span data-ttu-id="cf0f6-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="cf0f6-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printUsageSummaryByUser",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 268

{
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "userPrincipalName": "username@contoso.com",
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
  "description": "List monthlyPrintUsageSummariesByUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


