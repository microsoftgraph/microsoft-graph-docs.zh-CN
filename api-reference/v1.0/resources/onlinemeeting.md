---
title: onlineMeeting 资源类型
description: 包含有关会议的信息，包括联接 URL、与会者列表和说明。
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 812f094667b217d167509be324843227e552e0a5
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556224"
---
# <a name="onlinemeeting-resource-type"></a>onlineMeeting 资源类型

命名空间：microsoft.graph

包含有关会议的信息，包括用于加入会议的 URL、与会者列表和说明。

## <a name="methods"></a>Methods

| 方法         | 返回类型 | 说明 |
|:---------------|:--------|:----------|
| [创建 onlineMeeting](../api/application-post-onlineMeetings.md) | [onlineMeeting](onlinemeeting.md) | 创建联机会议。 |
| [获取 onlineMeeting](../api/onlinemeeting-get.md) | [onlineMeeting](onlinemeeting.md) | 读取**onlineMeeting**对象的属性和关系。 |
| [删除 onlineMeeting](../api/onlinemeeting-delete.md) | 无 | 删除联机会议。 |
| [创建或获取 onlineMeeting](../api/onlinemeeting-createorget.md) | [onlineMeeting](onlinemeeting.md) | 使用自定义外部 ID 创建联机会议。 如果会议已存在，请检索其属性。 |

## <a name="properties"></a>属性

| 属性                  | 类型                                                   | 说明                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| audioConferencing         | [audioConferencing](audioconferencing.md)              | 联机会议的电话访问（拨入）信息。 只读。 |
| chatInfo                  | [chatInfo](chatinfo.md)                                | 与此联机会议关联的聊天信息。 |
| creationDateTime          | 日期/时间                                               | 以 UTC 表示的会议创建时间。 只读。 |
| startDateTime             | 日期/时间                                               | 以 UTC 表示的会议开始时间。 |
| endDateTime               | 日期/时间                                               | 以 UTC 表示的会议结束时间。 |
| id                        | 字符串                                                 | 与联机会议关联的默认 ID。 只读。 |
| joinWebUrl                | String                                                 | 联机会议的加入 URL。 只读。|
| participants              | [meetingParticipants](meetingparticipants.md)          | 与联机会议关联的参与者。  这包括组织者和与会者。 |
| subject                   | String                                                 | 联机会议的主题。 |
| videoTeleconferenceId     | String                                                 | 视频电话会议 ID。 只读。 |
| joinInformation | [itemBody](itembody.md) | 请求 HTTP 标头中指定的语言和区域设置变量中的联接信息 `Accept-Language` 。 只读。 |

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onlineMeeting"
}-->
```json
{
  "audioConferencing": {"@odata.type": "#microsoft.graph.audioConferencing"},
  "chatInfo": {"@odata.type": "#microsoft.graph.chatInfo"},
  "creationDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "joinWebUrl": "String",
  "participants": {"@odata.type": "#microsoft.graph.meetingParticipants"},
  "startDateTime": "String (timestamp)",
  "subject": "String",
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
