---
title: onlineMeeting 资源类型
description: 包含有关会议的信息，包括联接 URL、与会者列表和说明。
author: VinodRavichandran
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 64b2c1880edafe1241367ac91889440a513964d9
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006611"
---
# <a name="onlinemeeting-resource-type"></a>onlineMeeting 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含有关会议的信息，包括用于加入会议的 URL、与会者列表和说明。

## <a name="methods"></a>Methods

| 方法         | 返回类型 | 说明 |
|:---------------|:--------|:----------|
| [创建 onlineMeeting](../api/application-post-onlineMeetings.md) | [onlineMeeting](onlinemeeting.md) | 创建联机会议。 |
| [获取 onlineMeeting](../api/onlinemeeting-get.md) | [onlineMeeting](onlinemeeting.md) | 读取**onlineMeeting**对象的属性和关系。 |

## <a name="properties"></a>属性

| 属性                  | 类型                                                   | 说明                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| autoAdmittedUsers         | String                                                 | 指定将自动允许加入联机会议的参与者类型的设置。 只读。 可能的值为`everyone`： `everyoneInSameAndFederatedCompany`、 `everyoneInCompany`、 `invitedUsersInCompany`、`organizer`|
| audioConferencing         | [audioConferencing](audioconferencing.md)              | 联机会议的电话访问（拨入）信息。 只读。 |
| canceledDateTime          | 日期时间                                               | 取消会议时的 UTC 时间（以 UTC 为单位）。 只读。 |
| chatInfo                  | [chatInfo](chatinfo.md)                                | 与此联机会议关联的聊天信息。 |
| creationDateTime          | 日期时间                                               | 以 UTC 表示的会议创建时间。 只读。 |
| startDateTime             | 日期时间                                               | 以 UTC 表示的会议开始时间。 |
| endDateTime               | 日期时间                                               | 以 UTC 表示的会议结束时间。 |
| id                        | 字符串                                                 | 与联机会议关联的默认 ID。 只读。 |
| isCanceled                | 布尔                                                | 指示是否已取消会议。 只读。 |
| joinUrl                   | String                                                 | 联机会议的加入 URL。 只读。|
| isBroadcast               | 布尔                                                | 指示会议是否为广播会议。 |
| participants              | [meetingParticipants](meetingparticipants.md)          | 与联机会议关联的参与者。  这包括组织者和与会者。 |
| subject                   | String                                                 | 联机会议的主题。 |
| capabilities              | String 集合                                      | 会议功能的列表。 可能的值是`questionAndAnswer`：。 |
| videoTeleconferenceId     | String                                                 | Videio 电话会议 ID。 只读。 |

### <a name="autoadmittedusers-values"></a>autoAdmittedUsers 值
| 值 | 说明  |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| 组织者 | 仅会议组织者被直接承认。  其他人将在大厅中等待，直到组织者承认  |
| invitedUsersInCompany | 会议组织者和组织者邀请的同一家公司中的用户直接加入会议。  其他人在大厅等待，直到被许可。  |
| everyoneInCompany | 与组织者在同一公司中的所有人都直接加入会议。  联合匿名用户在大厅等待，直到被许可。  |
| everyoneInSameAndFederatedCompany |  与组织者和联合公司在同一公司中的所有人都直接加入会议。  匿名用户在大厅等待，直到被许可。  |
| 成员 | 任何用户都是允许的，这意味着每个人（包括匿名用户）都可以直接加入会议，而无需在会议厅中等待。  |


## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onlineMeeting"
}-->
```json
{
  "autoAdmittedUsers": "everyone | everyoneInSameAndFederatedCompany | everyoneInCompany | invitedUsersInCompany | organizer",
  "audioConferencing": {"@odata.type": "#microsoft.graph.audioConferencing"},
  "canceledDateTime": "String (timestamp)",
  "chatInfo": {"@odata.type": "#microsoft.graph.chatInfo"},
  "creationDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "isCanceled": false,
  "joinUrl": "String",
  "isBroadcast": false,
  "participants": {"@odata.type": "#microsoft.graph.meetingParticipants"},
  "startDateTime": "String (timestamp)",
  "subject": "String",
  "capabilities": [ "questionAndAnswer" ],
  "videoTeleconferenceId": "String"
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
