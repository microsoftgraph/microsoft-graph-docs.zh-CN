# <a name="networkconnection-resource-type"></a>networkConnection 资源类型

包含有关与通知相关的网络连接的有状态信息。

## <a name="properties"></a>属性

| 属性   | 类型|说明|
|:---------------|:--------|:----------|
|applicationName|字符串|管理网络连接的应用程序的名称 （例如，Facebook、SMTP 等）。|
|destinationAddress|字符串|（网络连接的）目标 IP 地址。|
|destinationDomain|字符串|目标 URL 的目标域部分。 (例如“www.contoso.com”)。|
|destinationPort|字符串|（网络连接的）目标端口。|
|destinationUrl|字符串|网络连接 URL/URI 字符串 - 不包括参数。 (例如“www.contoso.com/products/default.html”)|
|direction|connectionDirection|网络连接方向。 可取值为：`unknown`、`inbound`、`outbound`。|
|domainRegisteredDateTime|DateTimeOffset|注册目标域时的日期。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示： `'2014-01-01T00:00:00Z'`|
|localDnsName|字符串|出现在主机本地 DNS 缓存中的本地 DNS 名称解析（例如，假使“hosts”文件被篡改）。|
|natDestinationAddress|字符串|网络地址转换目标 IP 地址。|
|natDestinationPort|字符串|网络地址转换目标端口。|
|natSourceAddress|字符串|网络地址转换源 IP 地址。|
|natSourcePort|字符串|网络地址转换源端口。|
|protocol|[securityNetworkProtocol](securitynetworkprotocol.md)|网络协议。 可取值为：`unknown`、`ip`、`icmp`、`igmp`、`ggp`、`ipv4`、`tcp`、`pup`、`udp`、`idp`、`ipv6`、`ipv6RoutingHeader`、`ipv6FragmentHeader`、`ipSecEncapsulatingSecurityPayload`、`ipSecAuthenticationHeader`、`icmpV6`、`ipv6NoNextHeader`、`ipv6DestinationOptions`、`nd`、`raw`、`ipx`、`spx`、`spxII`。|
|riskScore|字符串|提供程序生成/计算得出的网络连接风险分数。 建议值的范围为 0-1，相当于百分比。|
|sourceAddress|字符串|（网络连接的）源（即原始）IP 地址。|
|sourcePort|字符串|源（即原始）IP 端口（网络连接）。|
|status|connectionStatus|网络连接状态。 可取值为：`unknown`、`attempted`、`succeeded`、`blocked`、`failed`。|
|urlParameters|字符串|目标 URL 的参数（后缀）。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.networkConnection"
}-->

```json
{
  "applicationName": "String",
  "destinationAddress": "String",
  "destinationDomain": "String",
  "destinationPort": "String",
  "destinationUrl": "String",
  "direction": "@odata.type: microsoft.graph.connectionDirection",
  "domainRegisteredDateTime": "String (timestamp)",
  "localDnsName": "String",
  "natDestinationAddress": "String",
  "natDestinationPort": "String",
  "natSourceAddress": "String",
  "natSourcePort": "String",
  "protocol": "@odata.type: microsoft.graph.securityNetworkProtocol",
  "riskScore": "String",
  "sourceAddress": "String",
  "sourcePort": "String",
  "status": "@odata.type: microsoft.graph.connectionStatus",
  "urlParameters": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "networkConnection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->