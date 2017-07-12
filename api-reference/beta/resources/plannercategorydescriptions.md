<a id="plannercategorydescriptions-resource-type" class="xliff"></a>

# plannerCategoryDescriptions 资源类型

**plannerCategoryDescriptions** 资源表示已为计划定义的类别的描述性标签。它属于[计划详细信息](plannerplandetails.md)对象。最多可定义 6 个类别。 


<a id="properties" class="xliff"></a>

## 属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|category1|String|与类别 1 相关联的标签|
|category2|String|与类别 2 相关联的标签|
|category3|String|与类别 3 相关联的标签|
|category4|String|与类别 4 相关联的标签|
|category5|String|与类别 5 相关联的标签|
|category6|String|与类别 6 相关联的标签|

<a id="json-representation" class="xliff"></a>

## JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerCategoryDescriptions"
}-->

```json
{
  "category1": "String",
  "category2": "String",
  "category3": "String",
  "category4": "String",
  "category5": "String",
  "category6": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerCategoryDescriptions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->