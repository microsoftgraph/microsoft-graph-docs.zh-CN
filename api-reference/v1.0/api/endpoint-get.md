---
title: Get endpoint
description: 检索特定终结点对象的属性和关系。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: yyuank
ms.openlocfilehash: 2b91fccac9811c7347618ef98ad8c5bd033f533f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070224"
---
# <a name="get-endpoint"></a><span data-ttu-id="8c26b-103">Get endpoint</span><span class="sxs-lookup"><span data-stu-id="8c26b-103">Get endpoint</span></span>

<span data-ttu-id="8c26b-104">检索特定 [终结点](../resources/endpoint.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8c26b-104">Retrieve the properties and relationships of a specific [endpoint](../resources/endpoint.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8c26b-105">权限</span><span class="sxs-lookup"><span data-stu-id="8c26b-105">Permissions</span></span>
<span data-ttu-id="8c26b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8c26b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8c26b-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="8c26b-108">Permission type</span></span>      | <span data-ttu-id="8c26b-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8c26b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c26b-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8c26b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8c26b-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c26b-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8c26b-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8c26b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c26b-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="8c26b-113">Not supported.</span></span>    |
|<span data-ttu-id="8c26b-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="8c26b-114">Application</span></span> | <span data-ttu-id="8c26b-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c26b-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c26b-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8c26b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/endpoints/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8c26b-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8c26b-117">Optional query parameters</span></span>
<span data-ttu-id="8c26b-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8c26b-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8c26b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8c26b-119">Request headers</span></span>
| <span data-ttu-id="8c26b-120">名称</span><span class="sxs-lookup"><span data-stu-id="8c26b-120">Name</span></span>      |<span data-ttu-id="8c26b-121">说明</span><span class="sxs-lookup"><span data-stu-id="8c26b-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8c26b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c26b-122">Authorization</span></span>  | <span data-ttu-id="8c26b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8c26b-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c26b-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="8c26b-125">Request body</span></span>
<span data-ttu-id="8c26b-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8c26b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c26b-127">响应</span><span class="sxs-lookup"><span data-stu-id="8c26b-127">Response</span></span>

<span data-ttu-id="8c26b-128">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [终结点](../resources/endpoint.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8c26b-128">If successful, this method returns a `200 OK` response code and an [Endpoint](../resources/endpoint.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8c26b-129">示例</span><span class="sxs-lookup"><span data-stu-id="8c26b-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="8c26b-130">请求</span><span class="sxs-lookup"><span data-stu-id="8c26b-130">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="8c26b-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="8c26b-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_endpoint"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/endpoints/{id}
```
# <a name="c"></a>[<span data-ttu-id="8c26b-132">C#</span><span class="sxs-lookup"><span data-stu-id="8c26b-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-endpoint-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8c26b-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8c26b-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-endpoint-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8c26b-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8c26b-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-endpoint-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8c26b-135">响应</span><span class="sxs-lookup"><span data-stu-id="8c26b-135">Response</span></span>
<span data-ttu-id="8c26b-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8c26b-136">Here is an example of the response.</span></span>
><span data-ttu-id="8c26b-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8c26b-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.endpoint"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 208

{
  "capability": "Conversations",
  "providerId": "{Yammer GUID}",
  "providerName": "Yammer",
  "uri": "uri-value",
  "providerResourceId": "Yammer.FeedURL",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get Endpoint",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

