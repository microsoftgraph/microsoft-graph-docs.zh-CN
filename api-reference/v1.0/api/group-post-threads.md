---
title: 创建对话线程
description: '首先，通过创建线程来启动新的组对话。 '
ms.openlocfilehash: 4618a33cb22c327d9fe2b8400b99fa50959a6669
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009775"
---
# <a name="create-conversation-thread"></a><span data-ttu-id="b429d-103">创建对话线程</span><span class="sxs-lookup"><span data-stu-id="b429d-103">Create conversation thread</span></span>
<span data-ttu-id="b429d-104">首先，通过创建线程来启动新的组对话。</span><span class="sxs-lookup"><span data-stu-id="b429d-104">Start a new group conversation by first creating a thread.</span></span> 

<span data-ttu-id="b429d-p101">创建新会话、会话线程，然后可在组中创建帖子。使用 [回复线程](conversationthread-reply.md) 或 [回复帖子](post-reply.md) 进一步发布到该线程。</span><span class="sxs-lookup"><span data-stu-id="b429d-p101">A new conversation, conversation thread, and post are created in the group. Use [reply thread](conversationthread-reply.md) or [reply post](post-reply.md) to further post to that thread.</span></span>

<span data-ttu-id="b429d-107">注意：你还可以 [在现有会话中启动新线程](conversation-post-threads.md)。</span><span class="sxs-lookup"><span data-stu-id="b429d-107">Note: You can also [start a new thread in an existing conversation](conversation-post-threads.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="b429d-108">权限</span><span class="sxs-lookup"><span data-stu-id="b429d-108">Permissions</span></span>
<span data-ttu-id="b429d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b429d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b429d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b429d-111">Permission type</span></span>      | <span data-ttu-id="b429d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b429d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b429d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b429d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b429d-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b429d-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b429d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b429d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b429d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b429d-116">Not supported.</span></span>    |
|<span data-ttu-id="b429d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b429d-117">Application</span></span> | <span data-ttu-id="b429d-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="b429d-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b429d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b429d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="b429d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b429d-120">Request headers</span></span>
| <span data-ttu-id="b429d-121">标头</span><span class="sxs-lookup"><span data-stu-id="b429d-121">Header</span></span>       | <span data-ttu-id="b429d-122">值</span><span class="sxs-lookup"><span data-stu-id="b429d-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b429d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b429d-123">Authorization</span></span>  | <span data-ttu-id="b429d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b429d-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b429d-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b429d-126">Content-Type</span></span>  | <span data-ttu-id="b429d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b429d-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b429d-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="b429d-128">Request body</span></span>
<span data-ttu-id="b429d-129">在请求正文中，提供代表包括 [帖子](../resources/post.md) 的 [conversationThread](../resources/conversationthread.md) 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b429d-129">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object containing a [post](../resources/post.md).</span></span>

## <a name="response"></a><span data-ttu-id="b429d-130">响应</span><span class="sxs-lookup"><span data-stu-id="b429d-130">Response</span></span>
<span data-ttu-id="b429d-131">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [conversationThread](../resources/conversationthread.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b429d-131">If successful, this method returns `201 Created` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b429d-132">示例</span><span class="sxs-lookup"><span data-stu-id="b429d-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="b429d-133">请求</span><span class="sxs-lookup"><span data-stu-id="b429d-133">Request</span></span>
<span data-ttu-id="b429d-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b429d-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_conversationthread_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads
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
#### <a name="response"></a><span data-ttu-id="b429d-135">响应</span><span class="sxs-lookup"><span data-stu-id="b429d-135">Response</span></span>
<span data-ttu-id="b429d-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b429d-136">The following is an example of the response.</span></span>
><span data-ttu-id="b429d-137">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b429d-137">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b429d-138">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b429d-138">All the properties will be returned from an actual call.</span></span>
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
  "lastDeliveredDateTime": "datetime-value",
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
