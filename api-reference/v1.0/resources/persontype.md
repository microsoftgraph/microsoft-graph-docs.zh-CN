# <a name="persontype-resource-type"></a>personType 资源类型

表示人员类型。


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.persontype
}-->

```json
{
  "class": "string",
  "subclass": "string"
}

```
## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|class|String|数据源的类型，例如 Person。|
|subclass|String|数据源的次要类型，例如 OrganizationUser。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "persontype resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
