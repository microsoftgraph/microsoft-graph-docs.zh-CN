---
title: vpnOnDemandRule 资源类型
description: VPN 按需规则定义。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b1bccd015e45291b344e7c77df4ac5c0a0af07d0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161584"
---
# <a name="vpnondemandrule-resource-type"></a>vpnOnDemandRule 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

VPN 按需规则定义。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|ssid|String collection|网络服务集标识符 (ssid)。|
|dnsSearchDomains|String collection|DNS 搜索域。|
|probeUrl|String|要探测的 URL。 如果此 URL 已成功获取 (返回 200 HTTP 状态代码) 而不进行重定向, 则此规则匹配。|
|action|[vpnOnDemandRuleConnectionAction](../resources/intune-deviceconfig-vpnondemandruleconnectionaction.md)|退货. 可取值为：`connect`、`evaluateConnection`、`ignore`、`disconnect`。|
|domainAction|[vpnOnDemandRuleConnectionDomainAction](../resources/intune-deviceconfig-vpnondemandruleconnectiondomainaction.md)|域操作 (仅适用于操作评估连接时)。 可取值为：`connectIfNeeded`、`neverConnect`。|
|域|String collection|域 (仅当操作为 "评估连接时" 时适用)。|
|probeRequiredUrl|String|探测器必需 Url (仅在操作评估连接时适用, 如果需要, DomainAction 将进行连接)。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnOnDemandRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnOnDemandRule",
  "ssids": [
    "String"
  ],
  "dnsSearchDomains": [
    "String"
  ],
  "probeUrl": "String",
  "action": "String",
  "domainAction": "String",
  "domains": [
    "String"
  ],
  "probeRequiredUrl": "String"
}
```




