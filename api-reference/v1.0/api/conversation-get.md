---
title: 获取对话
description: 检索 conversation 对象的属性和关系。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: c11db4311f105e9f18311f18dfb36d6f4cd3a7e3
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52035664"
---
# <a name="get-conversation"></a><span data-ttu-id="716be-103">获取对话</span><span class="sxs-lookup"><span data-stu-id="716be-103">Get conversation</span></span>

<span data-ttu-id="716be-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="716be-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="716be-105">检索 conversation 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="716be-105">Retrieve the properties and relationships of conversation object.</span></span>
## <a name="permissions"></a><span data-ttu-id="716be-106">权限</span><span class="sxs-lookup"><span data-stu-id="716be-106">Permissions</span></span>
<span data-ttu-id="716be-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="716be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="716be-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="716be-109">Permission type</span></span>      | <span data-ttu-id="716be-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="716be-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="716be-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="716be-111">Delegated (work or school account)</span></span> | <span data-ttu-id="716be-112">Group.ReadWrite.All、Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="716be-112">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="716be-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="716be-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="716be-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="716be-114">Not supported.</span></span>    |
|<span data-ttu-id="716be-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="716be-115">Application</span></span> | <span data-ttu-id="716be-116">Group.ReadWrite.All、Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="716be-116">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="716be-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="716be-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}

```
## <a name="optional-query-parameters"></a><span data-ttu-id="716be-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="716be-118">Optional query parameters</span></span>
<span data-ttu-id="716be-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="716be-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="716be-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="716be-120">Request headers</span></span>
| <span data-ttu-id="716be-121">标头</span><span class="sxs-lookup"><span data-stu-id="716be-121">Header</span></span>       | <span data-ttu-id="716be-122">值</span><span class="sxs-lookup"><span data-stu-id="716be-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="716be-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="716be-123">Authorization</span></span>  | <span data-ttu-id="716be-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="716be-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="716be-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="716be-126">Request body</span></span>
<span data-ttu-id="716be-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="716be-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="716be-128">响应</span><span class="sxs-lookup"><span data-stu-id="716be-128">Response</span></span>

<span data-ttu-id="716be-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [conversation](../resources/conversation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="716be-129">If successful, this method returns a `200 OK` response code and [conversation](../resources/conversation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="716be-130">示例</span><span class="sxs-lookup"><span data-stu-id="716be-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="716be-131">请求</span><span class="sxs-lookup"><span data-stu-id="716be-131">Request</span></span>
<span data-ttu-id="716be-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="716be-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="716be-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="716be-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversation"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/conversations/{id}
```
# <a name="c"></a>[<span data-ttu-id="716be-134">C#</span><span class="sxs-lookup"><span data-stu-id="716be-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="716be-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="716be-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="716be-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="716be-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="716be-137">Java</span><span class="sxs-lookup"><span data-stu-id="716be-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-conversation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="716be-138">响应</span><span class="sxs-lookup"><span data-stu-id="716be-138">Response</span></span>
<span data-ttu-id="716be-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="716be-139">Here is an example of the response.</span></span> <span data-ttu-id="716be-140">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="716be-140">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "topic": "topic-value",
  "hasAttachments": true,
  "lastDeliveredDateTime": "datetime-value",
  "uniqueSenders": [
    "uniqueSenders-value"
  ],
  "preview": "preview-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
