---
title: 创建对话
description: '通过包括线程和帖子创建新对话。 '
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: d72280e295f69a03267a25138f2d6e44151695af
ms.sourcegitcommit: 258974d689cb8f04ff542ec8bc5fe5793da5cc05
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/08/2020
ms.locfileid: "48385798"
---
# <a name="create-conversation"></a><span data-ttu-id="112ac-103">创建对话</span><span class="sxs-lookup"><span data-stu-id="112ac-103">Create conversation</span></span>

<span data-ttu-id="112ac-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="112ac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="112ac-105">通过添加线程和帖子来新建[对话](../resources/conversation.md)。</span><span class="sxs-lookup"><span data-stu-id="112ac-105">Create a new [conversation](../resources/conversation.md) by including a thread and a post.</span></span> 

<span data-ttu-id="112ac-106">使用[回复线程](conversationthread-reply.md)或[回复帖子](post-reply.md)进一步发布到该对话。</span><span class="sxs-lookup"><span data-stu-id="112ac-106">Use [reply thread](conversationthread-reply.md) or [reply post](post-reply.md) to further post to that conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="112ac-107">权限</span><span class="sxs-lookup"><span data-stu-id="112ac-107">Permissions</span></span>
<span data-ttu-id="112ac-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="112ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="112ac-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="112ac-110">Permission type</span></span>      | <span data-ttu-id="112ac-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="112ac-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="112ac-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="112ac-112">Delegated (work or school account)</span></span> | <span data-ttu-id="112ac-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="112ac-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="112ac-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="112ac-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="112ac-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="112ac-115">Not supported.</span></span>    |
|<span data-ttu-id="112ac-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="112ac-116">Application</span></span> | <span data-ttu-id="112ac-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="112ac-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="112ac-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="112ac-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations
```

## <a name="request-headers"></a><span data-ttu-id="112ac-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="112ac-119">Request headers</span></span>
| <span data-ttu-id="112ac-120">标头</span><span class="sxs-lookup"><span data-stu-id="112ac-120">Header</span></span>       | <span data-ttu-id="112ac-121">值</span><span class="sxs-lookup"><span data-stu-id="112ac-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="112ac-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="112ac-122">Authorization</span></span>  | <span data-ttu-id="112ac-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="112ac-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="112ac-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="112ac-125">Content-Type</span></span>  | <span data-ttu-id="112ac-126">application/json</span><span class="sxs-lookup"><span data-stu-id="112ac-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="112ac-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="112ac-127">Request body</span></span>
<span data-ttu-id="112ac-128">在请求正文中，提供包括 [conversationThread](../resources/conversationthread.md) 和 [帖子](../resources/post.md) 的 [conversation](../resources/conversation.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="112ac-128">In the request body, supply a JSON representation of [conversation](../resources/conversation.md) object containing a [conversationThread](../resources/conversationthread.md) and a [post](../resources/post.md).</span></span>

## <a name="response"></a><span data-ttu-id="112ac-129">响应</span><span class="sxs-lookup"><span data-stu-id="112ac-129">Response</span></span>
<span data-ttu-id="112ac-130">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [conversation](../resources/conversation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="112ac-130">If successful, this method returns `201 Created` response code and [conversation](../resources/conversation.md) object in the response body.</span></span> 

<span data-ttu-id="112ac-131">响应包括新对话和线程的 ID，这些 ID 也可用于[列出帖子](conversationthread-list-posts.md)操作，从而获取新帖子。</span><span class="sxs-lookup"><span data-stu-id="112ac-131">The response includes the IDs for the new conversation and thread, which you can use in the [list posts](conversationthread-list-posts.md) operation to get the new post as well.</span></span>

## <a name="example"></a><span data-ttu-id="112ac-132">示例</span><span class="sxs-lookup"><span data-stu-id="112ac-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="112ac-133">请求</span><span class="sxs-lookup"><span data-stu-id="112ac-133">Request</span></span>
<span data-ttu-id="112ac-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="112ac-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "create_conversation_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups/29981b6a-0e57-42dc-94c9-cd24f5306196/conversations
Content-type: application/json

{
  "topic":"New head count",
  "threads":[
    {
      "posts":[
        {
          "body":{
            "contentType":"html",
            "content":"The confirmation will come by the end of the week."
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

#### <a name="response"></a><span data-ttu-id="112ac-135">响应</span><span class="sxs-lookup"><span data-stu-id="112ac-135">Response</span></span>
<span data-ttu-id="112ac-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="112ac-136">The following is an example of the response.</span></span>
><span data-ttu-id="112ac-137">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="112ac-137">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="112ac-138">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="112ac-138">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups('29981b6a-0e57-42dc-94c9-cd24f5306196')/conversations/$entity",
  "id":"AAQkADPxBgqECsrFDTuM=",
  "threads@odata.context":"https://graph.microsoft.com/beta/$metadata#groups('29981b6a-0e57-42dc-94c9-cd24f5306196')/conversations('AAQkADPxBgqECsrFDTuM%3D')/threads",
  "threads":[
    {
      "id":"AAQkADUNO4xAAMbGA93Sw-EGCoQKysUNO4w=="
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


