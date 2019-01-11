---
title: 呼叫资源类型
description: 没有传入呼叫的应用程序或应用程序创建新的传出呼叫通过时创建的**呼叫**资源`POST`上`app/calls`。
author: VinodRavichandran
localization_priority: Priority
ms.openlocfilehash: d2748b410352effb7119a569bdf48c86f2f7c2ad
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810701"
---
# <a name="call-resource-type"></a>呼叫资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

没有传入呼叫的应用程序或应用程序创建新的传出呼叫通过时创建的**呼叫**资源`POST`上`app/calls`。

作为对等或多方呼叫，可以设置呼叫。 创建或加入多方呼叫，提供`chatInfo`和`meetingInfo`。 如果这些未提供，将自动创建新的临时会议。 用于传入呼叫，高度可用的存储中, 记录这些值，以便您的应用程序事件您的应用程序崩溃中重新加入呼叫。

虽然不能多次邀请相同的标识，很可能要加入同一会议多次应用程序。 每次应用程序联接，不同呼叫`id`提供加入会议的呼叫。 我们建议使用单独的标识顺序为客户端显示它们为不同的参与者加入会议。

## <a name="methods"></a>方法

| 方法                                                            | 返回类型                                       | 说明                                  |
|:------------------------------------------------------------------|:--------------------------------------------------|:---------------------------------------------|
| [获取呼叫](../api/call-get.md)                                    | [呼叫](call.md)                                   | 阅读**呼叫**对象的属性。      |
| [删除](../api/call-delete.md)                                   |                                                   | 删除或活动**呼叫**的挂机。        |
| **呼叫处理**                                                 |                                                   |                                              |
| [答案](../api/call-answer.md)                                   |                                                   | 应答传入呼叫。                     |
| [Reject](../api/call-reject.md)                                   |                                                   | 拒绝传入的呼叫。                     |
| [重定向](../api/call-redirect.md)                               |                                                   | 重定向传入呼叫。                   |
| [Transfer](../api/call-transfer.md)                               |                                                   | 将呼叫转接                              |
| **多方**                                                   |                                                   |                                              |
| [参与者列表](../api/call-list-participants.md)             | [参与者](participant.md)集合          | 获取参与者对象集合。         |
| [邀请参与者](../api/participant-invite.md)               | [commsOperation](commsoperation.md)               | 邀请参与者加入活动呼叫。      |
| [将所有参与者设为都静音](../api/participant-muteall.md)            | [commsOperation](commsoperation.md)               | 将呼叫中的所有参与者设为都静音。           |
| [配置音频混音器](../api/participant-configuremixer.md)     | [commsOperation](commsoperation.md)               | 配置进行多方对话中的音频。  |
| [创建 audioRoutingGroup](../api/call-post-audioroutinggroups.md)| [audioRoutingGroup](audioroutinggroup.md)         | 通过发布到 audioRoutingGroups 集合中创建新 audioRoutingGroup。 |
| [列表 audioRoutingGroups](../api/call-list-audioroutinggroups.md) | [audioRoutingGroup](audioroutinggroup.md)集合|获取 audioRoutingGroup 对象集合。  |
| **互动语音响应**                                    |                                                   |                                              |
| [PlayPrompt](../api/call-playprompt.md)                           | [playPromptOperation](playpromptoperation.md)     | 播放提示呼叫中。                     |
| [Record](../api/call-record.md)                                   | [recordOperation](recordoperation.md)             | 记录呼叫。                             |
| [CancelMediaProcessing](../api/call-cancelmediaprocessing.md)     | [commsOperation](commsoperation.md)               | 取消处理媒体。                     |
| [SubscribeToTone](../api/call-subscribetotone.md)                 | [commsOperation](commsoperation.md)               | 订阅 DTMF 声音信号。                     |
| **自我参与者操作**                                   |                                                   |                                              |
| [设置为静音](../api/call-mute.md)                                       | [commsOperation](commsoperation.md)               | 在呼叫中的静音自我。                       |
| [取消静音](../api/call-unmute.md)                                   | [commsOperation](commsoperation.md)               | 在呼叫中的取消静音自我。                     |
| [UpdateMetadata](../api/call-updatemetadata.md)                   | [commsOperation](commsoperation.md)               | 在名单中的自助更新元数据。          |
| [ChangeScreenSharingRole](../api/call-changescreensharingrole.md) |                                                   | 启动和停止共享的调用中的屏幕                                             |

