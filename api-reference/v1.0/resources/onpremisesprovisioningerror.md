# <a name="onpremisesprovisioningerror-resource-type"></a>onPremisesProvisioningError 资源类型

表示同步本地目录到 Azure Active Directory 目录时 [user](user.md) 和 [group](group.md) 实体的目录同步错误。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
|category|字符串| 设置错误的类别。 注意：当前只有一个可能的值。 可能的值：*PropertyConflict* - 指示属性值不唯一。 其他对象包含属性的相同值。 |
|occurredDateTime|DateTimeOffset| 发生错误的日期 和时间。 |
|propertyCausingError|字符串| 导致此错误的目录属性的名称。 当前的可能值：*UserPrincipalName* 或 *ProxyAddress* |
|value|字符串| 导致错误的属性的值。 |

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesProvisioningError"
}-->

```json
{
  "category": "String",
  "occurredDateTime": "String (timestamp)",
  "propertyCausingError": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesProvisioningError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->