---
title: hostSecurityState 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: security
author: preetikr
ms.openlocfilehash: 55a947e26b8ebb147ac0ef52d5764435846d30ea
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65899643"
---
# <a name="hostsecuritystate-resource-type"></a>hostSecurityState 资源类型

命名空间：microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含有关主机 (的有状态信息，包括设备、计算机等) 。

## <a name="properties"></a>属性

| 属性   | 类型|说明|
|:---------------|:--------|:----------|
|Fqdn|String|例如，主机 FQDN (完全限定的域名)  (machine.company.com) 。|
|isAzureAadJoined|Boolean|如此 如果主机已加入 Azure Active Directory 域服务的域。|
|isAzureAadRegistered|Boolean|如此 如果在 Azure Active Directory 设备注册中注册的主机 (BYOD 设备，即并非完全由企业) 管理。|
|isHybridAzureDomainJoined|Boolean|如此 如果主机已将域联接到本地 Active Directory 域。|
|netBiosName|String|本地主机名，不带 DNS 域名。|
|os|String|主机操作系统。  (例如 Windows10、MacOS、RHEL 等) 。|
|privateIpAddress|String|专用 (无法路由) IPv4 或 IPv6 地址， (在警报时查看 [RFC 1918](https://tools.ietf.org/html/rfc1918)) 。|
|publicIpAddress|String|可公开路由的 IPv4 或 IPv6 地址 (在警报时查看 [RFC 1918](https://tools.ietf.org/html/rfc1918)) 。|
|riskScore|String|主机的提供程序生成/计算风险分数。  建议的值范围为 0-1，这等同于百分比。|

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
<!--
{
  "type": "#page.annotation",
  "description": "hostSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


