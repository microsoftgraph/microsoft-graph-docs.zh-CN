---
title: vpnOnDemandRule 资源类型
description: VPN 点播规则定义。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8164d1c12aeb172120bb9803d7f3dd98366ec948
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421457"
---
# <a name="vpnondemandrule-resource-type"></a>vpnOnDemandRule 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

VPN 点播规则定义。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|ssid|String 集合|网络服务设置标识符 (Ssid)。|
|dnsSearchDomains|String 集合|DNS 搜索域。|
|probeUrl|String|调查 URL。 如果此 URL 是成功不使用重定向中提取 （返回 200 HTTP 状态代码），此规则匹配。|
|action|[vpnOnDemandRuleConnectionAction](../resources/intune-deviceconfig-vpnondemandruleconnectionaction.md)|操作。 可取值为：`connect`、`evaluateConnection`、`ignore`、`disconnect`。|
|domainAction|[vpnOnDemandRuleConnectionDomainAction](../resources/intune-deviceconfig-vpnondemandruleconnectiondomainaction.md)|域操作 （仅当操作是计算连接时才适用）。 可取值为：`connectIfNeeded`、`neverConnect`。|
|域|String 集合|域 （仅当操作是计算连接时才适用）。|
|probeRequiredUrl|String|探测器所需的 Url （仅操作评估连接并 DomainAction 是连接，必要时才适用）。|

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




