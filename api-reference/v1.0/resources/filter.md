# <a name="filter-resource-type"></a>筛选器资源类型

管理表格列的筛选。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[Apply](../api/filter_apply.md)|无|在给定列中应用给定的筛选条件。|
|[Clear](../api/filter_clear.md)|无|清除给定列上的筛选器。|

## <a name="properties"></a>属性

| 名称 | 类型   |说明|
|:---------------|:--------|:----------|
|criteria|[WorkbookFilterCriteria](filtercriteria.md)|给定列上当前应用的筛选器。只读。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookFilter"
}-->

```json
{
  "criteria": {"@odata.type": "microsoft.graph.workbookFilterCriteria" }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->