---
title: networkConnection 资源类型
description: 包含有关与警报相关的网络连接的有状态信息。
localization_priority: Normal
author: chinguyen1
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 5671726ead3da811c109a9a2afe01c49b665e513
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50719008"
---
# <a name="networkconnection-resource-type"></a>networkConnection 资源类型

命名空间：microsoft.graph

包含有关与警报相关的网络连接的有状态信息。

## <a name="properties"></a>属性

| 属性   | 类型|说明|
|:---------------|:--------|:----------|
|applicationName|String|管理网络连接应用程序的名称 (例如 Facebook 或 SMTP) 。|
|destinationAddress|字符串|网络连接 (的目标 IP 地址) 。|
|destinationLocation|字符串|位置 (IP 地址映射) 网络连接目标关联的位置。|
|destinationDomain|字符串|目标 URL 的目标域部分。  (例如"www.contoso.com") 。|
|destinationPort|字符串|网络连接 (的目标端口) 。|
|destinationUrl|字符串|网络连接 URL/URI 字符串 - 不包括参数。  (例如"www.contoso.com/products/default.html') |
|direction|connectionDirection|网络连接方向。 可取值为：`unknown`、`inbound`、`outbound`。|
|domainRegisteredDateTime|DateTimeOffset|目标域的注册日期。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|localDnsName|字符串|显示在主机本地 DNS 缓存中的本地 DNS 名称解析 (例如，如果"主机"文件被篡改) 。|
|natDestinationAddress|字符串|网络地址转换目标 IP 地址。|
|natDestinationPort|字符串|网络地址转换目标端口。|
|natSourceAddress|字符串|网络地址转换源 IP 地址。|
|natSourcePort|字符串|网络地址转换源端口。|
|协议|[securityNetworkProtocol](securitynetworkprotocol.md)|网络协议。 可能的值是 `unknown` `ip` `icmp` ：、、、、、、、、、、 `igmp` `ggp` `ipv4` `tcp` `pup` `udp` `idp` `ipv6` `ipv6RoutingHeader` `ipv6FragmentHeader` `ipSecEncapsulatingSecurityPayload` `ipSecAuthenticationHeader` `icmpV6` `ipv6NoNextHeader` `ipv6DestinationOptions` `nd` `raw` `ipx` `spx` `spxII` 。|
|riskScore|字符串|提供商生成/计算网络连接的风险评分。 建议的值范围为 0-1，等于百分比。|
|sourceAddress|字符串|源 (，即) 网络连接 (源 IP 地址) 。|
|sourceLocation|字符串|位置 (IP 地址映射) 网络连接源关联的 IP 地址映射。|
|sourcePort|字符串|源 (，即) 网络 (源 IP 端口) 。|
|状态|connectionStatus|网络连接状态。 可取值为：`unknown`、`attempted`、`succeeded`、`blocked`、`failed`。|
|urlParameters|字符串|参数 (URL) 后缀。|

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

