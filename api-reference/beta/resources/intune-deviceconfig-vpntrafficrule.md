---
title: vpnTrafficRule 资源类型
description: VPN 流量规则定义。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 79bb70575ad6351a443776637ff07ef139aaafb8
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49276299"
---
# <a name="vpntrafficrule-resource-type"></a>vpnTrafficRule 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

VPN 流量规则定义。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|name|字符串|别名.|
|协议|Int32|协议 (0-255) 。 有效值为0至255|
|localPortRanges|[numberRange](../resources/intune-deviceconfig-numberrange.md) 集合|仅当协议为 TCP 或 UDP (6 或 17) 时，才能设置本地端口范围。 该集合最多可包含 500 个元素。|
|remotePortRanges|[numberRange](../resources/intune-deviceconfig-numberrange.md) 集合|仅当协议为 TCP 或 UDP (6 或 17) 时，才能设置远程端口范围。 该集合最多可包含 500 个元素。|
|localAddressRanges|[iPv4Range](../resources/intune-shared-ipv4range.md) 集合|本地地址范围。 该集合最多可包含 500 个元素。|
|remoteAddressRanges|[iPv4Range](../resources/intune-shared-ipv4range.md) 集合|远程地址范围。 该集合最多可包含 500 个元素。|
|appId|String|应用程序标识符（如果应用程序触发此流量规则）。|
|appType|[vpnTrafficRuleAppType](../resources/intune-deviceconfig-vpntrafficruleapptype.md)|应用程序类型（如果应用程序触发此流量规则）。 可取值为：`none`、`desktop`、`universal`。|
|routingPolicyType|[vpnTrafficRuleRoutingPolicyType](../resources/intune-deviceconfig-vpntrafficruleroutingpolicytype.md)|当应用程序触发时，指示是否要沿此路由启用拆分隧道。 可取值为：`none`、`splitTunnel`、`forceTunnel`。|
|声称|字符串|与此流量规则关联的声明。|

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




