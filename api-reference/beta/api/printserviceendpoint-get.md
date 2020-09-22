---
title: 获取 printServiceEndpoint
description: 检索打印服务终结点的属性和关系。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: f211f737fc49762168db14ba5bdde5b974a64e97
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48035349"
---
# <a name="get-printserviceendpoint"></a><span data-ttu-id="4aa1d-103">获取 printServiceEndpoint</span><span class="sxs-lookup"><span data-stu-id="4aa1d-103">Get printServiceEndpoint</span></span>

<span data-ttu-id="4aa1d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4aa1d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4aa1d-105">检索打印服务终结点的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4aa1d-105">Retrieve the properties and relationships of a print service endpoint.</span></span>

## <a name="permissions"></a><span data-ttu-id="4aa1d-106">权限</span><span class="sxs-lookup"><span data-stu-id="4aa1d-106">Permissions</span></span>
<span data-ttu-id="4aa1d-107">不需要任何权限即可调用此 API，但若要使用通用打印服务，用户或应用的租户必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="4aa1d-107">No permissions are needed to call this API, but to use the Universal Print service, the user or app's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="4aa1d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="4aa1d-108">Permission type</span></span> | <span data-ttu-id="4aa1d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4aa1d-109">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="4aa1d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4aa1d-110">Delegated (work or school account)</span></span>|<span data-ttu-id="4aa1d-111">无。</span><span class="sxs-lookup"><span data-stu-id="4aa1d-111">None.</span></span>|
|<span data-ttu-id="4aa1d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4aa1d-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4aa1d-113">无。</span><span class="sxs-lookup"><span data-stu-id="4aa1d-113">None.</span></span>|
|<span data-ttu-id="4aa1d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="4aa1d-114">Application</span></span>|<span data-ttu-id="4aa1d-115">无。</span><span class="sxs-lookup"><span data-stu-id="4aa1d-115">None.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4aa1d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4aa1d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/services/{id}/endpoints/{name}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4aa1d-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4aa1d-117">Optional query parameters</span></span>
<span data-ttu-id="4aa1d-118">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4aa1d-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="4aa1d-119">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="4aa1d-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="4aa1d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4aa1d-120">Request headers</span></span>
| <span data-ttu-id="4aa1d-121">名称</span><span class="sxs-lookup"><span data-stu-id="4aa1d-121">Name</span></span>      |<span data-ttu-id="4aa1d-122">说明</span><span class="sxs-lookup"><span data-stu-id="4aa1d-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4aa1d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4aa1d-123">Authorization</span></span> | <span data-ttu-id="4aa1d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4aa1d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4aa1d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4aa1d-126">Request body</span></span>
<span data-ttu-id="4aa1d-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4aa1d-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="4aa1d-128">响应</span><span class="sxs-lookup"><span data-stu-id="4aa1d-128">Response</span></span>
<span data-ttu-id="4aa1d-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [printServiceEndpoint](../resources/printserviceendpoint.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4aa1d-129">If successful, this method returns a `200 OK` response code and a [printServiceEndpoint](../resources/printserviceendpoint.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4aa1d-130">示例</span><span class="sxs-lookup"><span data-stu-id="4aa1d-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4aa1d-131">请求</span><span class="sxs-lookup"><span data-stu-id="4aa1d-131">Request</span></span>
<span data-ttu-id="4aa1d-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4aa1d-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4aa1d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="4aa1d-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printserviceendpoint"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/services/{id}/endpoints/{name}
```
# <a name="c"></a>[<span data-ttu-id="4aa1d-134">C#</span><span class="sxs-lookup"><span data-stu-id="4aa1d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printserviceendpoint-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4aa1d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4aa1d-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printserviceendpoint-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4aa1d-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4aa1d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printserviceendpoint-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4aa1d-137">响应</span><span class="sxs-lookup"><span data-stu-id="4aa1d-137">Response</span></span>
<span data-ttu-id="4aa1d-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4aa1d-138">The following is an example of the response.</span></span>
><span data-ttu-id="4aa1d-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4aa1d-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printServiceEndpoint"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 260

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.printServiceEndpoint)",
  "id": "mpsdiscovery",
  "displayName": "Microsoft Universal Print Discovery Service",
  "uri": "https://discovery.print.microsoft.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get printServiceEndpoint",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


