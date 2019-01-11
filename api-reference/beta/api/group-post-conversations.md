---
title: 创建对话
description: '通过包括线程和帖子来创建新会话。 '
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 8fe80c3a7d226aaa2bfa3e4834623a84aa91a940
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870096"
---
# <a name="create-conversation"></a><span data-ttu-id="486ad-103">创建对话</span><span class="sxs-lookup"><span data-stu-id="486ad-103">Create conversation</span></span>

> <span data-ttu-id="486ad-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="486ad-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="486ad-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="486ad-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="486ad-106">通过添加线程和帖子来新建[对话](../resources/conversation.md)。</span><span class="sxs-lookup"><span data-stu-id="486ad-106">Create a new [conversation](../resources/conversation.md) by including a thread and a post.</span></span> 

<span data-ttu-id="486ad-107">使用[回复线程](conversationthread-reply.md)或[回复帖子](post-reply.md)进一步发布到该对话。</span><span class="sxs-lookup"><span data-stu-id="486ad-107">Use [reply thread](conversationthread-reply.md) or [reply post](post-reply.md) to further post to that conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="486ad-108">权限</span><span class="sxs-lookup"><span data-stu-id="486ad-108">Permissions</span></span>
<span data-ttu-id="486ad-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="486ad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="486ad-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="486ad-111">Permission type</span></span>      | <span data-ttu-id="486ad-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="486ad-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="486ad-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="486ad-113">Delegated (work or school account)</span></span> | <span data-ttu-id="486ad-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="486ad-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="486ad-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="486ad-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="486ad-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="486ad-116">Not supported.</span></span>    |
|<span data-ttu-id="486ad-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="486ad-117">Application</span></span> | <span data-ttu-id="486ad-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="486ad-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="486ad-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="486ad-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations
```

## <a name="request-headers"></a><span data-ttu-id="486ad-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="486ad-120">Request headers</span></span>
| <span data-ttu-id="486ad-121">标头</span><span class="sxs-lookup"><span data-stu-id="486ad-121">Header</span></span>       | <span data-ttu-id="486ad-122">值</span><span class="sxs-lookup"><span data-stu-id="486ad-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="486ad-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="486ad-123">Authorization</span></span>  | <span data-ttu-id="486ad-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="486ad-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="486ad-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="486ad-126">Content-Type</span></span>  | <span data-ttu-id="486ad-127">application/json</span><span class="sxs-lookup"><span data-stu-id="486ad-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="486ad-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="486ad-128">Request body</span></span>
<span data-ttu-id="486ad-129">在请求正文中，提供包括 [conversationThread](../resources/conversationthread.md) 和 [帖子](../resources/post.md) 的 [conversation](../resources/conversation.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="486ad-129">In the request body, supply a JSON representation of [conversation](../resources/conversation.md) object containing a [conversationThread](../resources/conversationthread.md) and a [post](../resources/post.md).</span></span>

## <a name="response"></a><span data-ttu-id="486ad-130">响应</span><span class="sxs-lookup"><span data-stu-id="486ad-130">Response</span></span>
<span data-ttu-id="486ad-131">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [conversation](../resources/conversation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="486ad-131">If successful, this method returns `201 Created` response code and [conversation](../resources/conversation.md) object in the response body.</span></span> 

<span data-ttu-id="486ad-132">响应包括新对话和线程的 ID，这些 ID 也可用于[列出帖子](conversationthread-list-posts.md)操作，从而获取新帖子。</span><span class="sxs-lookup"><span data-stu-id="486ad-132">The response includes the IDs for the new conversation and thread, which you can use in the [list posts](conversationthread-list-posts.md) operation to get the new post as well.</span></span>

## <a name="example"></a><span data-ttu-id="486ad-133">示例</span><span class="sxs-lookup"><span data-stu-id="486ad-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="486ad-134">请求</span><span class="sxs-lookup"><span data-stu-id="486ad-134">Request</span></span>
<span data-ttu-id="486ad-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="486ad-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_conversation_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups('29981b6a-0e57-42dc-94c9-cd24f5306196')/conversations
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

#### <a name="response"></a><span data-ttu-id="486ad-136">响应</span><span class="sxs-lookup"><span data-stu-id="486ad-136">Response</span></span>
<span data-ttu-id="486ad-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="486ad-137">The following is an example of the response.</span></span>
><span data-ttu-id="486ad-138">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="486ad-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="486ad-139">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="486ad-139">All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create Conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
