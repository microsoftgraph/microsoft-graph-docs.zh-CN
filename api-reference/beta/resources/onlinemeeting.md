---
title: onlineMeeting 资源类型
description: 包含有关会议的信息。
author: mkhribech
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 876260fe4e6eb85a212db1a04417faed7c422bc3
ms.sourcegitcommit: 9adff6756e27aabbf36a9adbc2269b13c7fa74ef
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2022
ms.locfileid: "65883843"
---
# <a name="onlinemeeting-resource-type"></a>onlineMeeting 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含有关会议的信息，包括用于加入会议的 URL、与会者列表和说明。

此资源支持订阅 [更改通知](/graph/webhooks)。

## <a name="methods"></a>方法

| 方法 | 返回类型 |说明 |
| ------ | ----------- | ---------- |
| [创建](../api/application-post-onlineMeetings.md) | [onlineMeeting](onlinemeeting.md) | 创建联机会议。 |
| [获取](../api/onlinemeeting-get.md) | [onlineMeeting](onlinemeeting.md) | 读取 **onlineMeeting** 对象的属性和关系。 |
| [Update](../api/onlinemeeting-update.md) | [onlineMeeting](onlinemeeting.md) | 更新 **onlineMeeting** 对象的属性。 |
| [删除](../api/onlinemeeting-delete.md) | 无 | 删除 **onlineMeeting** 对象。 |
| [创建或获取 onlineMeeting](../api/onlinemeeting-createorget.md) | [onlineMeeting](onlinemeeting.md) | 使用自定义外部 ID 创建联机会议。 如果会议已存在，请检索其属性。 |

## <a name="properties"></a>属性

| 属性              | 类型                                          | 说明    |
| :-------------------- | :-------------------------------------------- | :------------------------------------ |
| allowedPresenters     | [onlineMeetingPresenters](#onlinemeetingpresenters-values)| 指定谁可以在会议中担任演示者。 |
| allowAttendeeToEnableCamera | Boolean | 指示与会者是否可以打开相机。 |
| allowAttendeeToEnableMic | 布尔 | 指示与会者是否可以打开麦克风。 |
| allowMeetingChat      | [meetingChatMode](#meetingchatmode-values) | 指定会议聊天模式。 |
| allowTeamworkReactions | 布尔 | 指示是否为会议启用了 Teams 反应。 |
| alternativeRecording  | Stream | [Microsoft Teams 实时事件](/microsoftteams/teams-live-events/what-are-teams-live-events)的替代录制的内容流。 只读。 |
| attendeeReport        | Stream | [Teams 直播活动的](/microsoftteams/teams-live-events/what-are-teams-live-events)与会者报告的内容流。 只读。   |
| audioConferencing     | [audioConferencing](audioconferencing.md)     | 电话访问 (电话拨入) 联机会议的信息。 只读。 |
| broadcastSettings     | [broadcastMeetingSettings](broadcastMeetingSettings.md)     | 与实时事件相关的设置。      |
| chatInfo              | [chatInfo](chatinfo.md) | 与此联机会议关联的聊天信息。  |
| creationDateTime      | 日期时间 | UTC 中的会议创建时间。 只读。     |
| endDateTime           | 日期时间 | UTC 中的会议结束时间。   |
| externalId            | String | 外部 ID。 自定义 ID。 可选。      |
| id | String | 与联机会议关联的默认 ID。 只读。    |
| isBroadcast | Boolean | 指示这是否是 [Teams 直播活动](/microsoftteams/teams-live-events/what-are-teams-live-events)。 |
| isEntryExitAnnounced  | 布尔 | 指示在呼叫者加入或离开时是要宣布的。 |
| joinWebUrl | String | 联机会议的联接 URL。 只读。 |
| joinInformation | [itemBody](itembody.md) | “Accept-Language”请求 HTTP 标头中指定的语言和区域设置变体中的联接信息。 只读。 |
| lobbyBypassSettings | [lobbyBypassSettings](lobbyBypassSettings.md) | 指定哪些参与者可以绕过会议大厅。 |
| participants | [meetingParticipants](meetingparticipants.md) | 与联机会议关联的参与者。 这包括组织者和与会者。 |
| recordAutomatically | Boolean | 指示是否自动录制会议。 |
| 记录 | Stream | [Teams 实时事件](/microsoftteams/teams-live-events/what-are-teams-live-events)录制的内容流。 只读。 |
| startDateTime | 日期时间 | 会议开始时间（UTC）。 |
| subject | String | 联机会议的主题。 |
| videoTeleconferenceId | String | 视频电话会议 ID。 只读。 |
| autoAdmittedUsers (已弃用)  | String | 指定将自动允许进入联机会议的参与者类型的设置。 可取值为：`everyone`、`everyoneInSameAndFederatedCompany`、`everyoneInCompany`、`invitedUsersInCompany`、`organizer`。 只读。 |
| 功能 (已弃用)  | meetingCapabilities 集合 | 会议功能列表。 可能的值为： `questionAndAnswer`，`unknownFutureValue`。 |

> [!CAUTION]
>
>- **autoAdmittedUsers** 属性已弃用。 请改用 [lobbyBypassSettings](lobbyBypassSettings.md) **的范围** 属性。
>- **功能属性** 已弃用。 请改用 [broadcastMeetingSettings](broadcastMeetingSettings.md) 的 **isQuestionAndAnswerEnabled** 属性。

### <a name="onlinemeetingpresenters-values"></a>onlineMeetingPresenters 值

| 值              | 说明                                                   |
| ------------------ | ------------------------------------------------------------- |
| 每个人 都           | 每个人都是演示者 (这是默认选项) 。             |
| 组织       | 组织者组织中的每个人都是演示者。          |
| roleIsPresenter    | 只有角色为演示者的参与者才是演示者。 |
| 组织者          | 只有组织者是演示者。                           |
| unknownFutureValue | 未知的未来值。                                         |

> [!TIP]
>
> 创建或更新设置为 `roleIsPresenter`**allowedPresenters** 的联机会议时，请在请求正文中包含具有指定与会者 **角色**`presenter`的 **与会者** 的完整列表。

### <a name="meetingchatmode-values"></a>meetingChatMode 值

| 值              | 说明                                                            |
| ------------------ | ---------------------------------------------------------------------- |
| 已启用            | 已启用会议聊天。                                               |
| 禁用           | 会议聊天已禁用。                                              |
| 有限            | 会议聊天已启用，但仅在会议呼叫期间启用。 |
| unknownFutureValue | 未知的未来值。                                                  |

## <a name="relationships"></a>关系

| 关系 | 类型 | 说明 |
| ------------ | ---- | ----------- |
| attendanceReports | [meetingAttendanceReport](meetingAttendanceReport.md)  集合 | 联机会议的出席情况报告。 只读。 |
| 注册 | [meetingRegistrationBase](meetingregistrationbase.md) | 已为联机会议启用的注册。 一个联机会议只能启用一个注册。|
| meetingAttendanceReport (已弃用)  | [meetingAttendanceReport](meetingAttendanceReport.md) | 最新联机会议会话的出席情况报告。 只读。 |

> [!TIP]
>
>- 已弃用 **meetingAttendanceReport** 属性。 为了向后兼容，它将保留在 beta 中。 今后，请使用 **attendanceReports** 属性检索联机会议的出席情况报告。
>- **注册** 类型可以是 [meetingRegistration](meetingregistration.md) 或 [externalMeetingRegistration](externalmeetingregistration.md)，这两者都继承自 [meetingRegistrationBase](meetingregistrationbase.md)。

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
