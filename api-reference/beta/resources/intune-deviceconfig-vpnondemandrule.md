---
title: vpnOnDemandRule 资源类型
description: VPN 点播规则定义。
ms.openlocfilehash: 366dd373d31b04d4f245c2394a7a6e476710cf84
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043535"
---
# <a name="vpnondemandrule-resource-type"></a>vpnOnDemandRule 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

VPN 点播规则定义。
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|ssid|String 集合|网络服务设置标识符 (Ssid)。|
|dnsSearchDomains|String 集合|DNS 搜索域。|
|probeUrl|字符串|调查 URL。 如果此 URL 是成功不使用重定向中提取 （返回 200 HTTP 状态代码），此规则匹配。|
|action|[vpnOnDemandRuleConnectionAction](../resources/intune-deviceconfig-vpnondemandruleconnectionaction.md)|操作。 可取值为：`connect`、`evaluateConnection`、`ignore`、`disconnect`。|
|domainAction|[vpnOnDemandRuleConnectionDomainAction](../resources/intune-deviceconfig-vpnondemandruleconnectiondomainaction.md)|域操作 （仅当操作是计算连接时才适用）。 可取值为：`connectIfNeeded`、`neverConnect`。|
|域|String 集合|域 （仅当操作是计算连接时才适用）。|
|probeRequiredUrl|字符串|探测器所需的 Url （仅操作评估连接并 DomainAction 是连接，必要时才适用）。|

## <a name="relationships"></a>Relationships
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





