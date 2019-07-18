---
title: 获取了 chatmessage
description: 在聊天中检索一条消息。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: c4f59c4f881f971a514b4922e572619a5d9a757b
ms.sourcegitcommit: 9cee9d8229fc84dd7ef97670ff27c145e1a78408
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/18/2019
ms.locfileid: "35778388"
---
# <a name="get-chatmessage"></a><span data-ttu-id="b4bb3-103">获取了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="b4bb3-103">Get chatMessage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4bb3-104">在[聊天](../resources/chat.md)中检索一条[消息](../resources/chatmessage.md)。</span><span class="sxs-lookup"><span data-stu-id="b4bb3-104">Retrieve a single [message](../resources/chatmessage.md) in a [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b4bb3-105">权限</span><span class="sxs-lookup"><span data-stu-id="b4bb3-105">Permissions</span></span>

<span data-ttu-id="b4bb3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b4bb3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4bb3-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b4bb3-108">Permission type</span></span>      | <span data-ttu-id="b4bb3-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b4bb3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b4bb3-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b4bb3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b4bb3-111">聊天、阅读和读写</span><span class="sxs-lookup"><span data-stu-id="b4bb3-111">Chat.Read, Chat.ReadWrite</span></span>   |
|<span data-ttu-id="b4bb3-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b4bb3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4bb3-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="b4bb3-113">Not supported.</span></span>    |
|<span data-ttu-id="b4bb3-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="b4bb3-114">Application</span></span> | <span data-ttu-id="b4bb3-115">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="b4bb3-115">Chat.Read.All</span></span>   |

> [!NOTE]
> <span data-ttu-id="b4bb3-116">在使用应用程序权限调用此 API 之前, 您必须请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="b4bb3-116">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="b4bb3-117">有关详细信息, 请参阅[Microsoft 团队中的受保护 api](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="b4bb3-117">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="b4bb3-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b4bb3-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/chats/{id}/messages/{id}
GET /users/{id}/chats/{id}/messages/{id}
GET /chats/{id}/messages/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b4bb3-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b4bb3-119">Optional query parameters</span></span>

<span data-ttu-id="b4bb3-120">此操作当前不支持使用 [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b4bb3-120">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b4bb3-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="b4bb3-121">Request headers</span></span>
| <span data-ttu-id="b4bb3-122">标头</span><span class="sxs-lookup"><span data-stu-id="b4bb3-122">Header</span></span>       | <span data-ttu-id="b4bb3-123">值</span><span class="sxs-lookup"><span data-stu-id="b4bb3-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b4bb3-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4bb3-124">Authorization</span></span>  | <span data-ttu-id="b4bb3-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b4bb3-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b4bb3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b4bb3-127">Request body</span></span>
<span data-ttu-id="b4bb3-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b4bb3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b4bb3-129">响应</span><span class="sxs-lookup"><span data-stu-id="b4bb3-129">Response</span></span>

<span data-ttu-id="b4bb3-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [chatmessage](../resources/chatmessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b4bb3-130">If successful, this method returns a `200 OK` response code and a [chatmessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4bb3-131">示例</span><span class="sxs-lookup"><span data-stu-id="b4bb3-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b4bb3-132">请求</span><span class="sxs-lookup"><span data-stu-id="b4bb3-132">Request</span></span>
<span data-ttu-id="b4bb3-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b4bb3-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b4bb3-134">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="b4bb3-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chat_message"
}-->
```http
GET https://graph.microsoft.com/beta/me/chats/{id}/messages/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b4bb3-135">C#</span><span class="sxs-lookup"><span data-stu-id="b4bb3-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chat-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b4bb3-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="b4bb3-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chat-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b4bb3-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="b4bb3-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chat-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b4bb3-138">响应</span><span class="sxs-lookup"><span data-stu-id="b4bb3-138">Response</span></span>
<span data-ttu-id="b4bb3-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b4bb3-139">Here is an example of the response.</span></span> 

><span data-ttu-id="b4bb3-140">**注意：** 为提高可读性，缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b4bb3-140">**Note:** The response object shown here is shortened for readability.</span></span> <span data-ttu-id="b4bb3-141">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b4bb3-141">All the properties will be returned from an actual call.</span></span>
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
