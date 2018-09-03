# <a name="rangeformat-resource-type"></a>RangeFormat 资源类型

一个格式对象，其中封装了区域的字体、填充、边框、对齐方式和其他属性。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 RangeFormat](../api/rangeformat_get.md) | [WorkbookRangeFormat](rangeformat.md) |读取 rangeFormat 对象的属性和关系。|
|[创建 RangeBorder](../api/rangeformat_post_borders.md) |[WorkbookRangeBorder](rangeborder.md)| 通过发布到边框集合创建新的 RangeBorder。|
|[列举边框](../api/rangeformat_list_borders.md) |[WorkbookRangeBorder](rangeborder.md) 集合| 获取 RangeBorder 对象集合。|
|[更新](../api/rangeformat_update.md) | [WorkbookRangeFormat](rangeformat.md) |更新 RangeFormat 对象。 |
|[Autofitcolumns](../api/rangeformat_autofitcolumns.md)|无|根据列中的当前数据更改当前区域的列宽，以达到最佳宽度。|
|[Autofitrows](../api/rangeformat_autofitrows.md)|无|根据列中的当前数据更改当前区域的行高，以达到最佳高度。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|columnWidth|翻倍|获取或设置区域内的所有列的宽度。如果列宽不统一，则返回 NULL。|
|horizontalAlignment|字符串|代表指定对象的水平对齐方式。 可取值为：`General`、`Left`、`Center`、`Right`、`Fill`、`Justify`、`CenterAcrossSelection`、`Distributed`。|
|rowHeight|翻倍|获取或设置区域中所有行的高度。如果行高不统一，则返回 NULL。|
|verticalAlignment|字符串|代表指定对象的垂直对齐方式。 可取值为：`Top`、`Center`、`Bottom`、`Justify`、`Distributed`。|
|wrapText|布尔值|指示 Excel 是否将对象中的文本换行。指示整个区域不具有统一换行设置的空值|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|边框|[WorkbookRangeBorder](rangeborder.md) 集合|应用于所选整个区域的边框的对象集合。只读。|
|填充|[WorkbookRangeFill](rangefill.md)|返回整个区域内定义的填充对象。只读。|
|字体|[WorkbookRangeFont](rangefont.md)|返回所选整个区域内定义的字体对象。只读。|
|保护|[WorkbookFormatProtection](formatprotection.md)|返回区域的格式保护对象。只读。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookRangeFormat"
}-->

```json
{
  "columnWidth": 1024,
  "horizontalAlignment": "string",
  "rowHeight": 1024,
  "verticalAlignment": "string",
  "wrapText": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->