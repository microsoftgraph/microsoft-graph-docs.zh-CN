---
title: networkConnection 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
ms.openlocfilehash: a20520a729076c7e63079c6dfc803659ace45b9d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880057"
---
# <a name="networkconnection-resource-type"></a>networkConnection 资源类型

 > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

包含有关与通知相关的网络连接的状态信息。

## <a name="properties"></a>属性

| 属性   | 类型|Description|
|:---------------|:--------|:----------|
|applicationName|String|管理网络连接 （例如，Facebook、 SMTP 等） 的应用程序的名称。|
|destinationAddress|字符串|目标 IP 地址 （的网络连接）。|
|destinationDomain|字符串|目标 URL 的目标域部分。 (例如 www.contoso.com)。|
|destinationPort|字符串|目标端口 （的网络连接）。|
|destinationUrl|字符串|网络连接 URL/URI 字符串-排除参数。 (例如 www.contoso.com/products/default.html)|
|方向|connectionDirection|网络连接方向。 可取值为：`unknown`、`inbound`、`outbound`。|
|domainRegisteredDateTime|DateTimeOffset|目标域注册时的日期。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|localDnsName|字符串|在本地 DNS 名称解析 （例如，在情况下的主机文件已被篡改） 出现在主机的本地 DNS 缓存中。|
|natDestinationAddress|字符串|网络地址转换目标 IP 地址。|
|natDestinationPort|字符串|网络地址转换目标端口。|
|natSourceAddress|字符串|网络地址转换源 IP 地址。|
|natSourcePort|字符串|网络地址转换源端口。|
|protocol|[securityNetworkProtocol](securitynetworkprotocolenumtype.md)|网络协议。 可能的值为： `unknown`， `ip`， `icmp`， `igmp`， `ggp`， `ipv4`， `tcp`， `pup`， `udp`， `idp`， `ipv6`， `ipv6RoutingHeader`， `ipv6FragmentHeader`， `ipSecEncapsulatingSecurityPayload`， `ipSecAuthenticationHeader`， `icmpV6`， `ipv6NoNextHeader`， `ipv6DestinationOptions`， `nd`, `raw`, `ipx`, `spx`, `spxII`.|
|riskScore|字符串|提供程序生成/计算风险的网络连接的分数。 建议值的范围为 0-1，这相当于百分比。|
|sourceAddress|字符串|源 （即原点） IP 地址 （的网络连接）。|
|sourcePort|字符串|源 （即原点） IP （网络连接端口）。|
|status|connectionStatus|网络连接状态。 可取值为：`unknown`、`attempted`、`succeeded`、`blocked`、`failed`。|
|urlParameters|字符串|目标 URL 参数 （后缀）。|

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
