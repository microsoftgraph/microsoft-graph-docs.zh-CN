---
title: networkConnection 资源类型
description: 包含有关与警报相关的网络连接的有状态信息。
ms.localizationpriority: medium
author: chinguyen1
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: edddb2f14458a0c4afd60465c687f618937f43e8
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59006912"
---
# <a name="networkconnection-resource-type"></a>networkConnection 资源类型

命名空间：microsoft.graph

包含有关与警报相关的网络连接的有状态信息。

## <a name="properties"></a>属性

| 属性   | 类型|说明|
|:---------------|:--------|:----------|
|applicationName|String|管理网络连接应用程序的名称 (例如 Facebook 或 SMTP) 。|
|destinationAddress|String|网络连接 (的目标 IP 地址) 。|
|destinationLocation|String|位置 (IP 地址映射) 网络连接目标相关联的位置。|
|destinationDomain|String|目标 URL 的目标域部分。  (例如"www.contoso.com") 。|
|destinationPort|String|网络连接 (的目标) 。|
|destinationUrl|String|网络连接 URL/URI 字符串 - 不包括参数。  (例如"www.contoso.com/products/default.html") |
|direction|connectionDirection|网络连接方向。 可取值为：`unknown`、`inbound`、`outbound`。|
|domainRegisteredDateTime|DateTimeOffset|目标域的注册日期。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|localDnsName|String|显示在主机本地 DNS 缓存中的本地 DNS 名称解析 (例如，如果"主机"文件被篡改) 。|
|natDestinationAddress|String|网络地址转换目标 IP 地址。|
|natDestinationPort|String|网络地址转换目标端口。|
|natSourceAddress|String|网络地址转换源 IP 地址。|
|natSourcePort|String|网络地址转换源端口。|
|协议|[securityNetworkProtocol](securitynetworkprotocol.md)|网络协议。 可能的值是 `unknown` `ip` `icmp` ：、、、、、、、、、、 `igmp` `ggp` `ipv4` `tcp` `pup` `udp` `idp` `ipv6` `ipv6RoutingHeader` `ipv6FragmentHeader` `ipSecEncapsulatingSecurityPayload` `ipSecAuthenticationHeader` `icmpV6` `ipv6NoNextHeader` `ipv6DestinationOptions` `nd` `raw` `ipx` `spx` `spxII` 。|
|riskScore|String|提供商生成/计算网络连接的风险评分。 建议的值范围为 0-1，等于百分比。|
|sourceAddress|String|源 (，即) 网络连接 (源 IP 地址) 。|
|sourceLocation|String|位置 (IP 地址映射) 网络连接源关联的 IP 地址映射。|
|sourcePort|String|源 (，即) 的 (源 IP 端口) 。|
|status|connectionStatus|网络连接状态。 可取值为：`unknown`、`attempted`、`succeeded`、`blocked`、`failed`。|
|urlParameters|String|参数 (URL) 后缀。|

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

