---
title: onlineMeeting 资源类型
description: 包含有关会议的信息，包括联接 URL、与会者列表和说明。
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: bfc1055b3e700b951957ffd1bce0fe7a541846b0
ms.sourcegitcommit: 93b6781adf2c889235022d34ab50e2a4d62760c5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/07/2020
ms.locfileid: "46589254"
---
# <a name="onlinemeeting-resource-type"></a>onlineMeeting 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含有关会议的信息，包括用于加入会议的 URL、与会者列表和说明。

## <a name="methods"></a>方法

| 方法         | 返回类型 | 说明 |
|:---------------|:--------|:----------|
| [创建](../api/application-post-onlineMeetings.md) | [onlineMeeting](onlinemeeting.md) | 创建联机会议。 |
| [获取](../api/onlinemeeting-get.md) | [onlineMeeting](onlinemeeting.md) | 读取**onlineMeeting**对象的属性和关系。 |
| [创建或获取 onlineMeeting](../api/onlinemeeting-createorget.md) | [onlineMeeting](onlinemeeting.md) | 使用自定义外部 ID 创建联机会议。 如果会议已存在，请检索其属性。 |
| [更新](../api/onlinemeeting-update.md) | [onlineMeeting](onlinemeeting.md) | 更新联机会议的 " **startDateTime**"、" **endDateTime**"、"**主题**" 和 "**参与者**" 属性。 |
| [删除](../api/onlinemeeting-delete.md) | 无 | 删除**onlineMeeting**资源。 |

## <a name="properties"></a>属性

| 属性                  | 类型                                                   | 说明                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| autoAdmittedUsers         | String                                                 | 指定将自动允许加入联机会议的参与者类型的设置。 可取值为：`everyone`、`everyoneInSameAndFederatedCompany`、`everyoneInCompany`、`invitedUsersInCompany`、`organizer`。 只读。|
| audioConferencing         | [audioConferencing](audioconferencing.md)              | 电话访问 (电话拨入) 联机会议的信息。 只读。 |
| chatInfo                  | [chatInfo](chatinfo.md)                                | 与此联机会议关联的聊天信息。 |
| creationDateTime          | DateTime                                               | 以 UTC 表示的会议创建时间。 只读。 |
| startDateTime             | DateTime                                               | 以 UTC 表示的会议开始时间。 |
| endDateTime               | DateTime                                               | 以 UTC 表示的会议结束时间。 |
| id                        | String                                                 | 与联机会议关联的默认 ID。 只读。 |
| joinWebUrl                   | String                                                 | 联机会议的加入 URL。 只读。|
| participants              | [meetingParticipants](meetingparticipants.md)          | 与联机会议关联的参与者。  这包括组织者和与会者。 |
| subject                   | String                                                 | 联机会议的主题。 |
| capabilities              | String collection                                      | 会议功能的列表。 可能的值是： `questionAndAnswer` 。 |
| videoTeleconferenceId     | String                                                 | 视频电话会议 ID。 只读。 |
| joinInformation | [itemBody](itembody.md) | 在 "Accept-Language" 请求 HTTP 标头中指定的语言和区域设置变量形式的联接信息。 只读 |
| externalId                | String                                                 | 外部 ID。 自定义 ID。 可选。 |

### <a name="autoadmittedusers-values"></a>autoAdmittedUsers 值
| 值 | 说明  |
| :------------------------ | :----------------------------------------------------- |
| organizer － 组织者 | 仅会议组织者被直接承认。  其他人将在大厅中等待，直到组织者承认  |
| invitedUsersInCompany | 会议组织者和组织者邀请的同一家公司中的用户直接加入会议。  其他人在大厅等待，直到被许可。  |
| everyoneInCompany | 与组织者在同一公司中的所有人都直接加入会议。  联合匿名用户在大厅等待，直到被许可。  |
| everyoneInSameAndFederatedCompany |  与组织者和联合公司在同一公司中的所有人都直接加入会议。  匿名用户在大厅等待，直到被许可。  |
| 成员 | 允许任何用户，这意味着每个人 (包括匿名用户) 可以直接加入会议，而无需在会议厅中等待。  |


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
  "autoAdmittedUsers": "everyone | everyoneInSameAndFederatedCompany | everyoneInCompany | invitedUsersInCompany | organizer",
  "audioConferencing": {"@odata.type": "#microsoft.graph.audioConferencing"},
  "chatInfo": {"@odata.type": "#microsoft.graph.chatInfo"},
  "creationDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "joinWebUrl": "String",
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
