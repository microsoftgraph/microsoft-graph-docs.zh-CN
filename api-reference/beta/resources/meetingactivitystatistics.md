---
title: meetingActivityStatistics 资源类型
description: 表示有关用户的会议活动的信息。
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: aa0e4b12ed260c0f6660544e7f48cfe1ca9cd3dc
ms.sourcegitcommit: 9cd96fcbaae9d2ebaa3f3b69e440a1aea106f535
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/17/2019
ms.locfileid: "36450723"
---
# <a name="meetingactivitystatistics-resource-type"></a>meetingActivityStatistics 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关用户在 Microsoft Outlook、Microsoft 团队或 Skype for Business 会议中所用时间的数据。 这基于[activityStatistics](../resources/activitystatistics.md)。
<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get meetingActivityStatistics](../api/meetingactivitystatistics-get.md) | [meetingActivityStatistics](meetingactivitystatistics.md) | Read properties and relationships of meetingActivityStatistics object; name of the activity for which statistics are returned as “meeting.” |
-->
## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|activity|analyticsActivityType| 为其返回统计信息的会议活动。|
|duration|持续时间|会议上花费的总小时数。 值以 ISO 8601 格式表示, 持续时间。|
|endDate|Date|会议活动结束的日期。 对于日历日期, 该值以 ISO 8601 格式表示。 例如, 属性值可以是 "2019-07-04", 它遵循 YYYY-MM-DD 格式。|
|id|String| 会议活动的只读 ID。|
|startDate|日期|会议活动的开始日期。 对于日历日期, 该值以 ISO 8601 格式表示。 例如, 属性值可以是 "2019-07-03", 它遵循 YYYY-MM-DD 格式。|
|timeZoneUsed|String|用户在 Outlook 日历中设置的 Outlook 时区用于计算。 例如, 属性值可以是 "太平洋标准时间"。|
|afterHours|持续时间|在会议上花费的时间超出工作时间, 基于用户的 Outlook 日历设置的工作时间。 值以 ISO 8601 格式表示, 持续时间。|
|存在|持续时间|在冲突会议中花费的时间 (会议与接受人员的人以及将人员的状态设置为 "忙碌" 的其他会议重叠)。 值以 ISO 8601 格式表示, 持续时间。|
|long|持续时间|长会议花费的时间 (持续时间超过一个小时)。 值以 ISO 8601 格式表示, 持续时间。|
|多|持续时间|人员在会议中花费的时间, 在这种情况下, 用户进行了多任务处理 (读取/发送的电子邮件数量超过最少, 并/或发送的邮件数超过团队或 Skype for Business 中的最少邮件数)。 值以 ISO 8601 格式表示, 持续时间。|
|有条不紊|持续时间|由用户组织的会议所用的时间。 值以 ISO 8601 格式表示, 持续时间。|
|重复性|持续时间|对定期会议花费的时间。 值以 ISO 8601 格式表示, 持续时间。|

## <a name="relationships"></a>关系

无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingActivityStatistics"
}--> 

```json
{
  "activity": "string",
  "duration": "String (ISO 8601 duration)",
  "endDate": "String (ISO 8601)",
  "id": "String (identifier)",
  "startDate": "String (ISO 8601)",
  "timeZoneUsed": "String",
  "afterHours": "String (ISO 8601 duration)",
  "conflicting": "String (ISO 8601 duration)",
  "long": "String (ISO 8601 duration)",
  "multitasking": "String (ISO 8601 duration)",
  "organized": "String (ISO 8601 duration)",
  "recurring": "String (ISO 8601 duration)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingActivityStatistics resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->