---
title: call 资源类型
description: 当应用程序有传入呼叫或应用程序通过 `app/calls` 上的 `POST` 创建新的传出呼叫时，将创建 **call** 资源。
author: VinodRavichandran
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e4c36dc781a0e8887c218cf11f3e78d7098d9c99
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/07/2019
ms.locfileid: "36792833"
---
# <a name="call-resource-type"></a>call 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

当应用程序有传入呼叫或应用程序通过 `app/calls` 上的 `POST` 创建新的传出呼叫时，将创建 **call** 资源。

呼叫可以设置为对等呼叫或多方呼叫。 若要创建或加入多方呼叫，需要提供 `chatInfo` 和 `meetingInfo`。 如果未提供，则会自动创建新的临时会议。 对于传入呼叫，将这些值记录在高可用性存储中，以便在应用程序崩溃时它可以重新加入呼叫。

尽管不能多次邀请相同的身份，但应用程序可以多次加入同一会议。 每次应用程序加入时，都会为该会议呼叫提供一个不同的呼叫 `id`。 我们建议你使用单独的身份加入会议，以便客户端将其显示为不同的参与者。

## <a name="methods"></a>方法

| 方法                                                            | 返回类型                                       | 说明                                  |
|:------------------------------------------------------------------|:--------------------------------------------------|:---------------------------------------------|
| [Get call](../api/call-get.md)                                    | [call](call.md)                                   | 读取 **call** 对象的属性。      |
| [Delete](../api/call-delete.md)                                   |                                                   | 删除或挂断活动**呼叫**。        |
| **Call Handling**                                                 |                                                   |                                              |
| [Answer](../api/call-answer.md)                                   |                                                   | 应答传入呼叫。                     |
| [Reject](../api/call-reject.md)                                   |                                                   | 拒绝传入呼叫。                     |
| [Redirect](../api/call-redirect.md)                               |                                                   | 重定向传入呼叫。                   |
| [Transfer](../api/call-transfer.md)                               |                                                   | 转接呼叫                              |
| **Multi-party**                                                   |                                                   |                                              |
| [List participants](../api/call-list-participants.md)             | [participant](participant.md) 集合          | 获取参与者对象集合。         |
| [Invite Participants](../api/participant-invite.md)               | [commsOperation](commsoperation.md)               | 邀请参与者加入活动呼叫。      |
| [Mute All Participants](../api/participant-muteall.md)            | [commsOperation](commsoperation.md)               | 将呼叫中的所有参与者设为静音。           |
| [参与者静音](../api/participant-mute.md)                    | [commsOperation](commsoperation.md)               | 群组通话中参与者静音。        |
| [Configure Audio Mixer](../api/participant-configuremixer.md)     | [commsOperation](commsoperation.md)               | 在多方对话中配置音频。  |
| [Create audioRoutingGroup](../api/call-post-audioroutinggroups.md)| [audioRoutingGroup](audioroutinggroup.md)         | 通过发布到 audioRoutingGroups 集合创建一个新的 audioRoutingGroup。 |
| [List audioRoutingGroups](../api/call-list-audioroutinggroups.md) | [audioRoutingGroup](audioroutinggroup.md) 集合|获取 audioRoutingGroup 对象集合。  |
| **Interactive-Voice-Response**                                    |                                                   |                                              |
| [PlayPrompt](../api/call-playprompt.md)                           | [playPromptOperation](playpromptoperation.md)     | 在呼叫中播放提示。                     |
| [Record](../api/call-record.md)                                   | [recordOperation](recordoperation.md)             | 录制来自通话的短音频剪辑。     |
| [CancelMediaProcessing](../api/call-cancelmediaprocessing.md)     | [commsOperation](commsoperation.md)               | 取消媒体处理。                     |
| [SubscribeToTone](../api/call-subscribetotone.md)                 | [commsOperation](commsoperation.md)               | 订阅 DTMF 音。                     |
| **Self Participant Operations**                                   |                                                   |                                              |
| [Mute](../api/call-mute.md)                                       | [commsOperation](commsoperation.md)               | 在呼叫中将自己设为静音。                       |
| [Unmute](../api/call-unmute.md)                                   | [commsOperation](commsoperation.md)               | 在呼叫中将自己取消静音。                     |
| [ChangeScreenSharingRole](../api/call-changescreensharingrole.md) |                                                   | 在呼叫中开始和停止共享屏幕。   |

## <a name="properties"></a>属性

