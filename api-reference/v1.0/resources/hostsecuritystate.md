---
title: hostSecurityState 资源类型
description: 包含有关主机设备的有 (信息，包括设备、计算机等) 。
ms.localizationpriority: medium
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 3513342aaadb2eaf80a787b26988ff2a638813ac
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59007206"
---
# <a name="hostsecuritystate-resource-type"></a>hostSecurityState 资源类型

命名空间：microsoft.graph

包含有关主机设备的有 (信息，包括设备、计算机等) 。

## <a name="properties"></a>属性

| 属性   | 类型|说明|
|:---------------|:--------|:----------|
|fqdn|String|主机 FQDN (完全限定域名)  (例如 `machine.company.com` ，) 。|
|isAzureAadJoined|Boolean|如此 如果主机已加入域Azure Active Directory域服务。|
|isAzureAadRegistered|Boolean|如果在 BYOD 设备Azure Active Directory注册 (主机（即不是由企业注册完全管理）的主机，) 。|
|isHybridAzureDomainJoined|Boolean|如果主机已加入本地 Active Directory 域，则其为 True。|
|netBiosName|String|本地主机名，不带 DNS 域名。|
|os|String|主机操作系统。  (例如，Windows10、MacOS、RHEL 等) 。|
|privateIpAddress|String|专用 (IPv4) IPv6 地址不可路由 (请参阅 [RFC 1918](https://tools.ietf.org/html/rfc1918)) 警报时显示。|
|publicIpAddress|String|可公开路由的 IPv4 或 IPv6 (请参阅 [RFC 1918](https://tools.ietf.org/html/rfc1918)) 警报时显示的地址。|
|riskScore|String|提供商生成/计算的主机风险评分。  建议的值范围为 0-1，等于百分比。|

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

