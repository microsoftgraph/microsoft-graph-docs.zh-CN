---
title: 使用 Microsoft Graph 获取聊天的更改通知
description: 了解如何使用 Microsoft Graph API 获取聊天更改（创建和更新）的通知。
author: RamjotSingh
ms.localizationpriority: high
ms.prod: microsoft-teams
ms.custom: scenarios:getting-started
ms.openlocfilehash: c4effe9ff408f8bd2c26baca0bc0146e0be9da6f
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65898481"
---
# <a name="get-change-notifications-for-chats-using-microsoft-graph"></a>使用 Microsoft Graph 获取聊天的更改通知

更改通知使你能够订阅聊天的更改（创建和更新）。 每当创建或更新聊天时，你都可以收到通知。 你还可以在通知中获取资源数据，因此避免调用 API 来获取有效负载。

## <a name="subscribe-to-changes-in-any-chat-at-tenant-level"></a>在租户级别订阅任何聊天中的更改

要获取与租户中任何聊天相关的所有更改（创建、更新和删除）的更改通知，请订阅 `/chats`。 此资源支持在通知中[包括资源数据](webhooks-with-resource-data.md)。

### <a name="permissions"></a>权限

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | 不支持。 |
|委派（个人 Microsoft 帐户） | 不支持。    |
|Application | Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All   |

### <a name="example"></a>示例

```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/chats",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

## <a name="subscribe-to-changes-in-a-particular-chat"></a>订阅特定聊天中的更改


要获取特定聊天相关的所有更改的更改通知，请订阅 `/chats/{id}`。 此资源支持在通知中[包括资源数据](webhooks-with-resource-data.md)。

### <a name="permissions"></a>权限

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Chat.ReadBasic, Chat.Read, Chat.ReadWrite |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | ChatSettings.Read.Chat *、ChatSettings.ReadWrite.Chat*、Chat.Manage.Chat*、Chat.ReadBasic.All、Chat.Read.All、Chat.ReadWrite.All |

> **注意**：标有 * 的权限用于 [特定于资源的同意](/microsoftteams/platform/graph-api/rsc/resource-specific-consent)。

### <a name="example"></a>示例

```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-Type: application/json

