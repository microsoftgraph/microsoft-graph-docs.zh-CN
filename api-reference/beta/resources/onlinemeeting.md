---
title: onlineMeeting 资源类型
description: 捕获有关会议，包括加入 URL、 与会者列表中，及其说明的信息。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d7009ceaf815986d50c8eb3b64d2541c32f01a88
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519596"
---
# <a name="onlinemeeting-resource-type"></a>onlineMeeting 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

捕获有关会议，包括加入 URL、 与会者列表中，及其说明的信息。

## <a name="methods"></a>方法

| 方法         | 返回类型 | 说明 |
|:---------------|:--------|:----------|
| [获取 onlineMeeting](../api/onlinemeeting-get.md) | [onlineMeeting](onlinemeeting.md) | 读取属性和 onlineMeeting 对象的关系。 |

## <a name="properties"></a>属性

| 属性                  | 类型                                                   | 说明                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| AccessLevel               | String                                                 | 控制允许加入联机会议的访问级别。 可取值为：`everyone`、`invited`、`locked`、`sameEnterprise`、`unknown`。 |
| audioConferencing         | [audioConferencing](audioconferencing.md)              | 代表 onlineMeeting 电话访问信息。 |
| canceledDateTime          | 日期/时间                                               | 当取消会议的时间。 |
| chatInfo                  | [chatInfo](chatinfo.md)                                | 与此会议聊天。 |
| creationDateTime          | 日期/时间                                               | 已创建会议的时间。 ReadOnly
| endDateTime               | 日期/时间                                               | 会议结束时间。 |
| entryExitAnnouncement     | Boolean                                                | 联机会议助理通知状态。 如果启用了出勤通知，联机会议将通过音频会议宣布 participantswho 联接的名称。 |
| expirationDateTime        | 日期/时间                                               | 绝对协调世界时 (UTC) 日期和时间之后可以删除的联机会议。 日期和时间必须在前，一年之间十年后，当前日期和时间的服务器上。 |
| id                        | String                                                 | 与联机会议相关的 ID。 获取 HTTP 请求中用作 id。 只读。 生成的服务器。 |
| isCancelled               | Boolean                                                | 是否已被取消会议。 |
| joinUrl                   | String                                                 | 从 web 加入联机会议时所使用的 URL。 |
| meetingType               | String                                                 | 可取值为：`meetNow`、`scheduled`、`recurring`。 |
| participants              | [meetingParticipants](meetingparticipants.md)          | 相关联的联机会议参与者。  这包括组织者和与会者。 |
| startDateTime             | 日期/时间                                               | 会议的开始时间。 |
| subject                   | String                                                 | 联机会议的主题。 |

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onlineMeeting"
}-->
```json
{
  "accessLevel": "everyone | invited | locked | sameEnterprise",
  "audioConferencing": {"@odata.type": "#microsoft.graph.audioConferencing"},
  "canceledDateTime": "String (timestamp)",
  "chatInfo": {"@odata.type": "#microsoft.graph.chatInfo"},
  "creationDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "entryExitAnnouncement": true,
  "expirationDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "isCancelled": false,
  "joinUrl": "String",
  "meetingType": "meetNow | scheduled | recurring | broadcast",
  "participants": {"@odata.type": "#microsoft.graph.meetingParticipants"},
  "startDateTime": "String (timestamp)",
  "subject": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onlineMeeting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onlinemeeting.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
