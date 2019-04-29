---
title: 获取聊天消息
description: 在聊天中检索一条消息。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 02c31f7df35821e7706cabe3852ae5f441edf15a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33327591"
---
# <a name="get-chat-message"></a><span data-ttu-id="ad1d9-103">获取聊天消息</span><span class="sxs-lookup"><span data-stu-id="ad1d9-103">Get chat message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad1d9-104">在[聊天](../resources/chat.md)中检索一条[消息](../resources/chatmessage.md)。</span><span class="sxs-lookup"><span data-stu-id="ad1d9-104">Retrieve a single [message](../resources/chatmessage.md) in a [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ad1d9-105">权限</span><span class="sxs-lookup"><span data-stu-id="ad1d9-105">Permissions</span></span>

<span data-ttu-id="ad1d9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ad1d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad1d9-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ad1d9-108">Permission type</span></span>      | <span data-ttu-id="ad1d9-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ad1d9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad1d9-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ad1d9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ad1d9-111">Chat.Read</span><span class="sxs-lookup"><span data-stu-id="ad1d9-111">Chat.Read</span></span>   |
|<span data-ttu-id="ad1d9-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ad1d9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad1d9-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="ad1d9-113">Not supported.</span></span>    |
|<span data-ttu-id="ad1d9-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ad1d9-114">Application</span></span> | <span data-ttu-id="ad1d9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ad1d9-115">Not supported.</span></span>   |

## <a name="http-request"></a><span data-ttu-id="ad1d9-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ad1d9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/chats/{id}/messages/{id}
GET /users/{id}/chats/{id}/messages/{id}
GET /chats/{id}/messages/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ad1d9-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ad1d9-117">Optional query parameters</span></span>

<span data-ttu-id="ad1d9-118">此操作当前不支持使用 [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ad1d9-118">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ad1d9-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ad1d9-119">Request headers</span></span>
| <span data-ttu-id="ad1d9-120">标头</span><span class="sxs-lookup"><span data-stu-id="ad1d9-120">Header</span></span>       | <span data-ttu-id="ad1d9-121">值</span><span class="sxs-lookup"><span data-stu-id="ad1d9-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ad1d9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad1d9-122">Authorization</span></span>  | <span data-ttu-id="ad1d9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ad1d9-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ad1d9-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="ad1d9-125">Request body</span></span>
<span data-ttu-id="ad1d9-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ad1d9-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad1d9-127">响应</span><span class="sxs-lookup"><span data-stu-id="ad1d9-127">Response</span></span>

<span data-ttu-id="ad1d9-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [chatmessage](../resources/chatmessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ad1d9-128">If successful, this method returns a `200 OK` response code and a [team](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad1d9-129">示例</span><span class="sxs-lookup"><span data-stu-id="ad1d9-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ad1d9-130">请求</span><span class="sxs-lookup"><span data-stu-id="ad1d9-130">Request</span></span>
<span data-ttu-id="ad1d9-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ad1d9-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_chat_message"
}-->
```http
GET https://graph.microsoft.com/beta/me/chats/{id}/messages/{id}
```

##### <a name="response"></a><span data-ttu-id="ad1d9-132">响应</span><span class="sxs-lookup"><span data-stu-id="ad1d9-132">Response</span></span>
<span data-ttu-id="ad1d9-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ad1d9-133">Here is an example of the response.</span></span> 

><span data-ttu-id="ad1d9-134">**注意：** 为提高可读性，缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ad1d9-134">**Note:** The response object shown here are shortened for readability.</span></span> <span data-ttu-id="ad1d9-135">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ad1d9-135">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('8b081ef6-4792-4def-b2c9-c363a1bf41d5')/chats('19%3A8b081ef6-4792-4def-b2c9-c363a1bf41d5_877192bd-9183-47d3-a74c-8aa0426716cf%40unq.gbl.spaces')/messages/$entity",
    "id": "1555631722147",
    "replyToId": null,
    "etag": "1555631722147",
    "messageType": "message",
    "createdDateTime": "2019-04-18T23:55:22.147Z",
    "lastModifiedDateTime": null,
    "deletedDateTime": null,
    "subject": null,
    "summary": null,
    "importance": "normal",
    "locale": "en-us",
    "policyViolation": null,
    "from": {
        "device": null,
        "user": null,
        "conversation": null,
        "application": {
            "id": "877192bd-9183-47d3-a74c-8aa0426716cf",
            "displayName": "TestBot",
            "applicationIdentityType": "bot"
        }
    },
    "body": {
        "contentType": "html",
        "content": "<attachment id=\"bcb243ec589a4537b3c650356421e696\"></attachment>"
    },
    "attachments": [
        {
            "id": "bcb243ec589a4537b3c650356421e696",
            "contentType": "application/vnd.microsoft.card.signin",
            "contentUrl": null,
            "content": "{\r\n  \"text\": \"Please sign in to sample to proceed.\",\r\n  \"buttons\": [\r\n    {\r\n      \"type\": \"signin\",\r\n      \"title\": \"Sign In\",\r\n      \"value\": \"https://token.botframework.com/api/oauth/signin?signin=921d46120f7695632ce6ca4b0da2e3ae15fea54c47\"\r\n    }\r\n  ]\r\n}",
            "name": null,
            "thumbnailUrl": null
        }
    ],
    "mentions": [],
    "reactions": []
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get chat message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
