---
title: 使用 Microsoft Graph 获取 Teams 频道和聊天中消息的更改通知
description: 更改通知使你能够收听对频道或聊天中消息的更改
author: RamjotSingh
localization_priority: Priority
ms.prod: microsoft-teams
ms.custom: scenarios:getting-started
ms.openlocfilehash: 78718b1b486231ae2549323433312aa878806210
ms.sourcegitcommit: e4461c7eb8c3d265fc1aa766125e81b58c6e1099
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2021
ms.locfileid: "52941422"
---
# <a name="get-change-notifications-for-messages-in-teams-channels-and-chats-using-microsoft-graph"></a>使用 Microsoft Graph 获取 Teams 频道和聊天中消息的更改通知

更改通知使你能够订阅频道或聊天中消息的更改（创建、更新和删除）。 更改通知允许你维护订阅，从而提供低延迟模式。 你还可以在通知中获取资源数据，因此避免调用 API 来获取有效负载。

## <a name="subscribe-to-changes-at-the-tenant-level"></a>订阅租户级别的更改

若要跟踪与租户中的消息相关的所有更改，你可以使用租户级别的订阅来处理频道和聊天消息。 这需要你创建两个订阅：一个用于跟踪[频道](/graph/api/resources/channel?preserve-view=true)中的所有消息，另一个用于跟踪[聊天](/graph/api/resources/chat?preserve-view=true)中的所有消息。

### <a name="subscribe-to-messages-across-channels"></a>跨频道订阅消息

若要跨租户中的频道获取所有消息和回复的更改通知，请订阅 `/teams/getAllMessages`。 此资源支持在通知中[包括资源数据](webhooks-with-resource-data.md)。

#### <a name="permissions"></a>权限

|权限类型      | 权限（从最低特权到最高特权）              | 支持的版本 |
|:--------------------|:---------------------------------------------------------|:-------------------|
|委派（工作或学校帐户） | 不支持。 | 不支持。 |
|委派（个人 Microsoft 帐户） | 不支持。    | 不支持。 |
|应用程序 | ChannelMessage.Read.All | beta, v1.0 |

#### <a name="example"></a>示例

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/getAllMessages",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

### <a name="subscribe-to-messages-across-chats"></a>跨聊天订阅消息

若要跨租户中的聊天获取所有消息的更改通知，请订阅 `/chats/getAllMessages`。 此资源支持在通知中[包括资源数据](webhooks-with-resource-data.md)。

#### <a name="permissions"></a>权限

|权限类型      | 权限（从最低特权到最高特权）              | 支持的版本 |
|:--------------------|:---------------------------------------------------------|:-------------------|
|委派（工作或学校帐户） | 不支持。 | 不支持。 |
|委派（个人 Microsoft 帐户） | 不支持。    | 不支持。 |
|应用程序 | Chat.Read.All | beta, v1.0 |

#### <a name="example"></a>示例

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated,deleted",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/chats/getAllMessages",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

## <a name="subscribe-to-messages-in-a-channel"></a>订阅频道中的消息

若要跟踪频道中的消息和回复，可在频道级别创建更改通知订阅。 为此，请订阅 `/teams{id}/channels/{id}/messages`。 此资源支持在 *仅限应用程序模式* 下 [包括通知中的资源数据](webhooks-with-resource-data.md)。

频道级别订阅还支持通过 `$search` 查询参数进行基于关键字的搜索。

### <a name="permissions"></a>权限

|权限类型      | 权限（从最低特权到最高特权）              |版本支持 |
|:--------------------|:---------------------------------------------------------|:--------------------|
|委派（工作或学校帐户） | ChannelMessage.Read.All | beta, v1.0 |
|委派（个人 Microsoft 帐户） | 不支持。    | 不支持。 |
|应用程序 | ChannelMessage.Read.All, ChannelMessage.Read.Group* | beta, v1.0 |

>**注意：** ChannelMessage.Read.Group 作为 [资源特定许可](/microsoftteams/platform/graph-api/rsc/resource-specific-consent)的一部分受支持。

