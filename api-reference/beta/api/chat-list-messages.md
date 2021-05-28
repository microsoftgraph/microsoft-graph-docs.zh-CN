---
title: 列出聊天中的消息
description: '在聊天中检索消息列表。 '
localization_priority: Priority
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 91f45f57fab749e0f9ec47937bd8b8897b55cea4
ms.sourcegitcommit: a9a035e7cf7b500aebe5477c05361552e7c3a7ab
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/28/2021
ms.locfileid: "52696119"
---
# <a name="list-messages-in-a-chat"></a><span data-ttu-id="f58c1-103">列出聊天中的消息</span><span class="sxs-lookup"><span data-stu-id="f58c1-103">List messages in a chat</span></span>

<span data-ttu-id="f58c1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f58c1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f58c1-105">在[聊天](../resources/chat.md)中检索[消息](../resources/chatmessage.md)列表。</span><span class="sxs-lookup"><span data-stu-id="f58c1-105">Retrieve the list of [messages](../resources/chatmessage.md) in a [chat](../resources/chat.md).</span></span>

> <span data-ttu-id="f58c1-106">**注意**：此 API 支持使用 [更改通知](../resources/webhooks.md)订阅更改（创建、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="f58c1-106">**Note**: This API supports subscribing to changes (create, update, and delete) using [change notifications](../resources/webhooks.md).</span></span> <span data-ttu-id="f58c1-107">这使呼叫方可以实时订阅和获取更改。</span><span class="sxs-lookup"><span data-stu-id="f58c1-107">This allows callers to subscribe and get changes in real time.</span></span> <span data-ttu-id="f58c1-108">有关详细信息，请参阅[获取消息通知](/graph/teams-changenotifications-chatmessage)。</span><span class="sxs-lookup"><span data-stu-id="f58c1-108">For details, see [Get notifications for messages](/graph/teams-changenotifications-chatmessage).</span></span>

## <a name="permissions"></a><span data-ttu-id="f58c1-109">权限</span><span class="sxs-lookup"><span data-stu-id="f58c1-109">Permissions</span></span>

<span data-ttu-id="f58c1-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f58c1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f58c1-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="f58c1-112">Permission type</span></span>      | <span data-ttu-id="f58c1-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f58c1-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f58c1-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f58c1-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f58c1-115">Chat.Read、Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f58c1-115">Chat.Read, Chat.ReadWrite</span></span> |
|<span data-ttu-id="f58c1-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f58c1-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f58c1-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f58c1-117">Not supported.</span></span>    |
|<span data-ttu-id="f58c1-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="f58c1-118">Application</span></span> | <span data-ttu-id="f58c1-119">Chat.Read.All、Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f58c1-119">Chat.Read.All, Chat.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="f58c1-120">在使用应用程序权限调用此 API 之前，你必须先请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="f58c1-120">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="f58c1-121">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="f58c1-121">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="f58c1-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f58c1-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/chats/{chat-id}/messages
GET /users/{user-id | user-principal-name}/chats/{chat-id}/messages
GET /chats/{chat-id}/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f58c1-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f58c1-123">Optional query parameters</span></span>

