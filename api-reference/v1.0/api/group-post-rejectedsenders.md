---
title: 创建 rejectedSender
description: 将新用户或组添加到 acceptedSender 列表中。
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 421914c6b0de8af68177051226c33c737b5b47b8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48042063"
---
# <a name="create-rejectedsender"></a><span data-ttu-id="f9d97-103">创建 rejectedSender</span><span class="sxs-lookup"><span data-stu-id="f9d97-103">Create rejectedSender</span></span>

<span data-ttu-id="f9d97-104">命名空间： microsoft 将新用户或组添加到 rejectedSender 列表中。</span><span class="sxs-lookup"><span data-stu-id="f9d97-104">Namespace: microsoft.graph Add a new user or group to the rejectedSender list.</span></span>

<span data-ttu-id="f9d97-p101">在请求主体的 `@odata.id` 中指定用户或组。已拒绝的发件人列表中的用户无法发布到组对话（在 POST 请求 URL 中标识）。确保未在拒绝的发件人和接受的发件人列表中指定同一用户或组，否则会发生错误。</span><span class="sxs-lookup"><span data-stu-id="f9d97-p101">Specify the user or group in `@odata.id` in the request body. Users in the rejected senders list cannot post to conversations of the group (identified in the POST request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="f9d97-108">权限</span><span class="sxs-lookup"><span data-stu-id="f9d97-108">Permissions</span></span>
<span data-ttu-id="f9d97-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f9d97-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9d97-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f9d97-111">Permission type</span></span>      | <span data-ttu-id="f9d97-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f9d97-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f9d97-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f9d97-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f9d97-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9d97-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f9d97-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f9d97-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9d97-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f9d97-116">Not supported.</span></span>    |
|<span data-ttu-id="f9d97-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f9d97-117">Application</span></span> | <span data-ttu-id="f9d97-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="f9d97-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f9d97-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f9d97-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/rejectedSenders/$ref
```
## <a name="request-headers"></a><span data-ttu-id="f9d97-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f9d97-120">Request headers</span></span>
| <span data-ttu-id="f9d97-121">标头</span><span class="sxs-lookup"><span data-stu-id="f9d97-121">Header</span></span>       | <span data-ttu-id="f9d97-122">值</span><span class="sxs-lookup"><span data-stu-id="f9d97-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f9d97-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9d97-123">Authorization</span></span>  | <span data-ttu-id="f9d97-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f9d97-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f9d97-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f9d97-126">Request body</span></span>
<span data-ttu-id="f9d97-127">在请求正文中，提供 user 或 group 对象的 ID。</span><span class="sxs-lookup"><span data-stu-id="f9d97-127">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="f9d97-128">响应</span><span class="sxs-lookup"><span data-stu-id="f9d97-128">Response</span></span>
<span data-ttu-id="f9d97-129">此方法返回 `204 No Content` 响应代码，不返回任何响应正文。</span><span class="sxs-lookup"><span data-stu-id="f9d97-129">This method returns `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9d97-130">示例</span><span class="sxs-lookup"><span data-stu-id="f9d97-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f9d97-131">请求</span><span class="sxs-lookup"><span data-stu-id="f9d97-131">Request</span></span>
<span data-ttu-id="f9d97-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f9d97-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f9d97-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f9d97-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_rejectedsenders_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/rejectedSenders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id":"https://graph.microsoft.com/v1.0/users/alexd@contoso.com"
}
```
# <a name="javascript"></a>[<span data-ttu-id="f9d97-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f9d97-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-rejectedsenders-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f9d97-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f9d97-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-rejectedsenders-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="f9d97-136">C#</span><span class="sxs-lookup"><span data-stu-id="f9d97-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-rejectedsenders-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f9d97-137">Java</span><span class="sxs-lookup"><span data-stu-id="f9d97-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-rejectedsenders-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="f9d97-138">响应</span><span class="sxs-lookup"><span data-stu-id="f9d97-138">Response</span></span>
<span data-ttu-id="f9d97-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f9d97-139">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create rejectedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

