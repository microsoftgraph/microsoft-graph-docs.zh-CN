---
title: activityStatistics 资源类型
description: 表示在工作活动上花费的时间，包括电子邮件、会议、焦点工作、聊天和呼叫。
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 18d675b38dd3155b5a06c67fc3164fd315d7c0b2
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/20/2020
ms.locfileid: "42162496"
---
# <a name="activitystatistics-resource-type"></a>activityStatistics 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示用户在工作时间内和工作时间以外的各种工作活动所花费的时间，用于请求中的指定时间范围，这将使用一天的聚合周期。

以下类型的统计信息派生自**activityStatistics**：

* [Call](callactivitystatistics.md)
* [参与](chatactivitystatistics.md)
* [电子邮件](emailactivitystatistics.md)
* [焦点](focusactivitystatistics.md)
* [要求](meetingactivitystatistics.md)

<!--  removing per Mathew 2/6/2020   ### Activity id property

In an HTTP request, to get a specific type of activity statistics within a date range, you can express this information as an ID to the user's collection of activityStatistics in the following format, where `{startdate}` and `{enddate}` are expressed in ISO 8601 calendar date format and `{activity}` can be "call", "chat", "email", "focus", or "meeting":

```
{activity}_{startdate}_{enddate}
```

For example, the ID "email_2019-08-10_2019-08-12" represents the emailActivityStatistics for the specified user between August 10, 2019 and August 12, 2019.
-->
## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 activityStatistics](../api/activitystatistics-list.md) | [activityStatistics](activitystatistics.md) | 在最后一个完整的星期检索用户的活动统计信息集合的属性。|

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|activity|analyticsActivityType| 返回其统计信息的活动的类型。 可能的值为： `call`、 `chat`、 `email` `focus`、和`meeting`。|
|duration|持续时间|活动所用的总小时数。 值以 ISO 8601 格式表示，持续时间。|
|endDate|Date|活动结束的日期，以 ISO 8601 格式表示的日历日期。 例如，属性值可以是 "2019-07-03"，它遵循 YYYY-MM-DD 格式。|
|id|String| 活动的只读 ID，表示`{activity}_{startdate}_{enddate}`为。|
|startDate|日期|活动启动的日期，以 ISO 8601 格式表示的日历日期。 例如，属性值可以是 "2019-07-04"，它遵循 YYYY-MM-DD 格式。|
|timeZoneUsed|String|用户在 Microsoft Outlook 中设置的时区用于计算。 例如，属性值可以是 "太平洋标准时间"。|

## <a name="relationships"></a>关系

无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- { 
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.activityStatistics",
  "keyProperty": "id"
}-->

```json
{
  "activity": "String",
  "duration": "String (ISO 8601 duration)",
  "endDate": "String (ISO 8601 format)",
  "id": "String (identifier)",
  "startDate": "String (ISO 8601 format)",
  "timeZoneUsed": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "activityStatistics resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}--> 