## <a name="properties"></a>属性

| 属性            | 类型                                                                                                   | Description                                                                                                                                                                                         |
| :------------------ | :------------------------------------------------------------------------------------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| activeModalities    | 字符串集合                                                                                      | 活动的形式的列表。 可取值为：`unknown`、`audio`、`video`、`videoBasedScreenSharing`、`data`。 此为只读属性。 生成的服务器。                                                    |
| answeredBy          | [participantInfo](participantinfo.md)                                                                  | 应答呼叫参与者。 此为只读属性。 生成的服务器。                                                                                                                                |
| callRoutes          | [callRoute](callroute.md)集合                                                                   | 呼叫已重定目标路由信息。 此为只读属性。 生成的服务器。                                                                                                                |
| callbackUri         | 字符串                                                                                                 | 将在其传递回调回调或订阅 ID。                                                                                                                               |
| chatInfo            | [chatInfo](chatinfo.md)                                                                                | 聊天的信息。                                                                                                                                                                               |
| 方向           | 字符串                                                                                                 | 呼叫的方向。 可能的值是`incoming`或`outgoing`。 此为只读属性。 生成的服务器。                                                                                            |
| id                  | String                                                                                                 | 只读。 生成的服务器。                                                                                                                                                                        |
| mediaConfig         | [appHostedMediaConfig](apphostedmediaconfig.md)或[serviceHostedMediaConfig](servicehostedmediaconfig.md) | 媒体配置。                                                                                                                                                                        |
| meetingCapability   | [meetingCapability](meetingcapability.md)                                                              | 包含会议的功能。                                                                                                                                                             |
| meetingInfo         | [organizerMeetingInfo](organizermeetinginfo.md)或[tokenMeetingInfo](tokenmeetinginfo.md)             | 会议信息。                                                                                                                                                                            |
| myParticipantId     | String                                                                                                 | 只读。 生成的服务器。                                                                                                                                                                        |
| requestedModalities | String 集合                                                                                      | 请求的形式的列表。 | 可取值为：`unknown`、`audio`、`video`、`videoBasedScreenSharing`、`data`。                                                                            |
| resultInfo          | [resultInfo](resultinfo.md)                                                                            | 结果的信息。 例如可以保留终止原因。 此为只读属性。 生成的服务器。                                                                                                       |
| ringingTimeoutInSeconds | Int32                                                                                              | 传出的对等呼叫的的响铃超时                                                                                                                                                     |
| routingPolicies     | String 集合                                                                                      | 可取值为：`none`、`noMissedCall`、`disableForwardingExceptPhone`、`disableForwarding`。                                                                                                   |
| 源              | [participantInfo](participantinfo.md)                                                                  | 呼叫发起方。                                                                                                                                                                         |
| state               | 字符串                                                                                                 | 呼叫状态。 可取值为：`incoming`、`establishing`、`ringing`、`established`、`hold`、`transferring`、`transferAccepted`、`redirecting`、`terminating`、`terminated`。 此为只读属性。 生成的服务器。                         |
| subject             | 字符串                                                                                                 | 对话的主题。                                                                                                                                                                    |
| 目标             | [participantInfo](participantinfo.md)集合                                                       | 呼叫的目标。                                                                                                                                                                            |
| tenantId            | 字符串                                                                                                 | Azure Active Directory 中的 tenantId。                                                                                                                                                                 |
| terminationReason   | String                                                                                                 | 只读。 生成的服务器。                                                                                                                                                                        |
| toneInfo            | [toneInfo](toneinfo.md)                                                                                | 此为只读属性。 生成的服务器。                                                                                                                                                                        |

