---
title: activityStatistics 资源类型
description: 表示在工作活动上花费的时间, 包括电子邮件、会议、焦点工作、聊天和呼叫。
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 5cee94c1ff36bf30d977b7eb97d77f11d4d2ff5e
ms.sourcegitcommit: 9cd96fcbaae9d2ebaa3f3b69e440a1aea106f535
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/17/2019
ms.locfileid: "36450721"
---
# <a name="activitystatistics-resource-type"></a>activityStatistics 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示用户在工作时间内和工作时间以外的各种工作活动所花费的时间, 用于请求中的指定时间范围, 这将使用一天的聚合周期。

以下类型的统计信息派生自**activityStatistics**:

* [Call](callactivitystatistics.md)
* [聊天](chatactivitystatistics.md)
* [Email](emailactivitystatistics.md)
* [焦点](focusactivitystatistics.md)
* [要求](meetingactivitystatistics.md)

### <a name="activity-id-property"></a>"活动 id" 属性

在 HTTP 请求中, 若要获取某个日期范围内的特定类型的活动统计信息, 可以将此信息表示为以下格式的用户的 activityStatistics 集合的 ID, 其中`{startdate}`和`{enddate}`在 ISO 8601 日历中表示日期格式, `{activity}`可以是 "通话"、"聊天"、"电子邮件"、"焦点" 或 "会议":

```
{activity}_{startdate}_{enddate}
```

例如, ID "email_2019-08-10 _2019-12" 表示指定用户的 emailActivityStatistics 介于2019年8月10日和 2019 12 月12日之间。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [获取 activityStatistics](../api/activitystatistics-get.md) | [activityStatistics](activitystatistics.md) | 在指定的时间范围内获取用户的指定活动的统计信息的属性。 |
| [列出 activityStatistics](../api/activitystatistics-list.md) | [activityStatistics](activitystatistics.md) | 在最后一个完整的星期检索用户的活动统计信息集合的属性。|

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|activity|analyticsActivityType| 返回其统计信息的活动的类型。 可能的值为: `call`、 `chat`、 `email` `focus`、和`meeting`。|
|duration|持续时间|活动所用的总小时数。 值以 ISO 8601 格式表示, 持续时间。|
|endDate|Date|活动结束的日期, 以 ISO 8601 格式表示的日历日期。 例如, 属性值可以是 "2019-07-03", 它遵循 YYYY-MM-DD 格式。|
|id|String| 活动的只读 ID, 表示`{activity}_{startdate}_{enddate}`为。|
|startDate|日期|活动启动的日期, 以 ISO 8601 格式表示的日历日期。 例如, 属性值可以是 "2019-07-04", 它遵循 YYYY-MM-DD 格式。|
|timeZoneUsed|String|用户在 Microsoft Outlook 中设置的时区用于计算。 例如, 属性值可以是 "太平洋标准时间"。|

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