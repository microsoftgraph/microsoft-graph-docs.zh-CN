---
title: 创建对话
description: '通过包括线程和帖子创建新对话。 '
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: a91b88067384962f98154448b0eadcef6a6cb44f
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680582"
---
# <a name="create-conversation"></a><span data-ttu-id="9cc02-103">创建对话</span><span class="sxs-lookup"><span data-stu-id="9cc02-103">Create conversation</span></span>

<span data-ttu-id="9cc02-104">命名空间：microsoft.graph 通过包含线程 [和](../resources/conversation.md) 帖子创建新对话。</span><span class="sxs-lookup"><span data-stu-id="9cc02-104">Namespace: microsoft.graph Create a new [conversation](../resources/conversation.md) by including a thread and a post.</span></span> 

<span data-ttu-id="9cc02-105">使用[回复线程](conversationthread-reply.md)或[回复帖子](post-reply.md)进一步发布到该对话。</span><span class="sxs-lookup"><span data-stu-id="9cc02-105">Use [reply thread](conversationthread-reply.md) or [reply post](post-reply.md) to further post to that conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="9cc02-106">权限</span><span class="sxs-lookup"><span data-stu-id="9cc02-106">Permissions</span></span>
<span data-ttu-id="9cc02-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9cc02-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9cc02-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9cc02-109">Permission type</span></span>      | <span data-ttu-id="9cc02-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9cc02-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9cc02-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9cc02-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9cc02-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cc02-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9cc02-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9cc02-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9cc02-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9cc02-114">Not supported.</span></span>    |
|<span data-ttu-id="9cc02-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9cc02-115">Application</span></span> | <span data-ttu-id="9cc02-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9cc02-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9cc02-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9cc02-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations
```

## <a name="request-headers"></a><span data-ttu-id="9cc02-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="9cc02-118">Request headers</span></span>
| <span data-ttu-id="9cc02-119">标头</span><span class="sxs-lookup"><span data-stu-id="9cc02-119">Header</span></span>       | <span data-ttu-id="9cc02-120">值</span><span class="sxs-lookup"><span data-stu-id="9cc02-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9cc02-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9cc02-121">Authorization</span></span>  | <span data-ttu-id="9cc02-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9cc02-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9cc02-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9cc02-124">Content-Type</span></span>  | <span data-ttu-id="9cc02-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9cc02-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9cc02-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9cc02-126">Request body</span></span>
<span data-ttu-id="9cc02-127">在请求正文中，提供包括 [conversationThread](../resources/conversationthread.md) 和 [帖子](../resources/post.md) 的 [conversation](../resources/conversation.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9cc02-127">In the request body, supply a JSON representation of [conversation](../resources/conversation.md) object containing a [conversationThread](../resources/conversationthread.md) and a [post](../resources/post.md).</span></span>

## <a name="response"></a><span data-ttu-id="9cc02-128">响应</span><span class="sxs-lookup"><span data-stu-id="9cc02-128">Response</span></span>
<span data-ttu-id="9cc02-129">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [conversation](../resources/conversation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9cc02-129">If successful, this method returns `201 Created` response code and [conversation](../resources/conversation.md) object in the response body.</span></span>

<span data-ttu-id="9cc02-130">响应包括新对话和线程的 ID，这些 ID 也可用于[列出帖子](conversationthread-list-posts.md)操作，从而获取新帖子。</span><span class="sxs-lookup"><span data-stu-id="9cc02-130">The response includes the IDs for the new conversation and thread, which you can use in the [list posts](conversationthread-list-posts.md) operation to get the new post as well.</span></span>

## <a name="example"></a><span data-ttu-id="9cc02-131">示例</span><span class="sxs-lookup"><span data-stu-id="9cc02-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="9cc02-132">请求</span><span class="sxs-lookup"><span data-stu-id="9cc02-132">Request</span></span>
<span data-ttu-id="9cc02-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9cc02-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9cc02-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="9cc02-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["29981b6a-0e57-42dc-94c9-cd24f5306196"],
  "name": "create_conversation_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/29981b6a-0e57-42dc-94c9-cd24f5306196/conversations
Content-type: application/json

{
  "topic":"New locations for this quarter",
  "threads":[
    {
      "posts":[
        {
          "body":{
            "contentType":"html",
            "content":"What do we know so far?"
          },
          "newParticipants":[
            {
              "emailAddress":{
                "name":"Adele Vance",
                "address":"AdeleV@contoso.onmicrosoft.com"
              }
            }
          ]
        }
      ]
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="9cc02-135">C#</span><span class="sxs-lookup"><span data-stu-id="9cc02-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversation-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9cc02-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9cc02-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversation-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9cc02-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9cc02-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversation-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9cc02-138">Java</span><span class="sxs-lookup"><span data-stu-id="9cc02-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conversation-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9cc02-139">响应</span><span class="sxs-lookup"><span data-stu-id="9cc02-139">Response</span></span>
<span data-ttu-id="9cc02-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9cc02-140">The following is an example of the response.</span></span>
><span data-ttu-id="9cc02-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9cc02-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups('29981b6a-0e57-42dc-94c9-cd24f5306196')/conversations/$entity",
  "id":"AAQkADDVKtMlRp4Txc6k=",
  "threads@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups('29981b6a-0e57-42dc-94c9-cd24f5306196')/conversations('AAQkADDVKtMlRp4Txc6k%3D')/threads",
  "threads":[
    {
      "id":"AAQkADQDarUNUq0yVGnhPFzqQ=="
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

