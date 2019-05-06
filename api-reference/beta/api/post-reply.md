---
title: 'post: reply'
description: '在组对话中答复帖子，并向指定线程中添加新帖子。 您可以指定 '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: a5e1ec5d3ed2bca3b03c2298239f3168ff5b3699
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33595234"
---
# <a name="post-reply"></a><span data-ttu-id="eb562-104">post: reply</span><span class="sxs-lookup"><span data-stu-id="eb562-104">post: reply</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb562-p102">回复帖子，并向组对话中的指定线程添加新帖子。可以在请求中同时指定父对话和线程，或者仅指定父线程，而不指定父对话。</span><span class="sxs-lookup"><span data-stu-id="eb562-p102">Reply to a post and add a new post to the specified thread in a group conversation. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="eb562-107">权限</span><span class="sxs-lookup"><span data-stu-id="eb562-107">Permissions</span></span>
<span data-ttu-id="eb562-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eb562-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb562-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="eb562-110">Permission type</span></span>      | <span data-ttu-id="eb562-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="eb562-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb562-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eb562-112">Delegated (work or school account)</span></span> | <span data-ttu-id="eb562-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb562-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="eb562-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eb562-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb562-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="eb562-115">Not supported.</span></span>    |
|<span data-ttu-id="eb562-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="eb562-116">Application</span></span> | <span data-ttu-id="eb562-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb562-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb562-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eb562-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/reply

```
## <a name="request-headers"></a><span data-ttu-id="eb562-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="eb562-119">Request headers</span></span>
| <span data-ttu-id="eb562-120">标头</span><span class="sxs-lookup"><span data-stu-id="eb562-120">Header</span></span>       | <span data-ttu-id="eb562-121">值</span><span class="sxs-lookup"><span data-stu-id="eb562-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="eb562-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb562-122">Authorization</span></span>  | <span data-ttu-id="eb562-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="eb562-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="eb562-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="eb562-125">Request body</span></span>
<span data-ttu-id="eb562-126">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="eb562-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="eb562-127">参数</span><span class="sxs-lookup"><span data-stu-id="eb562-127">Parameter</span></span>    | <span data-ttu-id="eb562-128">类型</span><span class="sxs-lookup"><span data-stu-id="eb562-128">Type</span></span>   |<span data-ttu-id="eb562-129">说明</span><span class="sxs-lookup"><span data-stu-id="eb562-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eb562-130">帖子</span><span class="sxs-lookup"><span data-stu-id="eb562-130">post</span></span>|[<span data-ttu-id="eb562-131">帖子</span><span class="sxs-lookup"><span data-stu-id="eb562-131">post</span></span>](../resources/post.md)|<span data-ttu-id="eb562-132">正在回复的新帖子。</span><span class="sxs-lookup"><span data-stu-id="eb562-132">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="eb562-133">响应</span><span class="sxs-lookup"><span data-stu-id="eb562-133">Response</span></span>

<span data-ttu-id="eb562-p105">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="eb562-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb562-136">示例</span><span class="sxs-lookup"><span data-stu-id="eb562-136">Example</span></span>
<span data-ttu-id="eb562-137">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="eb562-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="eb562-138">请求</span><span class="sxs-lookup"><span data-stu-id="eb562-138">Request</span></span>
<span data-ttu-id="eb562-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="eb562-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_reply"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}/reply
Content-type: application/json
Content-length: 1131

{
  "post": {
    "body": {
      "contentType": "",
      "content": "content-value"
    },
    "receivedDateTime": "2016-10-19T10:37:00Z",
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
    "createdDateTime": "2016-10-19T10:37:00Z",
    "lastModifiedDateTime": "2016-10-19T10:37:00Z",
    "changeKey": "changeKey-value",
    "categories": [
      "categories-value"
    ],
    "id": "id-value",
    "inReplyTo": {
    },
    "attachments": [
      {
        "lastModifiedDateTime": "2016-10-19T10:37:00Z",
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

##### <a name="response"></a><span data-ttu-id="eb562-140">响应</span><span class="sxs-lookup"><span data-stu-id="eb562-140">Response</span></span>
##### <a name="response"></a><span data-ttu-id="eb562-141">响应</span><span class="sxs-lookup"><span data-stu-id="eb562-141">Response</span></span>
<span data-ttu-id="eb562-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="eb562-142">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="eb562-143">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="eb562-143">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="eb562-144">语言</span><span class="sxs-lookup"><span data-stu-id="eb562-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/post_reply-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="eb562-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="eb562-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/post_reply-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "post: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/post-reply.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/post-reply.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
