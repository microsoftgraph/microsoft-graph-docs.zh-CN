---
title: recurrencePattern 资源类型
description: 描述了定期事件的重复发生频率。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: harini84
ms.openlocfilehash: 04f35e8ca2a1bb46757cb0d8ff1cc46579c8c07f
ms.sourcegitcommit: 1a607ea5bee096944e0fea14167d372f1ff652f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2021
ms.locfileid: "61545373"
---
# <a name="recurrencepattern-resource-type"></a>recurrencePattern 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

描述了定期事件的重复发生频率。 此共享对象用于定义访问评审、日历[事件](event.md)和访问包分配在Azure AD。 [](accessreviewscheduledefinition.md) [](accesspackageassignment.md)

可以使用下面的 6 种方法之一（具体视方案而定），指定定期事件的定期模式。 对于每种类型的模式，请指定时间间隔。 在为事件指定的日期范围内，实际发生的定期事件始终遵循此模式。 定期事件始终由 **recurrencePattern**（事件的重复发生频率）和 [recurrenceRange](recurrencerange.md)（事件在哪个日期范围内重复发生）进行定义。

**type** 属性可用于指定不同类型的 **recurrencePattern**，**interval** 属性可用于指定时间间隔，可以是天数、周数、月数或年数，具体视 **type** 而定。 请注意每种类型的必需属性，如下表所述。

> **注意**：仅添加定期模式需要的属性。 如果添加的任何属性没有受支持的值，则会引发错误。

## <a name="properties"></a>属性

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|dayOfMonth|Int32|事件在相应月份的多少号发生。 如果 **type** 为 `absoluteMonthly` 或 `absoluteYearly`，此为必需属性。 |
|daysOfWeek|dayOfWeek 集合|事件在星期几（一系列值）发生。 可取值包括：`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`。 <br>如果 **type** 为 `relativeMonthly` 或 `relativeYearly`，且 **daysOfWeek** 指定超过一天，事件遵循相应模式的第一天规则。 <br> 如果 **type** 为 `weekly`、`relativeMonthly` 或 `relativeYearly`，此为必需属性。|
|firstDayOfWeek|dayOfWeek|周的第一天。 可取值包括：`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`。 默认值为 `sunday`。 如果 **type** 为 `weekly`，此为必需属性。 |
|index|weekIndex|指定在 **daysOfWeek** 中指定的允许天数的实例发生，从当月的第一个实例开始计数。 可能的值包括 `first`、`second`、`third`、`fourth`、`last`。 默认值为 `first`。 如果 **type** 为 `relativeMonthly` 或 `relativeYearly`，请使用此可选属性。 |
|interval|Int32|间隔的单元数，可以是天数、周数、月数或年数，具体视 **type** 而定。 此为必需属性。 |
|month|Int32|事件发生的月份。  这是一个介于 1 到 12 之间的数字。|
|type|recurrencePatternType|定期模式类型：`daily`、`weekly`、`absoluteMonthly`、`relativeMonthly`、`absoluteYearly` 或 `relativeYearly`。 此为必需属性。 有关详细信息，请参阅 [类型属性的值](#values-of-type-property)。|


> [!IMPORTANT]
> 对于访问评审，仅 **支持 dayOfMonth** **、interval** 和 **type** (`weekly` `absoluteMonthly` ，) 属性。

### <a name="values-of-type-property"></a>type 属性的值

<!-- Note that this isn't a compliant enums declaration format. The recurrencePatternType enum has been declared in the enums.md file so that this H3 section can be customized to provide additional details -->

| type 属性值 | 说明 | 示例 | 必需属性 |
|:--------|:--------|:--------|:----------|
| `daily` | 事件按 **interval** 指定的时间间隔天数重复发生。 | 事件每 3 天重复发生一次。 | **type**、**interval** |
| `weekly` | 事件按时间间隔周数在一周内的一天或几天重复发生。 | 事件每两个星期一和星期二重复发生一次。 | **type**、**interval**、**daysOfWeek**、**firstDayOfWeek** <br/><br/> **注意：** 对于访问评审， **仅支持 interval** **和 type** 属性。|
| `absoluteMonthly` | 事件按时间间隔月数在相应月份的指定一天（例如 15 号）重复发生。 | 事件每季度（每 3 个月）的 15 号重复发生一次。 | **type**、**interval**、**dayOfMonth** <br/><br/> **注意：** 对于访问评审，**仅支持 interval** **、dayOfMonth****和 type** 属性。|
| `relativeMonthly` | 事件按时间间隔月数在一周内的指定一天或几天（相应月份的同一相对位置）重复发生。 | 事件每 3 个月的第二个星期四或星期五重复发生一次。 | **type**、**interval**、**daysOfWeek** |
| `absoluteYearly` | 事件按时间间隔年数在指定月份的一天重复发生。 | 事件每 3 年在 3 月 15 日重复发生一次。 | **type**、**interval**、**dayOfMonth**、**month** |
| `relativeYearly` | 事件按时间间隔年数在一周内的指定一天或几天（相应年份和月份的同一相对位置）重复发生。 | 事件每 3 年在 11 月的第二个星期四或星期五重复发生一次。 | **type**、**interval**、**daysOfWeek**、**month** |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recurrencePattern"
}-->

```json
{
  "dayOfMonth": 1024,
  "daysOfWeek": ["String"],
  "firstDayOfWeek": "String",
  "index": "String",
  "interval": 1024,
  "month": 1024,
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "recurrencePattern resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


