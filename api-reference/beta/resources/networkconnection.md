---
title: networkConnection 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 2221f38c4ba8f8e71030d540985fb93f415bfa19
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722109"
---
# <a name="networkconnection-resource-type"></a>networkConnection 资源类型

命名空间：microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含有关与警报相关的网络连接的有状态信息。

## <a name="properties"></a>属性

| 属性   | 类型|说明|
|:---------------|:--------|:----------|
|applicationName|String|管理网络连接应用程序的名称 (例如 Facebook、SMTP 等) 。|
|destinationAddress|String|网络连接 (目标 IP 地址) 。|
|destinationDomain|String|目标 URL 的目标域部分。  ("www.contoso.com") 。|
|destinationLocation|String|位置 (IP 地址映射) 网络连接目标关联的位置。|
|destinationPort|String|网络连接 (目标端口) 。|
|destinationUrl|String|网络连接 URL/URI 字符串 - 不包括参数。  (例如"www.contoso.com/products/default.html') |
|direction|connectionDirection|网络连接方向。 可取值为：`unknown`、`inbound`、`outbound`。|
|domainRegisteredDateTime|DateTimeOffset|目标域的注册日期。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|localDnsName|String|显示在主机的本地 DNS 缓存中的本地 DNS 名称解析 (例如，如果"主机"文件被篡改) 。|
|natDestinationAddress|String|网络地址转换目标 IP 地址。|
|natDestinationPort|String|网络地址转换目标端口。|
|natSourceAddress|String|网络地址转换源 IP 地址。|
|natSourcePort|String|网络地址转换源端口。|
|协议|securityNetworkProtocol|网络协议。 可能的值是： `unknown` ， ， ， ， ， ， `ip` ， `icmp` `igmp` `ggp` `ipv4` `tcp` `pup` `udp` `idp` `ipv6` `ipv6RoutingHeader` `ipv6FragmentHeader` `ipSecEncapsulatingSecurityPayload` `ipSecAuthenticationHeader` `icmpV6` `ipv6NoNextHeader` `ipv6DestinationOptions` `nd` `raw` `ipx` `spx` `spxII` 。|
|riskScore|String|网络连接的提供程序生成/计算的风险评分。 建议的值范围为 0-1，等于百分比。|
|sourceAddress|String|源 (，即) 的 IP 地址 (的 ip 地址) 。|
|sourceLocation|String|位置 (与网络连接) 关联的 IP 地址映射。|
|sourcePort|String|源 (，例如) IP 端口 (的) 。|
|状态|connectionStatus|网络连接状态。 可取值为：`unknown`、`attempted`、`succeeded`、`blocked`、`failed`。|
|urlParameters|String|参数 (URL) 后缀。|

### <a name="securitynetworkprotocol-values"></a>securityNetworkProtocol 值

|成员|值|说明|
|:---|:---|:---|
|unknown|-1|未知协议。|
|ip|0|Internet 协议。|
|icmp|1| Internet 控制消息协议。|
|i|2 | Internet 组管理协议。|
|ggp|3 | 网关到网关协议。|
|ipv4|4 | Internet 协议版本 4。|
|tcp|6 | 传输控制协议。|
|pup|12 | PARC 通用数据包协议。|
|udp|17 | 用户数据报协议。|
|idp|22| Internet 数据报协议。|
|ipv6|41| Internet 协议版本 6 (ipv6) 。|
|ipv6RoutingHeader|43| ipv6 路由标头。|
|ipv6FragmentHeader|44| ipv6 片段标头。|
|ipSecEncapsulatingSecurityPayload|50| ipv6 封装安全有效负载标头。|
|ipSecAuthenticationHeader|51| ipv6 身份验证标头。|
|icmpV6|58| 适用于 ipv6 的 Internet 控制消息协议。|
|ipv6NoNextHeader|59| ipv6 无下一个标头。|
|ipv6DestinationOptions|60| ipv6 目标选项标头。|
|nd|77| Net Disk Protocol (非正式) 。|
|raw|255| 原始 IP 数据包协议。|
|ipx|1000| Internet 数据包交换协议。|
|spx|1256| 已排序的数据包交换协议。|
|spxII|1257| 已排序的数据包交换版本 2 协议。|

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
  "destinationLocation": "String",
  "destinationPort": "String",
  "destinationUrl": "String",
  "direction": "String",
  "domainRegisteredDateTime": "String (timestamp)",
  "localDnsName": "String",
  "natDestinationAddress": "String",
  "natDestinationPort": "String",
  "natSourceAddress": "String",
  "natSourcePort": "String",
  "protocol": "string",
  "riskScore": "String",
  "sourceAddress": "String",
  "sourceLocation": "String",
  "sourcePort": "String",
  "status": "String",
  "urlParameters": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "networkConnection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


