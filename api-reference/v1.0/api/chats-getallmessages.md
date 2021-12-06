---
title: 聊天： getAllMessages
description: 从用户参与的所有聊天中获取消息。
author: RamjotSingh
ms.localizationpriority: high
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 998be54216d3e961b89527f39bd657ac63dd2c3e
ms.sourcegitcommit: 70b3caded085ba8ef15e389f81fa005506f1e2fb
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/20/2021
ms.locfileid: "61131906"
---
# <a name="chats-getallmessages"></a>聊天： getAllMessages

命名空间：microsoft.graph

从用户参与的所有 [聊天](../resources/chat.md) 中获取所有 [消息](../resources/chatmessage.md)，包括一对一聊天、群组聊天和会议聊天。

[!INCLUDE [teams-model-A-and-B-disclaimer](../../includes/teams-model-A-and-B-disclaimer.md)]

## <a name="permissions"></a>权限

以下权限需要调用此 API。要了解详细信息，包括如何选择权限，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）| 不支持。 |
|委派（个人 Microsoft 帐户） | 不支持。 |
|应用程序 | Chat.Read.All、Chat.ReadWrite.All |

> [!NOTE]
> 在使用应用程序权限调用此 API 之前，必须先请求访问权限。 有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->
``` http
GET /users/{id | user-principal-name}/chats/getAllMessages
```

## <a name="optional-query-parameters"></a>可选的查询参数

可以使用 `model` 查询支持基于首选许可和付款要求的 `A` 和 `B` 值的参数，如以下示例所示。  

```http
GET /users/{id | user-principal-name}/chats/getAllMessages?model=A
GET /users/{id | user-principal-name}/chats/getAllMessages?model=B
```
如果未指定 `model`，将使用 [评估模式](/graph/teams-licenses#evaluation-mode-default-requirements)。

此操作还支持 [日期范围参数](/graph/query-parameters)来自定义响应，如下例所示。

``` http
GET /users/{id}/chats/getAllMessages?$top=50&$filter=lastModifiedDateTime gt 2020-06-04T18:03:11.591Z and lastModifiedDateTime lt 2020-06-05T21:00:09.413Z
```

## <a name="request-headers"></a>请求标头
| 标头       | 值 |
|:---------------|:--------|
| Authorization  | Bearer {token}。必需。 |

## <a name="response"></a>响应

如果成功，此方法将在正文中返回 `200 OK` 响应代码和[chatMessages](../resources/chatmessage.md) 的列表。

## <a name="example"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chat_getallmessages_1"
}-->
``` http
GET https://graph.microsoft.com/v1.0/users/0b4f1cf6-54c8-4820-bbb7-2a1f4257ade5/chats/getAllMessages?$top=2
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chat-getallmessages-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chat-getallmessages-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chat-getallmessages-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chat-getallmessages-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/chat-getallmessages-1-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->
``` http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(chatMessage)",
    "@odata.count": 2,
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/users('0b4f1cf6-54c8-4820-bbb7-2a1f4257ade5')/chats/getallMessages?$top=2&$skiptoken=U2tpcFZhbHVlPTIjTWFpbGJveEZvbGRlcj1NYWlsRm9sZGVycy9UZWFtc01lc3NhZ2VzRGF0YQ%3d%3d",
    "value": [
        {
            "@odata.type": "#microsoft.graph.chatMessage",
            "id": "1621973534864",
            "replyToId": null,
            "etag": "1621973534864",
            "messageType": "message",
            "createdDateTime": "2021-05-25T20:12:14.864Z",
            "lastModifiedDateTime": "2021-05-25T20:12:14.864Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": "19:3c9e92a344704332bbf5bda58f4d37b1@thread.v2",
            "importance": "normal",
            "locale": "en-us",
            "webUrl": null,
            "channelIdentity": null,
            "policyViolation": null,
            "eventDetail": null,
            "from": {
                "application": null,
                "device": null,
                "user": {
                    "id": "0b4f1cf6-54c8-4820-bbb7-2a1f4257ade5",
                    "displayName": "user1 a",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "text",
                "content": "Hello user2, user 3"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
        },
        {
            "@odata.type": "#microsoft.graph.chatMessage",
            "id": "1622762567488",
            "replyToId": null,
            "etag": "1622762567488",
            "messageType": "message",
            "createdDateTime": "2021-06-03T23:22:47.488Z",
            "lastModifiedDateTime": "2021-06-03T23:22:47.488Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": "19:0b4f1cf6-54c8-4820-bbb7-2a1f4257ade5_0d7c63d3-1306-4eec-8f21-588a70fb6ef1@unq.gbl.spaces",
            "importance": "normal",
            "locale": "en-us",
            "webUrl": null,
            "channelIdentity": null,
            "policyViolation": null,
            "eventDetail": null,
            "from": {
                "application": null,
                "device": null,
                "user": {
                    "id": "0b4f1cf6-54c8-4820-bbb7-2a1f4257ade5",
                    "displayName": "user1 a",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "text",
                "content": "hi user2"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
        }
    ]
}
```
