---
title: 创建 rejectedSender
description: 将新用户或组添加到 acceptedSender 列表中。
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 78574fbf0d739075da252e1794c0c1c5f63df295
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52681356"
---
# <a name="create-rejectedsender"></a><span data-ttu-id="a8e5f-103">创建 rejectedSender</span><span class="sxs-lookup"><span data-stu-id="a8e5f-103">Create rejectedSender</span></span>

<span data-ttu-id="a8e5f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8e5f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8e5f-105">将新用户或组添加到 acceptedSender 列表中。</span><span class="sxs-lookup"><span data-stu-id="a8e5f-105">Add a new user or group to the rejectedSender list.</span></span>

<span data-ttu-id="a8e5f-p101">在请求主体的 `@odata.id` 中指定用户或组。已拒绝的发件人列表中的用户无法发布到组对话（在 POST 请求 URL 中标识）。确保未在拒绝的发件人和接受的发件人列表中指定同一用户或组，否则会发生错误。</span><span class="sxs-lookup"><span data-stu-id="a8e5f-p101">Specify the user or group in `@odata.id` in the request body. Users in the rejected senders list cannot post to conversations of the group (identified in the POST request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="a8e5f-109">权限</span><span class="sxs-lookup"><span data-stu-id="a8e5f-109">Permissions</span></span>
<span data-ttu-id="a8e5f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a8e5f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8e5f-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="a8e5f-112">Permission type</span></span>      | <span data-ttu-id="a8e5f-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a8e5f-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a8e5f-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a8e5f-114">Delegated (work or school account)</span></span> | <span data-ttu-id="a8e5f-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8e5f-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a8e5f-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a8e5f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8e5f-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a8e5f-117">Not supported.</span></span>    |
|<span data-ttu-id="a8e5f-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="a8e5f-118">Application</span></span> | <span data-ttu-id="a8e5f-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="a8e5f-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a8e5f-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a8e5f-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/rejectedSenders/$ref
```

## <a name="request-headers"></a><span data-ttu-id="a8e5f-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="a8e5f-121">Request headers</span></span>
| <span data-ttu-id="a8e5f-122">标头</span><span class="sxs-lookup"><span data-stu-id="a8e5f-122">Header</span></span>       | <span data-ttu-id="a8e5f-123">值</span><span class="sxs-lookup"><span data-stu-id="a8e5f-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a8e5f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8e5f-124">Authorization</span></span>  | <span data-ttu-id="a8e5f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a8e5f-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a8e5f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a8e5f-127">Request body</span></span>
<span data-ttu-id="a8e5f-128">在请求正文中，提供 user 或 group 对象的 ID。</span><span class="sxs-lookup"><span data-stu-id="a8e5f-128">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="a8e5f-129">响应</span><span class="sxs-lookup"><span data-stu-id="a8e5f-129">Response</span></span>
<span data-ttu-id="a8e5f-130">此方法返回 `204 No Content` 响应代码，不返回任何响应正文。</span><span class="sxs-lookup"><span data-stu-id="a8e5f-130">This method returns `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8e5f-131">示例</span><span class="sxs-lookup"><span data-stu-id="a8e5f-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a8e5f-132">请求</span><span class="sxs-lookup"><span data-stu-id="a8e5f-132">Request</span></span>
<span data-ttu-id="a8e5f-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a8e5f-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a8e5f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="a8e5f-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_rejectedsender"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/rejectedSenders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id":"https://graph.microsoft.com/beta/users/alexd@contoso.com"
}
```
# <a name="javascript"></a>[<span data-ttu-id="a8e5f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a8e5f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-rejectedsender-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a8e5f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a8e5f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-rejectedsender-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="a8e5f-137">C#</span><span class="sxs-lookup"><span data-stu-id="a8e5f-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-rejectedsender-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a8e5f-138">Java</span><span class="sxs-lookup"><span data-stu-id="a8e5f-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-rejectedsender-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a8e5f-139">响应</span><span class="sxs-lookup"><span data-stu-id="a8e5f-139">Response</span></span>
<span data-ttu-id="a8e5f-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a8e5f-140">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create rejectedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


