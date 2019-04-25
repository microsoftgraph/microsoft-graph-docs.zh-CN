---
title: 工作表资源类型
description: Excel 工作表是由单元格组成的网格。 它可以包含数据、表、图表等。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: beffb9747045d0d3792d994237710e886ff0b3d8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523467"
---
# <a name="worksheet-resource-type"></a>工作表资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Excel 工作表是由单元格组成的网格。 它可以包含数据、表、图表等。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取工作表](../api/worksheet-get.md) | [Worksheet](worksheet.md) |读取 worksheet 对象的属性和关系。|
|[创建图表](../api/worksheet-post-charts.md) |[图表](chart.md)| 通过发布到图表集合创建新的图表。|
|[列出名称](../api/worksheet-list-names.md) |[NamedItem](nameditem.md) 集合| 获取与工作表相关联的已命名项目集合。|
|[列出图表](../api/worksheet-list-charts.md) |[图表](chart.md) 集合| 获取 Chart 对象集合。|
|[创建表](../api/worksheet-post-tables.md) |[表](table.md)| 通过发布到表集合创建新表。|
|[列出表](../api/worksheet-list-tables.md) |[Table](table.md) 集合| 获取 Table 对象集合。|
|[更新](../api/worksheet-update.md) | [Worksheet](worksheet.md)   |更新 Worksheet 对象。 |
|[单元格](../api/worksheet-cell.md)|[Range](range.md)|根据行和列编号获取包含单个单元格的 range 对象。单元格可以位于父区域外部，只要其保持在工作表网格内即可。|
|[区域](../api/worksheet-range.md)|[Range](range.md)|获取地址或名称指定的 range 对象。|
|[Usedrange](../api/worksheet-usedrange.md)|[区域](range.md)|使用的区域是包含分配了值或格式化的任何单元格的最小区域。如果工作表为空，此函数将返回左上角的单元格。|
|[删除](../api/worksheet-delete.md)|无|从工作簿中删除工作表。|
|[列出](../api/worksheet-list.md) | [工作表](worksheet.md) 集合 |获取 worksheet 对象集合。 |
|[添加](../api/worksheetcollection-add.md)|[工作表](worksheet.md)|向工作簿添加新工作表。将工作表添加到现有工作表的末尾。 |
|[List pivotTables](../api/workbookworksheet-list-pivottables.md) |[workbookPivotTable](workbookpivottable.md) 集合| 获取一组 workbookPivotTable 对象。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|string|返回用于唯一标识指定工作簿中工作表的值。即使工作表被重命名或移动，标识符的值仍然相同。只读。|
|name|string|工作表的显示名称。|
|position|int|工作表在工作簿中的位置，从零开始。|
|visibility|string|工作表的可见性。可能的值是：`Visible`、`Hidden`、`VeryHidden`。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|图表|[图表](chart.md) 集合|返回属于工作表的图表的集合。只读。|
|names|[NamedItem](nameditem.md) 集合|返回与工作表相关联的名称的集合。 只读。|
|数据|[workbookPivotTable](workbookpivottable.md) 集合| 一组属于工作表的数据透视表对象。 |
|protection|[WorksheetProtection](worksheetprotection.md)|返回表工作表的工作表保护对象。只读。|
|表格|[Table](table.md) 集合|属于工作表的表的集合。只读。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.worksheet"
}-->

```json
{
  "id": "string",
  "name": "string",
  "position": 1024,
  "visibility": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Worksheet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/worksheet.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
