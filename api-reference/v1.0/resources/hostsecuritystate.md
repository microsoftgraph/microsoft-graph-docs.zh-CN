---
title: hostSecurityState 资源类型
description: 包含状态信息 （包括设备、 计算机等） 的主机。
localization_priority: Normal
ms.openlocfilehash: 0646547b7f3e31dcf283c1ce423a52b4ae16f013
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816336"
---
# <a name="hostsecuritystate-resource-type"></a>hostSecurityState 资源类型

包含状态信息 （包括设备、 计算机等） 的主机。

## <a name="properties"></a>属性

| 属性   | 类型|Description|
|:---------------|:--------|:----------|
|fqdn|字符串|承载 FQDN （完全限定域名） (例如， `machine.company.com`)。|
|isAzureAadJoined|布尔|如果主机是加入到 Azure Active Directory 域服务的域，则为 true。|
|isAzureAadRegistered|布尔|如果主机注册 Azure Active Directory 设备注册 （BYOD 设备-，即不完全由企业管理），则为 true。|
|isHybridAzureDomainJoined|布尔|如果主机是加入本地 Active Directory 域的域，则为 true。|
|netBiosName|字符串|不带的 DNS 域名的本地主机名称。|
|操作系统|字符串|主机操作系统。 （例如，Windows10 MacOS、 RHEL，等）。|
|privateIpAddress|字符串|专用 （不可穿） 的 IPv4 或 IPv6 地址 （请参阅[RFC 1918](https://tools.ietf.org/html/rfc1918)） 在通知的时间。|
|publicIpAddress|字符串|公共可路由的 IPv4 或 IPv6 地址 （请参阅[RFC 1918](https://tools.ietf.org/html/rfc1918)） 在通知的时间。|
|riskScore|字符串|带有提供程序生成/计算风险的主机的分数。  建议值的范围为 0-1，这相当于百分比。|

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
