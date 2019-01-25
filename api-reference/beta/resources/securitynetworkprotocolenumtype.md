---
title: securityNetworkProtocol 枚举
description: 网络协议的可能值。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: b9b4d29bb3af7e52665c00801e5e38e9b208455b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511469"
---
# <a name="securitynetworkprotocol-enum"></a>securityNetworkProtocol 枚举

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

网络协议的可能值。

## <a name="members"></a>成员

|成员|值|说明|
|:---|:---|:---|
|unknown|-1|未知的协议。|
|IP|0%|Internet 协议。|
|icmp|$1| Internet 消息控制协议。|
|igmp|-2| Internet 组管理协议。|
|ggp|-3| 网关之间的协议。|
|ipv4|-4| Internet 协议版本 4。|
|tcp|-6| 传输控制协议。|
|pup|1.2| PARC 通用数据包协议。|
|udp|1.7| 用户数据报协议。|
|idp|2.2| Internet 数据报协议。|
|ipv6|4.1| Internet 协议版本 6 (ipv6)。|
|ipv6RoutingHeader|4.3| ipv6 路由标头。|
|ipv6FragmentHeader|4.4| ipv6 片段标头。|
|ipSecEncapsulatingSecurityPayload|50%| ipv6 正在封装安全负载标头。|
|ipSecAuthenticationHeader|5.1| ipv6 身份验证标头。|
|icmpV6|5.8| Ipv6 的 Internet 控件消息协议。|
|ipv6NoNextHeader|5.9| ipv6 不下一页眉。|
|ipv6DestinationOptions|-60| ipv6 目标选项标头。|
|和|7.7| Net 磁盘协议 （非正式）。|
|Raw|255| 原始 IP 数据包协议。|
|ipx|-1000| Internet 数据包 Exchange 协议。|
|spx|1256| 排序的包交换协议。|
|spxII|1257| 排序的包交换版本 2 协议。|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/securitynetworkprotocolenumtype.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
