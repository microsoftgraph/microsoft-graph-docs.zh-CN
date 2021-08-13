---
title: 工作表资源类型
description: Excel 工作表是由单元格组成的网格。它可以包含数据、表、图表等。
localization_priority: Priority
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 41712584a612e8f9445c7bc67c25394188d3efc8e0328683a1128bbafce26605
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54141264"
---
# <a name="worksheet-resource-type"></a>工作表资源类型

命名空间：microsoft.graph

Excel 工作表是由单元格组成的网格。它可以包含数据、表、图表等。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取工作表](../api/worksheet-get.md) | [WorkbookWorksheet](worksheet.md) |读取 worksheet 对象的属性和关系。|
|[创建图表](../api/worksheet-post-charts.md) |[WorkbookChart](chart.md)| 通过发布到图表集合创建新的图表。|
|[列出名称](../api/worksheet-list-names.md) |[WorkbookNamedItem](nameditem.md) 集合| 获取与工作表关联的命名项的集合。|
|[列出图表](../api/worksheet-list-charts.md) |[WorkbookChart](chart.md) 集合| 获取 Chart 对象集合。|
|[创建表](../api/worksheet-post-tables.md) |[WorkbookTable](table.md)| 通过发布到表集合创建新表。|
|[列出表](../api/worksheet-list-tables.md) |[WorkbookTable](table.md) 集合| 获取 Table 对象集合。|
|[更新](../api/worksheet-update.md) | [WorkbookWorksheet](worksheet.md)   |更新 Worksheet 对象。 |
|[单元格](../api/worksheet-cell.md)|[区域](range.md)|根据行和列编号获取包含单个单元格的 range 对象。单元格可以位于父区域外部，只要其保持在工作表网格内即可。|
|[区域](../api/worksheet-range.md)|[区域](range.md)|获取地址或名称指定的 range 对象。|
|[Usedrange](../api/worksheet-usedrange.md)|[区域](range.md)|使用的区域是包含分配了值或格式化的任何单元格的最小区域。如果工作表为空，此函数将返回左上角的单元格。|
|[删除](../api/worksheet-delete.md)|无|从工作簿中删除工作表。|
|[List](../api/worksheet-list.md) | [WorkbookWorksheet](worksheet.md) 集合 |获取 worksheet 对象集合。 |
|[Add](../api/worksheetcollection-add.md)|[WorkbookWorksheet](worksheet.md)|向工作簿添加新工作表。将工作表添加到现有工作表的末尾。 |
|[List pivotTables](../api/workbookworksheet-list-pivottables.md) |[workbookPivotTable](workbookpivottable.md) 集合| 获取一组 workbookPivotTable 对象。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|string|返回用于唯一标识指定工作簿中工作表的值。即使工作表被重命名或移动，标识符的值仍然相同。只读。|
|name|string|工作表的显示名称。|
|position|int|工作表在工作簿中的位置，从零开始。|
|visibility|string|工作表的可见性。 可能的值包括 `Visible`、`Hidden`、`VeryHidden`。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|图表|[WorkbookChart](chart.md) 集合|返回属于工作表的图表的集合。只读。|
|names|[WorkbookNamedItem](nameditem.md) 集合|返回与该工作表关联的名称集合。只读。|
|pivotTables|[workbookPivotTable](workbookpivottable.md) 集合| 一组属于工作表的数据透视表对象。 |
|保护|[WorkbookWorksheetProtection](worksheetprotection.md)|返回表工作表的工作表保护对象。只读。|
|表格|[WorkbookTable](table.md) 集合|属于工作表的集合。只读。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookWorksheet"
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
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

