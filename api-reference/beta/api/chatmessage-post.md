---
title: 在频道或聊天中发送 chatMessage
description: 在指定的频道或聊天中发送新的 chatMessage。
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 2595ac4d8c9a1cafc1465a074221cd705fa20771
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2021
ms.locfileid: "51582674"
---
# <a name="send-chatmessage-in-a-channel-or-a-chat"></a><span data-ttu-id="09730-103">在频道或聊天中发送 chatMessage</span><span class="sxs-lookup"><span data-stu-id="09730-103">Send chatMessage in a channel or a chat</span></span>

<span data-ttu-id="09730-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09730-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09730-105">在指定的频道或聊天中[发送新的](../resources/channel.md)[chatMessage。](../resources/chatmessage.md) [](../resources/chat.md)</span><span class="sxs-lookup"><span data-stu-id="09730-105">Send a new [chatMessage](../resources/chatmessage.md) in the specified [channel](../resources/channel.md) or a [chat](../resources/chat.md).</span></span>

> <span data-ttu-id="09730-106">**注意**：不建议使用此 API 进行数据迁移。</span><span class="sxs-lookup"><span data-stu-id="09730-106">**Note**: We don't recommend that you use this API for data migration.</span></span> <span data-ttu-id="09730-107">它不具有典型迁移所需的吞吐量。</span><span class="sxs-lookup"><span data-stu-id="09730-107">It does not have the throughput necessary for a typical migration.</span></span>

> <span data-ttu-id="09730-108">**注意**：使用 Microsoft Teams [](/legal/microsoft-apis/terms-of-use)作为 microsoft Teams 日志文件。</span><span class="sxs-lookup"><span data-stu-id="09730-108">**Note**: It is a violation of the [terms of use](/legal/microsoft-apis/terms-of-use) to use Microsoft Teams as a log file.</span></span> <span data-ttu-id="09730-109">仅发送用户将阅读的邮件。</span><span class="sxs-lookup"><span data-stu-id="09730-109">Only send messages that people will read.</span></span>

## <a name="permissions"></a><span data-ttu-id="09730-110">权限</span><span class="sxs-lookup"><span data-stu-id="09730-110">Permissions</span></span>

<span data-ttu-id="09730-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="09730-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-for-channel"></a><span data-ttu-id="09730-113">频道权限</span><span class="sxs-lookup"><span data-stu-id="09730-113">Permissions for channel</span></span>
| <span data-ttu-id="09730-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="09730-114">Permission type</span></span>                        | <span data-ttu-id="09730-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="09730-115">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="09730-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="09730-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="09730-117">ChannelMessage.Send、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09730-117">ChannelMessage.Send, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="09730-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="09730-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09730-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="09730-119">Not supported.</span></span> |
| <span data-ttu-id="09730-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="09730-120">Application</span></span>                            | <span data-ttu-id="09730-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="09730-121">Not supported.</span></span> |

### <a name="permissions-for-chat"></a><span data-ttu-id="09730-122">聊天权限</span><span class="sxs-lookup"><span data-stu-id="09730-122">Permissions for chat</span></span>
| <span data-ttu-id="09730-123">权限类型</span><span class="sxs-lookup"><span data-stu-id="09730-123">Permission type</span></span>                        | <span data-ttu-id="09730-124">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="09730-124">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="09730-125">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="09730-125">Delegated (work or school account)</span></span>     | <span data-ttu-id="09730-126">ChatMessage.Send、Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="09730-126">ChatMessage.Send, Chat.ReadWrite</span></span> |
| <span data-ttu-id="09730-127">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="09730-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09730-128">不支持。</span><span class="sxs-lookup"><span data-stu-id="09730-128">Not supported.</span></span> |
| <span data-ttu-id="09730-129">应用程序</span><span class="sxs-lookup"><span data-stu-id="09730-129">Application</span></span>                            | <span data-ttu-id="09730-130">不支持。</span><span class="sxs-lookup"><span data-stu-id="09730-130">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="09730-131">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="09730-131">HTTP request</span></span>

<span data-ttu-id="09730-132">**在频道中发送消息**</span><span class="sxs-lookup"><span data-stu-id="09730-132">**Sending message in a channel**</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{team-id}/channels/{channel-id}/messages
```

<span data-ttu-id="09730-133">**在频道中发送回复**</span><span class="sxs-lookup"><span data-stu-id="09730-133">**Sending replies in a channel**</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{team-id}/channels/{channel-id}/messages/{message-id}/replies
```

