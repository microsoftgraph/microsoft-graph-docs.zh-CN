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
# <a name="applevpnalwaysonconfiguration-resource-type"></a><span data-ttu-id="c5d6e-103">appleVpnAlwaysOnConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="c5d6e-103">appleVpnAlwaysOnConfiguration resource type</span></span>

> <span data-ttu-id="c5d6e-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c5d6e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5d6e-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c5d6e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5d6e-106">Always On MacOS 和 iOS IKEv2 的 VPN 配置</span><span class="sxs-lookup"><span data-stu-id="c5d6e-106">Always On VPN configuration for MacOS and iOS IKEv2</span></span>

## <a name="properties"></a><span data-ttu-id="c5d6e-107">属性</span><span class="sxs-lookup"><span data-stu-id="c5d6e-107">Properties</span></span>
|<span data-ttu-id="c5d6e-108">属性</span><span class="sxs-lookup"><span data-stu-id="c5d6e-108">Property</span></span>|<span data-ttu-id="c5d6e-109">类型</span><span class="sxs-lookup"><span data-stu-id="c5d6e-109">Type</span></span>|<span data-ttu-id="c5d6e-110">Description</span><span class="sxs-lookup"><span data-stu-id="c5d6e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5d6e-111">tunnelConfiguration</span><span class="sxs-lookup"><span data-stu-id="c5d6e-111">tunnelConfiguration</span></span>|[<span data-ttu-id="c5d6e-112">vpnTunnelConfigurationType</span><span class="sxs-lookup"><span data-stu-id="c5d6e-112">vpnTunnelConfigurationType</span></span>](../resources/intune-deviceconfig-vpntunnelconfigurationtype.md)|<span data-ttu-id="c5d6e-113">确定特定隧道配置应用于哪些连接。</span><span class="sxs-lookup"><span data-stu-id="c5d6e-113">Determines what connections the specific tunnel configuration applies to.</span></span> <span data-ttu-id="c5d6e-114">可取值为：`wifiAndCellular`、`cellular`、`wifi`。</span><span class="sxs-lookup"><span data-stu-id="c5d6e-114">Possible values are: `wifiAndCellular`, `cellular`, `wifi`.</span></span>|
|<span data-ttu-id="c5d6e-115">userToggleEnabled</span><span class="sxs-lookup"><span data-stu-id="c5d6e-115">userToggleEnabled</span></span>|<span data-ttu-id="c5d6e-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5d6e-116">Boolean</span></span>|<span data-ttu-id="c5d6e-117">允许用户使用 UI 切换 VPN 配置</span><span class="sxs-lookup"><span data-stu-id="c5d6e-117">Allow the user to toggle the VPN configuration using the UI</span></span>|
|<span data-ttu-id="c5d6e-118">voicemailExceptionAction</span><span class="sxs-lookup"><span data-stu-id="c5d6e-118">voicemailExceptionAction</span></span>|[<span data-ttu-id="c5d6e-119">vpnServiceExceptionAction</span><span class="sxs-lookup"><span data-stu-id="c5d6e-119">vpnServiceExceptionAction</span></span>](../resources/intune-deviceconfig-vpnserviceexceptionaction.md)|<span data-ttu-id="c5d6e-120">确定是否将语音邮件服务从始终打开的 VPN 连接中排除。</span><span class="sxs-lookup"><span data-stu-id="c5d6e-120">Determine whether voicemail service will be exempt from the always-on VPN connection.</span></span> <span data-ttu-id="c5d6e-121">可取值为：`forceTrafficViaVPN`、`allowTrafficOutside`、`dropTraffic`。</span><span class="sxs-lookup"><span data-stu-id="c5d6e-121">Possible values are: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.</span></span>|
|<span data-ttu-id="c5d6e-122">airPrintExceptionAction</span><span class="sxs-lookup"><span data-stu-id="c5d6e-122">airPrintExceptionAction</span></span>|[<span data-ttu-id="c5d6e-123">vpnServiceExceptionAction</span><span class="sxs-lookup"><span data-stu-id="c5d6e-123">vpnServiceExceptionAction</span></span>](../resources/intune-deviceconfig-vpnserviceexceptionaction.md)|<span data-ttu-id="c5d6e-124">确定 AirPrint 服务是否将从 always on VPN 连接免除。</span><span class="sxs-lookup"><span data-stu-id="c5d6e-124">Determine whether AirPrint service will be exempt from the always-on VPN connection.</span></span> <span data-ttu-id="c5d6e-125">可取值为：`forceTrafficViaVPN`、`allowTrafficOutside`、`dropTraffic`。</span><span class="sxs-lookup"><span data-stu-id="c5d6e-125">Possible values are: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.</span></span>|
|<span data-ttu-id="c5d6e-126">cellularExceptionAction</span><span class="sxs-lookup"><span data-stu-id="c5d6e-126">cellularExceptionAction</span></span>|[<span data-ttu-id="c5d6e-127">vpnServiceExceptionAction</span><span class="sxs-lookup"><span data-stu-id="c5d6e-127">vpnServiceExceptionAction</span></span>](../resources/intune-deviceconfig-vpnserviceexceptionaction.md)|<span data-ttu-id="c5d6e-128">确定是否将从 "始终打开" VPN 连接中排除手机网络服务。</span><span class="sxs-lookup"><span data-stu-id="c5d6e-128">Determine whether Cellular service will be exempt from the always-on VPN connection.</span></span> <span data-ttu-id="c5d6e-129">可取值为：`forceTrafficViaVPN`、`allowTrafficOutside`、`dropTraffic`。</span><span class="sxs-lookup"><span data-stu-id="c5d6e-129">Possible values are: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.</span></span>|
|<span data-ttu-id="c5d6e-130">allowAllCaptiveNetworkPlugins</span><span class="sxs-lookup"><span data-stu-id="c5d6e-130">allowAllCaptiveNetworkPlugins</span></span>|<span data-ttu-id="c5d6e-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5d6e-131">Boolean</span></span>|<span data-ttu-id="c5d6e-132">指定是否应允许在 vpn 外部使用来自所有固定网络插件的流量</span><span class="sxs-lookup"><span data-stu-id="c5d6e-132">Specifies whether traffic from all captive network plugins should be allowed outside the vpn</span></span>|
|<span data-ttu-id="c5d6e-133">allowedCaptiveNetworkPlugins</span><span class="sxs-lookup"><span data-stu-id="c5d6e-133">allowedCaptiveNetworkPlugins</span></span>|[<span data-ttu-id="c5d6e-134">specifiedCaptiveNetworkPlugins</span><span class="sxs-lookup"><span data-stu-id="c5d6e-134">specifiedCaptiveNetworkPlugins</span></span>](../resources/intune-deviceconfig-specifiedcaptivenetworkplugins.md)|<span data-ttu-id="c5d6e-135">确定是否允许所有、部分或没有本地的固定网络应用</span><span class="sxs-lookup"><span data-stu-id="c5d6e-135">Determines whether all, some, or no non-native captive networking apps are allowed</span></span>|
|<span data-ttu-id="c5d6e-136">allowCaptiveWebSheet</span><span class="sxs-lookup"><span data-stu-id="c5d6e-136">allowCaptiveWebSheet</span></span>|<span data-ttu-id="c5d6e-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5d6e-137">Boolean</span></span>|<span data-ttu-id="c5d6e-138">确定是否允许来自 Websheet 应用的流量在 VPN 之外</span><span class="sxs-lookup"><span data-stu-id="c5d6e-138">Determines whether traffic from the Websheet app is allowed outside of the VPN</span></span>|
|<span data-ttu-id="c5d6e-139">natKeepAliveIntervalInSeconds</span><span class="sxs-lookup"><span data-stu-id="c5d6e-139">natKeepAliveIntervalInSeconds</span></span>|<span data-ttu-id="c5d6e-140">Int32</span><span class="sxs-lookup"><span data-stu-id="c5d6e-140">Int32</span></span>|<span data-ttu-id="c5d6e-141">指定通过 VPN 发送网络地址转换保活程序包的频率（以秒为单位）</span><span class="sxs-lookup"><span data-stu-id="c5d6e-141">Specifies how often in seconds to send a network address translation keepalive package through the VPN</span></span>|
|<span data-ttu-id="c5d6e-142">natKeepAliveOffloadEnable</span><span class="sxs-lookup"><span data-stu-id="c5d6e-142">natKeepAliveOffloadEnable</span></span>|<span data-ttu-id="c5d6e-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5d6e-143">Boolean</span></span>|<span data-ttu-id="c5d6e-144">设备处于睡眠状态时启用 NAT 保活信号的硬件卸载</span><span class="sxs-lookup"><span data-stu-id="c5d6e-144">Enable hardware offloading of NAT keepalive signals when the device is asleep</span></span>|

## <a name="relationships"></a><span data-ttu-id="c5d6e-145">关系</span><span class="sxs-lookup"><span data-stu-id="c5d6e-145">Relationships</span></span>
<span data-ttu-id="c5d6e-146">无</span><span class="sxs-lookup"><span data-stu-id="c5d6e-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c5d6e-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c5d6e-147">JSON Representation</span></span>
<span data-ttu-id="c5d6e-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c5d6e-148">Here is a JSON representation of the resource.</span></span>
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



