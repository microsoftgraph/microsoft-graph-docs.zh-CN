# <a name="extensionschemaproperty-resource-type"></a>extensionSchemaProperty 资源类型

使用 **extensionSchemaProperty** 资源将属性的名称及其类型定义为 [schemaExtension](schemaextension.md) 定义的一部分。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|名称|String| 被定义为架构扩展组成部分的强类型属性的名称。|
|type|String| 被定义为架构扩展组成部分的属性的类型。允许的值为 *Binary、Boolean、DateTime、Integer* 或 *String*。请参阅下表获取更多详细信息。|

#### <a name="supported-property-data-types"></a>受支持的属性数据类型 
在架构扩展中定义属性时，支持以下数据类型：

| 属性类型 | 备注 |
|-------------|------------|
| Binary | 最多 256 字节。 |
| Boolean | 不受联系人、邮件、活动和帖子支持。 |
| DateTime | 必须以 ISO 8601 格式进行指定。存储为 UTC 格式。 |
| Integer | 32 位值。 不受联系人、邮件、活动和帖子支持。 |
| String | 最多 256 个字符。 |

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.extensionSchemaProperty"
}-->

```json
{
  "name": "String",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "extensionSchemaProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
