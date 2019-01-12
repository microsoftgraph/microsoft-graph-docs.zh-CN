---
title: vpnTrafficRule 资源类型
description: VPN 流量规则定义。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5ebabdb491a9b41efdd6d3abb87fd41a0c803df3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923241"
---
# <a name="vpntrafficrule-resource-type"></a>vpnTrafficRule 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

VPN 流量规则定义。
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|name|字符串|名称。|
|协议|Int32|协议 (0-255)。 0 到 255 之间的有效值|
|localPortRanges|[numberRange](../resources/intune-deviceconfig-numberrange.md)集合|仅当协议是 TCP 或 UDP （6 或 17） 时，可以设置本地端口范围。 该集合最多可包含 500 个元素。|
|remotePortRanges|[numberRange](../resources/intune-deviceconfig-numberrange.md)集合|仅当协议是 TCP 或 UDP （6 或 17） 时，可以设置远程端口范围。 该集合最多可包含 500 个元素。|
|localAddressRanges|[iPv4Range](../resources/intune-shared-ipv4range.md)集合|本地地址范围。 该集合最多可包含 500 个元素。|
|remoteAddressRanges|[iPv4Range](../resources/intune-shared-ipv4range.md)集合|远程地址范围。 该集合最多可包含 500 个元素。|
|appId|String|应用程序标识符，如果此通信规则触发应用程序。|
|appType|[vpnTrafficRuleAppType](../resources/intune-deviceconfig-vpntrafficruleapptype.md)|应用程序类型，如果此通信规则触发应用程序。 可取值为：`none`、`desktop`、`universal`。|
|routingPolicyType|[vpnTrafficRuleRoutingPolicyType](../resources/intune-deviceconfig-vpntrafficruleroutingpolicytype.md)|当应用程序触发，该值指示是否启用拆分隧道此路由。 可取值为：`none`、`splitTunnel`、`forceTunnel`。|
|声明|字符串|与此通信规则关联的声明。|

## <a name="relationships"></a>Relationships
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





