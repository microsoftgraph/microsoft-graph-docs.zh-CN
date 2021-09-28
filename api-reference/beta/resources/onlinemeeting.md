---
title: onlineMeeting 资源类型
description: 包含有关会议的信息。
author: mkhribech
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 5f84034463044d3f8c832f1a8b0e0c17656c0f3a
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979430"
---
# <a name="onlinemeeting-resource-type"></a>onlineMeeting 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含有关会议的信息，包括用于加入会议的 URL、与会者列表和说明。

## <a name="methods"></a>方法

| 方法                                                             | 返回类型                       | 说明                                                                                                       |
| :----------------------------------------------------------------- | :-------------------------------- | :---------------------------------------------------------------------------------------------------------------- |
| [Create](../api/application-post-onlineMeetings.md)                | [onlineMeeting](onlinemeeting.md) | 创建联机会议。                                                                                         |
| [Get](../api/onlinemeeting-get.md)                                 | [onlineMeeting](onlinemeeting.md) | 读取 **onlineMeeting 对象的属性和** 关系。                                             |
| [更新](../api/onlinemeeting-update.md)                           | [onlineMeeting](onlinemeeting.md) | 更新 **onlineMeeting 对象** 的属性。 |
| [删除](../api/onlinemeeting-delete.md)                           | 无                              | 删除 **onlineMeeting** 对象。                                                                             |
| [创建或获取 onlineMeeting](../api/onlinemeeting-createorget.md) | [onlineMeeting](onlinemeeting.md) | 使用自定义外部 ID 创建联机会议。 如果会议已存在，请检索其属性。      |

## <a name="properties"></a>属性

