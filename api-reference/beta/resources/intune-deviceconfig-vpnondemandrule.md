---
title: vpnOnDemandRule 资源类型
description: VPN 按需规则定义。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 71bfbf09f9fcb8de63956855ec3c13fed60a2d604d1a3b1601c1b2f6007e8867
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54131176"
---
# <a name="vpnondemandrule-resource-type"></a>vpnOnDemandRule 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

VPN 按需规则定义。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|ssids|String collection|网络服务集标识符 (SSIDs) 。|
|dnsSearchDomains|String collection|DNS 搜索域。|
|probeUrl|String|探测器的 URL。 如果成功获取此 URL， (不重定向) 200 HTTP 状态代码，则此规则匹配。|
|action|[vpnOnDemandRuleConnectionAction](../resources/intune-deviceconfig-vpnondemandruleconnectionaction.md)|操作。 可取值为：`connect`、`evaluateConnection`、`ignore`、`disconnect`。|
|domainAction|[vpnOnDemandRuleConnectionDomainAction](../resources/intune-deviceconfig-vpnondemandruleconnectiondomainaction.md)|域操作 (仅在 Action 评估连接) 。 可取值为：`connectIfNeeded`、`neverConnect`。|
|domains|String collection|域 (仅在 Action 评估连接连接) 。|
|probeRequiredUrl|字符串|Probe 所需的 URL (仅在 Action 评估连接且 DomainAction 已连接（如果需要）) 。|

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