### <a name="example-1-subscribe-to-all-messages-and-replies-in-a-channel"></a>示例 1：订阅频道中的所有消息（和回复）

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{id}/channels/{id}/messages",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

### <a name="example-2-subscribe-to-messages-and-replies-in-a-channel-that-contain-certain-text"></a>示例 2：订阅频道中包含特定文本的消息（和回复）

以下请求将向订阅者发送包含 `Hello` 的消息。

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{id}/channels/{id}/messages?$search=Hello",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

### <a name="example-3-subscribe-to-messages-and-replies-in-a-channel-without-resource-data"></a>示例 3：订阅频道中的消息（和回复），不含资源数据

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{id}/channels/{id}/messages",
  "includeResourceData": false,
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

### <a name="example-4-subscribe-to-messages-and-replies-in-a-channel-that-mention-a-specific-user"></a>示例 4：订阅频道中提到特定用户的消息（和回复）

要仅获得提到特定用户的消息，你可以在查询中指定用户的 ID（在此示例中为 `9a6eb4d1-826b-48b1-9627-b50836c8fee9`）。

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{id}/channels/{id}/messages?$filter=mentions/any(u: u/mentioned/user/id eq '9a6eb4d1-826b-48b1-9627-b50836c8fee9')",
  "includeResourceData": false,
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

## <a name="subscribe-to-messages-in-a-chat"></a>订阅聊天中的消息

若要跟踪聊天中的消息，你可以在聊天级别创建更改通知订阅。 为此，请订阅 `/chats{id}/messages`。 此资源支持在 *仅限应用程序模式* 下 [包括通知中的资源数据](webhooks-with-resource-data.md)。

聊天级别订阅还支持通过 `$search` 查询参数进行基于关键字的搜索。

> **注意。** 订阅聊天中的消息目前在预览中。

### <a name="permissions"></a>权限

|权限类型      | 权限（从最低特权到最高特权）              | 版本支持 |
|:--------------------|:---------------------------------------------------------|:---------------------|
|委派（工作或学校帐户） | Chat.Read | beta, v1.0 |
|委派（个人 Microsoft 帐户） | 不支持。    | 不支持。 |
|应用程序 | Chat.Read.All | beta, v1.0 |

### <a name="example-1-subscribe-to-messages-in-a-chat"></a>示例 1：订阅聊天中的消息

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/chats/{id}/messages",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

### <a name="example-2-subscribe-to-messages-in-a-chat-that-contain-certain-text"></a>示例 2：订阅聊天中包含特定文本的消息

以下请求将向订阅者发送包含 `Hello` 的消息。

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/chats/{id}/messages?$search=Hello",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

