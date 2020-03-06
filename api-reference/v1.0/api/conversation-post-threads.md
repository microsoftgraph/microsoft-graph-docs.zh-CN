---
title: 创建线程
description: '在指定会话中创建新线程。 '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 58ae743f26d729a2b18fbfaa5bf0bbc0dcf48d70
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518194"
---
# <a name="create-thread"></a><span data-ttu-id="c91b2-103">创建线程</span><span class="sxs-lookup"><span data-stu-id="c91b2-103">Create thread</span></span>

<span data-ttu-id="c91b2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c91b2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c91b2-105">在指定会话中创建新线程。</span><span class="sxs-lookup"><span data-stu-id="c91b2-105">Create a new thread in the specified conversation.</span></span> 

<span data-ttu-id="c91b2-p101">按指定方式创建线程和帖子。使用 [回复线程](conversationthread-reply.md) 进一步发布到该线程。或者，如果你获得帖子 ID，还可以在该线程中 [回复](post-reply.md) 帖子。</span><span class="sxs-lookup"><span data-stu-id="c91b2-p101">A thread and post are created as specified. Use [reply thread](conversationthread-reply.md) to further post to that thread. Or, if you get the post ID, you can also [reply](post-reply.md) to that post in that thread.</span></span>

<span data-ttu-id="c91b2-109">注意：还可以 [通过首先创建一个线程启动一个新的对话](group-post-threads.md)</span><span class="sxs-lookup"><span data-stu-id="c91b2-109">Note: You can also [start a new conversation by first creating a thread](group-post-threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c91b2-110">权限</span><span class="sxs-lookup"><span data-stu-id="c91b2-110">Permissions</span></span>
<span data-ttu-id="c91b2-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c91b2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c91b2-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="c91b2-113">Permission type</span></span>      | <span data-ttu-id="c91b2-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c91b2-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c91b2-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c91b2-115">Delegated (work or school account)</span></span> | <span data-ttu-id="c91b2-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c91b2-116">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c91b2-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c91b2-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c91b2-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c91b2-118">Not supported.</span></span>    |
|<span data-ttu-id="c91b2-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="c91b2-119">Application</span></span> | <span data-ttu-id="c91b2-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="c91b2-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c91b2-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c91b2-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="c91b2-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="c91b2-122">Request headers</span></span>
| <span data-ttu-id="c91b2-123">名称</span><span class="sxs-lookup"><span data-stu-id="c91b2-123">Name</span></span>       | <span data-ttu-id="c91b2-124">类型</span><span class="sxs-lookup"><span data-stu-id="c91b2-124">Type</span></span> | <span data-ttu-id="c91b2-125">说明</span><span class="sxs-lookup"><span data-stu-id="c91b2-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c91b2-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="c91b2-126">Authorization</span></span>  | <span data-ttu-id="c91b2-127">string</span><span class="sxs-lookup"><span data-stu-id="c91b2-127">string</span></span>  | <span data-ttu-id="c91b2-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c91b2-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c91b2-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="c91b2-130">Request body</span></span>
<span data-ttu-id="c91b2-131">在请求正文中，提供 [ConversationThread](../resources/conversationthread.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c91b2-131">In the request body, supply a JSON representation of [ConversationThread](../resources/conversationthread.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c91b2-132">响应</span><span class="sxs-lookup"><span data-stu-id="c91b2-132">Response</span></span>

<span data-ttu-id="c91b2-133">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [ConversationThread](../resources/conversationthread.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c91b2-133">If successful, this method returns `201 Created` response code and [ConversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c91b2-134">示例</span><span class="sxs-lookup"><span data-stu-id="c91b2-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c91b2-135">请求</span><span class="sxs-lookup"><span data-stu-id="c91b2-135">Request</span></span>
<span data-ttu-id="c91b2-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c91b2-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c91b2-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="c91b2-137">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c91b2-138">C#</span><span class="sxs-lookup"><span data-stu-id="c91b2-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversationthread-from-conversation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c91b2-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c91b2-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversationthread-from-conversation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c91b2-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c91b2-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversationthread-from-conversation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c91b2-141">Java</span><span class="sxs-lookup"><span data-stu-id="c91b2-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conversationthread-from-conversation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="c91b2-142">在请求正文中，提供 [ConversationThread](../resources/conversationthread.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c91b2-142">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="c91b2-143">响应</span><span class="sxs-lookup"><span data-stu-id="c91b2-143">Response</span></span>

<span data-ttu-id="c91b2-p104">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和新线程的 `id`。下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c91b2-p104">If successful, this method returns `201 Created` response code and the `id` of the new thread in the response body. Here is an example of the response.</span></span> 
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
