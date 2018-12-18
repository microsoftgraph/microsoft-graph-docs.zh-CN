---
title: 创建线程
description: '在指定会话中创建新线程。 '
author: dkershaw10
ms.openlocfilehash: e2c93e0c2a677afa584d0442ff1545f1926c7ec8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304912"
---
# <a name="create-thread"></a><span data-ttu-id="e3a7e-103">创建线程</span><span class="sxs-lookup"><span data-stu-id="e3a7e-103">Create thread</span></span>

<span data-ttu-id="e3a7e-104">在指定会话中创建新线程。</span><span class="sxs-lookup"><span data-stu-id="e3a7e-104">Create a new thread in the specified conversation.</span></span> 

<span data-ttu-id="e3a7e-p101">按指定方式创建线程和帖子。使用 [回复线程](conversationthread-reply.md) 进一步发布到该线程。或者，如果你获得帖子 ID，还可以在该线程中 [回复](post-reply.md) 帖子。</span><span class="sxs-lookup"><span data-stu-id="e3a7e-p101">A thread and post are created as specified. Use [reply thread](conversationthread-reply.md) to further post to that thread. Or, if you get the post ID, you can also [reply](post-reply.md) to that post in that thread.</span></span>

<span data-ttu-id="e3a7e-108">注意：还可以 [通过首先创建一个线程启动一个新的对话](group-post-threads.md)</span><span class="sxs-lookup"><span data-stu-id="e3a7e-108">Note: You can also [start a new conversation by first creating a thread](group-post-threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e3a7e-109">权限</span><span class="sxs-lookup"><span data-stu-id="e3a7e-109">Permissions</span></span>
<span data-ttu-id="e3a7e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e3a7e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3a7e-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="e3a7e-112">Permission type</span></span>      | <span data-ttu-id="e3a7e-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e3a7e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3a7e-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e3a7e-114">Delegated (work or school account)</span></span> | <span data-ttu-id="e3a7e-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3a7e-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e3a7e-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e3a7e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3a7e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e3a7e-117">Not supported.</span></span>    |
|<span data-ttu-id="e3a7e-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="e3a7e-118">Application</span></span> | <span data-ttu-id="e3a7e-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3a7e-119">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e3a7e-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e3a7e-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="e3a7e-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="e3a7e-121">Request headers</span></span>
| <span data-ttu-id="e3a7e-122">Name</span><span class="sxs-lookup"><span data-stu-id="e3a7e-122">Name</span></span>       | <span data-ttu-id="e3a7e-123">类型</span><span class="sxs-lookup"><span data-stu-id="e3a7e-123">Type</span></span> | <span data-ttu-id="e3a7e-124">说明</span><span class="sxs-lookup"><span data-stu-id="e3a7e-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e3a7e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3a7e-125">Authorization</span></span>  | <span data-ttu-id="e3a7e-126">string</span><span class="sxs-lookup"><span data-stu-id="e3a7e-126">string</span></span>  | <span data-ttu-id="e3a7e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e3a7e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e3a7e-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="e3a7e-129">Request body</span></span>
<span data-ttu-id="e3a7e-130">在请求正文中，提供 [ConversationThread](../resources/conversationthread.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e3a7e-130">In the request body, supply a JSON representation of [ConversationThread](../resources/conversationthread.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e3a7e-131">响应</span><span class="sxs-lookup"><span data-stu-id="e3a7e-131">Response</span></span>

<span data-ttu-id="e3a7e-132">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [ConversationThread](../resources/conversationthread.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e3a7e-132">If successful, this method returns `201 Created` response code and [ConversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3a7e-133">示例</span><span class="sxs-lookup"><span data-stu-id="e3a7e-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e3a7e-134">请求</span><span class="sxs-lookup"><span data-stu-id="e3a7e-134">Request</span></span>
<span data-ttu-id="e3a7e-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e3a7e-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_conversationthread_from_conversation"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/conversations/{id}/threads
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
<span data-ttu-id="e3a7e-136">在请求正文中，提供 [ConversationThread](../resources/conversationthread.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e3a7e-136">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="e3a7e-137">响应</span><span class="sxs-lookup"><span data-stu-id="e3a7e-137">Response</span></span>

<span data-ttu-id="e3a7e-p104">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和新线程的 `id`。下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e3a7e-p104">If successful, this method returns `201 Created` response code and the `id` of the new thread in the response body. Here is an example of the response.</span></span> 
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
