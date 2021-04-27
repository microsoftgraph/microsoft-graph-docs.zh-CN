---
title: Get endpoint
description: 检索特定终结点对象的属性和关系。
localization_priority: Normal
doc_type: apiPageType
ms.prod: groups
author: yyuank
ms.openlocfilehash: 8b5cc003787b9a389842389d3aabd7c75726c8f5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52042644"
---
# <a name="get-endpoint"></a><span data-ttu-id="46a96-103">Get endpoint</span><span class="sxs-lookup"><span data-stu-id="46a96-103">Get endpoint</span></span>

<span data-ttu-id="46a96-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46a96-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46a96-105">检索特定终结点对象的属性 [和](../resources/endpoint.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="46a96-105">Retrieve the properties and relationships of a specific [endpoint](../resources/endpoint.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="46a96-106">权限</span><span class="sxs-lookup"><span data-stu-id="46a96-106">Permissions</span></span>
<span data-ttu-id="46a96-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="46a96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="46a96-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="46a96-109">Permission type</span></span>      | <span data-ttu-id="46a96-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="46a96-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="46a96-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="46a96-111">Delegated (work or school account)</span></span> | <span data-ttu-id="46a96-112">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46a96-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="46a96-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="46a96-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46a96-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="46a96-114">Not supported.</span></span>    |
|<span data-ttu-id="46a96-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="46a96-115">Application</span></span> | <span data-ttu-id="46a96-116">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46a96-116">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="46a96-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="46a96-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/endpoints/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="46a96-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="46a96-118">Optional query parameters</span></span>
<span data-ttu-id="46a96-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="46a96-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="46a96-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="46a96-120">Request headers</span></span>
| <span data-ttu-id="46a96-121">名称</span><span class="sxs-lookup"><span data-stu-id="46a96-121">Name</span></span>      |<span data-ttu-id="46a96-122">说明</span><span class="sxs-lookup"><span data-stu-id="46a96-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="46a96-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="46a96-123">Authorization</span></span>  | <span data-ttu-id="46a96-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="46a96-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="46a96-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="46a96-126">Request body</span></span>
<span data-ttu-id="46a96-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="46a96-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46a96-128">响应</span><span class="sxs-lookup"><span data-stu-id="46a96-128">Response</span></span>

<span data-ttu-id="46a96-129">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [Endpoint](../resources/endpoint.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="46a96-129">If successful, this method returns a `200 OK` response code and an [Endpoint](../resources/endpoint.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="46a96-130">示例</span><span class="sxs-lookup"><span data-stu-id="46a96-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="46a96-131">请求</span><span class="sxs-lookup"><span data-stu-id="46a96-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="46a96-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="46a96-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_endpoint"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/endpoints/{id}
```
# <a name="c"></a>[<span data-ttu-id="46a96-133">C#</span><span class="sxs-lookup"><span data-stu-id="46a96-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-endpoint-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="46a96-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="46a96-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-endpoint-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="46a96-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="46a96-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-endpoint-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="46a96-136">Java</span><span class="sxs-lookup"><span data-stu-id="46a96-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-endpoint-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="46a96-137">响应</span><span class="sxs-lookup"><span data-stu-id="46a96-137">Response</span></span>
<span data-ttu-id="46a96-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="46a96-138">Here is an example of the response.</span></span>
><span data-ttu-id="46a96-139">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="46a96-139">Note: The response object shown here might be shortened for readability.</span></span>
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
