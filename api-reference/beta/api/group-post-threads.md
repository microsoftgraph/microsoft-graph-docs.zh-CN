---
title: 创建对话线程
description: '首先，通过创建线程来启动新的组对话。 '
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 06dfeaa50fc10907d71684602df40aaf2cbda428
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52681286"
---
# <a name="create-conversation-thread"></a><span data-ttu-id="a396e-103">创建对话线程</span><span class="sxs-lookup"><span data-stu-id="a396e-103">Create conversation thread</span></span>

<span data-ttu-id="a396e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a396e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a396e-105">首先，通过创建线程来启动新的组对话。</span><span class="sxs-lookup"><span data-stu-id="a396e-105">Start a new group conversation by first creating a thread.</span></span> 

<span data-ttu-id="a396e-p101">创建新会话、会话线程，然后可在组中创建帖子。使用 [回复线程](conversationthread-reply.md) 或 [回复帖子](post-reply.md) 进一步发布到该线程。</span><span class="sxs-lookup"><span data-stu-id="a396e-p101">A new conversation, conversation thread, and post are created in the group. Use [reply thread](conversationthread-reply.md) or [reply post](post-reply.md) to further post to that thread.</span></span>

<span data-ttu-id="a396e-108">注意：你还可以 [在现有会话中启动新线程](conversation-post-threads.md)。</span><span class="sxs-lookup"><span data-stu-id="a396e-108">Note: You can also [start a new thread in an existing conversation](conversation-post-threads.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="a396e-109">权限</span><span class="sxs-lookup"><span data-stu-id="a396e-109">Permissions</span></span>
<span data-ttu-id="a396e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a396e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a396e-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="a396e-112">Permission type</span></span>      | <span data-ttu-id="a396e-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a396e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a396e-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a396e-114">Delegated (work or school account)</span></span> | <span data-ttu-id="a396e-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a396e-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a396e-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a396e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a396e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a396e-117">Not supported.</span></span>    |
|<span data-ttu-id="a396e-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="a396e-118">Application</span></span> | <span data-ttu-id="a396e-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="a396e-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a396e-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a396e-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="a396e-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="a396e-121">Request headers</span></span>
| <span data-ttu-id="a396e-122">标头</span><span class="sxs-lookup"><span data-stu-id="a396e-122">Header</span></span>       | <span data-ttu-id="a396e-123">值</span><span class="sxs-lookup"><span data-stu-id="a396e-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a396e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a396e-124">Authorization</span></span>  | <span data-ttu-id="a396e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a396e-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a396e-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a396e-127">Content-Type</span></span>  | <span data-ttu-id="a396e-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a396e-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a396e-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="a396e-129">Request body</span></span>
<span data-ttu-id="a396e-130">在请求正文中，提供代表包括 [帖子](../resources/post.md) 的 [conversationThread](../resources/conversationthread.md) 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a396e-130">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object containing a [post](../resources/post.md).</span></span>

## <a name="response"></a><span data-ttu-id="a396e-131">响应</span><span class="sxs-lookup"><span data-stu-id="a396e-131">Response</span></span>
<span data-ttu-id="a396e-132">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [conversationThread](../resources/conversationthread.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a396e-132">If successful, this method returns `201 Created` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a396e-133">示例</span><span class="sxs-lookup"><span data-stu-id="a396e-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a396e-134">请求</span><span class="sxs-lookup"><span data-stu-id="a396e-134">Request</span></span>
<span data-ttu-id="a396e-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a396e-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a396e-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="a396e-136">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a396e-137">C#</span><span class="sxs-lookup"><span data-stu-id="a396e-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversationthread-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a396e-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a396e-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversationthread-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a396e-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a396e-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversationthread-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a396e-140">Java</span><span class="sxs-lookup"><span data-stu-id="a396e-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conversationthread-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a396e-141">响应</span><span class="sxs-lookup"><span data-stu-id="a396e-141">Response</span></span>
<span data-ttu-id="a396e-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a396e-142">The following is an example of the response.</span></span>
><span data-ttu-id="a396e-143">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a396e-143">**Note:** The response object shown here might be shortened for readability.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


