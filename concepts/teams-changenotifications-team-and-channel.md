---
title: 使用 Microsoft Graph 获取团队和频道的更改通知
description: 了解如何使用 Microsoft Graph API 获取团队和频道的更改（创建、更新和删除）通知。
author: anandab
ms.localizationpriority: high
ms.prod: microsoft-teams
ms.custom: scenarios:getting-started
ms.openlocfilehash: 08a6b996d3ddbe721775a888b161e14788a485a9
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59507764"
---
# <a name="get-change-notifications-for-teams-and-channels-using-microsoft-graph"></a>使用 Microsoft Graph 获取团队和频道的更改通知

通过更改通知，可以订阅对团队和频道所做的更改（创建、更新和删除）。 每当创建、更新或删除团队或频道时，你都可以收到通知。 你还可以在通知中获取资源数据，因此避免调用 API 来获取有效负载。

## <a name="subscribe-to-changes-in-any-team-at-tenant-level"></a>订阅租户级别上任何团队中的更改

要获取与租户中的任何团队相关的所有更改（创建、更新和删除）的更改通知，请订阅 `/teams`。 此资源支持在通知中[包括资源数据](webhooks-with-resource-data.md)。

### <a name="permissions"></a>权限

|权限类型      | 权限（从最低特权到最高特权）              | 支持的版本 |
|:--------------------|:---------------------------------------------------------|:-------------------|
|委派（工作或学校帐户） | 不支持。 | 不支持。 |
|委派（个人 Microsoft 帐户） | 不支持。    | 不支持。 |
|应用程序 | Team.ReadBasic.All，TeamSettings.Read.All，TeamSettings.ReadWrite.All   | beta 版|

### <a name="example"></a>示例

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,deleted,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

## <a name="subscribe-to-changes-in-a-particular-team"></a>订阅特定团队中的更改


要获取与租户中特定团队相关的所有更改的更改通知，请订阅 `/teams/{team-id}`。 此资源支持在通知中[包括资源数据](webhooks-with-resource-data.md)。

### <a name="permissions"></a>权限

|权限类型      | 权限（从最低特权到最高特权）              | 支持的版本 |
|:--------------------|:---------------------------------------------------------|:-------------------|
|委派（工作或学校帐户） | Team.ReadBasic.All，TeamSettings.Read.All，TeamSettings.ReadWrite.All | beta 版 |
|委派（个人 Microsoft 帐户） | 不支持。    | 不支持。 |
|应用程序 | TeamSettings.Read.Group *、TeamSettings.ReadWrite.Group*、Team.ReadBasic.All、TeamSettings.Read.All、TeamSettings.ReadWrite.All    | beta 版 |

>**注意：** 带有 * 标记的权限作为 [ 资源特定的许可](/microsoftteams/platform/graph-api/rsc/resource-specific-consent) 的一部分受到支持。

### <a name="example"></a>示例

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "deleted,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{team-id}",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```


## <a name="subscribe-to-changes-in-any-channel-at-tenant-level"></a>订阅租户级别上任何频道中的更改

要获取与租户中任何频道相关的所有更改（创建、更新和删除）的更改通知，请订阅 `/teams/getAllChannels`。 此资源支持在通知中[包括资源数据](webhooks-with-resource-data.md)。


### <a name="permissions"></a>权限

|权限类型      | 权限（从最低特权到最高特权）              | 支持的版本 |
|:--------------------|:---------------------------------------------------------|:-------------------|
|委派（工作或学校帐户） | 不支持。 | 不支持。 |
|委派（个人 Microsoft 帐户） | 不支持。    | 不支持。 |
|应用程序 | Channel.ReadBasic.All、ChannelSettings.Read.All、ChannelSettings.ReadWrite.All | beta 版 |

### <a name="example"></a>示例

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,deleted,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/getAllChannels",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

## <a name="subscribe-to-changes-in-any-channel-of-a-particular-team"></a>订阅特定团队的任何频道中的更改


要获取与特定团队中任何频道相关的所有更改的更改通知，请订阅 `/teams/{team-id}/channels`。 此资源支持在通知中[包括资源数据](webhooks-with-resource-data.md)。 委派上下文中不支持专用频道更改通知。 在这种情况下，委派上下文中此资源的订阅者将仅接收特定团队下的标准频道的通知，而不是专用频道的通知。


### <a name="permissions"></a>权限

|权限类型      | 权限（从最低特权到最高特权）              | 支持的版本 |
|:--------------------|:---------------------------------------------------------|:-------------------|
|委派（工作或学校帐户） | Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All | beta 版 |
|委派（个人 Microsoft 帐户） | 不支持。    | 不支持。 |
|应用程序 | ChannelSettings.Read.Group *, ChannelSettings.ReadWrite.Group*, Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All   | beta 版 |

>**注意：** 带有 * 标记的权限作为 [ 资源特定的许可](/microsoftteams/platform/graph-api/rsc/resource-specific-consent) 的一部分受到支持。

### <a name="example"></a>示例

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,deleted,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{team-id}/channels",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```


