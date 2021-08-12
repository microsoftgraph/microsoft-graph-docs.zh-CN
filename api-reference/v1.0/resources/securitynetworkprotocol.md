---
title: securityNetworkProtocol 枚举类型
description: 网络协议的可能值。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: enumPageType
ms.openlocfilehash: 657d13f25707baa7f351622700700aa16a5d277b0d5dd1019843661af3491cb9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54126289"
---
# <a name="securitynetworkprotocol-enum-type"></a>securityNetworkProtocol 枚举类型

命名空间：microsoft.graph

网络协议的可能值。

## <a name="members"></a>成员

|成员|值|说明|
|:---|:---|:---|
|unknown|-1|未知协议。|
|ip|0|Internet 协议。|
|icmp|1| Internet 控制消息协议。|
|ipm|2| Internet 组管理协议。|
|ggp|3| 网关到网关协议。|
|ipv4|4 | Internet 协议版本 4。|
|tcp|6 | 传输控制协议。|
|pup|12 | PARC 通用数据包协议。|
|udp|17 | 用户数据报协议。|
|idp|22| Internet 数据报协议。|
|ipv6|41| Internet 协议版本 6 (ipv6) 。|
|ipv6RoutingHeader|43| ipv6 路由标头。|
|ipv6FragmentHeader|44| ipv6 Fragment 标头。|
|ipSecEncapsulatingSecurityPayload|50| ipv6 封装安全有效负载标头。|
|ipSecAuthenticationHeader|51| ipv6 身份验证标头。|
|icmpV6|58| 适用于 ipv6 的 Internet 控制消息协议。|
|ipv6NoNextHeader|59| ipv6 下一个标题。|
|ipv6DestinationOptions|60| ipv6 目标选项标头。|
|nd|77| Net Disk Protocol (非正式) 。|
|raw|255| 原始 IP 数据包协议。|
|ipx|1000| Internet 数据包Exchange协议。|
|spx|1256| 顺序数据包Exchange协议。|
|spxII|1257| 排序数据包Exchange版本 2 协议。|

