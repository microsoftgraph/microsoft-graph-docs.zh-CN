---
title: call 资源类型
description: 当应用程序有传入呼叫或应用程序通过 `app/calls` 上的 `POST` 创建新的传出呼叫时，将创建 **call** 资源。
author: ananmishr
ms.localizationpriority: high
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: b12d80ae786abc93d9b3e00358f7b18d42b89140
ms.sourcegitcommit: 9bbcce5784a89768ece55a66e3651080d56e1e92
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/19/2022
ms.locfileid: "64917771"
---
# <a name="call-resource-type"></a>call 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

当应用程序有传入呼叫或应用程序通过 `app/calls` 上的 `POST` 创建新的传出呼叫时，将创建 **call** 资源。

呼叫可设置为对等呼叫或群组通话。 要创建或加入群组通话，请提供 `chatInfo` 和 `meetingInfo`。 如果未提供这些项，则自动创建一个新的群组通话。 对于传入呼叫，将这些值记录在高可用性存储中，以便在应用程序崩溃时它可以重新加入呼叫。

尽管不能多次邀请相同的身份，但应用程序可以多次加入同一会议。 应用程序每次想要加入时，都必须提供单独的标识，以便客户端将其显示为不同的参与者。

> **请注意：** 可从通过 Microsoft Teams 计划的会议中获取加入 URL。 从所示 URL 中提取数据来填充 `chatInfo` 和 `meetingInfo`。

```http
https://teams.microsoft.com/l/meetup-join/19%3ameeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk%40thread.v2/0?context=%7b%22Tid%22%3a%2272f988bf-86f1-41af-91ab-2d7cd011db47%22%2c%22Oid%22%3a%224b444206-207c-42f8-92a6-e332b41c88a2%22%7d
```
变为：
```http
https://teams.microsoft.com/l/meetup-join/19:meeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk@thread.v2/0?context={"Tid":"72f988bf-86f1-41af-91ab-2d7cd011db47","Oid":"4b444206-207c-42f8-92a6-e332b41c88a2"}
```


## <a name="methods"></a>方法

| 方法                                                             | 返回类型                                                 | 说明                                                                     |
|:-------------------------------------------------------------------|:------------------------------------------------------------|:--------------------------------------------------------------------------------|
| [Get](../api/call-get.md)                                     | [call](call.md)                                             | 读取 **call** 对象的属性。                                         |
| [删除](../api/call-delete.md)                                    | 无                                                            | 删除或挂断活动 **呼叫**。                                           |
| [KeepAlive](../api/call-keepalive.md)                             | 无                                                  | 确保通话不中断。
| **呼叫处理**                                                  |                                                        |                                                                                 |
| [Answer](../api/call-answer.md)                                    | 无                                                            | 应答传入呼叫。                                                        |
| [Reject](../api/call-reject.md)                                    | 无                                                            | 拒绝传入呼叫。                                                        |
| [重定向](../api/call-redirect.md)                                | 无                                                            | 重定向传入呼叫。                                                      |
| [Transfer](../api/call-transfer.md)                                | 无                                                            | 转接呼叫                                                                 |
| **群组呼叫**                                                    |                                                             |                                                                            |
| [List participants](../api/call-list-participants.md)              | [participant](participant.md) 集合                    | 获取参与者对象集合。                                            |
| [邀请参与者](../api/participant-invite.md)                | [commsOperation](commsoperation.md)                         | 邀请参与者加入活动呼叫。                                         |
| [所有参与者静音](../api/participant-muteall.md)             | [commsOperation](commsoperation.md)                         | 将呼叫中的所有参与者设为静音。                                              |
| [参与者静音](../api/participant-mute.md)                     | [muteParticipantOperation](muteparticipantoperation.md)     | 群组通话中参与者静音。                                           |
| [配置 Audio Mixer](../api/participant-configuremixer.md)      | [commsOperation](commsoperation.md)                         | 在多方对话中配置音频。                                     |
| [Create audioRoutingGroup](../api/call-post-audioroutinggroups.md) | [audioRoutingGroup](audioroutinggroup.md)                   | 通过发布到 audioRoutingGroups 集合创建一个新的 audioRoutingGroup。 |
| [List audioRoutingGroups](../api/call-list-audioroutinggroups.md)  | [audioRoutingGroup](audioroutinggroup.md) 集合        | 获取 audioRoutingGroup 对象集合。                                      |
| **Interactive-Voice-Response**                                     |                                                             |                                                                                 |
| [PlayPrompt](../api/call-playprompt.md)                            | [playPromptOperation](playpromptoperation.md)               | 在呼叫中播放提示。                                                        |
| [RecordResponse](../api/call-record.md)                            | [recordOperation](recordoperation.md)                       | 录制来自呼叫方的简短音频回复。                                        |
| [CancelMediaProcessing](../api/call-cancelmediaprocessing.md)      | [commsOperation](commsoperation.md)                         | 取消媒体处理。                                                        |
| [SubscribeToTone](../api/call-subscribetotone.md)                  | [commsOperation](commsoperation.md)                         | 订阅 DTMF 音。                                                        |
| **Self Participant Operations**                                    |                                                             |                                                                                 |
| [Mute](../api/call-mute.md)                                        | [muteParticipantOperation](muteparticipantoperation.md)     | 在呼叫中将自己设为静音。                                                          |
| [Unmute](../api/call-unmute.md)                                    | [unmuteParticipantOperation](unmuteparticipantoperation.md) | 在呼叫中将自己取消静音。                                                        |
| [ChangeScreenSharingRole](../api/call-changescreensharingrole.md)  | 无                                                        | 在呼叫中开始和停止共享屏幕。                                      |
| **记录操作**                                           |                                                             |                                              |
| [UpdateRecordingStatus](../api/call-updaterecordingstatus.md)      | [updateRecordingStatusOperation](updateRecordingStatusOperation.md)               | 更新记录状态。                      |
| **日志记录操作**                                           |                                                             |                                              |
| [记录设备质量数据](../api/call-logteleconferencedevicequality.md)| [teleconferenceDeviceQuality](teleconferencedevicequality.md) | 记录视频电话会议设备质量数据。|