<span data-ttu-id="f58c1-124">可以使用 [$top](/graph/query-parameters#top-parameter) 查询参数控制每个响应中的项目数。</span><span class="sxs-lookup"><span data-stu-id="f58c1-124">You can use the [$top](/graph/query-parameters#top-parameter) query parameter to control the number of items per response.</span></span> <span data-ttu-id="f58c1-125">允许的最大 `$top` 值为 50。</span><span class="sxs-lookup"><span data-stu-id="f58c1-125">Maximum allowed `$top` value is 50.</span></span>
<span data-ttu-id="f58c1-126">目前不支持其他 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="f58c1-126">The other [OData query parameters](/graph/query-parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f58c1-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="f58c1-127">Request headers</span></span>

| <span data-ttu-id="f58c1-128">标头</span><span class="sxs-lookup"><span data-stu-id="f58c1-128">Header</span></span>       | <span data-ttu-id="f58c1-129">值</span><span class="sxs-lookup"><span data-stu-id="f58c1-129">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f58c1-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="f58c1-130">Authorization</span></span>  | <span data-ttu-id="f58c1-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f58c1-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f58c1-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="f58c1-133">Request body</span></span>

<span data-ttu-id="f58c1-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f58c1-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f58c1-135">响应</span><span class="sxs-lookup"><span data-stu-id="f58c1-135">Response</span></span>

<span data-ttu-id="f58c1-136">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [chatMessage](../resources/chatmessage.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f58c1-136">If successful, this method returns a `200 OK` response code and a collection of [chatMessage](../resources/chatmessage.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f58c1-137">示例</span><span class="sxs-lookup"><span data-stu-id="f58c1-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="f58c1-138">请求</span><span class="sxs-lookup"><span data-stu-id="f58c1-138">Request</span></span>

<span data-ttu-id="f58c1-139">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f58c1-139">The following is an example of the request.</span></span> <span data-ttu-id="f58c1-140">传递 `$top=2` 来检索两条消息。</span><span class="sxs-lookup"><span data-stu-id="f58c1-140">`$top=2` is passed to retrieve two messages.</span></span>


# <a name="http"></a>[<span data-ttu-id="f58c1-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="f58c1-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_allchatmessages_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/19:2da4c29f6d7041eca70b638b43d45437@thread.v2/messages?$top=2
```
# <a name="c"></a>[<span data-ttu-id="f58c1-142">C#</span><span class="sxs-lookup"><span data-stu-id="f58c1-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-allchatmessages-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f58c1-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f58c1-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-allchatmessages-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f58c1-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f58c1-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-allchatmessages-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f58c1-145">Java</span><span class="sxs-lookup"><span data-stu-id="f58c1-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-allchatmessages-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f58c1-146">响应</span><span class="sxs-lookup"><span data-stu-id="f58c1-146">Response</span></span>
<span data-ttu-id="f58c1-147">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="f58c1-147">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats('19%3A2da4c29f6d7041eca70b638b43d45437%40thread.v2')/messages",
    "@odata.count": 2,
    "@odata.nextLink": "https://graph.microsoft.com/beta/chats/19:2da4c29f6d7041eca70b638b43d45437@thread.v2/messages?$top=2&$skiptoken=M2UyZDAwMDAwMDMxMzkzYTMyNjQ2MTM0NjMzMjM5NjYzNjY0MzczMDM0MzE2NTYzNjEzNzMwNjIzNjMzMzg2MjM0MzM2NDM0MzUzNDMzMzc0MDc0Njg3MjY1NjE2NDJlNzYzMjAxZThmYjY4M2Y3ODAxMDAwMDg4NjA5ODdhNzgwMTAwMDB8MTYxNjk2NDUwOTgzMg%3d%3d",
    "value": [
        {
            "id": "1616964509832",
            "replyToId": null,
            "etag": "1616964509832",
            "messageType": "message",
            "createdDateTime": "2021-03-28T20:48:29.832Z",
            "lastModifiedDateTime": "2021-03-28T20:48:29.832Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": "19:2da4c29f6d7041eca70b638b43d45437@thread.v2",
            "importance": "normal",
            "locale": "en-us",
            "webUrl": null,
            "channelIdentity": null,
            "policyViolation": null,
            "from": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
                    "displayName": "Robin Kline",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "text",
                "content": "Hello world"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
        },
        {
            "id": "1615971548136",
            "replyToId": null,
            "etag": "1615971548136",
            "messageType": "message",
            "createdDateTime": "2021-03-17T08:59:08.136Z",
            "lastModifiedDateTime": "2021-03-17T08:59:08.136Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": "19:2da4c29f6d7041eca70b638b43d45437@thread.v2",
            "importance": "normal",
            "locale": "en-us",
            "webUrl": null,
            "channelIdentity": null,
            "policyViolation": null,
            "from": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
                    "displayName": "Robin Kline",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "html",
                "content": "<div><div><div><span><img height=\"63\" src=\"https://graph.microsoft.com/beta/chats/19:2da4c29f6d7041eca70b638b43d45437@thread.v2/messages/1615971548136/hostedContents/aWQ9eF8wLXd1cy1kOS1lNTRmNjM1NWYxYmJkNGQ3ZTNmNGJhZmU4NTI5MTBmNix0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kOS1lNTRmNjM1NWYxYmJkNGQ3ZTNmNGJhZmU4NTI5MTBmNi92aWV3cy9pbWdv/$value\" width=\"67\" style=\"vertical-align:bottom; width:67px; height:63px\"></span></div></div></div>"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get chat messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