<span data-ttu-id="09730-134">**在聊天中发送消息**</span><span class="sxs-lookup"><span data-stu-id="09730-134">**Sending message in a chat**</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /chats/{chat-id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="09730-135">请求标头</span><span class="sxs-lookup"><span data-stu-id="09730-135">Request headers</span></span>

| <span data-ttu-id="09730-136">名称</span><span class="sxs-lookup"><span data-stu-id="09730-136">Name</span></span>          | <span data-ttu-id="09730-137">说明</span><span class="sxs-lookup"><span data-stu-id="09730-137">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="09730-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="09730-138">Authorization</span></span> | <span data-ttu-id="09730-139">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="09730-139">Bearer {code}.</span></span> <span data-ttu-id="09730-140">必需。</span><span class="sxs-lookup"><span data-stu-id="09730-140">Required.</span></span> |
| <span data-ttu-id="09730-141">Content-type</span><span class="sxs-lookup"><span data-stu-id="09730-141">Content-type</span></span> | <span data-ttu-id="09730-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="09730-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="09730-144">请求正文</span><span class="sxs-lookup"><span data-stu-id="09730-144">Request body</span></span>

<span data-ttu-id="09730-145">在请求正文中，提供 [chatMessage](../resources/chatmessage.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="09730-145">In the request body, supply a JSON representation of a [chatMessage](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="09730-146">只有 body 属性是必需的;其他属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="09730-146">Only the body property is mandatory; other properties are optional.</span></span>


## <a name="response"></a><span data-ttu-id="09730-147">响应</span><span class="sxs-lookup"><span data-stu-id="09730-147">Response</span></span>

<span data-ttu-id="09730-148">如果成功，此方法在响应正文中返回 响应代码和新 `201 Created` [chatMessage](../resources/chatmessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="09730-148">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="09730-149">示例</span><span class="sxs-lookup"><span data-stu-id="09730-149">Examples</span></span>

<span data-ttu-id="09730-150">在下面的示例中，URL 可以使用所述的[HTTP](#http-request)语法向聊天[](chat-post-messages.md)发送消息、向频道发送消息或向[](channel-post-messages.md)频道[发送回复](chatmessage-post-replies.md)。</span><span class="sxs-lookup"><span data-stu-id="09730-150">In the following examples, the URL can use the [HTTP syntax](#http-request) described to [send a message to a chat](chat-post-messages.md), [send a message to a channel](channel-post-messages.md), or [send reply to a channel](chatmessage-post-replies.md).</span></span>

### <a name="example-1-send-a-hello-world-message-in-a-channel"></a><span data-ttu-id="09730-151">示例 1：在频道中发送 Hello World 消息</span><span class="sxs-lookup"><span data-stu-id="09730-151">Example 1: Send a Hello World message in a channel</span></span>

#### <a name="request"></a><span data-ttu-id="09730-152">请求</span><span class="sxs-lookup"><span data-stu-id="09730-152">Request</span></span>
<span data-ttu-id="09730-153">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="09730-153">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_chatmessage_1"
}-->
```http
POST https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages
Content-type: application/json

{
  "body": {
    "content": "Hello World"
  }
}
```

#### <a name="response"></a><span data-ttu-id="09730-154">响应</span><span class="sxs-lookup"><span data-stu-id="09730-154">Response</span></span>

<span data-ttu-id="09730-155">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="09730-155">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2')/messages/$entity",
    "id": "1616990032035",
    "replyToId": null,
    "etag": "1616990032035",
    "messageType": "message",
    "createdDateTime": "2021-03-29T03:53:52.035Z",
    "lastModifiedDateTime": "2021-03-29T03:53:52.035Z",
    "lastEditedDateTime": null,
    "deletedDateTime": null,
    "subject": null,
    "summary": null,
    "chatId": null,
    "importance": "normal",
    "locale": "en-us",
    "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616990032035?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616990032035&parentMessageId=1616990032035",
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
        "content": "Hello World"
    },
    "channelIdentity": {
        "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
        "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
    },
    "attachments": [],
    "mentions": [],
    "reactions": []
}
```

### <a name="example-2-mentions-a-user-in-a-channel-message"></a><span data-ttu-id="09730-156">示例 2：@mentions频道消息中通知用户</span><span class="sxs-lookup"><span data-stu-id="09730-156">Example 2: @mentions a user in a channel message</span></span>

#### <a name="request"></a><span data-ttu-id="09730-157">请求</span><span class="sxs-lookup"><span data-stu-id="09730-157">Request</span></span>
<span data-ttu-id="09730-158">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="09730-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_chatmessage_2"
}-->
```http
POST https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages
Content-type: application/json

{
  "body": {
    "contentType": "html",
    "content": "Hello World <at id=\"0\">Jane Smith</at>"
  },
  "mentions": [
    {
      "id": 0,
      "mentionText": "Jane Smith",
      "mentioned": {
        "user": {
          "displayName": "Jane Smith",
          "id": "ef1c916a-3135-4417-ba27-8eb7bd084193",
          "userIdentityType": "aadUser"
        }
      }
    }
  ]
}
```

#### <a name="response"></a><span data-ttu-id="09730-159">响应</span><span class="sxs-lookup"><span data-stu-id="09730-159">Response</span></span>

<span data-ttu-id="09730-160">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="09730-160">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2')/messages/$entity",
    "id": "1616965872395",
    "replyToId": null,
    "etag": "1616965872395",
    "messageType": "message",
    "createdDateTime": "2021-03-28T21:11:12.395Z",
    "lastModifiedDateTime": "2021-03-28T21:11:12.395Z",
    "lastEditedDateTime": null,
    "deletedDateTime": null,
    "subject": null,
    "summary": null,
    "chatId": null,
    "importance": "normal",
    "locale": "en-us",
    "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616965872395?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616965872395&parentMessageId=1616965872395",
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
        "content": "Hello World <at id=\"0\">Jane Smith</at>"
    },
    "channelIdentity": {
        "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
        "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
    },
    "attachments": [],
    "mentions": [
        {
            "id": 0,
            "mentionText": "Jane Smith",
            "mentioned": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "ef1c916a-3135-4417-ba27-8eb7bd084193",
                    "displayName": "Jane Smith",
                    "userIdentityType": "aadUser"
                }
            }
        }
    ],
    "reactions": []
}
```

### <a name="example-3-send-message-containing-cards"></a><span data-ttu-id="09730-161">示例 3：发送包含卡片的邮件</span><span class="sxs-lookup"><span data-stu-id="09730-161">Example 3: Send message containing cards</span></span>

#### <a name="request"></a><span data-ttu-id="09730-162">请求</span><span class="sxs-lookup"><span data-stu-id="09730-162">Request</span></span>
<span data-ttu-id="09730-163">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="09730-163">The following is an example of the request.</span></span>

> <span data-ttu-id="09730-164">**注意：** 附件的 ID 必须是唯一的，并且可以是随机生成的新 GUID。</span><span class="sxs-lookup"><span data-stu-id="09730-164">**Note:** The attachment's ID must be unique and can be a new randomly generated GUID.</span></span> <span data-ttu-id="09730-165">但是，附件的 ID 在 _body_ 和 attachments 元素中 _必须_ 相同。</span><span class="sxs-lookup"><span data-stu-id="09730-165">However, the attachment's ID must be the same in the _body_ and _attachments_ elements.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_chatmessage_3"
}-->
```http
POST https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages
Content-type: application/json

{
    "subject": null,
    "body": {
        "contentType": "html",
        "content": "<attachment id=\"74d20c7f34aa4a7fb74e2b30004247c5\"></attachment>"
    },
    "attachments": [
        {
            "id": "74d20c7f34aa4a7fb74e2b30004247c5",
            "contentType": "application/vnd.microsoft.card.thumbnail",
            "contentUrl": null,
            "content": "{\r\n  \"title\": \"This is an example of posting a card\",\r\n  \"subtitle\": \"<h3>This is the subtitle</h3>\",\r\n  \"text\": \"Here is some body text. <br>\\r\\nAnd a <a href=\\\"http://microsoft.com/\\\">hyperlink</a>. <br>\\r\\nAnd below that is some buttons:\",\r\n  \"buttons\": [\r\n    {\r\n      \"type\": \"messageBack\",\r\n      \"title\": \"Login to FakeBot\",\r\n      \"text\": \"login\",\r\n      \"displayText\": \"login\",\r\n      \"value\": \"login\"\r\n    }\r\n  ]\r\n}",
            "name": null,
            "thumbnailUrl": null
        }
    ]
}
```

#### <a name="response"></a><span data-ttu-id="09730-166">响应</span><span class="sxs-lookup"><span data-stu-id="09730-166">Response</span></span>

<span data-ttu-id="09730-167">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="09730-167">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2')/messages/$entity",
    "id": "1616991851162",
    "replyToId": null,
    "etag": "1616991851162",
    "messageType": "message",
    "createdDateTime": "2021-03-29T04:24:11.162Z",
    "lastModifiedDateTime": "2021-03-29T04:24:11.162Z",
    "lastEditedDateTime": null,
    "deletedDateTime": null,
    "subject": null,
    "summary": null,
    "chatId": null,
    "importance": "normal",
    "locale": "en-us",
    "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616991851162?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616991851162&parentMessageId=1616991851162",
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
        "content": "<attachment id=\"74d20c7f34aa4a7fb74e2b30004247c5\"></attachment>"
    },
    "channelIdentity": {
        "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
        "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
    },
    "attachments": [
        {
            "id": "74d20c7f34aa4a7fb74e2b30004247c5",
            "contentType": "application/vnd.microsoft.card.thumbnail",
            "contentUrl": null,
            "content": "{  \"title\": \"This is an example of posting a card\",  \"subtitle\": \"<h3>This is the subtitle</h3>\",  \"text\": \"Here is some body text. <br>\\\\And a <a href=\\\"http://microsoft.com/\\\">hyperlink</a>. <br>\\\\And below that is some buttons:\",  \"buttons\": [    {      \"type\": \"messageBack\",      \"title\": \"Login to FakeBot\",      \"text\": \"login\",      \"displayText\": \"login\",      \"value\": \"login\"    }  ]}",
            "name": null,
            "thumbnailUrl": null
        }
    ],
    "mentions": [],
    "reactions": []
}
```

### <a name="example-4-send-a-message-with-file-attachment-in-it"></a><span data-ttu-id="09730-168">示例 4：发送包含文件附件的邮件</span><span class="sxs-lookup"><span data-stu-id="09730-168">Example 4: Send a message with file attachment in it</span></span>

#### <a name="request"></a><span data-ttu-id="09730-169">请求</span><span class="sxs-lookup"><span data-stu-id="09730-169">Request</span></span>
<span data-ttu-id="09730-170">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="09730-170">The following is an example of the request.</span></span>

><span data-ttu-id="09730-171">**注意：** 文件必须已经在 SharePoint 中。</span><span class="sxs-lookup"><span data-stu-id="09730-171">**Note:** The file must already be in SharePoint.</span></span> <span data-ttu-id="09730-172">若要查找文件属性，请获取 **文件的 driveItem。**</span><span class="sxs-lookup"><span data-stu-id="09730-172">To find the file properties, GET the **driveItem** for the file.</span></span> <span data-ttu-id="09730-173">例如，/drives/{id}/items/{id}。</span><span class="sxs-lookup"><span data-stu-id="09730-173">For example, /drives/{id}/items/{id}.</span></span> <span data-ttu-id="09730-174">附件 ID 是 **driveItem** 的 **eTag** 中的 GUID，附件 contentURL 是 **driveItem** 文件夹的 **webUrl** 加上 **driveItem** 的名称，附件名称是 **driveItem** 的名称。 </span><span class="sxs-lookup"><span data-stu-id="09730-174">Your attachment ID is the GUID in the **eTag** of the **driveItem**, your attachment **contentURL** is the **webUrl** of the **driveItem**'s folder plus the **driveItem**'s name, and your attachment name is the **driveItem**'s name.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_chatmessage_4"
}-->
```http
POST https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages
Content-type: application/json

