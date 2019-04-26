---
title: securityNetworkProtocol 枚举
description: 网络协议的可能值。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: b9b4d29bb3af7e52665c00801e5e38e9b208455b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572449"
---
# <a name="securitynetworkprotocol-enum"></a>securityNetworkProtocol 枚举

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

网络协议的可能值。

## <a name="members"></a>成员

|成员|值|说明|
|:---|:---|:---|
|unknown|-1|未知协议。|
|ip|0|Internet 协议。|
|icmp|1| Internet 控制邮件协议。|
|igmp|2 | Internet 组管理协议。|
|ggp|3 | 网关到网关协议。|
|ipv4|4 | Internet 协议版本4。|
|tcp|6 | 传输控制协议。|
|pup|12 | PARC 通用数据包协议。|
|udp|×| 用户数据报协议。|
|idp|22| Internet 数据报协议。|
|ipv4|41| Internet 协议版本 6 (ipv6)。|
|ipv6RoutingHeader|43| ipv6 路由头。|
|ipv6FragmentHeader|44| ipv6 分段标头。|
|ipSecEncapsulatingSecurityPayload|50| ipv6 封装安全有效负载标头。|
|ipSecAuthenticationHeader|51| ipv6 身份验证标头。|
|icmpV6|58| ipv6 的 Internet 控制消息协议。|
|ipv6NoNextHeader|59| ipv6 无下一个标头。|
|ipv6DestinationOptions|60| ipv6 目标选项标头。|
|点|77| 网络磁盘协议 (非正式)。|
|原始|255| 原始 IP 数据包协议。|
|通讯|1000| Internet 数据包交换协议。|
|spx|1256| 序列化的数据包交换协议。|
|spxII|1257| 序列化数据包交换第2版协议。|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/securitynetworkprotocolenumtype.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
