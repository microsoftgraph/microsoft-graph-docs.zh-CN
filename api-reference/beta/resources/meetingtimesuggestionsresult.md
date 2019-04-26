---
title: meetingTimeSuggestionsResult 资源类型
description: 会议建议的集合 (如果有), 如果没有, 则为 "原因"。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 1e3fb99e7675544f39b359abd226875a7721e287
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342308"
---
# <a name="meetingtimesuggestionsresult-resource-type"></a>meetingTimeSuggestionsResult 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

会议建议的集合 (如果有), 如果没有, 则为 "原因"。

下面介绍了 [findMeetingTimes](../api/user-findmeetingtimes.md) 未返回任何会议时间建议的可能原因。

|**emptySuggestionsReason 值**|**原因**|
|:-----|:-----|
| attendeesUnavailable | 所有与会者的可用性都是已知的, 但没有足够的与会者可以达到[会议可信度](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion)阈值, 默认情况下, 在任何时间段中, 默认为 50%。|
| attendeesUnavailableOrUnknown | 部分或全部与会者的忙/闲状态未知，导致会议置信度下降至设定的阈值（默认为 50%）以下。如果与会者不是组织内部的，或获取忙/闲信息时出错了，与会者的忙/闲状态就会变成未知。|
| locationsUnavailable | 将**locationConstraint**参数的**isRequired**属性指定为 true, 但在计算的时间段中没有可用的位置。 |
| organizerUnavailable | **isOrganizerOptional** 参数为 false，但组织者在请求的时间范围内不空闲。 |
| unknown | 未返回任何会议时间建议的原因未知。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingTimeSuggestionsResult"
}-->

```json
{
  "emptySuggestionsReason": "String",
  "meetingTimeSuggestions": [{"@odata.type": "microsoft.graph.meetingTimeSuggestion"}]
}

```
## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|emptySuggestionsReason|String|未返回任何会议时间建议的原因。 可取值为：`attendeesUnavailable`、`attendeesUnavailableOrUnknown`、`locationsUnavailable`、`organizerUnavailable` 或 `unknown`。 如果**meetingTimeSuggestions**属性包含任何会议建议, 则此属性为空字符串。|
|meetingTimeSuggestions|[meetingTimeSuggestion](meetingtimesuggestion.md) 集合|一组会议时间建议。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingTimeSuggestionsResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
