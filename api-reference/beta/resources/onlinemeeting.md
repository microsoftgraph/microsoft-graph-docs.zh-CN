---
title: onlineMeeting 资源类型
description: 捕获有关会议的信息, 包括联接 URL、与会者列表和说明。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d7009ceaf815986d50c8eb3b64d2541c32f01a88
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568856"
---
# <a name="onlinemeeting-resource-type"></a>onlineMeeting 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

捕获有关会议的信息, 包括联接 URL、与会者列表和说明。

## <a name="methods"></a>方法

| 方法         | 返回类型 | 说明 |
|:---------------|:--------|:----------|
| [获取 onlineMeeting](../api/onlinemeeting-get.md) | [onlineMeeting](onlinemeeting.md) | 读取 onlineMeeting 对象的属性和关系。 |

## <a name="properties"></a>属性

| 属性                  | 类型                                                   | 说明                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| accessLevel               | String                                                 | 控制联机会议的许可的访问级别。 可取值为：`everyone`、`invited`、`locked`、`sameEnterprise` 或 `unknown`。 |
| audioConferencing         | [audioConferencing](audioconferencing.md)              | 表示 onlineMeeting 的电话访问信息。 |
| canceledDateTime          | 日期/时间                                               | 取消会议的时间。 |
| chatInfo                  | [chatInfo](chatinfo.md)                                | 与此会议关联的聊天。 |
| creationDateTime          | 日期/时间                                               | 会议的创建时间。 只读.
| endDateTime               | 日期/时间                                               | 会议的结束时间。 |
| entryExitAnnouncement     | Boolean                                                | 联机会议的出席通知状态。 启用出席通知后, 联机会议将宣布 participantswho 的名称通过音频加入会议。 |
| expirationDateTime        | 日期/时间                                               | 可在其后删除联机会议的绝对协调通用时间 (UTC) 日期和时间。 日期和时间必须在服务器上的当前日期和时间之后的一年前一年和之后10年。 |
| id                        | 字符串                                                 | 与联机会议相关联的 ID。 在 GET HTTP 请求中用作 ID。 只读。 由服务器生成。 |
| isCancelled               | Boolean                                                | 会议是否已被取消。 |
| joinUrl                   | String                                                 | 从 web 加入联机会议时使用的 URL。 |
| meetingType               | String                                                 | 可能的值是`meetNow`: `scheduled`、 `recurring`、、`broadcast` |
| participants              | [meetingParticipants](meetingparticipants.md)          | 与联机会议关联的参与者。  这包括组织者和与会者。 |
| startDateTime             | 日期/时间                                               | 会议的开始时间。 |
| 主题                   | String                                                 | 联机会议的主题。 |

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
