---
title: securityNetworkProtocol 枚举类型
description: 网络协议的可能值。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: enumPageType
ms.openlocfilehash: 7b9578977e5855f7b6d4b2fcebbcdda37c95eb7c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47983996"
---
# <a name="securitynetworkprotocol-enum-type"></a>securityNetworkProtocol 枚举类型

命名空间：microsoft.graph

网络协议的可能值。

## <a name="members"></a>成员

|成员|值|说明|
|:---|:---|:---|
|unknown|-1|未知协议。|
|ip|0|Internet 协议。|
|icmp|1 | Internet 控制邮件协议。|
|igmp|2 | Internet 组管理协议。|
|ggp|第三章| 网关到网关协议。|
|ipv4|4 | Internet 协议版本4。|
|tcp|6 | 传输控制协议。|
|pup|12 | PARC 通用数据包协议。|
|udp|17 | 用户数据报协议。|
|idp|22| Internet 数据报协议。|
|ipv4|41| Internet 协议版本 6 (ipv6) 。|
|ipv6RoutingHeader|43| ipv6 路由头。|
|ipv6FragmentHeader|44| ipv6 分段标头。|
|ipSecEncapsulatingSecurityPayload|50| ipv6 封装安全有效负载标头。|
|ipSecAuthenticationHeader|51| ipv6 身份验证标头。|
|icmpV6|58| Ipv6 的 Internet 控制消息协议。|
|ipv6NoNextHeader|59| ipv6 无下一个标头。|
|ipv6DestinationOptions|60| ipv6 目标选项标头。|
|点|77|  (非正式) 的网络磁盘协议。|
|原始|255| 原始 IP 数据包协议。|
|通讯|1000| Internet 数据包交换协议。|
|spx|1256| 序列化的数据包交换协议。|
|spxII|1257| 序列化数据包交换第2版协议。|

