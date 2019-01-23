---
title: vpnTrafficRule 资源类型
description: VPN 流量规则定义。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5b28d26356eea113f267c4eb0499f9600671f114
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415283"
---
# <a name="vpntrafficrule-resource-type"></a>vpnTrafficRule 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

VPN 流量规则定义。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|name|String|名称。|
|协议|Int32|协议 (0-255)。 0 到 255 之间的有效值|
|localPortRanges|[numberRange](../resources/intune-deviceconfig-numberrange.md)集合|仅当协议是 TCP 或 UDP （6 或 17） 时，可以设置本地端口范围。 该集合最多可包含 500 个元素。|
|remotePortRanges|[numberRange](../resources/intune-deviceconfig-numberrange.md)集合|仅当协议是 TCP 或 UDP （6 或 17） 时，可以设置远程端口范围。 该集合最多可包含 500 个元素。|
|localAddressRanges|[iPv4Range](../resources/intune-shared-ipv4range.md)集合|本地地址范围。 该集合最多可包含 500 个元素。|
|remoteAddressRanges|[iPv4Range](../resources/intune-shared-ipv4range.md)集合|远程地址范围。 该集合最多可包含 500 个元素。|
|appId|String|应用程序标识符，如果此通信规则触发应用程序。|
|appType|[vpnTrafficRuleAppType](../resources/intune-deviceconfig-vpntrafficruleapptype.md)|应用程序类型，如果此通信规则触发应用程序。 可取值为：`none`、`desktop`、`universal`。|
|routingPolicyType|[vpnTrafficRuleRoutingPolicyType](../resources/intune-deviceconfig-vpntrafficruleroutingpolicytype.md)|当应用程序触发，该值指示是否启用拆分隧道此路由。 可取值为：`none`、`splitTunnel`、`forceTunnel`。|
|声明|String|与此通信规则关联的声明。|

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