{
    "body": {
        "contentType": "html",
        "content": "Here's the latest budget. <attachment id=\"153fa47d-18c9-4179-be08-9879815a9f90\"></attachment>"
    },
    "attachments": [
        {
            "id": "153fa47d-18c9-4179-be08-9879815a9f90",
            "contentType": "reference",
            "contentUrl": "https://m365x987948.sharepoint.com/sites/test/Shared%20Documents/General/test%20doc.docx",
            "name": "Budget.docx"
        }
    ]
}
```

#### <a name="response"></a><span data-ttu-id="09730-175">响应</span><span class="sxs-lookup"><span data-stu-id="09730-175">Response</span></span>

<span data-ttu-id="09730-176">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="09730-176">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2')/messages/$entity",
    "id": "1616991899452",
    "replyToId": null,
    "etag": "1616991899452",
    "messageType": "message",
    "createdDateTime": "2021-03-29T04:24:59.452Z",
    "lastModifiedDateTime": "2021-03-29T04:24:59.452Z",
    "lastEditedDateTime": null,
    "deletedDateTime": null,
    "subject": null,
    "summary": null,
    "chatId": null,
    "importance": "normal",
    "locale": "en-us",
    "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616991899452?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616991899452&parentMessageId=1616991899452",
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
        "content": "Here's the latest budget. <attachment id=\"153fa47d-18c9-4179-be08-9879815a9f90\"></attachment>"
    },
    "channelIdentity": {
        "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
        "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
    },
    "attachments": [
        {
            "id": "153fa47d-18c9-4179-be08-9879815a9f90",
            "contentType": "reference",
            "contentUrl": "https://m365x987948.sharepoint.com/sites/test/Shared%20Documents/General/test%20doc.docx",
            "content": null,
            "name": "Budget.docx",
            "thumbnailUrl": null
        }
    ],
    "mentions": [],
    "reactions": []
}
```

### <a name="example-5-send-inline-images-along-with-the-message"></a><span data-ttu-id="09730-177">示例 5：随邮件一起发送内嵌图像</span><span class="sxs-lookup"><span data-stu-id="09730-177">Example 5: Send inline images along with the message</span></span>

#### <a name="request"></a><span data-ttu-id="09730-178">请求</span><span class="sxs-lookup"><span data-stu-id="09730-178">Request</span></span>
<span data-ttu-id="09730-179">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="09730-179">The following is an example of the request.</span></span>

> <span data-ttu-id="09730-180">**注意：\*\*\*\*hostedContents** 集合中的 **temporaryId** 是一个随机 ID，但在整个 **body** 和 **hostedContents** 元素中必须相同。</span><span class="sxs-lookup"><span data-stu-id="09730-180">**Note:** The **temporaryId** in the **hostedContents** collection is a random ID, but must be same across the **body** and **hostedContents** elements.</span></span> <span data-ttu-id="09730-181"> (注意 **temporaryId** 设置为 **1，** 正文中的引用设置为 `../hostedContents/1/$value` .) </span><span class="sxs-lookup"><span data-stu-id="09730-181">(Notice the **temporaryId** set to **1** and the reference in body as `../hostedContents/1/$value`.)</span></span>

<span data-ttu-id="09730-182">**contentBytes** 必须设置为二进制字符串 Base64 编码字节。</span><span class="sxs-lookup"><span data-stu-id="09730-182">**contentBytes** must be set to binary string Base64-encoded bytes.</span></span> <span data-ttu-id="09730-183">为此，可以使用 C# `Convert.ToBase64String(File.ReadAllBytes("image.png"));`</span><span class="sxs-lookup"><span data-stu-id="09730-183">You can do this in C# by using `Convert.ToBase64String(File.ReadAllBytes("image.png"));`</span></span>

<!-- {
  "blockType": "request",
  "name": "post_chatmessage_5"
}-->
```http
POST https://graph.microsoft.com/beta/chats/19:2da4c29f6d7041eca70b638b43d45437@thread.v2/messages
Content-type: application/json

{
    "body": {
        "contentType": "html",
        "content": "<div><div>\n<div><span><img height=\"297\" src=\"../hostedContents/1/$value\" width=\"297\" style=\"vertical-align:bottom; width:297px; height:297px\"></span>\n\n</div>\n\n\n</div>\n</div>"
    },
    "hostedContents":[
        {
          "@microsoft.graph.temporaryId": "1",
          "contentBytes": "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",
            "contentType": "image/png"
        }
    ]
}
```

#### <a name="response"></a><span data-ttu-id="09730-184">响应</span><span class="sxs-lookup"><span data-stu-id="09730-184">Response</span></span>