## <a name="properties"></a>属性

| 属性            | 类型                                                                                                   | 说明                                                                                                                                                                                         |
| :------------------ | :------------------------------------------------------------------------------------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| activeModalities    | modality 集合                                                                                      | 活动模态的列表。 可取值为：`unknown`、`audio`、`video`、`videoBasedScreenSharing`、`data`。 只读。                                                    |
| answeredBy          | [participantInfo](participantinfo.md)                                                                  | 已应答呼叫的参与者。只读。                                                                                                                                |
| callRoutes          | [callRoute](callroute.md) 集合                                                                   | 有关如何重定向呼叫的路由信息。只读。                                                                                                                |
| callbackUri         | 字符串                                                                                                 | 用于传递回拨的回拨 URL。必须为 `https`。                                                                                                                               |
| callChainId         | String                                                                                                 | 会议中所有参与者通话的唯一标识符，或 P2P 通话中两位参与者通话的唯一标识符。需要从 `Microsoft.Graph.Call.CallChainId` 复制它。 |
| callOptions            | [outgoingCallOptions](outgoingcalloptions.md)                                                         | 包含该通话的可选功能。   |
| chatInfo            | [chatInfo](chatinfo.md)                                                                                | 聊天信息。 会议情境所需的信息。                                                                                                                                |
| direction           | callDirection                                                                                                 | 呼叫的方向。 可取值为 `incoming` 或 `outgoing`。 只读。                                                                                            |
| id                  | 字符串                                                                                                 | 来电显示。只读。                                                                                                                                                                        |
| incomingContext     | [incomingContext](incomingcontext.md)                                                                  | 与来电相关的上下文。只读。由服务器生成。                                                                                                                                |
| mediaConfig         | [appHostedMediaConfig](apphostedmediaconfig.md) 或 [serviceHostedMediaConfig](servicehostedmediaconfig.md) | 媒体配置。创建对等呼叫或加入会议所需的信息。                                                                        |
| mediaState          | [callMediaState](callmediastate.md)                                                                    | 只读。通话媒体状态。 |
| meetingCapability   | [meetingCapability](meetingcapability.md)                                                              | 包含会议功能。只读。                                                                                                       |
| meetingInfo         | [organizerMeetingInfo](organizermeetinginfo.md) 或 [tokenMeetingInfo](tokenmeetinginfo.md)             | 会议信息。 会议情境所需的信息。                                                                                                              |
|transcription     | [callTranscriptionInfo](calltranscriptioninfo.md)                                                         | 通话的脚本信息。只读。                           |
myParticipantId     | String                                                                                                   | 只读。                                                                                                                                                                        |
| requestedModalities | modality 集合                                                                                      | 请求模态的列表。 可取值为：`unknown`、`audio`、`video`、`videoBasedScreenSharing`、`data`。                                                                            |
| resultInfo          | [resultInfo](resultinfo.md)                                                                            | 结果信息。 例如，可以保留终止原因。 只读。                                                                                                        |
| ringingTimeoutInSeconds | Int32                                                                                              | 传出对等呼叫的以秒为单位的响铃超时。 此属性的最大值为 115 秒。                                                                                        |
| routingPolicies     | routingPolicy 集合集合                                                                                      | 此属性仅适用于对等通话。可能的值为: `none`、`noMissedCall`、`disableForwardingExceptPhone`、`disableForwarding`、`preferSkypeForBusiness`、`unknownFutureValue`。                                                                                                   |
| source              | [participantInfo](participantinfo.md)                                                                  | 呼叫的发起方。                                                                                                                                                                         |
| state               | callState                                                                                                 | 呼叫状态。 可取值为：`incoming`、`establishing`、`ringing`、`established`、`hold`、`transferring`、`transferAccepted`、`redirecting`、`terminating`、`terminated`。 只读。                          |
| subject             | String                                                                                                 | 对话的主题。                                                                                                                                                                    |
| targets             | [invitationParticipantInfo](participantinfo.md) 集合                                             | 呼叫的目标。 创建对等呼叫所需的信息。                                                                                                            |
| tenantId            | 字符串                                                                                                 | 只读。 `tenantId` 在 Azure Active Directory 中。                                                                                                                        |
| terminationReason   | String                                                                                                 | 只读。                                                                                                                                                                       |
| toneInfo            | [toneInfo](toneinfo.md)                                                                                | 只读。                                                                                                                                                                        |

