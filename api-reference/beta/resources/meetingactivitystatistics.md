---
title: meetingActivityStatistics 资源类型
description: 表示有关用户的会议活动的信息。
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 039d2be82a08057c9f9a5405d3591898304a8bcc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522748"
---
# <a name="meetingactivitystatistics-resource-type"></a>meetingActivityStatistics 资源类型

命名空间：microsoft.graph

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
|duration|持续时间|会议上花费的总小时数。 值以 ISO 8601 格式表示，持续时间。|
|endDate|日期|会议活动结束的日期。 对于日历日期，该值以 ISO 8601 格式表示。 例如，属性值可以是 "2019-07-04"，它遵循 YYYY-MM-DD 格式。|
|id|String| 会议活动的只读 ID。|
|startDate|日期|会议活动的开始日期。 对于日历日期，该值以 ISO 8601 格式表示。 例如，属性值可以是 "2019-07-03"，它遵循 YYYY-MM-DD 格式。|
|timeZoneUsed|String|用户在 Outlook 日历中设置的 Outlook 时区用于计算。 例如，属性值可以是 "太平洋标准时间"。|
|afterHours|持续时间|在会议上花费的时间超出工作时间，基于用户的 Outlook 日历设置的工作时间。 值以 ISO 8601 格式表示，持续时间。|
|存在|持续时间|与接受的人员和人员的状态设置为 "忙碌") 的其他会议 (的会议冲突会议所用的时间。 值以 ISO 8601 格式表示，持续时间。|
|long|持续时间|长时间内会议花费的时间 (持续时间) 的一小时以上。 值以 ISO 8601 格式表示，持续时间。|
|多|持续时间|在会议中，人员在多任务工作 (读取/发送的最少电子邮件数和/或发送的邮件数超过最少数量的电子邮件和/或在 Skype for business) 中所用的时间。 值以 ISO 8601 格式表示，持续时间。|
|有条不紊|持续时间|由用户组织的会议所用的时间。 值以 ISO 8601 格式表示，持续时间。|
|重复性|持续时间|对定期会议花费的时间。 值以 ISO 8601 格式表示，持续时间。|

## <a name="relationships"></a>关系

无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.activityStatistics",
  "keyProperty": "id",
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