<span data-ttu-id="09730-185">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="09730-185">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats('19%3A2da4c29f6d7041eca70b638b43d45437%40thread.v2')/messages/$entity",
    "id": "1616991962672",
    "replyToId": null,
    "etag": "1616991962672",
    "messageType": "message",
    "createdDateTime": "2021-03-29T04:26:02.672Z",
    "lastModifiedDateTime": "2021-03-29T04:26:02.672Z",
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
        "content": "<div><div><div><span><img height=\"297\" src=\"https://graph.microsoft.com/beta/chats/19:2da4c29f6d7041eca70b638b43d45437@thread.v2/messages/1616991962672/hostedContents/aWQ9eF8wLXd1cy1kNy1kZTczYzM0YTYzZGVkYjViMDVlNjYyY2Y1NzQ5MGU5Yyx0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kNy1kZTczYzM0YTYzZGVkYjViMDVlNjYyY2Y1NzQ5MGU5Yy92aWV3cy9pbWdv/$value\" width=\"297\" style=\"vertical-align:bottom; width:297px; height:297px\"></span></div></div></div>"
    },
    "attachments": [],
    "mentions": [],
    "reactions": []
}
```

### <a name="example-6-send-a-card-with-inline-images"></a><span data-ttu-id="09730-186">示例 6：发送包含内联图像的卡片</span><span class="sxs-lookup"><span data-stu-id="09730-186">Example 6: Send a card with inline images</span></span>

#### <a name="request"></a><span data-ttu-id="09730-187">请求</span><span class="sxs-lookup"><span data-stu-id="09730-187">Request</span></span>
<span data-ttu-id="09730-188">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="09730-188">The following is an example of the request.</span></span>

> <span data-ttu-id="09730-189">**注意：** hostedContents 集合中的 **temporaryId** 是一个随机 ID，但必须在附件和 **hostedContents** (中的内容) 相同。</span><span class="sxs-lookup"><span data-stu-id="09730-189">**Note:** The **temporaryId** in the **hostedContents** collection is a random ID, but must be same across the **content** (in **attachments**) and **hostedContents** elements.</span></span> <span data-ttu-id="09730-190"> (请注意 **，temporaryId** 设置为 **1，** 内容中的引用设置为 `../hostedContents/1/$value` .) </span><span class="sxs-lookup"><span data-stu-id="09730-190">(Notice the **temporaryId** set to **1** and the reference in content as `../hostedContents/1/$value`.)</span></span>

<span data-ttu-id="09730-191">**contentBytes** 必须设置为二进制字符串 Base64 编码字节。</span><span class="sxs-lookup"><span data-stu-id="09730-191">**contentBytes** must be set to binary string Base64-encoded bytes.</span></span> <span data-ttu-id="09730-192">为此，可以使用 C# `Convert.ToBase64String(File.ReadAllBytes("image.png"));`</span><span class="sxs-lookup"><span data-stu-id="09730-192">You can do this in C# by using `Convert.ToBase64String(File.ReadAllBytes("image.png"));`</span></span>

<!-- {
  "blockType": "request",
  "name": "post_chatmessage_6"
}-->
```http
POST https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages
Content-type: application/json

