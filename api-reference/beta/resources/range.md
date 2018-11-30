---
title: 区域资源类型
description: 区域表示一个或多个相邻的单元格，例如单元格、行、列、单元格块等。
ms.openlocfilehash: 95951b45653309f1999ca5d8103c5c63a1249ada
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048345"
---
# <a name="range-resource-type"></a>区域资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

区域表示一个或多个相邻的单元格，例如单元格、行、列、单元格块等。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取区域](../api/range-get.md) | [Range](range.md) |读取 range 对象的属性和关系。|
|[Update](../api/range-update.md) | [Range](range.md)   |更新 Range 对象。 |
|[Boundingrect](../api/range-boundingrect.md)|[Range](range.md)|获取包含指定区域的最小 range 对象。例如，“B2:C5”和“D10:E15”的 GetBoundingRect 为“B2:E16”。|
|[Cell](../api/range-cell.md)|[Range](range.md)|根据行和列编号获取包含单个单元格的 range 对象。单元格可以位于父区域外部，只要其保持在工作表网格内即可。返回的单元格位于相对于区域左上角的单元格的位置。|
|[列](../api/range-column.md)|[Range](range.md)|获取范围中包含的列。|
|[Columnsafter](../api/workbookrange-columnsafter.md)|[workbookRangeView](workbookrangeview.md)|获取给定范围右侧的一定数量的列。|
|[Columnsbefore](../api/workbookrange-columnsbefore.md)|[workbookRangeView](workbookrangeview.md)|获取给定范围左侧的一定数量的列。|
|[Entirecolumn](../api/range-entirecolumn.md)|[Range](range.md)|获取表示范围整列的对象。|
|[Entirerow](../api/range-entirerow.md)|[Range](range.md)|获取表示范围整行的对象。|
|[Intersection](../api/range-intersection.md)|[Range](range.md)|获取表示给定范围的矩形交集的范围对象。|
|[Lastcell](../api/range-lastcell.md)|[Range](range.md)|获取区域内的最后一个单元格。例如，“B2:D5”的最后一个单元格是“D5”。|
|[Lastcolumn](../api/range-lastcolumn.md)|[Range](range.md)|获取区域内的最后一列。例如，“B2:D5”的最后一列是“D2:D5”。|
|[Lastrow](../api/range-lastrow.md)|[Range](range.md)|获取区域内的最后一行。例如，“B2:D5”的最后一行是“B5:D5”。|
|[Offsetrange](../api/range-offsetrange.md)|[Range](range.md)|获取表示与指定区域偏移的区域的对象。返回的区域的尺寸将与该区域匹配。如果强制使生成的区域位于工作表网格的边界之外，则会引发异常。|
|[行](../api/range-row.md)|[Range](range.md)|获取范围对象中包含的行。|
|[Rowsabove](../api/workbookrange-rowsabove.md)|[workbookRangeView](workbookrangeview.md)|获取给定范围上方的一定数量的行。|
|[Rowsbelow](../api/workbookrange-rowsbelow.md)|[workbookRangeView](workbookrangeview.md)|获取给定范围下方的一定数量的行。|
|[Usedrange](../api/range-usedrange.md)|[Range](range.md)|返回指定 range 对象的所用范围。|
|[Clear](../api/range-clear.md)|无|清除区域值、格式、填充、边框等。|
|[删除](../api/range-delete.md)|无|删除与区域相关的单元格。|
|[Insert](../api/range-insert.md)|[Range](range.md)|将单个单元格或一系列单元格插入到工作表中取代此区域，并移动其他单元格以留出空间。在现在空白的空间返回新的 Range 对象。|
|[Merge](../api/range-merge.md)|无|将范围单元格合并到工作表的一个区域内。|
|[Resizedrange](../api/workbookrange-resizedrange.md)|[workbookRangeView](workbookrangeview.md)|获取与当前范围对象类似的范围对象，但其右下角可通过一定数量的行和列进行展开（或合拢）。|
|[Unmerge](../api/range-unmerge.md)|无|将范围单元格取消合并为各个单元格。|
|[Visibleview](../api/workbookrange-visibleview.md)|[workbookRangeView](workbookrangeview.md)|获取筛选的范围中的可见范围。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|address|string|表示 A1 样式的区域引用。地址值将包含工作表引用（如 Sheet1!A1:B4）。只读。|
|addressLocal|string|以用户语言表示对指定区域的区域引用。只读。|
|cellCount|整数|区域中的单元格数目。只读。|
|columnCount|整数|表示区域中的列总数。只读。|
|columnHidden|boolean|表示当前区域中的所有列是否隐藏。|
|columnIndex|整数|表示区域中第一个单元格的列编号。从零开始编制索引。只读。|
|formulas|json|表示采用 A1 样式表示法的公式。|
|formulasLocal|json|表示采用 A1 样式表示法的公式，使用用户的语言和数字格式区域设置。例如，英语中的公式 "=SUM(A1, 1.5)" 在德语中将变为 "=SUMME(A1; 1,5)"。|
|formulasR1C1|json|表示采用 R1C1 样式表示法的公式。|
|hidden|boolean|表示当前区域中的所有单元格是否隐藏。只读。|
|numberFormat|json|表示 Excel 中指定单元格的数字格式代码。|
|rowCount|整数|返回区域中的总行数。只读。|
|rowHidden|boolean|表示当前区域中的所有行是否隐藏。|
|rowIndex|整数|返回区域中第一个单元格的行编号。从零开始编制索引。只读。|
|text|json|指定区域的文本值。文本值与单元格宽度无关。在 Excel UI 中替代 # 符号不会影响 API 返回的文本值。只读。|
|valueTypes|string|表示每个单元格的数据类型。可能的值是：`Unknown`、`Empty`、`String`、`Integer`、`Double`、`Boolean`、`Error`。只读。|
|values|json|表示指定区域的原始值。返回的数据类型可能是字符串、数字或布尔值。包含一个将返回错误字符串的错误的单元格。|

## <a name="relationships"></a>Relationships
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|格式|[RangeFormat](rangeformat.md)|返回一个格式对象，其中封装了区域的字体、填充、边框、对齐方式和其他属性。只读。|
|sort|[RangeSort](rangesort.md)|包含当前区域的工作表。只读。|
|工作表|[Worksheet](worksheet.md)|包含当前区域的工作表。只读。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.range"
}-->

```json
{
  "address": "string",
  "addressLocal": "string",
  "cellCount": 1024,
  "columnCount": 1024,
  "columnHidden": true,
  "columnIndex": 1024,
  "formulas": "json",
  "formulasLocal": "json",
  "formulasR1C1": "json",
  "hidden": true,
  "numberFormat": "json",
  "rowCount": 1024,
  "rowHidden": true,
  "rowIndex": 1024,
  "text": "json",
  "valueTypes": "string",
  "values": "json"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
