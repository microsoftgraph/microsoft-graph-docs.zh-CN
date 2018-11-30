---
title: meetingTimeSuggestionsResult 资源类型
description: 一组会议时间建议（若有）；如果没有建议，则返回原因。
ms.openlocfilehash: 5504971618e6b8f6fdb82b203142e84c23c595f4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008646"
---
# <a name="meetingtimesuggestionsresult-resource-type"></a>meetingTimeSuggestionsResult 资源类型

一组会议时间建议（若有）；如果没有建议，则返回原因。

下面介绍了 [findMeetingTimes](../api/user-findmeetingtimes.md) 未返回任何会议时间建议的可能原因。

|**emptySuggestionsReason 值**|**原因**|
|:-----|:-----|
| attendeesUnavailable | 所有与会者的忙/闲状态均已知，但任意时间段的与会者出席可能性达不到[会议置信度](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion)阈值（默认为 50%）。|
| attendeesUnavailableOrUnknown | 部分或全部与会者的忙/闲状态未知，导致会议置信度下降至设定的阈值（默认为 50%）以下。如果与会者不是组织内部的，或获取忙/闲信息时出错了，与会者的忙/闲状态就会变成未知。|
| locationsUnavailable | [locationConstraint](locationconstraint.md) 参数的 **isRequired** 属性被指定为必需，但在计算的时间段内尚无可用地点。 |
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
|emptySuggestionsReason|String|不返回任何会议建议的原因。 可能的值为： `attendeesUnavailable`， `attendeesUnavailableOrUnknown`， `locationsUnavailable`， `organizerUnavailable`，或`unknown`。 如果**meetingTimeSuggestions**属性包含任何会议建议，则此属性为空字符串。|
|meetingTimeSuggestions|[meetingTimeSuggestion](meetingtimesuggestion.md) 集合|一组会议时间建议。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeSuggestionsResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->