{
    "subject": null,
    "body": {
        "contentType": "html",
        "content": "<attachment id=\"74d20c7f34aa4a7fb74e2b30004247c5\"></attachment>"
    },
    "attachments": [{
        "id": "74d20c7f34aa4a7fb74e2b30004247c5",
        "contentType": "application/vnd.microsoft.card.adaptive",
        "contentUrl": null,
        "content": "{\r\n  \"$schema\": \"http://adaptivecards.io/schemas/adaptive-card.json\",\r\n  \"type\": \"AdaptiveCard\",\r\n  \"version\": \"1.2\",\r\n  \"speak\": \"The Seattle Seahawks beat the Carolina Panthers 40-7\",\r\n  \"body\": [\r\n    {\r\n      \"type\": \"Container\",\r\n      \"items\": [\r\n        {\r\n          \"type\": \"ColumnSet\",\r\n          \"columns\": [\r\n            {\r\n              \"type\": \"Column\",\r\n              \"width\": \"auto\",\r\n              \"items\": [\r\n                {\r\n                  \"type\": \"Image\",\r\n                  \"url\": \"../hostedContents/1/$value\",\r\n                  \"size\": \"Medium\"\r\n                },\r\n                {\r\n                  \"type\": \"TextBlock\",\r\n                  \"text\": \"SHADES\",\r\n                  \"horizontalAlignment\": \"Center\",\r\n                  \"weight\": \"Bolder\"\r\n                }\r\n              ]\r\n            },\r\n            {\r\n              \"type\": \"Column\",\r\n              \"width\": \"stretch\",\r\n              \"separator\": true,\r\n              \"spacing\": \"Medium\",\r\n              \"items\": [\r\n                {\r\n                  \"type\": \"TextBlock\",\r\n                  \"text\": \"2019-08-31T19:30:00Z\",\r\n                  \"horizontalAlignment\": \"Center\"\r\n                },\r\n                {\r\n                  \"type\": \"TextBlock\",\r\n                  \"text\": \"Final\",\r\n                  \"spacing\": \"None\",\r\n                  \"horizontalAlignment\": \"Center\"\r\n                },\r\n                {\r\n                  \"type\": \"TextBlock\",\r\n                  \"text\": \"40 - 7\",\r\n                  \"size\": \"ExtraLarge\",\r\n                  \"horizontalAlignment\": \"Center\"\r\n                }\r\n              ]\r\n            },\r\n            {\r\n              \"type\": \"Column\",\r\n              \"width\": \"auto\",\r\n              \"separator\": true,\r\n              \"spacing\": \"Medium\",\r\n              \"items\": [\r\n                {\r\n                  \"type\": \"Image\",\r\n                  \"url\": \"../hostedContents/2/$value\",\r\n                  \"size\": \"Medium\",\r\n                  \"horizontalAlignment\": \"Center\"\r\n                },\r\n                {\r\n                  \"type\": \"TextBlock\",\r\n                  \"text\": \"SKINS\",\r\n                  \"horizontalAlignment\": \"Center\",\r\n                  \"weight\": \"Bolder\"\r\n                }\r\n              ]\r\n            }\r\n          ]\r\n        }\r\n      ]\r\n    }\r\n  ]\r\n}",
        "name": null,
        "thumbnailUrl": null
    }],
    "hostedContents": [{
        "@microsoft.graph.temporaryId": "1",
        "contentBytes": "iVBORw0KGgoAAAANSUhEUgAAASkAAAEpCAYAAADPmdSCAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAAZdEVYdFNvZnR3YXJlAHBhaW50Lm5ldCA0LjAuMTZEaa/1AAAhr0lEQVR4Xu3d76tdV50GcP+EvJu3/QuGvJgXxSk0Y8QwzZRmCG2lQkjrkM4UjOmLgmAt0bQGLqipo1ghmIhSRBIMbV+UpmiIRSYV9IqmHaqNgRJbUGqoA30xMGe+z+1ZNyfrPuec/WN9115r7yfw6Y917zlnn+9e68ne66y9z8dms1kjTzzxxC6zxxw3h80d7Pekfti3832MfX3A7GK/J5IDbYxZJz1mbppZ5JJRBx4J7Etzar5vY8fZY0S80cZF6JxRZ41dN7vZY6Uetg8RUJvzfbrMWfZYEU+0MbBOicN+1lljOMo6zJ5Dymf7bvd8H7J9G9vDnkPEC20MrEMuO/Rf5hR7HimX7TOcyrN9ucwF9jwiXmhjYB0Sc06so66ieaoKYB+Zs/N91sYl9nwiXmhjgA4ZddCmNE9VMNs3OI1fN/+0jEJKsqKNATpk1EHb0DxVgWyfYBlJ0/knRiElWdHGAB0y6qBd6BOhQti+aDv/xCikJCvaGKBDRh20K5xaaJ5qIKi96TL/xCikJCvaGKBDRh20D5xiaJ4qM9TcdJ1/YhRSkhVtDNAhow6aguapMrFa45KWPvNPjEJKsqKNATpk1EFT0TyVM6vxuisFulJISVa0MUCHjDpoSjgF0UXKiVlNMf90YV5jDwopyYo2BuiQUQdNDaciuswiEatl6vknRiElWdHGAB0y6qBejrHXl+ashh7zT4xCSrKijQE6ZNRBPeEjci1T6MDq1vYayz4UUpIVbQzQIaMO6k3zVC1YrTD/lHsfKaQkK9oYoENGHTQHzVM1YDXC/BOukWQ19KSQkqxoY4AOGXXQnHQnyCWsNri1b475J0YhJVnRxgAdMuqgueGjdM1TLbB65Jx/YhRSkhVtDNAhow46BMxTTf5yGqvBEPNPjEJKsqKNATpk1EGHglObA2wb27hx40bnSXl7bKcjuq6PW2Tvvc3tfb0ppCQr2higQ0YddGid56ksLM6am6b1Udn8sZumVeDg9+eP63wZkL1nzD+xWgxFISVZ0cYAHTLqoCVoPU+FkDCzuVZBFT22cVDh9+a/Hx7bOqjsfaa6vUpKCinJijYG6JBRBy1F49sTIxwWgiJoFFT2O+yxa4MKP5//XvzYRkFl7w3zT96Xt3SlkJKsaGOADhl10JJgjmblbV8QClFILFoZVPazVY9dGlRon/+cPQ5WBpW9p7639/WmkJKsaGOADhl10BLRr9FCGEThwNCgsrYmj90RVPj/eTv7/UU0qOy9pLi9rzeFlGRFGwN0yKiDlgrbuR0YCIEoFFa5Lajsv9s8djuo8O/5/7PfY7aDCttuSpx/YhRSkhVtDNAhow5asq15Kgz+KAya2Aoq0+WxCKY75v9mP18FwdTn66WGoJCSrGhjgA4ZddCiPf300x9cv379f0kYFOub3/zm/7D3UrDkIXXz4393hzlrLk3IBaNrVBugjQE6ZNRBi7exsTG7du0aDYTSnDlzhr6HwiULKRukIZxmE4bAUlitQBsDdMiog1ahhqCqNKCgd0jZoFQ47aSwWoI2BuiQUQetRslBVXFAQeeQskGocFpPYRWhjQE6ZNRBq1JiUFUeUNA6pGzQKZzaU1jN0cYAHTLqoNUpKahGEFDQOKRskCmc+pt8WNHGAB0y6qBVKiGoRhJQsDakbFApnNKbbFjRxgAdMuqg1RoyqEYUULA0pGwQDRlOGMRdXDfs+UqFbZ5UWNHGAB0y6qBVu3LlCg0Rb2xbKrYjpGzQDBlOeN1eX95hjz9sFFaFoo0BOmTUQaumkEpiO6RskFQdTjF7PoVVgWhjgA4ZddCqKaSSwKAYVTjF7PkVVgWhjQE6ZNRBq6aQ6ufpo/8xe/1f/uG9aHDk4h5OMXs9hVUBaGNgHVMhlQDblpognC4f+DgbEDlkD6eYvb7CakC0MbAOqpBKgG1LDaYeTjHbHoXVAGhjYB1VIZUA25aSKZxWs+1TWGWEgrM3JJJb8eEUs+2tMayqo5CSoVUXTjHbfoWVn0sKKRlK9eEUs/ejsEpn+/RUISW5jS6cYvb+FFbd7Zg7U0hJLqMPp5i9X4VVc0sn9hVS4m1y4RSz96+wWm7tp44KKfEy+XCKWT0UVrc0XhKhkJLU3jR/zzqbfMTqM+WwahxOgUJKPNw0xw39Knr5iNVnSmHVOpwChZR4Ulg1YPUZc1h1DqdAISU5KKwasPqMKax6h1OgkJKcFFYNWH1qDqtk4RQopGQICqsGrD41hVXycAoUUjIkhVUDVp+Sw8otnAKFlJRAYdWA1aeksHIPp0AhJSVRWMkOCikpkcJKtimkpGQKK1FISRUUVhOmkJKaKKwmSCElNVJYTYhCSmqmsJoAhBR2MnXx4N3XX3zwUzPm9L/unT2w5x+r8vA9n5r9273/nB3blpI9s/+f6D6HAb/qahWEFdbtTAHu0zWpUKaNwRMrvnfvyJEjszvvvFNG6IEHHqD7HP7zyCEWEuIPizgPs3E6drQxsE6pkJoghVRRJhtOAW0MrFMqpCZIIVWEyYdTQBsD65QKqQlSSA1K4RShjYF1SoXUBCmkBqFwWoI2BtYpFVITpJDKSuG0Bm0MrFMqpCZoVUid+vfDH0aDTLpRODVEGwPrlEtDKvjc5z43e+ihh2Z33XUX7fC1uvfee2c//OEPZ7/+9a9nN27c2PLWW29ttX3605+mj6kV9h2C6bHHHqP7OIK1OmO6F3duCqeWaGOADhl10KUef/zx2f79++kgqM0XvvCF7WBa5rvf/S59bG327t279RcN26dLXAr9A4NtPujYYJTbKZw6oo0BOmTUQdeqPaiaBFSAoyr2HLVAQOEvF7YfV9gOqQCDbz4I2eCcOoVTT7QxQIeMOuha6PS1nvrhFI+F0SpHjx6lz1WDlkdQwY6QCjAY54OSDdapUTglQhsDdMiogzaCOSo2KEqHIyMWRKu89tpr9LlKd99999F918DSkAowOOeDlA3esVM4JUYbA3TIqIM2gr+h2cAoHQuhJnAExp6vZI888gjddw2sDakAg3U+aNlgHhuFkxPaGKBDRh20MTYwSoZP7FgANfHZz36WPmfJOsxFBY1DKsDgnQ9iNrhrp3ByRhsDdMiogzbGBkbJPvOZz9AAagKPZc9ZMrbPGmodUoEN5j1jw96npEUbA3TIqIM2dvfdd9PBUSocDbEAauLEiRP0OUvG9llDnUNKpAvaGKBDRh20sX379tHBUao+IfX1r3+dPmfJ2D5rSCElWdHGAB0y6qCN1bZeCkHDAqiJ2hZ24i8Qts8aUkhJVrQxQIeMOmhjuMyCDZBSdVl+ELzyyiv0OUuFv0DYPmtIISVZ0cYAHTLqoI3hI242QEqF9U4sgJpiz1kqrGNj+6whhZRkRRsDdMiogzaGj7jZACnRJz7xCRo8bdR00XHDC4mXUUhJVrQxQIeMOmgrtcxLtbleb5la5qXwqSvbVy1smj1z+iopcUcbA+uEvULq0KFDdKCUBnNKLHjawC1d2HOXZtW9onpCX4FT5rhBiO1m/UqkDdoYzDsd65CNlb5eqs9K8xiOyNhrlKTHSvM+cPR1wYTw0hGYNEYbA+tMvUOq9KOpn/zkJzRwuij9aKrHRcUerhsE1zGjIy5ZijYG1nl6hxSUejTVZwHnMqUeTeH2OQMdRTV10yi0ZAfaGFhnSRJSpd4Pve+yAwa3GManhez1htRz2cEQcKSF+a0DrG/KdNDGwDpIkpCCgwcP0sEzFHwax0ImBZxCstccSs/FmyXAUdZZo8CaINoYWKdIFlKA29WyQZRbiiUH65Ry0XHHWwSXLASW7kAwEbQxsI6QNKQwWLyDCpPDTz311Oz8+fOzzc3N2QcffLDt/Rdenr2378Gs/nLy2du2Adv08ssvzzY2Nra2lb2HVDAP1XPhZulwSohPDO9g/VfGgTYGtvOThhR4BRWCKQ4lJmdQxQHF/P73v98KrE9+8pP0fXU1gYCKYdJdR1cjRBsD2+nJQwoQVKlWoyOcMNBZACyTI6iaBNSid999d/btb387SViN8BSvDRxdHTZaizUStDGwHe0SUkGfL2zA3TCbHDkt4xlUbQNqEQL30Ucfpe+5CXxAwWo9QZi7wqmgwqpytDGwHewaUoAvbWh7gzycHrEB3pZHUPUJqEXf//736XtfBjXEUg9W44lTWFWONga2Y91DKsAAa3IKiAlxNqi7ShlUqQIqwDqudad/CCes6mc1ldsorCpFGwPbodlCKsCRFU4D2dFV6oAKUgRV6oAKcEobBxXmnHBa1/HLPadOYVUZ2hjYjsweUjEcYeEGevjYng3iVPoElVdABVevXt06WtLpXFIIK30VVQVoY2A7cfCQgnPnztHBm1qXoPIOqODnP/85rY30tnV/LNb/pQy0MbCdN3hIfe1rX6OD1kuboMoVUMHp06dpjSQJrLPSKWCBaGNgO23wkGq7BiqFJkGVO6Dgz3/+8+xLX/oSrZMkgVPAY2wsyHBoY2A7bNCQwje4sMGaw6qgGiKggpdeeonWSpJCv9ftYgpBG4P5zmI7MYt33nmHDtRcWFANGVCBjqayOc7GheRFGwPbSYOF1JBHUYsWg6qEgAIdTWWFiXVdwDwg2hjMdxDbce5++9vf0gE6BARVKQEFOMJkNRM3Wq4wINoItlNwzx62w9w988wzdHDKLfjUk9VOXOkTwAHQRtsRgwUUlHKqVzKd8g0Gd1nQpHpGOxpsBwwaUICFi2xgyi04HWa1k2x0+pfJbf9jhR88oKCk+aiSsdpJVmcXx4/42P4PFDzaAYNhA1J20lKEIuDDJc1TOdr6hxW5mIACNiBlp29961u0fpKd5qkcFRdQwAak7KSQKgqWKehCZQcIqcHWQi3DBqTspJAqkibUE0NI7TJFBRUbkLKTQqpYCqqEtv5hRS0qqNiAlJ2w6JXVT4qgT/4S2f4PKyqCqoj5qaEvLK4Fq50URUGVwI4GK+ypqNDZaZ3UerjPFqudFEdB1RNttMLiyxVZwbPAJR9sYMotup1wVRRUPdBGsMLuNvhYlRXdVe5bBtcI1zey2kmxFFQd0cbACnuHGWRCXfNSq2m1eZUUVB3QxpgVN/s81auvvkoHp3ww++Uvf0lrJlXQ3T5boo2MFfeAyXb6p3tKLaf1UdXTOqoWaOMyVlyc/mW7pbBu2bKTbtEyGgqqhmjjOlbgY1HBXeBoCl/jxAbrVOkoajRwVqKLkhugjU2gwMb9qErLEW7BPB2rkVQLQaUveViDNrZhRcZRletclRZ3fvTlC/pEb5R0P6o1aGNbVmTMVeEm9Wwn9IbBOeXTPrx3ffHCqF1g40o+Qhu7smLvMbgBGNsRvWCQTjWoTp8+TWsio6KlCUvQxr6s4LisJvkp4NSCCu9VK8snRTfNI2hjClZw3FXhuEkaVggqXFzLBrUXBAWOZnIGpE7xJkkT6QRtTMmKnjysMEeVYw0VJqsXgwJLInIEJD4o0CT5ZF1i42jKaKMHK37ysMKaIa9r/LD0YVlQnDt3zuWoSqd3Mqf5qQW00ZPtAITVyws7pDcM7BRhhZDAWqQmd7xEgCHIUoQVth3Bp6MnWaD5qTna6M12AI6o2I7pBadmCJk2gYWQwQW7CLquIYH5Kpx+tgksbCMeo0/uZAl8Sq71U4Y2erPiu4TUIgQOTgdxhIIjnhjCwWNiGkdheG72moBtanKkJmJOsfEzNbTRmxXfPaRERmLyp3200ZsVXiEl0szkT/toozcrukJKpLlJn/bRRm9W9CQh9ZWvfGX25JNP0p+JjMxkT/toozcreO+QOnPmzOzGjRtbNjc3tyal0baxsUF/X6Rym2wsTQFt9GYF7xVSiwG1zJUrV7aC6/nnn589++yzsxMnTtDnygFHe9gGbAu2Cdv25ptvKlClrWNsPI0dbfRmxe4cUk0CahUcdSEkLl68ODt//vyW5557bitEgqankIuPgfB8IYjwWmwbgmvXrimopA1crTG5SXTa6M0K3TmkMKgxuNmgrw1CTHNq0tLkvhaLNnqzQvc63RtDUCmgpIdJ3SmBNnqzIveeOK85qBRQ0tOk7pRAG71ZkXuHFNQYVAooSWQySxJoozcrcJKQgpqCSgElCU3maIo2erMCJwspqCGoFFDiYBJHU7TRmxU3aUhByUGlgBInkziaoo3erLjJQwouX75MQ2JoWMTJtlckgdEfTdFGb1bY5CGFxZksIEqBRahsu0V6Gv3RFG30ZoVNGlKlB1SgoBInu9k4Gwva6M2KmiykagmoQEElDka9Cp02erOiJgmp2gIqUFCJg9GuQqeN3qygvUOq1oAKFFSS2Gi/Bos2ekNBowK3UntABQoqSegmG2tjQBu9WUE7hxRuhcIGfK1wixf2PkU6OMzGW+1oozcrZueQwqJILI5kA742OCJk71Gko1EuR6CN3qyYvU73xhBUCihxMroJdNrozQrZe+K85qBSQImj0X2zDG30ZoXsHVJQY1ApoMTZdTbmakYbvVkhk4QU1BRUCijJZFTX89FGb1bEZCEFNQSVAkoyGtUKdNrozYqYNKSg5KBSQElmo1ozRRu9WRGThxRgzRELiaGxbRVxdoCNvRrRRm9WQIWUiK/RfMpHG71ZARVSIr5G8ykfbfRmBVRIifgbxX2maKM3K55CSsTfMTb+akMbvVnxFFIi/kZxLR9t9GbFU0iJ5LGLjcGa0EZvVjiFlEge1S9FoI3erHAKKZE8ql+KQBu9WeEUUiJ5VD8vRRu9WeEUUiKZxOOvNrTRmxVOISWST9V3RaCN3qxoCimRfKpeL0UbvVnRFFIi+Vxg47AWtNGbFU0hJZLPJhuHtaCN3qxoCimRjOIxWBPa6M2KppASyavayXPa6M0KppASyavaLw6ljd6sYAopkbyOs7FYA9roDQWLCpiEQkpkqWpXntNGb1YwhZRIXtV+wkcbvVnBFFIimcXjsBa00ZsVTCElkl+V95aijd6sWAopkfyqXIZAG71ZsRRSIvkppJqyYimkRPKrchkCbfSGYkXFS0IhJbKSQqopFCsqXhIKKZGVzrHxWDra6M2KpZASye+/2XgsHW30ZsVSSInkV+VXr9NGb1YshZRIfu+x8Vg62ujNiqWQEsnvr2w8lo42erNiKaREBhCPxRrQRm9WLIWUyADisVgD2ujNiqWQEhlAPBZrQBu9WbEUUiIDiMdiDWijNyuWQkpkAPFYrAFt9GSF2m1uLhYuFYVUGo899hhtl1Go7l7ntNGLFcgtoEAhlYZCavSqCira6MEK4xpQoJBKQyE1CdUEFW1MzQriHlCgkEpDITUZVQQVbUzJCpEloEAhlcajjz5K22WUig8q2piKFSBbQIFCKo1Dhw7RdhmtooOKNqZgbzxrQIFCKg2F1CQVG1S0MQV709ejIrhTSKVx//3303YZvSLvgU4bU7A3rCOpObatJTt48CBtl1E7y8ZxCWhjKvbGNSdl2LaW7J577qHtMlrFBhTQxpSsAPp0j2xryfbt2zd7/PHH6c9kdIoOKKCNqVkhsgSVQioNhNSRI0foz2RUig8ooI0erCDuQaWQSgMh9eCDD9KfyWhUEVBAG71YYVyDSiGVBkJq//799GcyCtUEFNBGT1Ygt6BSSKWBkLrrrrvoz6R6VQUU0EZPViSFVOEQUnfeeaeu4RsnhdQqViCd7lUghNRDDz1Efy7V0+keY4XRxHklQkjh3+znMgqaOF9kBXEPKFBIpRFCCrReatSqCCramJIVIktAgUIqjcWQ0sXGo1d8UNHGVKwA2QIKFFJpLIaUTvkmoeigoo0p2BvPGlCgkEpjMaTg6NGj9PdkVIoNKtqYgr3pS1ER3Cmk0ohDSqvPJ2Nyt2rZZTYXCuBOIZVGHFJa2DkJ07vpHdgbzxpUCqk04pACTaCP2jRvHxxYAbIF1cbGBg2JobFtLRkLqT179tDflepN+4sYAitEtqBiITE0tp0lYyEFOpoaneIDCmijBytIlqBiITE0tp0lWxZSOpoalSoCCmijFyuMe1BduXKFBsWQ2HaWbFlIgY6mRqGagALa6MkK5BpUFy9epEExJLadJVsVUjia0qUyVSsioGxc7DZ7zGFzbP7fdAnEjoYcrFDHo8Ilc+bMGRoUQ2LbWbJVIQVaN1WveCzmZGPhgLlgboaxscSmQXDtwuPok3mzYrmFVImf8LHtLNm6kMK6Ka1Cr1M8FnOwMYBwur44JhpCmB2nT+rNiuUWUvDmm2+yNzwYto0lWxdSgN9hj5WyxWPRk/X9XQZHTnRcNEWf3JsVyzWkSpuXYttYsiYhBbopXn3isejF+j0CCqdtdEy0QV/AmxXLNaSee+45+maHwraxZE1DSqd99YnHogfr88kCCuiLeLNiuYYUlHTKx7avZE1DCvbu3UufQ8oUj0UP1ucvxWOgD/oi3qxY7iF1/vx5+oaHwLavZG1CCg4ePEifR8oTj8XUrL8fj/t/X/SFvFmx3EPqxIkT9A0PgW1fydqGFGiRZx3isZiS9XWc5q1bXtAafTFvViz3kIJSJtDZtpWsS0iBvgKrfPFYTMn6evKjKKAv5s2KlSWkSjmaYttWsq4hhYl0BVXZ4rGYkvX1Lmuh1qIv5s2KlSWkoISjKbZdJesaUoCJdF02U654LKZi/RyXudD+3xd9QW9WrGwh9eSTT86uXbtG33wubLtK1iekQEFVrngspmL93OVUD+gLerNiZQspeP755+mbz4VtU8n6hhQoqMoUj8VUrJ+fjft9KvQFvVmxsoYUDHkLF7Y9JUsRUqCgKk88FlOxfp50bdQi+oLerFjZQ2rI0z62PSVLFVKgyfSyxGMxFevnCqkUhvqiBrYtJUsZUoCgOnLkCH0tySsei6lYP1dIpTLE/abYdpQsdUgFuiB5ePFYTMX6efJFnAF9QW9WrMFCCnIvS2DbUDKvkIL77rtP81QDisdiCtbHsdKc9v0U6It6s2INGlKQM6jY65fMM6QAtyDWPNUw4rGYgvVx3NSO9v0U6It6s2INHlKQK6jYa5fMO6QC3YY4v3gspmB93G35AdAX9WbFKiKkIMccFXvdkuUKKcAyBU2q5xOPxb6sf7ue6gF9YW9WrGJCCnCTPM/lCew1S5YzpALNVeURj8W+rH+7rTQP6At7s2IVFVKAi5E3Nzdpkfpir1eyIUIKsFQBp4AKKz/xWOzD+rbb9XqL6It7s2IVF1IBbpaX+qiKvU7JhgqpQGHlajcbk21Zv056i+BV6AZ4s0IVG1KAo6rLly/TgnXBXqNkQ4dUgLDCXT91H/WkjrMx2Zb1a9fJ8kV0A7yhUFHhioQV6imu+WPPXbJSQmrR/v37Z4888gjdXmnlutn60s0urD/jCCpbQAHdEG9WpCpCKkBY9VmuwJ6zZCWGVICjK0yyK7B6OcvG5TrWlzEHleUUbxHdGG9WpKpCKsBFyrjtS9ujK/ZcJSs5pBYhsHCEhfura3Foa42Dyvowjp7cP8Vbhm6UNytQlSG1CIGFpQsvvfTS2tBijy9ZLSEVQ2hh2zHpjiMtBddaOPU7zMao9VsEE1aSZz21Y3ZsXEr2AncYvFGk8CmDK6UvXb169ToGNuA0Cp+oYVHlxsYGK2QVEFqnT5/eej8/+9nPtr73LwjvFZPxeK84GsMpJHueEniGFJ7785///Ox73/vell/84hcUaoSff/WrX92aOMeCz64UVo389eTJk//1ne98Z/OnP/3p22+99dZ7NlZpaORGw6Ure0Kk72GD73/vfFU0BjQ6KT5lI8UsRjiS6vNFpFibhecoKaBTh9QXv/jF2Y9+9KPZr371K1qDJkqs09jhL14cPLzxxhtudzhogoZNW/ZEe4zLYSECC4ViRRwCghODxWOFOsIO4YzOwV47lxQhdf/9928dCfUJ8GXwnDgiHbpOU4Ijfzu6+pDtD280dJqyJ0A4ud3sahE65pBhhXDKdUEyAnDIQdgnpBBOL774In1fqQ1dp6lBnXONgUU0fNaxB2KuCad09Ek94bA/53wOdgwGAtsWbxiEQwRz15DCkZPHEeY6eE0cgbL3IumhT7L94IWG0Cr2oGNm0HNUwCmX99+gmP/wOF1pC6e8Oefn2obUww8/3Gu+KRX8BVb6POZY4C8Ftg880CBi7JezrzRdx7NT5twJTeBoARP1bFtTaxNSJ0+epNs7lKGOPqco5aVjq9BAitkvIqCyrzRtAp0y9Sc+Q5x3N5VjADYNqVxzT13gFJ29N0kHZzI5Tu9pKC2yX8JSeJfveE8pxeBF0XP97dAHQpRtfypNQqrkgAq86yR55qdoMAX2C5ggH3z+qam+p0OY+2HPWyLPAbgupGoIqEBB5c/7aIqGE9gPiz3FW6bPqV/Jp3jLeJ36rQqpmgIq0KmfL3yIxeqeyCkaUGA/zLL+KTUEVdtP/YZaYpCCx3KMZSFV2iR5G7k+dJgi9EFW8wRwkLRrWUANdsVzCjhtY8VkHAucRZdQXoeFFJYZsNevBeqk5Ql+WM17wjTT1l1EWUBluW+xtyaL+zC4S1gH1VebUG6ChVQJ66D6Sl0nucVhHG3fnYGFVFXzUMs0+ZvT+Vw6q5SnM3FIYSU5e80aaWW6j8QfOp1azKQ4oHAHA/agKq36ZAcBxh5TK/xNlvK0LwQUrsVD4LPXrJHH6bEkDakdN+NbDCh8mlfNcoOmlk0s1/hp3jqpPsX68pe/vB1SNX6at44+7UsvUUjRu4Vu/4f9wqiOogIszowLOrajqABHCfF77eIHP/jB9lEUe53a6WgqPVbnlpbeznj7P+yXil9V3lU8NzXGo6ig79qpb3zjG9shdfbsWfoaY6C5qXSwNpHVuIWV91vf+of9Eu4LxR48CouH9/gbdExzLDFcdL3Ygdp64YUXtkNqzHXCHB57/9Jez4vxb5skZ7b+Yb9Y1N0NUlvskDmuNRpan/VAf/rTn7ZCCrf8Zc89JroVcRr4i5HVdw3Mf9MvgYht/WP+APZEoxE6ZA0XEPfV9VQGyxjwByE1xgnzmCbQ++u4GBrLnBp/3TsCahSLN9cJA3fMpzAB+7Cgibffftv6xEchNYZFruv0PTWWTp/q4VujWn2DMkIKd9pkTzYqGLgJJviq0OVTPsxFhT8XLlygzztGrBbSTMu5KBw97bHuRYNoldHPRwU4MpjCfFTQZr4Fn+gt/nn11Vfpc46RxwXaU4D+1fCsBFNJx6xb0QBqAiFV5d0Ouqj5bgdtNb1MBgH14YcfWl+49ec3v/kNfc4x0lKE9hoGFMIJNypodWrHIKTYC4xSx08hqtRkUhhBFgcU/rzxxhv0OcdIk+ft4Mjzj3/84/+xWs5hvSUWhvcOp0AhNVKrBt9TTz01e+WVV2z/8z/vvPMOfc4x0p07m8H6whVnIjhqwrRR40/s2lBIjRTu8BB3NIQTJsjff/992/fL/0wppHT7ltUQTpjL/cMf/vC3qHaYCMcndZ0mw9uYVEhdvXqVto8RAhmnc4Cjpt/97ne2v5v9UUhNExYB43QOfvzjH7//+uuvv2undn+x/vCa1QqBhJUA7qF0u9nH/h+sBaOnOz4IxQAAAABJRU5ErkJggg==",
        "contentType": "image/png"
    }, {
        "@microsoft.graph.temporaryId": "2",
        "contentBytes": "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",
        "contentType": "image/png"
    }]
}
```

#### <a name="response"></a><span data-ttu-id="09730-193">响应</span><span class="sxs-lookup"><span data-stu-id="09730-193">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2')/messages/$entity",
    "id": "1616992043931",
    "replyToId": null,
    "etag": "1616992043931",
    "messageType": "message",
    "createdDateTime": "2021-03-29T04:27:23.931Z",
    "lastModifiedDateTime": "2021-03-29T04:27:23.931Z",
    "lastEditedDateTime": null,
    "deletedDateTime": null,
    "subject": null,
    "summary": null,
    "chatId": null,
    "importance": "normal",
    "locale": "en-us",
    "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616992043931?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616992043931&parentMessageId=1616992043931",
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
        "content": "<attachment id=\"74d20c7f34aa4a7fb74e2b30004247c5\"></attachment>"
    },
    "channelIdentity": {
        "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
        "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
    },
    "attachments": [
        {
            "id": "74d20c7f34aa4a7fb74e2b30004247c5",
            "contentType": "application/vnd.microsoft.card.adaptive",
            "contentUrl": null,
            "content": "{  \"type\": \"AdaptiveCard\",  \"body\": [    {      \"items\": [        {          \"columns\": [            {              \"width\": \"auto\",              \"items\": [                {                  \"size\": \"medium\",                  \"url\": \"https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/1616992043931/hostedContents/aWQ9LHR5cGU9MSx1cmw9aHR0cHM6Ly91cy1hcGkuYXNtLnNreXBlLmNvbS92MS9vYmplY3RzLzAtd3VzLWQyLWEyNDc1OWVjOGZiZDRmOWFjYTkxN2M5N2EyOGNlNTQ1L3ZpZXdzL2ltZ28=/$value\",                  \"height\": \"auto\",                  \"type\": \"Image\"                },                {                  \"horizontalAlignment\": \"center\",                  \"text\": \"SHADES\",                  \"weight\": \"bolder\",                  \"type\": \"TextBlock\"                }              ],              \"type\": \"Column\"            },            {              \"width\": \"stretch\",              \"items\": [                {                  \"horizontalAlignment\": \"center\",                  \"text\": \"08/31/2019 19:30:00\",                  \"type\": \"TextBlock\"                },                {                  \"horizontalAlignment\": \"center\",                  \"text\": \"Final\",                  \"spacing\": \"None\",                  \"type\": \"TextBlock\"                },                {                  \"horizontalAlignment\": \"center\",                  \"size\": \"extraLarge\",                  \"text\": \"40 - 7\",                  \"type\": \"TextBlock\"                }              ],              \"spacing\": \"Medium\",              \"separator\": true,              \"type\": \"Column\"            },            {              \"width\": \"auto\",              \"items\": [                {                  \"horizontalAlignment\": \"center\",                  \"size\": \"medium\",                  \"url\": \"https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/1616992043931/hostedContents/aWQ9LHR5cGU9MSx1cmw9aHR0cHM6Ly91cy1hcGkuYXNtLnNreXBlLmNvbS92MS9vYmplY3RzLzAtd3VzLWQ1LTg1ZmNmMDQyNDc3MDJjNjkxODdiOTMwZjcwNTY3OTFhL3ZpZXdzL2ltZ28=/$value\",                  \"height\": \"auto\",                  \"type\": \"Image\"                },                {                  \"horizontalAlignment\": \"center\",                  \"text\": \"SKINS\",                  \"weight\": \"bolder\",                  \"type\": \"TextBlock\"                }              ],              \"spacing\": \"Medium\",              \"separator\": true,              \"type\": \"Column\"            }          ],          \"type\": \"ColumnSet\"        }      ],      \"type\": \"Container\"    }  ],  \"speak\": \"The Seattle Seahawks beat the Carolina Panthers 40-7\",  \"$schema\": \"http://adaptivecards.io/schemas/adaptive-card.json\",  \"version\": \"1.2\"}",
            "name": null,
            "thumbnailUrl": null
        }
    ],
    "mentions": [],
    "reactions": []
}
```

## <a name="see-also"></a><span data-ttu-id="09730-194">另请参阅</span><span class="sxs-lookup"><span data-stu-id="09730-194">See also</span></span>

- [<span data-ttu-id="09730-195">卡参考</span><span class="sxs-lookup"><span data-stu-id="09730-195">Cards reference</span></span>](/microsoftteams/platform/concepts/cards/cards-reference)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Send message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
