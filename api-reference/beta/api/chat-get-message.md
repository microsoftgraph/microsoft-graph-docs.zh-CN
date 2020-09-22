---
title: 获取 chatMessage
description: 在聊天中检索一条消息。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0598a5cea110cbc7ba4ee1d1a2b6ff6e496c53e3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47982726"
---
# <a name="get-chatmessage"></a><span data-ttu-id="622fc-103">获取 chatMessage</span><span class="sxs-lookup"><span data-stu-id="622fc-103">Get chatMessage</span></span>

<span data-ttu-id="622fc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="622fc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="622fc-105">在[聊天](../resources/chat.md)中检索一条[消息](../resources/chatmessage.md)。</span><span class="sxs-lookup"><span data-stu-id="622fc-105">Retrieve a single [message](../resources/chatmessage.md) in a [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="622fc-106">权限</span><span class="sxs-lookup"><span data-stu-id="622fc-106">Permissions</span></span>

<span data-ttu-id="622fc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="622fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="622fc-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="622fc-109">Permission type</span></span>      | <span data-ttu-id="622fc-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="622fc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="622fc-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="622fc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="622fc-112">Chat.Read、Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="622fc-112">Chat.Read, Chat.ReadWrite</span></span> |
|<span data-ttu-id="622fc-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="622fc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="622fc-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="622fc-114">Not supported.</span></span>    |
|<span data-ttu-id="622fc-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="622fc-115">Application</span></span> | <span data-ttu-id="622fc-116">Chat.Read.All、Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="622fc-116">Chat.Read.All, Chat.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="622fc-117">在使用应用程序权限调用此 API 之前，你必须先请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="622fc-117">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="622fc-118">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="622fc-118">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="622fc-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="622fc-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/chats/{id}/messages/{id}
GET /users/{id}/chats/{id}/messages/{id}
GET /chats/{id}/messages/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="622fc-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="622fc-120">Optional query parameters</span></span>

<span data-ttu-id="622fc-121">此操作当前不支持使用 [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="622fc-121">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="622fc-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="622fc-122">Request headers</span></span>
| <span data-ttu-id="622fc-123">标头</span><span class="sxs-lookup"><span data-stu-id="622fc-123">Header</span></span>       | <span data-ttu-id="622fc-124">值</span><span class="sxs-lookup"><span data-stu-id="622fc-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="622fc-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="622fc-125">Authorization</span></span>  | <span data-ttu-id="622fc-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="622fc-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="622fc-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="622fc-128">Request body</span></span>
<span data-ttu-id="622fc-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="622fc-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="622fc-130">响应</span><span class="sxs-lookup"><span data-stu-id="622fc-130">Response</span></span>

<span data-ttu-id="622fc-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [chatmessage](../resources/chatmessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="622fc-131">If successful, this method returns a `200 OK` response code and a [chatmessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="622fc-132">示例</span><span class="sxs-lookup"><span data-stu-id="622fc-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="622fc-133">请求</span><span class="sxs-lookup"><span data-stu-id="622fc-133">Request</span></span>
<span data-ttu-id="622fc-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="622fc-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="622fc-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="622fc-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chat_message"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/chats/{id}/messages/{id}
```
# <a name="c"></a>[<span data-ttu-id="622fc-136">C#</span><span class="sxs-lookup"><span data-stu-id="622fc-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chat-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="622fc-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="622fc-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chat-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="622fc-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="622fc-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chat-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="622fc-139">响应</span><span class="sxs-lookup"><span data-stu-id="622fc-139">Response</span></span>
<span data-ttu-id="622fc-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="622fc-140">Here is an example of the response.</span></span> 

><span data-ttu-id="622fc-141">**注意：** 为提高可读性，缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="622fc-141">**Note:** The response object shown here is shortened for readability.</span></span> <span data-ttu-id="622fc-142">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="622fc-142">All the properties will be returned from an actual call.</span></span>
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
  "description": "Get chatMessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


