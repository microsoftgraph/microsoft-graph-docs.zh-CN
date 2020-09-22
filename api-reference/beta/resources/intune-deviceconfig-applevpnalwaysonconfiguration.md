---
title: appleVpnAlwaysOnConfiguration 资源类型
description: Always On MacOS 和 iOS IKEv2 的 VPN 配置
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5bf41b54e64f31cd02a362f7abfcbb2fc12fb434
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48042538"
---
# <a name="applevpnalwaysonconfiguration-resource-type"></a><span data-ttu-id="f4f49-103">appleVpnAlwaysOnConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="f4f49-103">appleVpnAlwaysOnConfiguration resource type</span></span>

<span data-ttu-id="f4f49-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4f49-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f4f49-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f4f49-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4f49-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f4f49-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4f49-107">Always On MacOS 和 iOS IKEv2 的 VPN 配置</span><span class="sxs-lookup"><span data-stu-id="f4f49-107">Always On VPN configuration for MacOS and iOS IKEv2</span></span>

## <a name="properties"></a><span data-ttu-id="f4f49-108">属性</span><span class="sxs-lookup"><span data-stu-id="f4f49-108">Properties</span></span>
|<span data-ttu-id="f4f49-109">属性</span><span class="sxs-lookup"><span data-stu-id="f4f49-109">Property</span></span>|<span data-ttu-id="f4f49-110">类型</span><span class="sxs-lookup"><span data-stu-id="f4f49-110">Type</span></span>|<span data-ttu-id="f4f49-111">说明</span><span class="sxs-lookup"><span data-stu-id="f4f49-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4f49-112">tunnelConfiguration</span><span class="sxs-lookup"><span data-stu-id="f4f49-112">tunnelConfiguration</span></span>|[<span data-ttu-id="f4f49-113">vpnTunnelConfigurationType</span><span class="sxs-lookup"><span data-stu-id="f4f49-113">vpnTunnelConfigurationType</span></span>](../resources/intune-deviceconfig-vpntunnelconfigurationtype.md)|<span data-ttu-id="f4f49-114">确定特定隧道配置应用于哪些连接。</span><span class="sxs-lookup"><span data-stu-id="f4f49-114">Determines what connections the specific tunnel configuration applies to.</span></span> <span data-ttu-id="f4f49-115">可取值为：`wifiAndCellular`、`cellular`、`wifi`。</span><span class="sxs-lookup"><span data-stu-id="f4f49-115">Possible values are: `wifiAndCellular`, `cellular`, `wifi`.</span></span>|
|<span data-ttu-id="f4f49-116">userToggleEnabled</span><span class="sxs-lookup"><span data-stu-id="f4f49-116">userToggleEnabled</span></span>|<span data-ttu-id="f4f49-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4f49-117">Boolean</span></span>|<span data-ttu-id="f4f49-118">允许用户使用 UI 切换 VPN 配置</span><span class="sxs-lookup"><span data-stu-id="f4f49-118">Allow the user to toggle the VPN configuration using the UI</span></span>|
|<span data-ttu-id="f4f49-119">voicemailExceptionAction</span><span class="sxs-lookup"><span data-stu-id="f4f49-119">voicemailExceptionAction</span></span>|[<span data-ttu-id="f4f49-120">vpnServiceExceptionAction</span><span class="sxs-lookup"><span data-stu-id="f4f49-120">vpnServiceExceptionAction</span></span>](../resources/intune-deviceconfig-vpnserviceexceptionaction.md)|<span data-ttu-id="f4f49-121">确定是否将语音邮件服务从始终打开的 VPN 连接中排除。</span><span class="sxs-lookup"><span data-stu-id="f4f49-121">Determine whether voicemail service will be exempt from the always-on VPN connection.</span></span> <span data-ttu-id="f4f49-122">可取值为：`forceTrafficViaVPN`、`allowTrafficOutside`、`dropTraffic`。</span><span class="sxs-lookup"><span data-stu-id="f4f49-122">Possible values are: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.</span></span>|
|<span data-ttu-id="f4f49-123">airPrintExceptionAction</span><span class="sxs-lookup"><span data-stu-id="f4f49-123">airPrintExceptionAction</span></span>|[<span data-ttu-id="f4f49-124">vpnServiceExceptionAction</span><span class="sxs-lookup"><span data-stu-id="f4f49-124">vpnServiceExceptionAction</span></span>](../resources/intune-deviceconfig-vpnserviceexceptionaction.md)|<span data-ttu-id="f4f49-125">确定 AirPrint 服务是否将从 always on VPN 连接免除。</span><span class="sxs-lookup"><span data-stu-id="f4f49-125">Determine whether AirPrint service will be exempt from the always-on VPN connection.</span></span> <span data-ttu-id="f4f49-126">可取值为：`forceTrafficViaVPN`、`allowTrafficOutside`、`dropTraffic`。</span><span class="sxs-lookup"><span data-stu-id="f4f49-126">Possible values are: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.</span></span>|
|<span data-ttu-id="f4f49-127">cellularExceptionAction</span><span class="sxs-lookup"><span data-stu-id="f4f49-127">cellularExceptionAction</span></span>|[<span data-ttu-id="f4f49-128">vpnServiceExceptionAction</span><span class="sxs-lookup"><span data-stu-id="f4f49-128">vpnServiceExceptionAction</span></span>](../resources/intune-deviceconfig-vpnserviceexceptionaction.md)|<span data-ttu-id="f4f49-129">确定是否将从 "始终打开" VPN 连接中排除手机网络服务。</span><span class="sxs-lookup"><span data-stu-id="f4f49-129">Determine whether Cellular service will be exempt from the always-on VPN connection.</span></span> <span data-ttu-id="f4f49-130">可取值为：`forceTrafficViaVPN`、`allowTrafficOutside`、`dropTraffic`。</span><span class="sxs-lookup"><span data-stu-id="f4f49-130">Possible values are: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.</span></span>|
|<span data-ttu-id="f4f49-131">allowAllCaptiveNetworkPlugins</span><span class="sxs-lookup"><span data-stu-id="f4f49-131">allowAllCaptiveNetworkPlugins</span></span>|<span data-ttu-id="f4f49-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4f49-132">Boolean</span></span>|<span data-ttu-id="f4f49-133">指定是否应允许在 vpn 外部使用来自所有固定网络插件的流量</span><span class="sxs-lookup"><span data-stu-id="f4f49-133">Specifies whether traffic from all captive network plugins should be allowed outside the vpn</span></span>|
|<span data-ttu-id="f4f49-134">allowedCaptiveNetworkPlugins</span><span class="sxs-lookup"><span data-stu-id="f4f49-134">allowedCaptiveNetworkPlugins</span></span>|[<span data-ttu-id="f4f49-135">specifiedCaptiveNetworkPlugins</span><span class="sxs-lookup"><span data-stu-id="f4f49-135">specifiedCaptiveNetworkPlugins</span></span>](../resources/intune-deviceconfig-specifiedcaptivenetworkplugins.md)|<span data-ttu-id="f4f49-136">确定是否允许所有、部分或没有本地的固定网络应用</span><span class="sxs-lookup"><span data-stu-id="f4f49-136">Determines whether all, some, or no non-native captive networking apps are allowed</span></span>|
|<span data-ttu-id="f4f49-137">allowCaptiveWebSheet</span><span class="sxs-lookup"><span data-stu-id="f4f49-137">allowCaptiveWebSheet</span></span>|<span data-ttu-id="f4f49-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4f49-138">Boolean</span></span>|<span data-ttu-id="f4f49-139">确定是否允许来自 Websheet 应用的流量在 VPN 之外</span><span class="sxs-lookup"><span data-stu-id="f4f49-139">Determines whether traffic from the Websheet app is allowed outside of the VPN</span></span>|
|<span data-ttu-id="f4f49-140">natKeepAliveIntervalInSeconds</span><span class="sxs-lookup"><span data-stu-id="f4f49-140">natKeepAliveIntervalInSeconds</span></span>|<span data-ttu-id="f4f49-141">Int32</span><span class="sxs-lookup"><span data-stu-id="f4f49-141">Int32</span></span>|<span data-ttu-id="f4f49-142">指定通过 VPN 发送网络地址转换保活程序包的频率（以秒为单位）</span><span class="sxs-lookup"><span data-stu-id="f4f49-142">Specifies how often in seconds to send a network address translation keepalive package through the VPN</span></span>|
|<span data-ttu-id="f4f49-143">natKeepAliveOffloadEnable</span><span class="sxs-lookup"><span data-stu-id="f4f49-143">natKeepAliveOffloadEnable</span></span>|<span data-ttu-id="f4f49-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4f49-144">Boolean</span></span>|<span data-ttu-id="f4f49-145">设备处于睡眠状态时启用 NAT 保活信号的硬件卸载</span><span class="sxs-lookup"><span data-stu-id="f4f49-145">Enable hardware offloading of NAT keepalive signals when the device is asleep</span></span>|

## <a name="relationships"></a><span data-ttu-id="f4f49-146">关系</span><span class="sxs-lookup"><span data-stu-id="f4f49-146">Relationships</span></span>
<span data-ttu-id="f4f49-147">无</span><span class="sxs-lookup"><span data-stu-id="f4f49-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f4f49-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f4f49-148">JSON Representation</span></span>
<span data-ttu-id="f4f49-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f4f49-149">Here is a JSON representation of the resource.</span></span>
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






