---
title: 使用 Microsoft Graph 获取 Teams 频道和聊天中消息的更改通知
description: 更改通知使你能够收听对频道或聊天中消息的更改
author: RamjotSingh
localization_priority: Priority
ms.prod: microsoft-teams
ms.custom: scenarios:getting-started
ms.openlocfilehash: 1d9767a913b5fe5878cb1cc8e72ec9900fcec4ac
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000713"
---
# <a name="get-change-notifications-for-messages-in-teams-channels-and-chats-using-microsoft-graph"></a>使用 Microsoft Graph 获取 Teams 频道和聊天中消息的更改通知

更改通知使你能够订阅对[频道](/graph/api/resources/channel?preserve-view=true)或[聊天](/graph/api/resources/chat?preserve-view=true)中[消息](/graph/api/resources/chatMessage?preserve-view=true)的更改（创建、更新和删除）。 更改通知允许你维护[订阅](/graph/api/resources/webhooks?preserve-view=true)，从而提供低延迟模式。 你还可以在通知中获取资源数据，因此避免调用 API 来获取有效负载。

>**注意：** 订阅的最长持续时间为 60 分钟；但是，订阅可以续订，直至呼叫方有权访问资源。

## <a name="subscribe-to-changes-at-the-tenant-level"></a>订阅租户级别的更改

若要跟踪与租户中的消息相关的所有更改，你可以使用租户级别的订阅来处理频道和聊天消息。 这需要你创建两个订阅：一个用于跟踪[频道](/graph/api/resources/channel?preserve-view=true)中的所有消息，另一个用于跟踪[聊天](/graph/api/resources/chat?preserve-view=true)中的所有消息。

### <a name="subscribe-to-messages-across-channels"></a>跨频道订阅消息

若要跨租户中的频道获取所有消息和回复的更改通知，请订阅 `/teams/getAllMessages`。 此资源支持在通知中[包括资源数据](webhooks-with-resource-data.md)。

#### <a name="permissions"></a>权限

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | 不支持。 |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | ChannelMessage.Read.All |

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

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | 不支持。 |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Chat.Read.All |

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

若要跟踪频道中的消息和回复，可在频道级别创建更改通知订阅。 为此，请订阅 `/teams{id}/channels/{id}/messages`。 此资源支持在 *仅限应用程序模式* 下[包括通知中的资源数据](webhooks-with-resource-data.md)。

频道级别订阅还支持通过 `$search` 查询参数进行基于关键字的搜索。

### <a name="permissions"></a>权限

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | ChannelMessage.Read.All |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | ChannelMessage.Read.All |

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

## <a name="subscribe-to-messages-in-a-chat"></a>订阅聊天中的消息

若要跟踪聊天中的消息，你可以在聊天级别创建更改通知订阅。 为此，请订阅 `/chats{id}/messages`。 此资源支持在 *仅限应用程序模式* 下[包括通知中的资源数据](webhooks-with-resource-data.md)。

聊天级别订阅还支持通过 `$search` 查询参数进行基于关键字的搜索。

### <a name="permissions"></a>权限

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Chat.Read |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Chat.Read.All |

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

## <a name="see-also"></a>另请参阅
- [Microsoft Graph 更改通知](webhooks.md)
- [Microsoft Teams API 概述](teams-concept-overview.md)
