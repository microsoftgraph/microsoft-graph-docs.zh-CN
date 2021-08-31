---
title: vpnTrafficRule 资源类型
description: VPN 流量规则定义。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d62c0d2357b3d46cce5654d460853ad063a351ad
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58800051"
---
# <a name="vpntrafficrule-resource-type"></a>vpnTrafficRule 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

VPN 流量规则定义。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|name|String|名称。|
|协议|Int32|协议 (0-255) 。 有效值为 0 到 255|
|localPortRanges|[numberRange](../resources/intune-deviceconfig-numberrange.md) 集合|本地端口范围只能在协议为 TCP 或 UDP (6 或 17 协议时) 。 该集合最多可包含 500 个元素。|
|remotePortRanges|[numberRange](../resources/intune-deviceconfig-numberrange.md) 集合|远程端口范围只能在协议为 TCP 或 UDP (6 或 17 协议时) 。 该集合最多可包含 500 个元素。|
|localAddressRanges|[iPv4Range](../resources/intune-shared-ipv4range.md) 集合|本地地址范围。 该集合最多可包含 500 个元素。|
|remoteAddressRanges|[iPv4Range](../resources/intune-shared-ipv4range.md) 集合|远程地址范围。 该集合最多可包含 500 个元素。|
|appId|String|应用标识符（如果此流量规则由应用触发）。|
|appType|[vpnTrafficRuleAppType](../resources/intune-deviceconfig-vpntrafficruleapptype.md)|应用类型（如果此流量规则由应用触发）。 可取值为：`none`、`desktop`、`universal`。|
|routingPolicyType|[vpnTrafficRuleRoutingPolicyType](../resources/intune-deviceconfig-vpntrafficruleroutingpolicytype.md)|当应用触发时，指示是否沿此路由启用拆分隧道。 可取值为：`none`、`splitTunnel`、`forceTunnel`。|
|claims|字符串|与此流量规则关联的声明。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnTrafficRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnTrafficRule",
  "name": "String",
  "protocols": 1024,
  "localPortRanges": [
    {
      "@odata.type": "microsoft.graph.numberRange",
      "lowerNumber": 1024,
      "upperNumber": 1024
    }
  ],
  "remotePortRanges": [
    {
      "@odata.type": "microsoft.graph.numberRange",
      "lowerNumber": 1024,
      "upperNumber": 1024
    }
  ],
  "localAddressRanges": [
    {
      "@odata.type": "microsoft.graph.iPv4Range",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ],
  "remoteAddressRanges": [
    {
      "@odata.type": "microsoft.graph.iPv4Range",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ],
  "appId": "String",
  "appType": "String",
  "routingPolicyType": "String",
  "claims": "String"
}
```