| 属性              | 类型                                          | 说明                                                                                                                                                                                                                                                 |
| :-------------------- | :-------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| allowedPresenters     | [onlineMeetingPresenters](#onlinemeetingpresenters-values)| 指定可在会议中成为演示者的人。 可能的值是 `everyone` `organization` `roleIsPresenter` 、、、 `organizer` 和 `unknownFutureValue` 。                                                                                                    |
| allowAttendeeToEnableCamera | 布尔值 | 指示与会者是否可以打开其相机。 |
| allowAttendeeToEnableMic | 布尔值 | 指示与会者是否可以打开其麦克风。 |
| allowMeetingChat      | [meetingChatMode](#meetingchatmode-values) | 指定会议聊天的模式。 |
| allowTeamworkReactions | 布尔值 | 指示是否Teams会议的反应。 |
| alternativeRecording  | Stream                                        | 实时事件的备用录制的内容流。 只读。                                                                                                                                                                                 |
| attendeeReport        | Stream                                        | 实时事件的与会者报告的内容流。 只读。                                                                                                                                                                                       |
| audioConferencing     | [audioConferencing](audioconferencing.md)     | 电话访问 (拨入) 联机会议的信息。 只读。                                                                                                                                                                                    |
| broadcastSettings     | [broadcastMeetingSettings](broadcastMeetingSettings.md)     | 设置实时事件相关。                                                                                                                                                                                                                     |
| chatInfo              | [chatInfo](chatinfo.md)                       | 与此联机会议关联的聊天信息。                                                                                                                                                                                                   |
| creationDateTime      | 日期时间                                      | 会议创建时间（UTC）。 只读。                                                                                                                                                                                                                |
| endDateTime           | 日期时间                                      | 会议结束时间（UTC）。                                                                                                                                                                                                                                |
| externalId            | String                                        | 外部 ID。 自定义 ID。 可选。                                                                                                                                                                                                                     |
| id                    | 字符串                                        | 与联机会议关联的默认 ID。 只读。                                                                                                                                                                                               |
| isBroadcast           | 布尔值                                       | 指示这是否是实时事件。                                                                                                                                                                                                                   |
| isEntryExitAnnounced  | 布尔值                                       | 指示呼叫者加入或离开时是否宣布。                                                                                                                                                                                                      |
| joinWebUrl            | 字符串                                        | 联机会议加入 URL。 只读。                                                                                                                                                                                                              |
| joinInformation       | [itemBody](itembody.md)                       | "Accept-Language"中指定的语言和区域设置变量中的联接信息请求 HTTP 标头。 只读                                                                                                                                       |
| lobbyBypassSettings   | [lobbyBypassSettings](lobbyBypassSettings.md) | 指定哪些参与者可以绕过会议厅。                                                                                                                                                                                                  |
| meetingAttendanceReport | [meetingAttendanceReport](meetingAttendanceReport.md) | 安排的会议的与会者报告。 只读。 |
| participants          | [meetingParticipants](meetingparticipants.md) | 与联机会议关联的参与者。 这包括组织者和与会者。                                                                                                                                                        |
| recordAutomatically | 布尔值 | 指示是否自动录制会议。 |
| recording             | Stream                                        | 录制实时事件的内容流。 只读。                                                                                                                                                                                             |
| startDateTime         | 日期时间                                      | 会议开始时间（UTC）。                                                                                                                                                                                                                              |
| subject               | String                                        | 联机会议的主题。                                                                                                                                                                                                                          |
| videoTeleconferenceId | 字符串                                        | 视频电话会议 ID。 只读。                                                                                                                                                                                                                   |
| autoAdmittedUsers (弃用)     | 字符串                                        | 用于指定将自动允许加入联机会议的参与者类型的设置。 可取值为：`everyone`、`everyoneInSameAndFederatedCompany`、`everyoneInCompany`、`invitedUsersInCompany`、`organizer`。 只读。 |
| 功能 (弃用)          | meetingCapabilities 集合                             | 会议功能列表。 可能的值是 `questionAndAnswer` `unknownFutureValue` ：、。                                                                                                                                                                                 |

> [!CAUTION]
>
>- **autoAdmittedUsers** 属性已弃用。 请 **改为使用** [lobbyBypassSettings 的 scope](lobbyBypassSettings.md) 属性。
>- **capabilities** 属性已弃用。 请改为使用 [broadcastMeetingSettings](broadcastMeetingSettings.md)的 **isQuestionAndAnswerEnabled** 属性。

### <a name="onlinemeetingpresenters-values"></a>onlineMeetingPresenters 值

| 值              | 说明                                                   |
| ------------------ | ------------------------------------------------------------- |
| everyone           | 每个人都是演示者 (这是默认选项) 。             |
| 组织       | 组织者组织中的每个人都是演示者。          |
| roleIsPresenter    | 只有其角色为演示者的参与者是演示者。 |
| 组织者          | 只有组织者是演示者。                           |
| unknownFutureValue | 未知未来值。                                         |

> [!TIP]
>
>- 创建或更新联机会议时，将 **allowedPresenters** 的值设置为 ，在请求正文中包括指定与会者的角色设置为 `roleIsPresenter` 的与会者 `presenter` 的完整列表。
>- 创建或更新联机会议时 **，allowedPresenters** 的值设置为除 其他值外，与会者的角色将在响应 `roleIsPresenter`  `null` 正文中显示。

### <a name="meetingchatmode-values"></a>meetingChatMode 值

| 值              | 说明                                                            |
| ------------------ | ---------------------------------------------------------------------- |
| 已启用            | 会议聊天已启用。                                               |
| disabled           | 会议聊天被禁用。                                              |
| limited            | 会议聊天已启用，但仅在会议呼叫期间启用。 |
| unknownFutureValue | 未知未来值。                                                  |

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  "externalId"
  ],
  "@odata.type": "microsoft.graph.onlineMeeting"
}-->
```json
{
  "audioConferencing": {"@odata.type": "microsoft.graph.audioConferencing"},
  "chatInfo": {"@odata.type": "microsoft.graph.chatInfo"},
  "creationDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "joinWebUrl": "String",
  "participants": {"@odata.type": "microsoft.graph.meetingParticipants"},
  "startDateTime": "String (timestamp)",
  "subject": "String",
  "videoTeleconferenceId": "String",
  "isEntryExitAnnounced": "Boolean",
  "lobbyBypassSettings": {"@odata.type": "microsoft.graph.lobbyBypassSettings"},
  "allowedPresenters": "String",
  "isBroadcast": "Boolean",
  "broadcastSettings": {"@odata.type": "microsoft.graph.broadcastSettings"},
  "allowMeetingChat": {"@odata.type": "microsoft.graph.meetingChatMode"},
  "allowTeamworkReactions": "Boolean",
  "allowAttendeeToEnableMic": "Boolean",
  "allowAttendeeToEnableCamera": "Boolean"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onlineMeeting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
