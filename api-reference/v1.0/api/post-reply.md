---
title: 'post: reply'
description: '在组对话中答复帖子，并向指定线程中添加新帖子。 您可以指定 '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 3be176aedf9c1237aa7c1057f7d3fa7518acd1c4
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33608481"
---
# <a name="post-reply"></a><span data-ttu-id="01d89-104">post: reply</span><span class="sxs-lookup"><span data-stu-id="01d89-104">post: reply</span></span>

<span data-ttu-id="01d89-p102">回复帖子，并向组对话中的指定线程添加新帖子。可以在请求中同时指定父对话和线程，或者仅指定父线程，而不指定父对话。</span><span class="sxs-lookup"><span data-stu-id="01d89-p102">Reply to a post and add a new post to the specified thread in a group conversation. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="01d89-107">权限</span><span class="sxs-lookup"><span data-stu-id="01d89-107">Permissions</span></span>
<span data-ttu-id="01d89-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="01d89-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01d89-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="01d89-110">Permission type</span></span>      | <span data-ttu-id="01d89-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="01d89-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01d89-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="01d89-112">Delegated (work or school account)</span></span> | <span data-ttu-id="01d89-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01d89-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="01d89-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="01d89-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01d89-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="01d89-115">Not supported.</span></span>    |
|<span data-ttu-id="01d89-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="01d89-116">Application</span></span> | <span data-ttu-id="01d89-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01d89-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="01d89-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="01d89-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/reply

```
## <a name="request-headers"></a><span data-ttu-id="01d89-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="01d89-119">Request headers</span></span>
| <span data-ttu-id="01d89-120">标头</span><span class="sxs-lookup"><span data-stu-id="01d89-120">Header</span></span>       | <span data-ttu-id="01d89-121">值</span><span class="sxs-lookup"><span data-stu-id="01d89-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="01d89-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="01d89-122">Authorization</span></span>  | <span data-ttu-id="01d89-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="01d89-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="01d89-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="01d89-125">Request body</span></span>
<span data-ttu-id="01d89-126">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="01d89-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="01d89-127">参数</span><span class="sxs-lookup"><span data-stu-id="01d89-127">Parameter</span></span>    | <span data-ttu-id="01d89-128">类型</span><span class="sxs-lookup"><span data-stu-id="01d89-128">Type</span></span>   |<span data-ttu-id="01d89-129">说明</span><span class="sxs-lookup"><span data-stu-id="01d89-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="01d89-130">帖子</span><span class="sxs-lookup"><span data-stu-id="01d89-130">post</span></span>|[<span data-ttu-id="01d89-131">帖子</span><span class="sxs-lookup"><span data-stu-id="01d89-131">post</span></span>](../resources/post.md)|<span data-ttu-id="01d89-132">正在回复的新帖子。</span><span class="sxs-lookup"><span data-stu-id="01d89-132">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="01d89-133">响应</span><span class="sxs-lookup"><span data-stu-id="01d89-133">Response</span></span>

<span data-ttu-id="01d89-p105">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="01d89-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01d89-136">示例</span><span class="sxs-lookup"><span data-stu-id="01d89-136">Example</span></span>
<span data-ttu-id="01d89-137">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="01d89-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="01d89-138">请求</span><span class="sxs-lookup"><span data-stu-id="01d89-138">Request</span></span>
<span data-ttu-id="01d89-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="01d89-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_reply"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/reply
Content-type: application/json
Content-length: 1131

{
  "post": {
    "body": {
      "contentType": "",
      "content": "content-value"
    },
    "receivedDateTime": "datetime-value",
    "hasAttachments": true,
    "from": {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    },
    "sender": {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    },
    "conversationThreadId": "conversationThreadId-value",
    "newParticipants": [
      {
        "emailAddress": {
          "name": "name-value",
          "address": "address-value"
        }
      }
    ],
    "conversationId": "conversationId-value",
    "createdDateTime": "datetime-value",
    "lastModifiedDateTime": "datetime-value",
    "changeKey": "changeKey-value",
    "categories": [
      "categories-value"
    ],
    "id": "id-value",
    "inReplyTo": {
    },
    "attachments": [
      {
        "lastModifiedDateTime": "datetime-value",
        "name": "name-value",
        "contentType": "contentType-value",
        "size": 99,
        "isInline": true,
        "id": "id-value"
      }
    ]
  }
}
```

##### <a name="response"></a><span data-ttu-id="01d89-140">响应</span><span class="sxs-lookup"><span data-stu-id="01d89-140">Response</span></span>
<span data-ttu-id="01d89-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="01d89-141">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="01d89-142">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="01d89-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="01d89-143">语言</span><span class="sxs-lookup"><span data-stu-id="01d89-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/post_reply-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="01d89-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="01d89-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/post_reply-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "post: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/post-reply.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/post-reply.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
