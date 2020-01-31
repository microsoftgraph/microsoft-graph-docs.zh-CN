---
title: appleVpnAlwaysOnConfiguration 资源类型
description: Always On MacOS 和 iOS IKEv2 的 VPN 配置
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c48c22acf2344a0be569835902c20bca21ed0355
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636656"
---
# <a name="applevpnalwaysonconfiguration-resource-type"></a>appleVpnAlwaysOnConfiguration 资源类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Always On MacOS 和 iOS IKEv2 的 VPN 配置

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|tunnelConfiguration|[vpnTunnelConfigurationType](../resources/intune-deviceconfig-vpntunnelconfigurationtype.md)|确定特定隧道配置应用于哪些连接。 可取值为：`wifiAndCellular`、`cellular`、`wifi`。|
|userToggleEnabled|Boolean|允许用户使用 UI 切换 VPN 配置|
|voicemailExceptionAction|[vpnServiceExceptionAction](../resources/intune-deviceconfig-vpnserviceexceptionaction.md)|确定是否将语音邮件服务从始终打开的 VPN 连接中排除。 可取值为：`forceTrafficViaVPN`、`allowTrafficOutside`、`dropTraffic`。|
|airPrintExceptionAction|[vpnServiceExceptionAction](../resources/intune-deviceconfig-vpnserviceexceptionaction.md)|确定 AirPrint 服务是否将从 always on VPN 连接免除。 可取值为：`forceTrafficViaVPN`、`allowTrafficOutside`、`dropTraffic`。|
|cellularExceptionAction|[vpnServiceExceptionAction](../resources/intune-deviceconfig-vpnserviceexceptionaction.md)|确定是否将从 "始终打开" VPN 连接中排除手机网络服务。 可取值为：`forceTrafficViaVPN`、`allowTrafficOutside`、`dropTraffic`。|
|allowAllCaptiveNetworkPlugins|Boolean|指定是否应允许在 vpn 外部使用来自所有固定网络插件的流量|
|allowedCaptiveNetworkPlugins|[specifiedCaptiveNetworkPlugins](../resources/intune-deviceconfig-specifiedcaptivenetworkplugins.md)|确定是否允许所有、部分或没有本地的固定网络应用|
|allowCaptiveWebSheet|Boolean|确定是否允许来自 Websheet 应用的流量在 VPN 之外|
|natKeepAliveIntervalInSeconds|Int32|指定通过 VPN 发送网络地址转换保活程序包的频率（以秒为单位）|
|natKeepAliveOffloadEnable|Boolean|设备处于睡眠状态时启用 NAT 保活信号的硬件卸载|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appleVpnAlwaysOnConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appleVpnAlwaysOnConfiguration",
  "tunnelConfiguration": "String",
  "userToggleEnabled": true,
  "voicemailExceptionAction": "String",
  "airPrintExceptionAction": "String",
  "cellularExceptionAction": "String",
  "allowAllCaptiveNetworkPlugins": true,
  "allowedCaptiveNetworkPlugins": {
    "@odata.type": "microsoft.graph.specifiedCaptiveNetworkPlugins",
    "allowedBundleIdentifiers": [
      "String"
    ]
  },
  "allowCaptiveWebSheet": true,
  "natKeepAliveIntervalInSeconds": 1024,
  "natKeepAliveOffloadEnable": true
}
```



