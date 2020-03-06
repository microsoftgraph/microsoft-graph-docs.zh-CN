---
title: hostSecurityState 资源类型
description: 包含有关主机的状态信息（包括设备、计算机等）。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 8993e9ac301bc1cc0ae4da4ec66cc131a3e06c18
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531348"
---
# <a name="hostsecuritystate-resource-type"></a>hostSecurityState 资源类型

命名空间：microsoft.graph

包含有关主机的状态信息（包括设备、计算机等）。

## <a name="properties"></a>属性

| 属性   | 类型|说明|
|:---------------|:--------|:----------|
|域名|字符串|主机 FQDN （完全限定的`machine.company.com`域名）（例如）。|
|isAzureAadJoined|Boolean|如此如果主机已加入域到 Azure Active Directory 域服务。|
|isAzureAadRegistered|Boolean|如果主机注册到 Azure Active Directory 设备注册（BYOD 设备，而不是由企业完全管理），则该属性值为 True。|
|isHybridAzureDomainJoined|Boolean|如此如果主机已加入域到本地 Active Directory 域。|
|netBiosName|字符串|本地主机名，不包含 DNS 域名。|
|os|字符串|主机操作系统。 （例如，Windows10、MacOS、RHEL 等）。|
|privateIpAddress|字符串|在出现警报时专用（不可路由） IPv4 或 IPv6 地址（请参阅[RFC 1918](https://tools.ietf.org/html/rfc1918)）。|
|publicIpAddress|字符串|在警报时可公开路由的 IPv4 或 IPv6 地址（请参阅[RFC 1918](https://tools.ietf.org/html/rfc1918)）。|
|riskScore|字符串|主机的提供程序生成/计算的风险分数。  建议的值范围为0-1，这相当于一个百分比。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.hostSecurityState"
}-->

```json
{
  "fqdn": "String",
  "isAzureAadJoined": true,
  "isAzureAadRegistered": true,
  "isHybridAzureDomainJoined": true,
  "netBiosName": "String",
  "os": "String",
  "privateIpAddress": "String",
  "publicIpAddress": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "hostSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
