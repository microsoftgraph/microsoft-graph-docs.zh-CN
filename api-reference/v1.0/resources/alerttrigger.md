# <a name="alerttrigger-resource-type"></a>alertTrigger 资源类型

包含有关触发检测属性的信息 （警报实体中存在属性）。

## <a name="properties"></a>属性

| 属性   | 类型|说明|
|:---------------|:--------|:----------|
|name|字符串|充当检测触发器属性的名称。|
|类型|字符串|用于解释：键值对中属性的类型。 例如，字符串、布尔值、等。|
|value|字符串|充当检测触发器属性的名称。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alertTrigger"
}-->

```json
{
  "name": "String",
  "type": "String",
  "value": "String"
}

```

## <a name="example"></a>示例

```json
{
  "name": "endpointAddress",
  "type": "networkConnection.sourceAddress",
  "value": "10.154.9.40"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alertTrigger resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->