---
title: hostSecurityState 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
ms.openlocfilehash: d6f566a2bd42163c570fe837d2419057c62664bb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547408"
---
# <a name="hostsecuritystate-resource-type"></a>hostSecurityState 资源类型

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含有关主机的状态信息 (包括设备、计算机等)。

## <a name="properties"></a>属性

| 属性   | 类型|说明|
|:---------------|:--------|:----------|
|域名|String|主机 FQDN (完全限定的域名) (例如, machine.company.com)。|
|isAzureAadJoined|布尔值|如此如果主机已加入域到 Azure Active Directory 域服务。|
|isAzureAadRegistered|布尔值|如果主机注册到 Azure Active Directory 设备注册 (BYOD 设备, 而不是由企业完全管理), 则该属性值为 True。|
|isHybridAzureDomainJoined|布尔值|如此如果主机已加入域到本地 Active Directory 域。|
|netBiosName|String|本地主机名, 不包含 DNS 域名。|
|os|String|主机操作系统。 (例如, Windows10、MacOS、RHEL 等)。|
|privateIpAddress|String|在出现警报时专用 (不可路由) IPv4 或 IPv6 地址 (请参阅[RFC 1918](https://tools.ietf.org/html/rfc1918))。|
|publicIpAddress|String|在警报时可公开路由的 IPv4 或 IPv6 地址 (请参阅[RFC 1918](https://tools.ietf.org/html/rfc1918))。|
|riskScore|String|主机的提供程序生成/计算的风险分数。  建议的值范围为 0-1, 这相当于一个百分比。|

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
  "suppressions": [
    "Error: /api-reference/beta/resources/hostsecuritystate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
