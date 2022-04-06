---
title: 列出聊天中的消息
description: '在聊天中检索消息列表。 '
ms.localizationpriority: high
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3fd8240f4d07e82e01c5893ac6c68a9a6dcd2296
ms.sourcegitcommit: 0e7927f34b7e55d323acbf281e11560cb40a89ed
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2022
ms.locfileid: "63671578"
---
# <a name="list-messages-in-a-chat"></a>列出聊天中的消息

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在[聊天](../resources/chat.md)中检索[消息](../resources/chatmessage.md)列表。

> **注意**：此 API 支持使用 [更改通知](../resources/webhooks.md)订阅更改（创建、更新和删除）。 这使呼叫方可以实时订阅和获取更改。 有关详细信息，请参阅[获取消息通知](/graph/teams-changenotifications-chatmessage)。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Chat.Read、Chat.ReadWrite |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | ChatMessage.Read.Chat*、Chat.Read.All、Chat.ReadWrite.All |

> **注意**：标有 * 的权限用于 [特定于资源的同意](/microsoftteams/platform/graph-api/rsc/resource-specific-consent)。

> [!NOTE]
> 在使用应用程序权限调用此 API 之前，你必须先请求访问权限。 有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->
```http
GET /me/chats/{chat-id}/messages
GET /users/{user-id | user-principal-name}/chats/{chat-id}/messages
GET /chats/{chat-id}/messages
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持以下 [OData 查询参数](/graph/query-parameters)。

| 名称      | 说明          |
|:----------|:---------------------|
| [$top](/graph/query-parameters#top-parameter)| 控制每个响应的项数。 允许的最大 `$top` 值为 50。 |
| [$orderBy](/graph/query-parameters#orderBy)  | 当前支持 **降序** 排序的 **LastModifiedDateTime（默认）** 和 **CreatedDateTime**。 目前不支持升序顺序。|

目前不支持其他 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头

| 标头       | 值 |
|:---------------|:--------|
| Authorization  | Bearer {token}。必需。  |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [chatMessage](../resources/chatmessage.md) 对象集合。

## <a name="example"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。 传递 `$top=2` 以检索两条消息，并传递 `$orderBy=createdDateTime` 以按 **createdDateTime** 对消息进行排序。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_allchatmessages_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/19:2da4c29f6d7041eca70b638b43d45437@thread.v2/messages?$top=2&$orderBy=createdDateTime desc
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-allchatmessages-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-allchatmessages-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-allchatmessages-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-allchatmessages-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-allchatmessages-1-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-allchatmessages-1-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应
以下示例显示了相应的响应。

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
    "@odata.count": 3,
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
            "onBehalfOf": null,
            "policyViolation": null,
            "eventDetail": null,
            "from": {
                "application": null,
                "device": null,
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
            "onBehalfOf": null,
            "policyViolation": null,
            "eventDetail": null,
            "from": {
                "application": null,
                "device": null,
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
        },
        {
            "id": "1615943825123",
            "replyToId": null,
            "etag": "1615943825123",
            "messageType": "systemEventMessage",
            "createdDateTime": "2021-03-1706:47:05.123Z",
            "lastModifiedDateTime": "2021-03-1706:47:05.123Z",
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
            "from": null,
            "body": {
                "contentType": "html",
                "content": "<systemEventMessage/>"
            },
            "attachments": [],
            "mentions": [],
            "onBehalfOf": {
                "application": null,
                "device": null,
                "user": {
                    "id": "6703568a-3b0e-4a3b-9d33-0e1bc5ff1521",
                    "displayName": "Test User",
                    "userIdentityType": "aadUser"
                }
            },
            "reactions": [],
            "eventDetail": {
                "@odata.type": "#microsoft.graph.chatRenamedEventMessageDetail",
                "chatId": "19:2da4c29f6d7041eca70b638b43d45437@thread.v2",
                "chatDisplayName": "Graph Members",
                "initiator": {
                    "application": null,
                    "device": null,
                    "user": {
                        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
                        "displayName": null,
                        "userIdentityType": "aadUser"
                    }
                }
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
  "description": "Get chat messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