{
  "changeType": "updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/chats/{id}",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```


### <a name="notifications-with-resource-data"></a>包含资源数据的通知

对于包含资源数据的通知，负载如下所示。 此有效负载用于聊天中的属性更改。

```json
{
    "value": [{
        "subscriptionId": "352887e3-9be0-4b6f-a4e6-dec118d857db",
        "changeType": "Created",
        "clientState": "<<--SpecifiedClientState-->>",
        "subscriptionExpirationDateTime": "2021-06-03T09:50:37.719033+00:00",
        "resource": "chats('19:1273a016-201d-4f95-8083-1b7f99b3edeb_976f4b31-fd01-4e0b-9178-29cc40c14438@unq.gbl.spaces')",
        "resourceData": {
            "id": "19:1273a016-201d-4f95-8083-1b7f99b3edeb_976f4b31-fd01-4e0b-9178-29cc40c14438@unq.gbl.spaces",
            "@odata.type": "#microsoft.graph.chat",
            "@odata.id": "chats('19:1273a016-201d-4f95-8083-1b7f99b3edeb_976f4b31-fd01-4e0b-9178-29cc40c14438@unq.gbl.spaces')"
        },
        "EncryptedContent": {
            "data": "<<--EncryptedContent-->>",
            "dataKey": "<<--EnryptedDataKeyUsedForEncryptingContent-->>",
            "encryptionCertificateId": "<<--IdOfTheCertificateUsedForEncryptingDataKey-->>",
            "encryptionCertificateThumbprint": "<<--ThumbprintOfTheCertificateUsedForEncryptingDataKey-->>"
        }
            "tenantId": "<<--TenantForWhichNotificationWasSent-->>"
        }],
    "validationTokens": ["<<--ValidationTokens-->>"]
}
```

有关如何验证令牌和解密负载的详细信息，请参阅[设置包含资源数据的更改通知](webhooks-with-resource-data.md)。

解密的通知负载如下所示。 有效负载符合 [聊天](/graph/api/resources/chat?preserve-view=true) 架构。 该负载类似于 GET 操作返回的负载。

```json
{
  "id": "19:1273a016-201d-4f95-8083-1b7f99b3edeb_976f4b31-fd01-4e0b-9178-29cc40c14438@unq.gbl.spaces",
  "topic": null,
  "createdDateTime": "2021-06-03T14:25:04+05:30",
  "lastUpdatedDateTime": "2021-06-03T14:25:04.387Z",
  "chatType": "oneOnOne",
  "members": [
    {
      "userId": "976f4b31-fd01-4e0b-9178-29cc40c14438",
      "email": null,
      "tenantId": "2432b57b-0abd-43db-aa7b-16eadd115d34",
      "id": "MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOToxMjczYTAxNi0yMDFkLTRmOTUtODA4My0xYjdmOTliM2VkZWJfOTc2ZjRiMzEtZmQwMS00ZTBiLTkxNzgtMjljYzQwYzE0NDM4QHVucS5nYmwuc3BhY2VzIyM5NzZmNGIzMS1mZDAxLTRlMGItOTE3OC0yOWNjNDBjMTQ0Mzg=",
      "roles": [],
      "displayName": null,
      "visibleHistoryStartDateTime": "1970-01-01T00:00:00Z",
      "user": null
    },
    {
      "userId": "ee723d3d-22d0-4394-9c32-5764d68f4672",
      "email": null,
      "tenantId": "2432b57b-0abd-43db-aa7b-16eadd115d34",
      "id": "MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOToxMjczYTAxNi0yMDFkLTRmOTUtODA4My0xYjdmOTliM2VkZWJfOTc2ZjRiMzEtZmQwMS00ZTBiLTkxNzgtMjljYzQwYzE0NDM4QHVucS5nYmwuc3BhY2VzIyNlZTcyM2QzZC0yMmQwLTQzOTQtOWMzMi01NzY0ZDY4ZjQ2NzI=",
      "roles": [],
      "displayName": null,
      "visibleHistoryStartDateTime": "1970-01-01T00:00:00Z",
      "user": null
    }
  ],
  "messages": [],
  "installedApps": [],
  "tabs": [],
  "permissionGrants": [],
  "operations": []
}
```

### <a name="notifications-without-resource-data"></a>不含资源数据的通知

以下有效负载描述在请求中发送的信息，以获取不含资源数据的通知。 此特定有效负载表示已创建新的聊天。

```json
{
    "subscriptionId": "8d85051d-779d-45bc-be92-e433f0a5d8ac",
    "changeType": "Created",
    "tenantId": "<<--TenantForWhichNotificationWasSent-->>",
    "clientState": "<<--SpecifiedClientState-->>",
    "subscriptionExpirationDateTime": "2021-06-03T10:26:09.8959595+00:00",
    "resource": "chats('19:1273a016-201d-4f95-8083-1b7f99b3edeb_976f4b31-fd01-4e0b-9178-29cc40c14438@unq.gbl.spaces')",
    "resourceData": {
        "id": "19:1273a016-201d-4f95-8083-1b7f99b3edeb_976f4b31-fd01-4e0b-9178-29cc40c14438@unq.gbl.spaces",
        "@odata.type": "#microsoft.graph.chat",
        "@odata.id": "chats('19:1273a016-201d-4f95-8083-1b7f99b3edeb_976f4b31-fd01-4e0b-9178-29cc40c14438@unq.gbl.spaces')"
    }
}
```

**resource** 和 **@odata.id** 属性可用于对 Microsoft Graph 进行调用以获取消息详细信息负载。 GET 调用将始终返回聊天详细信息的当前状态。 如果聊天详细信息在发送通知和检索聊天详细信息之间更新了，则该操作将返回更新的聊天详细信息。

## <a name="see-also"></a>另请参阅
- [Microsoft Graph 更改通知](webhooks.md)
- [Microsoft Teams API 概述](teams-concept-overview.md)
