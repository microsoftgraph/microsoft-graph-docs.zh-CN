---
title: 删除 acceptedSender
description: 向 acceptedSender 列表中添加新用户或组。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 827e6d12f8a237718993e49050cb7df2176b0637
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36420663"
---
# <a name="create-acceptedsender"></a><span data-ttu-id="e75ab-103">删除 acceptedSender</span><span class="sxs-lookup"><span data-stu-id="e75ab-103">Create acceptedSender</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e75ab-104">向 acceptedSender 列表中添加新用户或组。</span><span class="sxs-lookup"><span data-stu-id="e75ab-104">Add a new user or group to the acceptedSender list.</span></span>

<span data-ttu-id="e75ab-p101">在请求主体的 `@odata.id` 中指定用户或组。已接受的发件人列表中的用户可以发布到组对话。确保未在接受的发件人和拒绝的发件人列表中指定同一用户或组，否则会发生错误。</span><span class="sxs-lookup"><span data-stu-id="e75ab-p101">Specify the user or group in `@odata.id` in the request body. Users in the accepted senders list can post to conversations of the group . Make sure you do not specify the same user or group in the accepted senders and rejected senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="e75ab-108">权限</span><span class="sxs-lookup"><span data-stu-id="e75ab-108">Permissions</span></span>
<span data-ttu-id="e75ab-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e75ab-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e75ab-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e75ab-111">Permission type</span></span>      | <span data-ttu-id="e75ab-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e75ab-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e75ab-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e75ab-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e75ab-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e75ab-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e75ab-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e75ab-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e75ab-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e75ab-116">Not supported.</span></span>    |
|<span data-ttu-id="e75ab-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e75ab-117">Application</span></span> | <span data-ttu-id="e75ab-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e75ab-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e75ab-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e75ab-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/acceptedSenders/$ref
```
## <a name="request-headers"></a><span data-ttu-id="e75ab-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e75ab-120">Request headers</span></span>
| <span data-ttu-id="e75ab-121">标头</span><span class="sxs-lookup"><span data-stu-id="e75ab-121">Header</span></span>       | <span data-ttu-id="e75ab-122">值</span><span class="sxs-lookup"><span data-stu-id="e75ab-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e75ab-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e75ab-123">Authorization</span></span>  | <span data-ttu-id="e75ab-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e75ab-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e75ab-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e75ab-126">Request body</span></span>
<span data-ttu-id="e75ab-127">在请求正文中，提供 user 或 group 对象的 ID。</span><span class="sxs-lookup"><span data-stu-id="e75ab-127">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="e75ab-128">响应</span><span class="sxs-lookup"><span data-stu-id="e75ab-128">Response</span></span>
<span data-ttu-id="e75ab-129">此方法返回 `204 No Content` 响应代码，不返回任何响应正文。</span><span class="sxs-lookup"><span data-stu-id="e75ab-129">This method returns `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="e75ab-130">示例</span><span class="sxs-lookup"><span data-stu-id="e75ab-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="e75ab-131">请求</span><span class="sxs-lookup"><span data-stu-id="e75ab-131">Request</span></span>
<span data-ttu-id="e75ab-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e75ab-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e75ab-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="e75ab-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_acceptedsender"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/acceptedSenders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id":"https://graph.microsoft.com/beta/users/alexd@contoso.com"
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e75ab-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e75ab-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-acceptedsender-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e75ab-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="e75ab-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-acceptedsender-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="ctabcsharp"></a>[<span data-ttu-id="e75ab-136">C#</span><span class="sxs-lookup"><span data-stu-id="e75ab-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-acceptedsender-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e75ab-137">响应</span><span class="sxs-lookup"><span data-stu-id="e75ab-137">Response</span></span>
<span data-ttu-id="e75ab-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e75ab-138">The following is an example of the response.</span></span>
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
  "description": "Create acceptedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