> 注意： 属性标记为`Server generated`处理时，将忽略`POST`上`app/calls`。

## <a name="relationships"></a>Relationships

| 关系        | 类型                                                 | Description                                                         |
|:--------------------|:-----------------------------------------------------|:--------------------------------------------------------------------|
| audioRoutingGroups  | [audioRoutingGroup](audioroutinggroup.md)集合 | 只读。可为 NULL。                                                |
| operations          | [commsOperation](commsoperation.md)集合       | 只读。可为 NULL。                                                |
| participants        | [参与者](participant.md)集合             | 只读。可为 NULL。                                                |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "activeModalities",
    "answeredBy",
    "callRoutes",
    "chatInfo",
    "direction",
    "id",
    "meetingCapability",
    "meetingInfo",
    "myParticipantId",
    "resultInfo",
    "ringingTimeoutInSeconds",
    "routingPolicies",
    "state",
    "targets",
    "tenantId",
    "terminationReason",
    "toneInfo"
  ],
  "@odata.type": "microsoft.graph.call"
}-->
```json
{
  "activeModalities": ["unknown | audio | video | videoBasedScreenSharing | data"],
  "answeredBy": {"@odata.type": "#microsoft.graph.participantInfo"},
  "callRoutes": [{"@odata.type": "#microsoft.graph.callRoute"}],
  "callbackUri": "String",
  "chatInfo": {"@odata.type": "#microsoft.graph.chatInfo"},
  "direction": "incoming | outgoing",
  "id": "String (identifier)",
  "mediaConfig": {"@odata.type": "#microsoft.graph.mediaConfig"},
  "meetingCapability": {"@odata.type": "#microsoft.graph.meetingCapability"},
  "meetingInfo": {"@odata.type": "#microsoft.graph.meetingInfo"},
  "myParticipantId": "String",
  "requestedModalities": ["unknown | audio | video | videoBasedScreenSharing | data"],
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "ringingTimeoutInSeconds": 1024,
  "routingPolicies": ["none | noMissedCall | disableForwardingExceptPhone | disableForwarding"],
  "source": {"@odata.type": "#microsoft.graph.participantInfo"},
  "state": "incoming | establishing | ringing | established | hold | transferring | transferAccepted | redirecting | terminating | terminated",
  "subject": "String",
  "targets": [{"@odata.type": "#microsoft.graph.participantInfo"}],
  "tenantId": "String",
  "terminationReason": "String",
  "toneInfo": {"@odata.type": "#microsoft.graph.toneInfo"}
}
```

> **注意：** 您将了解从与 Microsoft 团队安排了会议加入 URL。 下面介绍了如何从 URL 和填充提取数据`chatInfo`和`meetingInfo`。

```http
https://teams.microsoft.com/l/meetup-join/19%3ameeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk%40thread.v2/0?context=%7b%22Tid%22%3a%2272f988bf-86f1-41af-91ab-2d7cd011db47%22%2c%22Oid%22%3a%224b444206-207c-42f8-92a6-e332b41c88a2%22%7d
decodes to:
https://teams.microsoft.com/l/meetup-join/19:meeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk@thread.v2/0?context={"Tid":"72f988bf-86f1-41af-91ab-2d7cd011db47","Oid":"4b444206-207c-42f8-92a6-e332b41c88a2"}
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.call",
  truncated: true
}-->
```json
{
  "chatInfo": {
    "threadId": "19:meeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk@thread.v2",
    "messageId": "0",
    "replyChainMessageId": "0"
  },
  "meetingInfo": {
    "@odata.type": "#microsoft.graph.organizerMeetingInfo",
    "organizer": {
      "user": {
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "id": "4b444206-207c-42f8-92a6-e332b41c88a2"
      }
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "call resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
