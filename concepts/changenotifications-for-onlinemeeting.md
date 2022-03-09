---
title: 获取 Microsoft Graph 中会议通话更新的更改通知
description: Microsoft Graph 中的更改通知让你可以订阅 Microsoft Teams 会议的通话开始/结束以及通话人名录更新。
author: benlee-msft
ms.localizationpriority: high
ms.prod: microsoft-teams
ms.custom: scenarios:getting-started
ms.openlocfilehash: bca104717d5b6c50f53eabe21e450ea3520d2a8b
ms.sourcegitcommit: efa06c63cd3154bcc7ecc993011f314c2dea9a92
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63376517"
---
# <a name="get-change-notifications-for-meeting-call-updates-in-microsoft-graph"></a>获取 Microsoft Graph 中会议通话更新的更改通知

Microsoft Graph 中的更改通知让你可以订阅 Microsoft Teams 会议的通话开始/结束以及通话人名录更新。 更改通知允许你维护订阅，从而提供低延迟模式。 你还可以在通知中获取资源数据，因此避免调用 API 来获取有效负载。

### <a name="subscribe-to-messages-across-all-channels"></a>跨频道订阅消息

若要获取应用程序中会议呼叫事件的更改通知，请订阅 `/communications/onlineMeetings/{meeting-id}`。 此资源支持在通知中[包括资源数据](webhooks-with-resource-data.md)。

#### <a name="permissions"></a>权限

|权限类型      | 权限（从最低特权到最高特权）              | 支持的版本 |
|:--------------------|:---------------------------------------------------------|:-------------------|
|委派（工作或学校帐户） | 不支持。 | 不支持。 |
|委派（个人 Microsoft 帐户） | 不支持。    | 不支持。 |
|应用程序 | OnlineMeetings.Read.All、OnlineMeetings.ReadWrite.All | beta 版 |

#### <a name="example"></a>示例

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/communications/onlineMeetings/{meeting-id}",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2021-02-01T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```
## <a name="notifications-with-encrypted-resource-data"></a>具有加密资源数据的通知
```json
{
  "value": [{
    "subscriptionId": "{Subscription id}",
    "clientState": "{secret client state}",
    "changeType": "updated",
    "tenantId": "{Organization/Tenant id}",
    "resource": "communications/onlineMeeting/{meeting-id}",
    "subscriptionExpirationDateTime": "2022-02-28T02:00:00-08:00",
    "resourceData": {
      "@odata.id": "communications/onlineMeetings/{meeting-id}",
      "@odata.type": "#microsoft.graph.onlineMeeting",
      "id": "communications/onlineMeetings/{meeting-id}"
    },
    "organizationId": "{Organization/Tenant id}",
    "encryptedContent": {
      "data": "{Encrypted content}",
      "dataSignature": "{Encrypted data signature}",
      "dataKey": "{Encrypted data key for encrypting content}",
      "encryptionCertificateId": "{User specified id of encryption certificate}",
      "encryptionCertificateThumbprint": "{Encrpytion certification thumbprint}"
    }
  }],
  "validationTokens": ["{Validation Tokens}"]
}
```

有关如何验证令牌和解密负载的详细信息，请参阅[设置包含资源数据的更改通知](webhooks-with-resource-data.md)。

解密的通知负载如下所示。
```json
{
  "@odata.type":"#microsoft.graph.onlineMeeting",
  "@odata.id":"communications/onlineMeetings/{meeting-id}",
  "id":"communications/onlineMeetings/{meeting-id}",
  "eventType":"Microsoft.Communication.CallStarted",
  "eventDateTime":"2022-02-28T18:41:33.0553203Z",
  "state":"active"
}
```

可以通过包括属性 **includeResourceData**，或将此值设置为订阅请求正文中的 `false` 来选择忽略加密。
## <a name="event-notifications-types"></a>事件通知类型
以下是受支持的会议事件：
- CallStarted - 在启动会议呼叫时发生。
- CallEnded - 在会议呼叫结束时发生。
- CallRosterUpdate - 在参与者加入或退出呼叫时发生。

**CallRosterUpdate** 事件将包括两个附加属性，即 **activeParticipants@delta** 和 **activeParticipants@remove**，用于描述 **在 resourceData** 属性中加入/离开会议呼叫的参与者。

## <a name="see-also"></a>另请参阅
- [Microsoft Graph 更改通知](webhooks.md)
- [Microsoft Teams API 概述](teams-concept-overview.md)
- [联机会议资源](/graph/api/resources/onlinemeeting.md)
