---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: NumberColumn
ms.openlocfilehash: 4aaff6539fc9c7ce77029463562c0f8fca57cac6
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2018
ms.locfileid: "23266504"
---
# <a name="numbercolumn-resource-type"></a>NumberColumn 资源类型

[columnDefinition](columnDefinition.md) 资源上的 **numberColumn** 指示该列的值为数字。

## <a name="json-representation"></a>JSON 表示形式

下面是 **numberColumn** 资源的 JSON 表示形式。
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.numberColumn" } -->

```json
{
  "decimalPlaces": "automatic | none | one | two | three | four | five",
  "displayAs": "number | percentage",
  "maximum": 10.551,
  "minimum": 99.993
}
```

## <a name="properties"></a>属性

| 属性名称      | 类型   | 说明
|:-------------------|:-------|:-----------------------------------------------
| **decimalPlaces**  | 字符串 | 要显示的小数位数。 有关可能的值的信息，请参阅以下信息。
| **displayAs**      | 字符串 | 值在用户体验中的显示方式。 必须为 `number` 或 `percentage` 的其中一个。 如果未指定，则视为 `number`。
| **最大值**        | 翻倍 | 最大允许值。
| **最小值**        | 翻倍 | 最小允许值。

## <a name="decimalplaces"></a>DecimalPlaces

| 值          | 说明
|:---------------|:--------------------------------------------------------------
| **自动的**  | 默认值。 根据需要自动显示小数位数。
| **无**       | 不显示任何小数位数。
| **一**        | 显示一位小数位数。
| **二**        | 显示两位小数位数。
| **三**      | 显示三位小数位数。
| **四**       | 显示四位小数位数。
| **五**       | 显示五位小数位数。

注意：**decimalPlaces** 和 **displayAs** 应用于数字的呈现方式，而不是存储方式。
这些属性可能会更新。

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/numbercolumn.md:
      Found potential enums in resource example that weren't defined in a table:(automatic,none,one,two,three,four,five) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/numbercolumn.md:
      Found potential enums in resource example that weren't defined in a table:(number,percentage) are in resource, but () are in table"
  ],
  "tocPath": "Resources/NumberColumn"
} -->
