# <a name="worksheet-resource-type"></a>工作表资源类型

Excel 工作表是由单元格组成的网格。它可以包含数据、表、图表等。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[Get Worksheet](../api/worksheet_get.md) | [WorkbookWorksheet](worksheet.md) |读取 worksheet 对象的属性和关系。|
|[Create Chart](../api/worksheet_post_charts.md) |[WorkbookChart](chart.md)| 通过发布到图表集合创建新的图表。|
|[List names](../api/worksheet_list_names.md) |[WorkbookNamedItem](nameditem.md) 集合| 获取与工作表关联的命名项的集合。|
|[List charts](../api/worksheet_list_charts.md) |[WorkbookChart](chart.md) 集合| 获取 Chart 对象集合。|
|[Create Table](../api/worksheet_post_tables.md) |[WorkbookTable](table.md)| 通过发布到表集合创建新表。|
|[List tables](../api/worksheet_list_tables.md) |[WorkbookTable](table.md) 集合| 获取 Table 对象集合。|
|[Update](../api/worksheet_update.md) | [WorkbookWorksheet](worksheet.md)   |更新 Worksheet 对象。 |
|[Cell](../api/worksheet_cell.md)|[Range](range.md)|根据行和列编号获取包含单个单元格的 range 对象。单元格可以位于父区域外部，只要其保持在工作表网格内即可。|
|[Range](../api/worksheet_range.md)|[Range](range.md)|获取地址或名称指定的 range 对象。|
|[Usedrange](../api/worksheet_usedrange.md)|[Range](range.md)|使用的区域是包含分配了值或格式化的任何单元格的最小区域。如果工作表为空，此函数将返回左上角的单元格。|
|[Delete](../api/worksheet_delete.md)|无|从工作簿中删除工作表。|
|[List](../api/worksheet_list.md) | [WorkbookWorksheet](worksheet.md) 集合 |获取 worksheet 对象集合。 |
|[Add](../api/worksheetcollection_add.md)|[WorkbookWorksheet](worksheet.md)|向工作簿添加新工作表。将工作表添加到现有工作表的末尾。 |
|[List pivotTables](../api/workbookworksheet_list_pivottables.md) |[workbookPivotTable](workbookpivottable.md) 集合| 获取 workbookPivotTable 对象集合。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|string|返回用于唯一标识指定工作簿中工作表的值。即使工作表被重命名或移动，标识符的值仍然相同。只读。|
|name|string|工作表的显示名称。|
|position|int|工作表在工作簿中的位置，从零开始。|
|visibility|string|工作表的可见性。 可取值为：`Visible`、`Hidden`、`VeryHidden`。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|图表|[WorkbookChart](chart.md) 集合|返回属于工作表的图表的集合。只读。|
|names|[WorkbookNamedItem](nameditem.md) 集合|返回与该工作表关联的名称集合。只读。|
|pivotTables|[workbookPivotTable](workbookpivottable.md) 集合| 属于工作表的 PivotTables 的集合。 |
|protection|[WorkbookWorksheetProtection](worksheetprotection.md)|返回表工作表的工作表保护对象。只读。|
|tables|[WorkbookTable](table.md) 集合|属于工作表的表的集合。只读。|

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
