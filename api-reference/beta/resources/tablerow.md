# <a name="tablerow-resource-type"></a>TableRow 资源类型

表示表中的行。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 TableRow](../api/tablerow_get.md) | [TableRow](tablerow.md) |读取 tableRow 对象的属性和关系。|
|[更新](../api/tablerow_update.md) | [TableRow](tablerow.md)    |更新 TableRow 对象。 |
|[区域](../api/tablerow_range.md)|[区域](range.md)|返回与整个行相关的 range 对象。|
|[删除](../api/tablerow_delete.md)|无|从表中删除行。|
|[列出](../api/tablerow_list.md) | [TableRow](tablerow.md) 集合 |获取 tableRow 对象的集合。 |
|[Itemat](../api/tablerowcollection_itemat.md)|[TableRow](tablerow.md)|根据其在集合中的位置获取行。|
|[添加](../api/tablerowcollection_add.md)|[TableRow](tablerow.md)|向表中添加新行。|

## <a name="properties"></a>属性
| 属性       | 类型    |说明|
|:---------------|:--------|:----------|
|index|int|返回表的行集合内行的索引编号。从零开始编制索引。只读。|
|values|json|表示指定区域的原始值。返回的数据类型可能是字符串、数字或布尔值。包含一个将返回错误字符串的错误的单元格。|

## <a name="relationships"></a>关系
无


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tableRow"
}-->

```json
{
  "index": 1024,
  "values": "json"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableRow resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->