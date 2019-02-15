---
title: meetingTimeSuggestion 资源类型
description: '会议建议, 其中包含会议时间、出勤可能性、个人等信息 '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 379bb4ac4be8e2d8d1bec494cf4d573550d46b55
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057027"
---
# <a name="meetingtimesuggestion-resource-type"></a>meetingTimeSuggestion 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
  "attendeeAvailability": [{"@odata.type": "microsoft.graph.attendeeAvailabilityDataModel"}],
  "confidence": 1024.0,
  "locations": [{"@odata.type": "microsoft.graph.locationDataModel"}],
  "meetingTimeSlot": {"@odata.type": "microsoft.graph.meetingTimeSlotDataModel"},
  "order": 1024,
  "organizerAvailability": "String",
  "suggestionReason": "String"
}

```
## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|attendeeAvailability|[attendeeAvailabilityDataModel](attendeeavailabilitydatamodel.md)集合|显示此会议时间建议中各个与会者的忙/闲状态的数组。|
|confidence|Double|表示所有与会者的出席可能性的百分比值。|
|locations|[locationDataModel](locationdatamodel.md)集合|指定此会议时间建议中各个会议地点的名称和地理位置的数组。|
|meetingTimeSlot|[meetingTimeSlotDataModel](meetingtimeslotdatamodel.md)|建议的会议时间段。|
|organizerAvailability|availabilityStatus| 此会议时间建议中会议组织者的忙/闲状态。可取值为：`free`、`tentative`、`busy`、`oof`、`workingElsewhere`、`unknown`。|
|suggestionReason|String|会议时间建议的理由。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingTimeSuggestion resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/meetingtimesuggestion.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
