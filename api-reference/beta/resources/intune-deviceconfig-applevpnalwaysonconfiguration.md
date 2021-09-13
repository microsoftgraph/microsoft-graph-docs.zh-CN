---
title: appleVpnAlwaysOnConfiguration 资源类型
description: MacOS 和 iOS IKEv2 的始终打开 VPN 配置
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 142b963b39501e06786284a265b5c7dd220537ce
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59106341"
---
# <a name="applevpnalwaysonconfiguration-resource-type"></a>appleVpnAlwaysOnConfiguration 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

MacOS 和 iOS IKEv2 的始终打开 VPN 配置

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|tunnelConfiguration|[vpnTunnelConfigurationType](../resources/intune-deviceconfig-vpntunnelconfigurationtype.md)|确定特定隧道配置应用于的连接。 可取值为：`wifiAndCellular`、`cellular`、`wifi`。|
|userToggleEnabled|Boolean|允许用户使用 UI 切换 VPN 配置|
|voicemailExceptionAction|[vpnServiceExceptionAction](../resources/intune-deviceconfig-vpnserviceexceptionaction.md)|确定是否将语音邮件服务从始终打开的 VPN 连接中排除。 可取值为：`forceTrafficViaVPN`、`allowTrafficOutside`、`dropTraffic`。|
|airPrintExceptionAction|[vpnServiceExceptionAction](../resources/intune-deviceconfig-vpnserviceexceptionaction.md)|确定是否将 AirPrint 服务从始终打开的 VPN 连接中排除。 可取值为：`forceTrafficViaVPN`、`allowTrafficOutside`、`dropTraffic`。|
|cellularExceptionAction|[vpnServiceExceptionAction](../resources/intune-deviceconfig-vpnserviceexceptionaction.md)|确定是否将手机网络服务从始终打开的 VPN 连接中排除。 可取值为：`forceTrafficViaVPN`、`allowTrafficOutside`、`dropTraffic`。|
|allowAllCaptiveNetworkPlugins|Boolean|指定是否应该允许来自所有强制网络插件的流量位于 vpn 之外|
|allowedCaptiveNetworkPlugins|[specifiedCaptiveNetworkPlugins](../resources/intune-deviceconfig-specifiedcaptivenetworkplugins.md)|确定是否允许所有、部分或任何非本机强制网络应用|
|allowCaptiveWebSheet|Boolean|确定是否允许来自 Websheet 应用的流量位于 VPN 之外|
|natKeepAliveIntervalInSeconds|Int32|指定通过 VPN 发送网络地址转换保留包的频繁时间（秒）|
|natKeepAliveOffloadEnable|Boolean|在设备打开时启用 NAT 保持连接信号的硬件卸载|

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



