---
title: recurrenceRange 资源类型
description: '描述了定期事件在哪个日期范围内重复发生。 '
localization_priority: Normal
author: harini84
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 3f3ca18320243eea6e6b1d31b32eb999cf457c99287bb5f3abc5bb2c3d78796a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54126366"
---
# <a name="recurrencerange-resource-type"></a>recurrenceRange 资源类型

命名空间：microsoft.graph

描述了定期[事件](event.md)在哪个日期范围内重复发生。

可以使用下面的 3 种方法之一（具体视方案而定），指定定期事件的日期范围。 虽然必须始终指定日期范围的 **startDate** 值，但定期事件的结束日期可以有多种指定方法。可以指定定期事件在特定日期前结束、没有结束日期或在重复发生特定次数后结束。 请注意，在日期范围内，实际发生的定期事件始终遵循为事件指定的定期模式。 定期事件始终由 [recurrencePattern](recurrencepattern.md)（事件的重复发生频率）和 **recurrenceRange**（事件在哪个日期范围内重复发生）进行定义。

## <a name="properties"></a>属性

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|endDate|Date|定期模式的停止应用日期。 会议的最后一次发生时间可能不是此日期，具体视事件的定期模式而定。 如果 **type** 为 `endDate`，此为必需属性。|
|numberOfOccurrences|Int32|事件重复发生次数。 如果 **type** 为 `numbered`，此为必需属性，且必须为正数。|
|recurrenceTimeZone|String |**startDate** 和 **endDate** 属性的时区。 此为可选属性。 如果未指定，使用的是事件时区。|
|startDate|Date|定期模式的开始应用日期。 会议的第一次发生时间可能是此日期，也可能晚于此日期，具体视事件的定期模式而定。 必须与定期 [事件](event.md)的 **start** 属性值相同。 此为必需属性。|
|type|recurrenceRangeType|定期范围。 可能的值包括 `endDate`、`noEnd`、`numbered`。 必填。|

**type** 属性可用于指定不同类型的 **recurrenceRange**。 请注意每种类型的必需属性，如下表所述。

| type 属性  | 定期范围类型 | 说明 | 示例 | 必需属性 |
|:-------|:---------------|:--------|:--------|:--------|
|`endDate` |有结束日期的范围 | 事件在 **startDate** 到 **endDate**（含边界值）之间遵循相应的定期模式重复发生。 | 事件在日期范围 2017 年 6 月 1 日到 2017 年 6 月 15 日之间重复发生。 | **type**、**startDate**、**endDate** |
|`noEnd`  |无结束日期的范围 | 事件从 **startDate** 起遵循相应的定期模式重复发生。 | 事件在从 2017 年 6 月 1 日起的无限期日期范围内重复发生。 | **type**、**startDate** |
|`numbered`|指定了特定发生次数的范围 | 从 **startDate** 起，事件遵循定期模式重复发生 **numberOfOccurrences** 次。 | 事件在从 2017 年 6 月 1 日起的日期范围内重复发生 10 次。  | **type**、**startDate**、**numberOfOccurrences** |


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recurrenceRange"
}-->

```json
{
  "endDate": "String (timestamp)",
  "numberOfOccurrences": 1024,
  "recurrenceTimeZone": "string",
  "startDate": "String (timestamp)",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recurrenceRange resource",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
  ],
  "tocPath": ""
}-->

