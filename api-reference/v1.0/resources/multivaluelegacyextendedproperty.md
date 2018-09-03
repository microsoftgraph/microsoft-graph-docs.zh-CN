# <a name="multivaluelegacyextendedproperty-resource-type"></a>multiValueLegacyExtendedProperty 资源类型

包含值集合的扩展属性。

有关何时使用开放扩展或扩展属性，以及如何指定扩展属性的详细信息，请参阅[扩展属性概述](../resources/extended-properties-overview.md)。

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[发布](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | 支持的资源实例有：[message](../resources/message.md)、[mailFolder](../resources/mailfolder.md)、[event](../resources/event.md)、[calendar](../resources/calendar.md)、[contact](../resources/contact.md) 或 [contactFolder](../resources/contactfolder.md)。请注意，不支持 [post](../resources/post.md) 组。 | 在新建或现有的支持资源实例中创建 **multiValueLegacyExtendedProperty**。 |
|[获取](../api/multivaluelegacyextendedproperty_get.md) |通过 [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 对象扩展的受支持的资源实例（[message](../resources/message.md)、[mailFolder](../resources/mailfolder.md)、[event](../resources/event.md)、[calendar](../resources/calendar.md)、[contact](../resources/contact.md)、[contactFolder](../resources/contactfolder.md) 或 [post](../resources/post.md) 组）。 |使用 `$expand` 获取具有扩展属性的资源实例。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|ID|字符串|属性标识符。只读。|
|值|字符串集合|属性值的集合。|

## <a name="relationships"></a>关系
无


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty"
}-->

```json
{
  "id": "string (identifier)",
  "value": ["string"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "multiValueLegacyExtendedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->