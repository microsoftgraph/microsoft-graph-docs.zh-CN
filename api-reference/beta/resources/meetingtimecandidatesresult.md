---
title: meetingTimeCandidatesResult 资源类型
description: 一组会议时间建议（若有）；如果没有建议，则返回原因。
ms.openlocfilehash: 38ca5b6be15d3cd268403f7f95645a8aaf31cf9d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042193"
---
# <a name="meetingtimecandidatesresult-resource-type"></a>meetingTimeCandidatesResult 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

一组会议时间建议（若有）；如果没有建议，则返回原因。

下面介绍了 [findMeetingTimes](../api/user-findmeetingtimes.md) 未返回任何会议时间建议的可能原因。

|**emptySuggestionsHint 值**|**原因**|
|:-----|:-----|
| attendeesUnavailable | 所有与会者的忙/闲状态均已知，但任意时间段的与会者出席可能性达不到会议置信度阈值（默认为 50%）。 此阈值基于与会者的忙/闲状态的建议会议的时间段，对应于 100%有机会在出勤、 未知的状态 50%，以及忙状态 0%的与会者的免费状态。|
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
  "@odata.type": "microsoft.graph.meetingTimeCandidatesResult"
}-->

```json
{
  "emptySuggestionsHint": "String",
  "meetingTimeSlots": [{"@odata.type": "microsoft.graph.meetingTimeCandidate"}]
}

```
## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|emptySuggestionsHint|字符串|未返回任何会议时间建议的原因。可取值为：`attendeesUnavailable`、`attendeesUnavailableOrUnknown`、`locationsUnavailable`、`organizerUnavailable` 或 `unknown`。|
|meetingTimeSlots|[meetingTimeCandidate](meetingtimecandidate.md)集合|一组会议时间建议。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeCandidatesResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->