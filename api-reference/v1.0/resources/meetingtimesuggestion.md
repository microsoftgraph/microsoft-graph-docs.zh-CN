---
title: meetingTimeSuggestion 资源类型
description: '会议建议，其中包含会议时间、出勤可能性、个人等信息 '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 048761f3d224cee916f7d1c869c0cbee2fbfb06e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534252"
---
# <a name="meetingtimesuggestion-resource-type"></a>meetingTimeSuggestion 资源类型

命名空间：microsoft.graph

会议时间建议包括会议时间、出席可能性、个人忙/闲状态和可用会议地点等信息。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingTimeSuggestion"
}-->

```json
{
  "attendeeAvailability": [{"@odata.type": "microsoft.graph.attendeeAvailability"}],
  "confidence": 100.0,
  "locations": [{"@odata.type": "microsoft.graph.location"}],
  "meetingTimeSlot": {"@odata.type": "microsoft.graph.timeSlot"},
  "order": 1024,
  "organizerAvailability": "String",
  "suggestionReason": "String"
}

```
## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|attendeeAvailability|[attendeeAvailability](attendeeavailability.md) 集合|显示此会议时间建议中各个与会者的忙/闲状态的数组。|
|confidence|Double|表示所有与会者的出席可能性的百分比值。|
|locations|[location](location.md) 集合|指定此会议时间建议中各个会议地点的名称和地理位置的数组。|
|meetingTimeSlot|[timeSlot](timeslot.md)|建议的会议时间段。|
|顺序|Int32|会议时间建议的顺序按其计算可信度值（从高到低）进行排序，然后按 chronology （如果有相同可信度的建议）。 |
|organizerAvailability|freeBusyStatus| 此会议时间建议中会议组织者的忙/闲状态。 可能的值包括 `free`、`tentative`、`busy`、`oof`、`workingElsewhere`、`unknown`。|
|suggestionReason|String|会议时间建议的理由。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeSuggestion resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
