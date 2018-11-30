---
title: 'post: reply'
description: '在组对话中答复帖子，并向指定线程中添加新帖子。 您可以指定 '
ms.openlocfilehash: 9698efa8fcd2670f5a837652b8db327ef5c5f55d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046183"
---
# <a name="post-reply"></a><span data-ttu-id="e2433-104">post: reply</span><span class="sxs-lookup"><span data-stu-id="e2433-104">post: reply</span></span>

> <span data-ttu-id="e2433-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e2433-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e2433-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e2433-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e2433-p103">回复帖子，并向组对话中的指定线程添加新帖子。可以在请求中同时指定父对话和线程，或者仅指定父线程，而不指定父对话。</span><span class="sxs-lookup"><span data-stu-id="e2433-p103">Reply to a post and add a new post to the specified thread in a group conversation. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="e2433-109">权限</span><span class="sxs-lookup"><span data-stu-id="e2433-109">Permissions</span></span>
<span data-ttu-id="e2433-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e2433-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2433-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="e2433-112">Permission type</span></span>      | <span data-ttu-id="e2433-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e2433-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2433-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e2433-114">Delegated (work or school account)</span></span> | <span data-ttu-id="e2433-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2433-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e2433-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e2433-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2433-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e2433-117">Not supported.</span></span>    |
|<span data-ttu-id="e2433-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="e2433-118">Application</span></span> | <span data-ttu-id="e2433-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2433-119">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2433-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e2433-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/reply

```
## <a name="request-headers"></a><span data-ttu-id="e2433-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="e2433-121">Request headers</span></span>
| <span data-ttu-id="e2433-122">标头</span><span class="sxs-lookup"><span data-stu-id="e2433-122">Header</span></span>       | <span data-ttu-id="e2433-123">值</span><span class="sxs-lookup"><span data-stu-id="e2433-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e2433-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2433-124">Authorization</span></span>  | <span data-ttu-id="e2433-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e2433-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e2433-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e2433-127">Request body</span></span>
<span data-ttu-id="e2433-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="e2433-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e2433-129">参数</span><span class="sxs-lookup"><span data-stu-id="e2433-129">Parameter</span></span>    | <span data-ttu-id="e2433-130">类型</span><span class="sxs-lookup"><span data-stu-id="e2433-130">Type</span></span>   |<span data-ttu-id="e2433-131">说明</span><span class="sxs-lookup"><span data-stu-id="e2433-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e2433-132">帖子</span><span class="sxs-lookup"><span data-stu-id="e2433-132">post</span></span>|[<span data-ttu-id="e2433-133">帖子</span><span class="sxs-lookup"><span data-stu-id="e2433-133">post</span></span>](../resources/post.md)|<span data-ttu-id="e2433-134">正在回复的新帖子。</span><span class="sxs-lookup"><span data-stu-id="e2433-134">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="e2433-135">响应</span><span class="sxs-lookup"><span data-stu-id="e2433-135">Response</span></span>

<span data-ttu-id="e2433-p106">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="e2433-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2433-138">示例</span><span class="sxs-lookup"><span data-stu-id="e2433-138">Example</span></span>
<span data-ttu-id="e2433-139">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="e2433-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e2433-140">请求</span><span class="sxs-lookup"><span data-stu-id="e2433-140">Request</span></span>
<span data-ttu-id="e2433-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e2433-141">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="e2433-142">响应</span><span class="sxs-lookup"><span data-stu-id="e2433-142">Response</span></span>
##### <a name="response"></a><span data-ttu-id="e2433-143">响应</span><span class="sxs-lookup"><span data-stu-id="e2433-143">Response</span></span>
<span data-ttu-id="e2433-144">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e2433-144">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "post: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
