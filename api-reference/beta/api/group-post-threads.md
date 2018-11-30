---
title: 创建对话线程
description: '首先，通过创建线程来启动新的组对话。 '
ms.openlocfilehash: a18c64b976562a609501c6c50c809b4d11e26866
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047622"
---
# <a name="create-conversation-thread"></a><span data-ttu-id="5246a-103">创建对话线程</span><span class="sxs-lookup"><span data-stu-id="5246a-103">Create conversation thread</span></span>

> <span data-ttu-id="5246a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5246a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5246a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5246a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5246a-106">首先，通过创建线程来启动新的组对话。</span><span class="sxs-lookup"><span data-stu-id="5246a-106">Start a new group conversation by first creating a thread.</span></span> 

<span data-ttu-id="5246a-p102">创建新会话、会话线程，然后可在组中创建帖子。使用 [回复线程](conversationthread-reply.md) 或 [回复帖子](post-reply.md) 进一步发布到该线程。</span><span class="sxs-lookup"><span data-stu-id="5246a-p102">A new conversation, conversation thread, and post are created in the group. Use [reply thread](conversationthread-reply.md) or [reply post](post-reply.md) to further post to that thread.</span></span>

<span data-ttu-id="5246a-109">注意：你还可以 [在现有会话中启动新线程](conversation-post-threads.md)。</span><span class="sxs-lookup"><span data-stu-id="5246a-109">Note: You can also [start a new thread in an existing conversation](conversation-post-threads.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="5246a-110">权限</span><span class="sxs-lookup"><span data-stu-id="5246a-110">Permissions</span></span>
<span data-ttu-id="5246a-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5246a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5246a-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="5246a-113">Permission type</span></span>      | <span data-ttu-id="5246a-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5246a-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5246a-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5246a-115">Delegated (work or school account)</span></span> | <span data-ttu-id="5246a-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5246a-116">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5246a-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5246a-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5246a-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="5246a-118">Not supported.</span></span>    |
|<span data-ttu-id="5246a-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="5246a-119">Application</span></span> | <span data-ttu-id="5246a-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="5246a-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5246a-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5246a-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="5246a-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="5246a-122">Request headers</span></span>
| <span data-ttu-id="5246a-123">标头</span><span class="sxs-lookup"><span data-stu-id="5246a-123">Header</span></span>       | <span data-ttu-id="5246a-124">值</span><span class="sxs-lookup"><span data-stu-id="5246a-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5246a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="5246a-125">Authorization</span></span>  | <span data-ttu-id="5246a-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5246a-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5246a-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5246a-128">Content-Type</span></span>  | <span data-ttu-id="5246a-129">application/json</span><span class="sxs-lookup"><span data-stu-id="5246a-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5246a-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="5246a-130">Request body</span></span>
<span data-ttu-id="5246a-131">在请求正文中，提供代表包括 [帖子](../resources/post.md) 的 [conversationThread](../resources/conversationthread.md) 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5246a-131">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object containing a [post](../resources/post.md).</span></span>

## <a name="response"></a><span data-ttu-id="5246a-132">响应</span><span class="sxs-lookup"><span data-stu-id="5246a-132">Response</span></span>
<span data-ttu-id="5246a-133">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [conversationThread](../resources/conversationthread.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5246a-133">If successful, this method returns `201 Created` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5246a-134">示例</span><span class="sxs-lookup"><span data-stu-id="5246a-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="5246a-135">请求</span><span class="sxs-lookup"><span data-stu-id="5246a-135">Request</span></span>
<span data-ttu-id="5246a-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5246a-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_conversationthread_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/threads
Content-type: application/json

{
  "topic": "New Conversation Thread Topic",
  "posts": [{
    "body": {
      "contentType": "html",
      "content": "this is body content"
    },
    "newParticipants": [{
      "emailAddress": {
        "name": "Alex Darrow",
        "address": "alexd@contoso.com"
      }
    }]
  }]
}
```

#### <a name="response"></a><span data-ttu-id="5246a-137">响应</span><span class="sxs-lookup"><span data-stu-id="5246a-137">Response</span></span>
<span data-ttu-id="5246a-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5246a-138">The following is an example of the response.</span></span>
><span data-ttu-id="5246a-139">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5246a-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5246a-140">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="5246a-140">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 201 OK
Content-type: application/json
Content-length: 419

{
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ],
  "topic": "topic-value",
  "hasAttachments": true,
  "lastDeliveredDateTime": "2016-10-19T10:37:00Z",
  "uniqueSenders": [
    "uniqueSenders-value"
  ],
  "ccRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
