---
title: 创建线程
description: 在指定会话中创建新线程。
ms.openlocfilehash: d545cc8fcc9ac78e9fcda1a7722bb622bf0d72ae
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042355"
---
# <a name="create-thread"></a><span data-ttu-id="e5635-103">创建线程</span><span class="sxs-lookup"><span data-stu-id="e5635-103">Create thread</span></span>

> <span data-ttu-id="e5635-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e5635-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e5635-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e5635-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e5635-106">在指定会话中创建新线程。</span><span class="sxs-lookup"><span data-stu-id="e5635-106">Create a new thread in the specified conversation.</span></span>

<span data-ttu-id="e5635-p102">按指定方式创建线程和帖子。使用 [回复线程](conversationthread-reply.md) 进一步发布到该线程。或者，如果你获得帖子 ID，还可以在该线程中 [回复](post-reply.md) 帖子。</span><span class="sxs-lookup"><span data-stu-id="e5635-p102">A thread and post are created as specified. Use [reply thread](conversationthread-reply.md) to further post to that thread. Or, if you get the post ID, you can also [reply](post-reply.md) to that post in that thread.</span></span>

<span data-ttu-id="e5635-110">注意：还可以 [通过首先创建一个线程启动一个新的对话](group-post-threads.md)</span><span class="sxs-lookup"><span data-stu-id="e5635-110">Note: You can also [start a new conversation by first creating a thread](group-post-threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e5635-111">权限</span><span class="sxs-lookup"><span data-stu-id="e5635-111">Permissions</span></span>
<span data-ttu-id="e5635-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e5635-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5635-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="e5635-114">Permission type</span></span>      | <span data-ttu-id="e5635-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e5635-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5635-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e5635-116">Delegated (work or school account)</span></span> | <span data-ttu-id="e5635-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5635-117">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e5635-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e5635-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5635-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="e5635-119">Not supported.</span></span>    |
|<span data-ttu-id="e5635-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="e5635-120">Application</span></span> | <span data-ttu-id="e5635-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5635-121">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e5635-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e5635-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="e5635-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="e5635-123">Request headers</span></span>
| <span data-ttu-id="e5635-124">名称</span><span class="sxs-lookup"><span data-stu-id="e5635-124">Name</span></span>       | <span data-ttu-id="e5635-125">类型</span><span class="sxs-lookup"><span data-stu-id="e5635-125">Type</span></span> | <span data-ttu-id="e5635-126">说明</span><span class="sxs-lookup"><span data-stu-id="e5635-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e5635-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5635-127">Authorization</span></span>  | <span data-ttu-id="e5635-128">string</span><span class="sxs-lookup"><span data-stu-id="e5635-128">string</span></span>  | <span data-ttu-id="e5635-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e5635-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e5635-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="e5635-131">Request body</span></span>
<span data-ttu-id="e5635-132">在请求正文中，提供 [ConversationThread](../resources/conversationthread.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e5635-132">In the request body, supply a JSON representation of [ConversationThread](../resources/conversationthread.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e5635-133">响应</span><span class="sxs-lookup"><span data-stu-id="e5635-133">Response</span></span>

<span data-ttu-id="e5635-134">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [ConversationThread](../resources/conversationthread.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e5635-134">If successful, this method returns `201 Created` response code and [ConversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5635-135">示例</span><span class="sxs-lookup"><span data-stu-id="e5635-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e5635-136">请求</span><span class="sxs-lookup"><span data-stu-id="e5635-136">Request</span></span>
<span data-ttu-id="e5635-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e5635-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_conversationthread_from_conversation"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/conversations/{id}/threads
Content-type: application/json

{
  "topic": "topic-value",
  "posts": [{
      "body": {
        "contentType": "html",
        "content": "this is body content"
      }
  }]
}
```
<span data-ttu-id="e5635-138">在请求正文中，提供 [ConversationThread](../resources/conversationthread.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e5635-138">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="e5635-139">响应</span><span class="sxs-lookup"><span data-stu-id="e5635-139">Response</span></span>

<span data-ttu-id="e5635-p105">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和新线程的 `id`。下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e5635-p105">If successful, this method returns `201 Created` response code and the `id` of the new thread in the response body. Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 346

{
  "id": "thread-id-value"
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