## <a name="relationships"></a>关系

| 关系        | 类型                                                 | 说明                                                         |
|:--------------------|:-----------------------------------------------------|:--------------------------------------------------------------------|
| audioRoutingGroups  | [audioRoutingGroup](audioroutinggroup.md) 集合 | 只读。可为空。                                                |
| operations          | [commsOperation](commsoperation.md) 集合       | 只读。可为空。                                                |
| participants        | [participant](participant.md) 集合             | 只读。可为空。                                                |
| contentSharingSessions        | [contentSharingSession](contentsharingsession.md) 集合             | 只读。可为空。                                                |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "activeModalities",
    "answeredBy",
    "callRoutes",
    "callChainId",
    "callOptions",
    "chatInfo",
    "contentSharingSessions",
    "direction",
    "id",
    "incomingContext",
    "mediaState",
    "meetingCapability",
    "meetingInfo",
    "transcription",
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
  "callChainId": "String",
  "callOptions": {"@odata.type": "#microsoft.graph.outgoingCallOptions"},
  "chatInfo": {"@odata.type": "#microsoft.graph.chatInfo"},
  "contentSharingSessions": [{ "@odata.type": "microsoft.graph.contentSharingSession" }],
  "direction": "incoming | outgoing",
  "id": "String (identifier)",
  "incomingContext": {"@odata.type": "#microsoft.graph.incomingContext"},
  "mediaConfig": {"@odata.type": "#microsoft.graph.mediaConfig"},
  "mediaState": {"@odata.type": "#microsoft.graph.callMediaState"},
  "meetingCapability": {"@odata.type": "#microsoft.graph.meetingCapability"},
  "meetingInfo": {"@odata.type": "#microsoft.graph.meetingInfo"},
  "transcription": {"@odata.type": "#microsoft.graph.callTranscriptionInfo"},
  "myParticipantId": "String",
  "replacesContext": "String",
  "requestedModalities": ["unknown | audio | video | videoBasedScreenSharing | data"],
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "ringingTimeoutInSeconds": 99,
  "routingPolicies": ["none | noMissedCall | disableForwardingExceptPhone | disableForwarding | preferSkypeForBusiness"],
  "source": {"@odata.type": "#microsoft.graph.participantInfo"},
  "state": "incoming | establishing | ringing | established | hold | transferring | transferAccepted | redirecting | terminating | terminated",
  "subject": "String",
  "targets": [{"@odata.type": "#microsoft.graph.invitationParticipantInfo"}],
  "tenantId": "String",
  "terminationReason": "String",
  "toneInfo": {"@odata.type": "#microsoft.graph.toneInfo"}
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


