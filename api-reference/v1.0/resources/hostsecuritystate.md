---
title: hostSecurityState 资源类型
description: 包含有关主机 (的有状态信息，包括设备、计算机等) 。
ms.localizationpriority: medium
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: ade1d89ee392eae5fe30cab8f85329c285e3590d
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65898936"
---
# <a name="hostsecuritystate-resource-type"></a>hostSecurityState 资源类型

命名空间：microsoft.graph

包含有关主机 (的有状态信息，包括设备、计算机等) 。

## <a name="properties"></a>属性

| 属性   | 类型|说明|
|:---------------|:--------|:----------|
|Fqdn|字符串|主机 FQDN (完全限定的域名)  (例如， `machine.company.com`) 。|
|isAzureAadJoined|Boolean|如此 如果主机已加入 Azure Active Directory 域服务的域。|
|isAzureAadRegistered|Boolean|如此 如果在 Azure Active Directory 设备注册中注册的主机 (BYOD 设备，即并非完全由企业) 管理。|
|isHybridAzureDomainJoined|Boolean|如此 如果主机已将域联接到本地 Active Directory 域。|
|netBiosName|字符串|本地主机名，不带 DNS 域名。|
|os|字符串|主机操作系统。  (例如 Windows10、MacOS、RHEL 等) 。|
|privateIpAddress|字符串|专用 (无法路由) IPv4 或 IPv6 地址， (在警报时查看 [RFC 1918](https://tools.ietf.org/html/rfc1918)) 。|
|publicIpAddress|字符串|可公开路由的 IPv4 或 IPv6 地址 (在警报时查看 [RFC 1918](https://tools.ietf.org/html/rfc1918)) 。|
|riskScore|字符串|主机的提供程序生成/计算风险分数。  建议的值范围为 0-1，这等同于百分比。|

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

