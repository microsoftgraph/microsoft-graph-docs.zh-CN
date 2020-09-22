---
title: shiftItem 资源类型
description: ShiftItem 代表班次的一个版本。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7b1522ee4b1819b168d5e261a5e8a53138a69ea4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48036966"
---
# <a name="shiftitem-resource-type"></a>shiftItem 资源类型

命名空间：microsoft.graph

代表 [班次](shift.md)的一个版本。

## <a name="properties"></a>属性
| 属性                         | 类型                    | 说明                                                                             |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| 注释               | 字符串                  | 的 shift 说明 `shiftItem` 。      |
| displayName               | string                  | 的 shift 标签 `shiftItem` 。 |
| startDateTime               | DateTimeOffset                  | 的开始日期和时间 `shiftItem` 。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。 必需。 |
| endDateTime               | DateTimeOffset                 | 的结束日期和时间 `shiftItem` 。 必需。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。 |
| theme | scheduleEntityTheme   |  支持的颜色：白色;变为表示紫粉色黄色底纹darkBlue;darkGreen;darkPurple;darkPink;darkYellow. |
| activities    | [shiftActivity](shiftactivity.md) 集合   | 班次的增量部分，可包含员工在班次中的时间和地点的详细信息。 例如，工作分配或计划工间休息或午餐。 此为必需属性。 |

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

