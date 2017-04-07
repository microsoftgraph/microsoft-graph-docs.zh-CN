# <a name="pivottable-resource-type"></a>pivotTable 资源类型

表示 Excel 数据透视表。

### <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[Get workbookPivotTable](../api/workbookpivottable_get.md) | [workbookPivotTable](workbookpivottable.md) |读取 workbookPivotTable 对象的属性和关系。|
|[Refresh](../api/workbookpivottable_refresh.md)|无|刷新数据透视表。    |
|[Refreshall](../api/workbookpivottable_refreshall.md)|无|刷新给定工作表内的所有表。请注意，只能对数据透视表集合执行此操作。|

### <a name="properties"></a>属性
| 属性       | 类型    |说明|
|:---------------|:--------|:----------|
|id|String| 数据透视表的 ID。  只读。|
|name|String|数据透视表对象的名称。    |

### <a name="relationships"></a>关系
| 关系 | 类型    |说明|
|:---------------|:--------|:----------|
|worksheet|[worksheet](worksheet.md)| 包含当前 PivotTable 对象的工作表。只读。    |

### <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookPivotTable"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String"
}

```
