---
title: 获取 Microsoft Graph 中联机会议的更改通知
description: Microsoft Graph 中的更改通知让你可以订阅 Microsoft Teams 会议的联机会议开始/结束以及名录更新。
author: benlee-msft
ms.localizationpriority: high
ms.prod: cloud-communications
ms.custom: scenarios:getting-started
ms.openlocfilehash: 90cae49f4f342a05eafe1e0099bb6eb60d3c2b04
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66436405"
---
# <a name="get-change-notifications-for-meeting-call-updates-in-microsoft-graph"></a>获取 Microsoft Graph 中会议通话更新的更改通知

Microsoft Graph 中的更改通知让你可以订阅 Microsoft Teams 会议的通话开始/结束以及通话人名录更新。 更改通知允许你维护订阅，从而提供低延迟模式。 你还可以在通知中获取资源数据，因此避免调用 API 来获取有效负载。

### <a name="subscribe-to-messages-across-all-channels"></a>跨频道订阅消息

若要获取应用程序中会议呼叫事件的更改通知，请订阅 `/communications/onlineMeetings/?$filter=JoinWebUrl eq '{JoinWebUrl}'`。 此资源支持在通知中[包括资源数据](/graph/webhooks-with-resource-data)。

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
  "resource": "/communications/onlineMeetings/?$filter=JoinWebUrl eq '{JoinWebUrl}'",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2021-02-01T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

## <a name="joinweburl"></a>JoinWebUrl
加入会议的 URL 包含在 [onlineMeeting](/graph/api/resources/onlineMeeting) 资源的 joinWebUrl 属性中，或会议的 Teams 客户端中。


## <a name="notifications-with-encrypted-resource-data"></a>具有加密资源数据的通知
```json
{
  "value": [{
    "subscriptionId": "{Subscription id}",
    "clientState": "{secret client state}",
    "changeType": "updated",
    "tenantId": "{Organization/Tenant id}",
    "resource": "communications/onlineMeetings?$filter=joinWebUrl+eq+'{joinWebUrl}'",
    "subscriptionExpirationDateTime": "2022-02-28T00:00:00.0000000Z",
    "resourceData": {
      "@odata.id": "communications/onlineMeetings?$filter=joinWebUrl+eq+'{joinWebUrl}'",
      "@odata.type": "#microsoft.graph.onlineMeeting",
      "id": "communications/onlineMeetings?$filter=joinWebUrl+eq+'{joinWebUrl}'"
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

有关如何验证令牌和解密负载的详细信息，请参阅[设置包含资源数据的更改通知](/graph/webhooks-with-resource-data)。

### <a name="event-notifications-types"></a>事件通知类型
以下是受支持的会议事件：
- CallStarted - 在启动会议呼叫时发生。
- CallEnded - 在会议呼叫结束时发生。
- CallRosterUpdate - 在参与者加入或退出呼叫时发生。

### <a name="decrypted-payload-examples"></a>解密的有效负载示例

#### <a name="callstartedcallended"></a>CallStarted/CallEnded.
```json
{
  "@odata.type":"#Microsoft.Graph.onlineMeeting",
  "@odata.id":"communications/onlineMeetings?$filter=joinWebUrl+eq+'{joinWebUrl}'",
  "id":"communications/onlineMeetings?$filter=joinWebUrl+eq+'{joinWebUrl}'",
  "eventType":"{Microsoft.Communication.CallStarted or Microsoft.Communication.CallEnded}",
  "eventDateTime":"2022-02-28T00:00:00.0000000Z",
  "state":"active"
}
```

#### <a name="callrosterupdate"></a>CallRosterUpdate
```json
{
  "@odata.type":"#Microsoft.Graph.onlineMeeting",
  "@odata.id":"communications/onlineMeetings?$filter=joinWebUrl+eq+'{joinWebUrl}'",
  "id":"communications/onlineMeetings?$filter=joinWebUrl+eq+'{joinWebUrl}'",
  "eventType":"Microsoft.Communication.CallRosterUpdate",
  "eventDateTime":"2022-02-28T00:00:00.0000000Z",
  "state":"active",
  "activeParticipants@delta": ["{meetingParticipantInfo list of users that joined}"],
  "activeParticipants@remove": ["{meetingParticipantInfo list of users that left}"]
}
```
**CallRosterUpdate** 事件将包括两个附加属性，**activeParticipants@delta** 描述添加到会议的参与者，以及 **activeParticipants@remove**，供离开联机会议的参与者使用。 有关参与者信息的详细信息，请参阅 [meetingParticipantInfo 资源类型](/graph/api/resources/meetingparticipants)。

可以通过包括属性 **includeResourceData**，或将此值设置为订阅请求正文中的 `false` 来选择忽略加密。 这样做会将属于加密有效负载的属性添加到 **resourceData**。


## <a name="see-also"></a>另请参阅
- [Microsoft Graph 更改通知](/graph/webhooks)
- [Microsoft Teams API 概述](/graph/teams-concept-overview)
- [联机会议资源](/graph/api/resources/onlineMeeting)