| 属性            | 类型                                                                                                   | 说明                                                                                                                                                                                         |
| :------------------ | :------------------------------------------------------------------------------------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| activeModalities    | String 集合                                                                                      | 活动模态的列表。 可取值为：`unknown`、`audio`、`video`、`videoBasedScreenSharing`、`data`。 只读。 由服务器生成。                                                    |
| answeredBy          | [participantInfo](participantinfo.md)                                                                  | 已应答呼叫的参与者。 只读。 由服务器生成。                                                                                                                                |
| callRoutes          | [callRoute](callroute.md) 集合                                                                   | 有关如何重定向呼叫的路由信息。 只读。 由服务器生成。                                                                                                                |
| callbackUri         | 字符串                                                                                                 | 用于传递回调的回调 URL。 必须是 `https`。                                                                                                                               |
| chatInfo            | [chatInfo](chatinfo.md)                                                                                | 聊天信息。 会议情境所需的信息。                                                                                                                                |
| direction           | String                                                                                                 | 呼叫的方向。 可取值为 `incoming` 或 `outgoing`。 只读。 由服务器生成。                                                                                            |
| id                  | 字符串                                                                                                 | 来电显示。只读。 由服务器生成。                                                                                                                                                                        |
| mediaConfig         | [appHostedMediaConfig](apphostedmediaconfig.md) 或 [serviceHostedMediaConfig](servicehostedmediaconfig.md) | 媒体配置。 创建对等呼叫或加入会议所需的信息。                                                                        |
| mediaState          | [callMediaState](callmediastate.md)                                                                    | 只读。 由服务器生成。 通话媒体状态。 |
| meetingCapability   | [meetingCapability](meetingcapability.md)                                                              | 包含会议功能。 只读。 由服务器生成。                                                                                                        |
| meetingInfo         | [organizerMeetingInfo](organizermeetinginfo.md) 或 [tokenMeetingInfo](tokenmeetinginfo.md)             | 会议信息。 会议情境所需的信息。                                                                                                              |
| myParticipantId     | String                                                                                                 | 只读。 由服务器生成。                                                                                                                                                                        |
| requestedModalities | String 集合                                                                                      | 请求模态的列表。 | 可取值为：`unknown`、`audio`、`video`、`videoBasedScreenSharing`、`data`。                                                                            |
| resultInfo          | [resultInfo](resultinfo.md)                                                                            | 结果信息。 例如，可以保留终止原因。 只读。 由服务器生成。                                                                                                       |
| ringingTimeoutInSeconds | Int32                                                                                              | 传出对等呼叫的以秒为单位的响铃超时。 此属性的最大值为 115 秒。                                                                                        |
| routingPolicies     | String collection                                                                                      | 此属性仅适用于对等呼叫。 可取值为：`none`、`noMissedCall`、`disableForwardingExceptPhone`、`disableForwarding`、`preferSkypeForBusiness`。                                                                                                   |
| source              | [participantInfo](participantinfo.md)                                                                  | 呼叫的发起方。                                                                                                                                                                         |
| state               | String                                                                                                 | 呼叫状态。 可取值为：`incoming`、`establishing`、`ringing`、`established`、`hold`、`transferring`、`transferAccepted`、`redirecting`、`terminating`、`terminated`。 只读。 由服务器生成。                         |
| subject             | String                                                                                                 | 对话的主题。                                                                                                                                                                    |
| targets             | [participantInfo](participantinfo.md) 集合                                                       | 呼叫的目标。 创建对等呼叫所需的信息。                                                                                                            |
| tenantId            | 字符串                                                                                                 | 只读。 由服务器生成。 `tenantId` 在 Azure Active Directory 中。                                                                                                                        |
| terminationReason   | String                                                                                                 | 只读。 由服务器生成。                                                                                                                                                                        |
| toneInfo            | [toneInfo](toneinfo.md)                                                                                | 只读。 由服务器生成。                                                                                                                                                                        |

> 注意：在 `app/calls` 上处理 `POST` 时，标记为 `Server generated` 的属性将被忽略。

## <a name="relationships"></a>关系

| 关系        | 类型                                                 | 说明                                                         |
|:--------------------|:-----------------------------------------------------|:--------------------------------------------------------------------|
| audioRoutingGroups  | [audioRoutingGroup](audioroutinggroup.md) 集合 | 只读。 可为 NULL。                                                |
| operations          | [commsOperation](commsoperation.md) 集合       | 只读。可为空。                                                |
| participants        | [participant](participant.md) 集合             | 只读。可为空。                                                |

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
    "mediaState",
    "meetingCapability",
    "meetingInfo",
    "myParticipantId",
    "replacesContext",
    "resultInfo",
    "ringingTimeoutInSeconds",
    "routingPolicies",
    "state",
    "source",
    "subject",
    "targets",
    "tenantId",
    "terminationReason",
    "toneInfo"
  ],
  "keyProperty":"id",
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
  "mediaState": {"@odata.type": "#microsoft.graph.callMediaState"},
  "meetingCapability": {"@odata.type": "#microsoft.graph.meetingCapability"},
  "meetingInfo": {"@odata.type": "#microsoft.graph.meetingInfo"},
  "myParticipantId": "String",
  "replacesContext": "String",
  "requestedModalities": ["unknown | audio | video | videoBasedScreenSharing | data"],
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "ringingTimeoutInSeconds": 99,
  "routingPolicies": ["none | noMissedCall | disableForwardingExceptPhone | disableForwarding | preferSkypeForBusiness"],
  "source": {"@odata.type": "#microsoft.graph.participantInfo"},
  "state": "incoming | establishing | ringing | established | hold | transferring | transferAccepted | redirecting | terminating | terminated",
  "subject": "String",
  "targets": [{"@odata.type": "#microsoft.graph.participantInfo"}],
  "tenantId": "String",
  "terminationReason": "String",
  "toneInfo": {"@odata.type": "#microsoft.graph.toneInfo"}
}
```

> **注意：** 你将在使用 Microsoft Teams 安排的会议中找到加入 URL。 下面介绍了如何从 URL 中提取数据并填充 `chatInfo` 和 `meetingInfo`。

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
<!--
{
  "type": "#page.annotation",
  "description": "call resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
