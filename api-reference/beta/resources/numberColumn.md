---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: NumberColumn
ms.openlocfilehash: 27d17d3e9b9d3d1debcd20f2beb916222801ebe9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049097"
---
# <a name="numbercolumn-resource-type"></a>NumberColumn 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

[columnDefinition](columndefinition.md) 资源上的 **numberColumn** 指示该列的值为数字。

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
| **decimalPlaces**  | string | 要显示的小数位数。 有关可能的值的信息，请参阅以下信息。
| **displayAs**      | string | 值在用户体验中的显示方式。 必须为 `number` 或 `percentage` 的其中一个。 如果未指定，则视为 `number`。
| **maximum**        | double | 最大允许值。
| **minimum**        | double | 最小允许值。

## <a name="decimalplaces-values"></a>DecimalPlaces 值

| 值          | 说明
|:---------------|:--------------------------------------------------------------
| **automatic**  | 默认值。 根据需要自动显示小数位数。
| **none**       | 不显示任何小数位数。
| **one**        | 显示一位小数位数。
| **two**        | 显示两位小数位数。
| **three**      | 显示三位小数位数。
| **four**       | 显示四位小数位数。
| **five**       | 显示五位小数位数。

注意：**decimalPlaces** 和 **displayAs** 应用于数字的呈现方式，而不是存储方式。
这些属性可能会更新。

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/NumberColumn"
} -->
