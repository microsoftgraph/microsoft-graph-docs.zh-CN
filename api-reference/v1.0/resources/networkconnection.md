---
title: networkConnection 资源类型
description: 包含有关与警报相关的网络连接的状态信息。
localization_priority: Normal
author: chinguyen1
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 926bfe67ec420ae386d0215b09c91d690f7f58f8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47965391"
---
# <a name="networkconnection-resource-type"></a>networkConnection 资源类型

命名空间：microsoft.graph

包含有关与警报相关的网络连接的状态信息。

## <a name="properties"></a>属性

| 属性   | 类型|说明|
|:---------------|:--------|:----------|
|applicationName|String|管理网络连接的应用程序的名称 (例如，Facebook 或 SMTP) 。|
|destinationAddress|String|网络连接) 的目标 IP 地址 (。|
|destinationLocation|String|通过 IP 地址映射)  (与网络连接的目标相关联的位置。|
|destinationDomain|String|目标 URL 的目标域部分。  (例如 "www.contoso.com" ) 。|
|destinationPort|String|网络连接) 的目标端口 (。|
|destinationUrl|String|网络连接 URL/URI 字符串-不包括参数。  (例如 "www.contoso.com/products/default.html" ) |
|direction|connectionDirection|网络连接方向。 可取值为：`unknown`、`inbound`、`outbound`。|
|domainRegisteredDateTime|DateTimeOffset|注册目标域的日期。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|localDnsName|String|在主机的本地 DNS 缓存中显示的本地 DNS 名称解析 (例如，如果 "hosts" 文件被篡改) 。|
|natDestinationAddress|String|网络地址转换目标 IP 地址。|
|natDestinationPort|String|网络地址转换目标端口。|
|natSourceAddress|String|网络地址转换源 IP 地址。|
|natSourcePort|String|网络地址转换源端口。|
|协议|[securityNetworkProtocol](securitynetworkprotocol.md)|网络协议。 可能的值为：、、、、、、、、、、、、、、、、、、、、、、 `unknown` `ip` `icmp` `igmp` `ggp` `ipv4` `tcp` `pup` `udp` `idp` `ipv6` `ipv6RoutingHeader` `ipv6FragmentHeader` `ipSecEncapsulatingSecurityPayload` `ipSecAuthenticationHeader` `icmpV6` `ipv6NoNextHeader` `ipv6DestinationOptions` `nd` `raw` `ipx` `spx` `spxII` 。|
|riskScore|String|提供程序生成/计算网络连接的风险分数。 建议的值范围为0-1，这相当于一个百分比。|
|sourceAddress|String|源 (（即网络连接) 的来源) IP 地址） (。|
|sourceLocation|String|与网络连接的源相关联的 IP 地址映射)  (位置。|
|sourcePort|String|源 (（即网络连接) 的 IP 端口 (）的来源) 。|
|状态|connectionStatus|网络连接状态。 可取值为：`unknown`、`attempted`、`succeeded`、`blocked`、`failed`。|
|urlParameters|String|参数 (后缀) 的目标 URL。|

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
  "destinationLocation": "String",
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
  "sourceLocation": "String",
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

