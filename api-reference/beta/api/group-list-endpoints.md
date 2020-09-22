---
title: List endpoints
description: 检索终结点对象的列表。
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 0e4f8e90571da3f4744ca7d913c38990006f21eb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48002150"
---
# <a name="list-endpoints"></a><span data-ttu-id="3cd3d-103">List endpoints</span><span class="sxs-lookup"><span data-stu-id="3cd3d-103">List endpoints</span></span>

<span data-ttu-id="3cd3d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3cd3d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3cd3d-105">检索 [终结点](../resources/endpoint.md) 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="3cd3d-105">Retrieve a list of [endpoint](../resources/endpoint.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="3cd3d-106">权限</span><span class="sxs-lookup"><span data-stu-id="3cd3d-106">Permissions</span></span>
<span data-ttu-id="3cd3d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3cd3d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3cd3d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3cd3d-109">Permission type</span></span>      | <span data-ttu-id="3cd3d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3cd3d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3cd3d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3cd3d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3cd3d-112">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3cd3d-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3cd3d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3cd3d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3cd3d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3cd3d-114">Not supported.</span></span>    |
|<span data-ttu-id="3cd3d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3cd3d-115">Application</span></span> | <span data-ttu-id="3cd3d-116">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3cd3d-116">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3cd3d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3cd3d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/endpoints
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3cd3d-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3cd3d-118">Optional query parameters</span></span>
<span data-ttu-id="3cd3d-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3cd3d-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3cd3d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3cd3d-120">Request headers</span></span>
| <span data-ttu-id="3cd3d-121">名称</span><span class="sxs-lookup"><span data-stu-id="3cd3d-121">Name</span></span>      |<span data-ttu-id="3cd3d-122">说明</span><span class="sxs-lookup"><span data-stu-id="3cd3d-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3cd3d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3cd3d-123">Authorization</span></span>  | <span data-ttu-id="3cd3d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3cd3d-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="3cd3d-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3cd3d-126">Content-Type</span></span>   | <span data-ttu-id="3cd3d-127">Application/Json</span><span class="sxs-lookup"><span data-stu-id="3cd3d-127">Application/Json</span></span> |

## <a name="request-body"></a><span data-ttu-id="3cd3d-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="3cd3d-128">Request body</span></span>
<span data-ttu-id="3cd3d-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3cd3d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3cd3d-130">响应</span><span class="sxs-lookup"><span data-stu-id="3cd3d-130">Response</span></span>

<span data-ttu-id="3cd3d-131">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [Endpoint](../resources/endpoint.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="3cd3d-131">If successful, this method returns a `200 OK` response code and a collection of [Endpoint](../resources/endpoint.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3cd3d-132">示例</span><span class="sxs-lookup"><span data-stu-id="3cd3d-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="3cd3d-133">请求</span><span class="sxs-lookup"><span data-stu-id="3cd3d-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="3cd3d-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="3cd3d-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_endpoints"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/endpoints
```
# <a name="c"></a>[<span data-ttu-id="3cd3d-135">C#</span><span class="sxs-lookup"><span data-stu-id="3cd3d-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-endpoints-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3cd3d-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3cd3d-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-endpoints-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3cd3d-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3cd3d-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-endpoints-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="3cd3d-138">响应</span><span class="sxs-lookup"><span data-stu-id="3cd3d-138">Response</span></span>
<span data-ttu-id="3cd3d-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3cd3d-139">Here is an example of the response.</span></span>
><span data-ttu-id="3cd3d-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3cd3d-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.endpoint",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 261

{
  "value": [
    {
      "capability": "Conversations",
      "providerId": "{Yammer GUID}",
      "providerName": "Yammer",
      "uri": "uri-value",
      "providerResourceId": "Yammer.FeedURL",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List endpoints",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