### <a name="example-3-subscribe-to-messages-and-replies-in-a-chat-without-resource-data"></a>示例 3：订阅聊天中的消息（和回复），不含资源数据

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json
{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/chats/{id}/messages",
  "includeResourceData": false,
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

### <a name="example-4-subscribe-to-message-in-a-chat-in-which-a-specific-user-is-mentioned"></a>示例 4：订阅聊天中提到特定用户的消息

要仅获得提到特定用户的消息，你可以在查询中指定用户的 ID（在此示例中为 `9a6eb4d1-826b-48b1-9627-b50836c8fee9`）。

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/chats/{id}/messages?$filter=mentions/any(u: u/mentioned/user/id eq '9a6eb4d1-826b-48b1-9627-b50836c8fee9')",
  "includeResourceData": false,
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

## <a name="notification-payloads"></a>通知负载

根据你的订阅，你可以获取包含或不含资源数据的通知。 通过订阅资源数据，你将在收到通知的同时获得消息负载，而无需回调并获取内容。

### <a name="notifications-with-resource-data"></a>包含资源数据的通知

对于包含资源数据的通知，负载如下所示。 此负载适用于在聊天中发送的消息。

```json
{
    "value": [{
        "subscriptionId": "10493aa0-4d29-4df5-bc0c-ef742cc6cd7f",
        "changeType": "created",
        "clientState": "<<--SpecifiedClientState-->>",
        "subscriptionExpirationDateTime": "2021-02-02T10:30:34.9097561-08:00",
        "resource": "chats('19:8ea0e38b-efb3-4757-924a-5f94061cf8c2_97f62344-57dc-409c-88ad-c4af14158ff5@unq.gbl.spaces')/messages('1612289765949')",
        "resourceData": {
            "id": "1612289765949",
            "@odata.type": "#Microsoft.Graph.chatMessage",
            "@odata.id": "chats('19:8ea0e38b-efb3-4757-924a-5f94061cf8c2_97f62344-57dc-409c-88ad-c4af14158ff5@unq.gbl.spaces')/messages('1612289765949')"
        },
        "encryptedContent": {
            "data": "<<--EncryptedContent-->",
            "dataKey": "<<--EnryptedDataKeyUsedForEncryptingContent-->>",
            "encryptionCertificateId": "<<--IdOfTheCertificateUsedForEncryptingDataKey-->>",
            "encryptionCertificateThumbprint": "<<--ThumbprintOfTheCertificateUsedForEncryptingDataKey-->>"
        },
        "tenantId": "<<--TenantForWhichNotificationWasSent-->>"
    }],
    "validationTokens": ["<<--ValidationTokens-->>"]
}
```

有关如何验证令牌和解密负载的详细信息，请参阅[设置包含资源数据的更改通知](webhooks-with-resource-data.md)。

解密的通知负载如下所示。 该负载符合 [chatMessage](/graph/api/resources/chatMessage?preserve-view=true) 架构。 该负载类似于 GET 操作返回的负载。

```json
{
  "id": "1612289992105",
  "replyToId": null,
  "etag": "1612289992105",
  "messageType": "message",
  "createdDateTime": "2021-02-02T18:19:52Z",
  "lastModifiedDateTime": "2021-02-02T18:19:52.105Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": "19:8ea0e38b-efb3-4757-924a-5f94061cf8c2_97f62344-57dc-409c-88ad-c4af14158ff5@unq.gbl.spaces",
  "importance": "normal",
  "locale": "en-us",
  "webUrl": null,
  "from": {
    "application": null,
    "device": null,
    "user": {
      "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
      "displayName": "Ramjot Singh",
      "userIdentityType": "aadUser"
    },
    "conversation": null
  },
  "body": {
    "contentType": "text",
    "content": "test"
  },
  "channelIdentity": null,
  "attachments": [],
  "mentions": [],
  "policyViolation": null,
  "reactions": [],
  "replies": [],
  "hostedContents": []
}
```

### <a name="notifications-without-resource-data"></a>不含资源数据的通知

不含资源数据的通知为你提供了足够的信息来进行 GET 调用以获取消息内容。 订阅不含资源数据的通知不需要加密证书（因为不会发送实际资源数据）。

该负载如下所示。 此负载适用于在频道中发送的消息。

```json
 {
  "subscriptionId": "9f9d1ed0-c9cc-42e7-8d80-a7fc4b0cda3c",
  "changeType": "created",
  "tenantId": "<<--TenantForWhichNotificationWasSent-->>",
  "clientState": "<<--SpecifiedClientState-->>",
  "subscriptionExpirationDateTime": "2021-02-02T11:26:41.0537895-08:00",
  "resource": "teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2')/messages('1612293113399')",
  "resourceData": {
    "id": "1612293113399",
    "@odata.type": "#Microsoft.Graph.chatMessage",
    "@odata.id": "teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2')/messages('1612293113399')"
  }
}
```

**resource** 和 **@odata.id** 属性可用于对 Microsoft Graph 进行调用以获取消息负载。 GET 调用将始终返回消息的当前状态。 如果在发送通知和检索消息之间更改了消息，则该操作将返回更新的消息。

## <a name="see-also"></a>另请参阅
- [Microsoft Graph 更改通知](webhooks.md)
- [Microsoft Teams API 概述](teams-concept-overview.md)
