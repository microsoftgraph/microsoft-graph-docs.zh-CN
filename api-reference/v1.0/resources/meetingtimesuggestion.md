---
title: meetingTimeSuggestion 资源类型
description: '包含会议时间、出席可能性、个人信息的会议建议 '
ms.localizationpriority: medium
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: ce0fec16e243120ff55739aa390c3232c42a0a89
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59118045"
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
|order|Int32|会议时间建议的顺序，按计算置信度值从高到低排序，然后按时间顺序排序（如果存在同样可信度的建议）。 |
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

