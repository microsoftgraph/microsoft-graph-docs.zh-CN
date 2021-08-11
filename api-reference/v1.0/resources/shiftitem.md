---
title: shiftItem 资源类型
description: shiftItem 表示班次的版本。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 97891ada6a9587f6ef679bdc13d58564ab407cc623c6c3b339fc7f4e289894c9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54189315"
---
# <a name="shiftitem-resource-type"></a>shiftItem 资源类型

命名空间：microsoft.graph

表示班次 [的版本](shift.md)。

## <a name="properties"></a>属性
| 属性                         | 类型                    | 说明                                                                             |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| notes               | string                  | 的班次说明 `shiftItem` 。      |
| displayName               | string                  | 的 Shift 标签 `shiftItem` 。 |
| startDateTime               | DateTimeOffset                  | 的开始日期和时间 `shiftItem` 。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 必需。 |
| endDateTime               | DateTimeOffset                 | 的结束日期和时间 `shiftItem` 。 必填。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 |
| theme | scheduleEntityTheme   |  支持的颜色：白色;blue;绿色;紫色;粉色;黄色;灰色;darkBlue;darkGreen;darkPurple;darkPink;darkYellow。 |
| activities    | [shiftActivity](shiftactivity.md) 集合   | 班次的增量部分，可涵盖员工在班次的何时及何处的详细信息。 例如，工作分配或计划的休息或午餐。 此为必需属性。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.shiftItem"
}-->
```json
{
  "displayName": "String",
  "notes": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "theme": "String",
  "activities": [{"@odata.type": "microsoft.graph.shiftActivity"}]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "shiftItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

