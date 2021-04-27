---
title: 列出 printServiceEndpoints
description: 检索打印服务公开的终结点列表。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 9441b8e704edb328afa2fe372204f0a2c1acc5ed
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053606"
---
# <a name="list-printserviceendpoints"></a><span data-ttu-id="90d03-103">列出 printServiceEndpoints</span><span class="sxs-lookup"><span data-stu-id="90d03-103">List printServiceEndpoints</span></span>

<span data-ttu-id="90d03-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90d03-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90d03-105">检索打印服务公开的终结点列表。</span><span class="sxs-lookup"><span data-stu-id="90d03-105">Retrieve a list of endpoints exposed by a print service.</span></span>

## <a name="permissions"></a><span data-ttu-id="90d03-106">权限</span><span class="sxs-lookup"><span data-stu-id="90d03-106">Permissions</span></span>
<span data-ttu-id="90d03-107">调用此 API 不需要任何权限，但若要使用通用打印服务，用户或应用的租户必须拥有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="90d03-107">No permissions are needed to call this API, but to use the Universal Print service, the user or app's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="90d03-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="90d03-108">Permission type</span></span> | <span data-ttu-id="90d03-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="90d03-109">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="90d03-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="90d03-110">Delegated (work or school account)</span></span>|<span data-ttu-id="90d03-111">无。</span><span class="sxs-lookup"><span data-stu-id="90d03-111">None.</span></span>|
|<span data-ttu-id="90d03-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="90d03-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90d03-113">无。</span><span class="sxs-lookup"><span data-stu-id="90d03-113">None.</span></span>|
|<span data-ttu-id="90d03-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="90d03-114">Application</span></span>|<span data-ttu-id="90d03-115">无。</span><span class="sxs-lookup"><span data-stu-id="90d03-115">None.</span></span>|

## <a name="http-request"></a><span data-ttu-id="90d03-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="90d03-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/services/{id}/endpoints
```

## <a name="optional-query-parameters"></a><span data-ttu-id="90d03-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="90d03-117">Optional query parameters</span></span>
<span data-ttu-id="90d03-118">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="90d03-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="90d03-119">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="90d03-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="90d03-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="90d03-120">Request headers</span></span>
| <span data-ttu-id="90d03-121">名称</span><span class="sxs-lookup"><span data-stu-id="90d03-121">Name</span></span>      |<span data-ttu-id="90d03-122">说明</span><span class="sxs-lookup"><span data-stu-id="90d03-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="90d03-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="90d03-123">Authorization</span></span> | <span data-ttu-id="90d03-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="90d03-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="90d03-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="90d03-126">Request body</span></span>
<span data-ttu-id="90d03-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="90d03-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="90d03-128">响应</span><span class="sxs-lookup"><span data-stu-id="90d03-128">Response</span></span>
<span data-ttu-id="90d03-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [printServiceEndpoint](../resources/printserviceendpoint.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="90d03-129">If successful, this method returns a `200 OK` response code and a collection of [printServiceEndpoint](../resources/printserviceendpoint.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="90d03-130">示例</span><span class="sxs-lookup"><span data-stu-id="90d03-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="90d03-131">请求</span><span class="sxs-lookup"><span data-stu-id="90d03-131">Request</span></span>
<span data-ttu-id="90d03-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="90d03-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="90d03-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="90d03-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_endpoints_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/services/{id}/endpoints
```
# <a name="c"></a>[<span data-ttu-id="90d03-134">C#</span><span class="sxs-lookup"><span data-stu-id="90d03-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-endpoints-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="90d03-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="90d03-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-endpoints-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="90d03-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="90d03-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-endpoints-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="90d03-137">Java</span><span class="sxs-lookup"><span data-stu-id="90d03-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-endpoints-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="90d03-138">响应</span><span class="sxs-lookup"><span data-stu-id="90d03-138">Response</span></span>
<span data-ttu-id="90d03-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="90d03-139">The following is an example of the response.</span></span>
><span data-ttu-id="90d03-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="90d03-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printServiceEndpoint",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 305

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.printServiceEndpoint)",
  "value": [
    {
      "id": "mpsdiscovery",
      "displayName": "Microsoft Universal Print Discovery Service",
      "uri": "https://discovery.print.microsoft.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List endpoints",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


