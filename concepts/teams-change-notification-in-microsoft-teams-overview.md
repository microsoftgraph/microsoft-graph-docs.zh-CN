---
title: 使用 Microsoft Graph 更改 Microsoft Teams 资源的通知
description: 了解如何使用 Microsoft Graph API 获取 Microsoft Teams 中资源的更改（创建、更新和删除）通知
author: anandab-msft
ms.localizationpriority: high
ms.prod: microsoft-teams
ms.custom: scenarios:getting-started
ms.openlocfilehash: 821c45642ecd50154f8d618496264657b98160b8
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59138937"
---
# <a name="change-notifications-for-microsoft-teams-resources-using-microsoft-graph"></a>使用 Microsoft Graph 更改 Microsoft Teams 资源的通知

通过更改通知，可以订阅资源的更改（创建、更新和删除）。 更改通知允许你维护[订阅](/graph/api/resources/webhooks?preserve-view=true)，从而提供低延迟模式。 你还可以在通知中获取资源数据，因此避免调用 API 来获取有效负载。

> **注意：** 订阅的最长持续时间为 60 分钟；但是，订阅可以续订，直至呼叫方有权访问资源。

## <a name="change-notification-types"></a>更改通知类型
Microsoft Teams 支持两种类型的更改通知：
- **更改通知以跟踪与租户中的资源相关的所有更改** - 例如，你可以订阅租户范围内任何通道中的消息更改，并在租户中的任何通道中创建、更新或删除消息时收到通知。
- **更改通知以跟踪特定资源的所有更改** - 例如，你可以订阅特定通道中的消息更改，并在该通道中创建、更新或删除消息时收到通知。

有关哪些资源支持哪些类型的更改通知的详细信息，请参阅 [Microsoft Graph 更改通知](webhooks.md)。
 

## <a name="notification-payloads"></a>通知有效负载

根据你的订阅，你可以获取包含或不含资源数据的通知。 通过订阅资源数据，可以在收到通知的同时获取消息有效负载，而无需回调并获取内容。

### <a name="notifications-with-resource-data"></a>包含资源数据的通知

对于包含资源数据的通知，负载如下所示。  此有效负载用于对应于聊天消息资源的通知。 实际通知包括 **资源** 和表示已触发该通知的 **resourceData** 属性。

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

解密的通知负载如下所示。 上一示例的已解密有效负载符合 [chatMessage](/graph/api/resources/chatMessage?preserve-view=true) 架构。 该负载类似于 GET 操作返回的负载。

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

不含资源数据的通知为你提供了足够的信息来进行 GET 调用以获取资源。 订阅不含资源数据的通知不需要加密证书（因为不会发送实际资源数据）。

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
上面的示例显示了对应于聊天消息资源的通知。 实际通知包括 **资源** 和表示已触发该通知的 **resourceData** 属性。 **资源** 和 **@odata.id** 属性可用于对 Microsoft Graph 进行调用以获取资源的有效负载。

> **注意** GET 调用将始终返回资源的当前状态。 如果在发送通知和检索资源之间更改了资源，则该操作将返回已更新的资源。

## <a name="see-also"></a>另请参阅
- [Microsoft Graph 更改通知](webhooks.md)
- [Microsoft Teams API 概述](teams-concept-overview.md)
