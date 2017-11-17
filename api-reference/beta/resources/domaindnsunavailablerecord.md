<a id="domaindnsunavailablerecord-resource-type" class="xliff"></a>

# domainDnsUnavailableRecord 资源类型

查询[域](domain.md)实体的导航属性 **serviceConfigurationRecords** 时，可能会返回一个或多个 [DomainDnsCnameRecord](domaindnscnamerecord.md)、[DomainDnsMxRecord](domaindnsmxrecord.md)、[DomainDnsSrvRecord](domaindnssrvrecord.md) 和/或 [DomainDnsTxtRecord](domaindnstxtrecord.md) 实体。这些实体指示 Microsoft Online Services 可以使用域前必须要添加到域的区域文件的 DNS 记录。无法生成这些实体时，将返回 DomainDnsUnavailableRecord 实体。继承自 [DomainDnsRecord](domaindnsrecord.md) 实体。

<a id="methods" class="xliff"></a>

## 方法
不支持对该资源进行直接查询。请参阅[域](domain.md)主题了解有关如何查询域服务记录的信息。

<a id="properties" class="xliff"></a>

## 属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|说明|String|提供返回 **DomainDnsUnavailableRecord** 实体的原因。 |

<a id="relationships" class="xliff"></a>

## 关系
无

<a id="json-representation" class="xliff"></a>

## JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsUnavailableRecord"
}-->

```json
{
  "canonicalName": "String",
  "description": "String",
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "text": "String",
  "ttl": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsUnavailableRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->