### <a name="notifications-with-resource-data"></a>包含资源数据的通知

对于包含资源数据的通知，负载如下所示。 此有效负载用于团队中的属性更改。

```json
{
    "value": [{
        "subscriptionId": "10493aa0-4d29-4df5-bc0c-ef742cc6cd7f",
        "changeType": "created",
        "clientState": "<<--SpecifiedClientState-->>",
        "subscriptionExpirationDateTime": "2021-02-02T10:30:34.9097561-08:00",
        "resource": "teams('fb82c19a-0f6d-41ed-90f0-cbb29a476ede')",
        "resourceData": {
            "id": "1612289765949",
            "@odata.type": "#Microsoft.Graph.Team",
            "@odata.id": "teams('fb82c19a-0f6d-41ed-90f0-cbb29a476ede')"
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



已解密的通知有效负载如下所示。 有效负载符合 [团队](/graph/api/resources/team?preserve-view=true) 架构。 该有效负载类似于 GET 操作返回的负载。

>**注意：** [discoverySettings](/graph/api/resources/teamdiscoverysettings?preserve-view=true) 和 [classSettings](/graph/api/resources/teamclasssettings?preserve-view=true) 不会在有效负载数据中公开。

```json
{
  "id": "4c533ad3-e1dd-4277-a672-92ab64ed225c",
  "createdDateTime": "2021-03-18T10:31:14.597Z",
  "displayName": "Sample name",
  "description": "Sample description",
  "internalId": "19:2077546f765a42c1ba71236f4df70aa2@thread.tacv2",
  "specialization": "none",
  "visibility": "public",
  "webUrl": "https://teams.microsoft.com/l/team/19:2077546f724a42c1ba71236f4df79aa2%40thread.tacv2/conversations?groupId=4c533ad3-e1dd-4277-a672-92ab64ed225c&tenantId=0f2e8f59-862a-483b-9ca8-82a10665e17d",
  "isArchived": false,
  "isMembershipLimitedToOwners": false,
  "memberSettings": {
    "allowCreateUpdateChannels": true,
    "allowCreatePrivateChannels": true,
    "allowDeleteChannels": true,
    "allowAddRemoveApps": true,
    "allowCreateUpdateRemoveTabs": true,
    "allowCreateUpdateRemoveConnectors": true
  },
  "guestSettings": {
    "allowCreateUpdateChannels": false,
    "allowDeleteChannels": false
  },
  "messagingSettings": {
    "allowUserEditMessages": true,
    "allowUserDeleteMessages": true,
    "allowOwnerDeleteMessages": true,
    "allowTeamMentions": true,
    "allowChannelMentions": true
  },
  "funSettings": {
    "allowGiphy": true,
    "giphyContentRating": "moderate",
    "allowStickersAndMemes": true,
    "allowCustomMemes": true
  }
}
```


对于包含资源数据的通知，有效负载如下所示。 此有效负载用于频道中的属性更改。

```json
{
    "value": [{
        "subscriptionId": "10493aa0-4d29-4df5-bc0c-ef742cc6cd7f",
        "changeType": "created",
        "clientState": "<<--SpecifiedClientState-->>",
        "subscriptionExpirationDateTime": "2021-02-02T10:30:34.9097561-08:00",
        "resource": "teams('fb82c19a-0f6d-41ed-90f0-cbb29a476ede')/channels('19:01f39f5ac52f45fb9a7ce01cedd57b1f@thread.tacv2')",
        "resourceData": {
            "id": "19:01f39f5ac52f45fb9a7ce01cedd57b1f@thread.tacv2",
            "@odata.type": "#Microsoft.Graph.Channel",
            "@odata.id": "teams('fb82c19a-0f6d-41ed-90f0-cbb29a476ede')/channels('19:01f39f5ac52f45fb9a7ce01cedd57b1f@thread.tacv2')"
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
  

已解密的通知有效负载如下所示。 有效负载符合 [频道](/graph/api/resources/channel?preserve-view=true) 架构。 该负载类似于 GET 操作返回的负载。

```json
{
  "id": "19:a3f841d969cd4ae0a7cbe847fc10b371@thread.tacv2",
  "createdDateTime": "2020-02-14T01:10:03.592Z",
  "displayName": "General",
  "description": "Sample Channel description",
  "isFavoriteByDefault": true,
  "email": "",
  "webUrl": "https://teams.microsoft.com/l/channel/19%3Aa3f841d969cd4ae0a7cbe847fc10b371%40thread.tacv2/General?groupId=7ed9bdab-9c7d-4c10-a25d-3f4ff0e34577&tenantId=0f2d8f49-862a-493b-9ca8-82a10637e17d",
  "membershipType": "standard",
  "moderationSettings": null
}
```


### <a name="notifications-without-resource-data"></a>不含资源数据的通知

不含资源数据的通知为你提供了足够的信息来进行 GET 调用以获取消息内容。 订阅不含资源数据的通知不需要加密证书（因为不会发送实际资源数据）。

对于不包含资源数据的通知，有效负载如下所示。 此有效负载用于团队中的属性更改。

```json
{
  "subscriptionId": "9f9d1ed0-c9cc-42e7-8d80-a7fc4b0cda3c",
  "changeType": "created",
  "tenantId": "<<--TenantForWhichNotificationWasSent-->>",
  "clientState": "<<--SpecifiedClientState-->>",
  "subscriptionExpirationDateTime": "2021-02-02T11:26:41.0537895-08:00",
  "resource": "teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')",
  "resourceData": {
    "id": "1612293113399",
    "@odata.type": "#Microsoft.Graph.Teams",
    "@odata.id": "teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')"
  }
}
```

**resource** 和 **@odata.id** 属性可用于对 Microsoft Graph 进行调用以获取消息负载。 GET 调用将始终返回消息的当前状态。 如果在发送通知和检索消息之间更改了消息，则该操作将返回更新的消息。


>**注意：** 有效负载中不返回频道电子邮件地址。

对于不包含资源数据的通知，有效负载如下所示。 此有效负载用于团队中的属性更改。

```json
{
  "id": "19:a3f841d969cd4ae0a7cbe847fc10b371@thread.tacv2",
  "createdDateTime": "2020-02-14T01:10:03.592Z",
  "displayName": "General",
  "description": "Sample Channel description",
  "isFavoriteByDefault": true,
  "email": "",
  "webUrl": "https://teams.microsoft.com/l/channel/19%3Aa3f841d969cd4ae0a7cbe847fc10b371%40thread.tacv2/General?groupId=7ed9bdab-9c7d-4c10-a25d-3f4ff0e34577&tenantId=0f2d8f49-862a-493b-9ca8-82a10637e17d",
  "membershipType": "standard",
  "moderationSettings": null
}
```


## <a name="see-also"></a>另请参阅
- [Microsoft Graph 更改通知](webhooks.md)
- [Microsoft Teams API 概述](teams-concept-overview.md)
