---
title: Get endpoint
description: 检索特定终结点对象的属性和关系。
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: f7ca844d59afe133781c0b3bce7d1577c79efb1e
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36720702"
---
# <a name="get-endpoint"></a><span data-ttu-id="1af6b-103">Get endpoint</span><span class="sxs-lookup"><span data-stu-id="1af6b-103">Get endpoint</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1af6b-104">检索特定[终结点](../resources/endpoint.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1af6b-104">Retrieve the properties and relationships of a specific [endpoint](../resources/endpoint.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1af6b-105">权限</span><span class="sxs-lookup"><span data-stu-id="1af6b-105">Permissions</span></span>
<span data-ttu-id="1af6b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1af6b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1af6b-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="1af6b-108">Permission type</span></span>      | <span data-ttu-id="1af6b-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1af6b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1af6b-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1af6b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1af6b-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1af6b-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1af6b-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1af6b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1af6b-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="1af6b-113">Not supported.</span></span>    |
|<span data-ttu-id="1af6b-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="1af6b-114">Application</span></span> | <span data-ttu-id="1af6b-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1af6b-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1af6b-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1af6b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/endpoints/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1af6b-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1af6b-117">Optional query parameters</span></span>
<span data-ttu-id="1af6b-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1af6b-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1af6b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1af6b-119">Request headers</span></span>
| <span data-ttu-id="1af6b-120">名称</span><span class="sxs-lookup"><span data-stu-id="1af6b-120">Name</span></span>      |<span data-ttu-id="1af6b-121">说明</span><span class="sxs-lookup"><span data-stu-id="1af6b-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1af6b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1af6b-122">Authorization</span></span>  | <span data-ttu-id="1af6b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1af6b-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="1af6b-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1af6b-125">Content-Type</span></span>   | <span data-ttu-id="1af6b-126">Application/Json</span><span class="sxs-lookup"><span data-stu-id="1af6b-126">Application/Json</span></span> |

## <a name="request-body"></a><span data-ttu-id="1af6b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1af6b-127">Request body</span></span>
<span data-ttu-id="1af6b-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1af6b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1af6b-129">响应</span><span class="sxs-lookup"><span data-stu-id="1af6b-129">Response</span></span>

<span data-ttu-id="1af6b-130">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[终结点](../resources/endpoint.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1af6b-130">If successful, this method returns a `200 OK` response code and [Endpoint](../resources/endpoint.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1af6b-131">示例</span><span class="sxs-lookup"><span data-stu-id="1af6b-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1af6b-132">请求</span><span class="sxs-lookup"><span data-stu-id="1af6b-132">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="1af6b-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="1af6b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_endpoint"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/endpoints/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1af6b-134">C#</span><span class="sxs-lookup"><span data-stu-id="1af6b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-endpoint-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1af6b-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1af6b-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-endpoint-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1af6b-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="1af6b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-endpoint-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1af6b-137">响应</span><span class="sxs-lookup"><span data-stu-id="1af6b-137">Response</span></span>
<span data-ttu-id="1af6b-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1af6b-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
