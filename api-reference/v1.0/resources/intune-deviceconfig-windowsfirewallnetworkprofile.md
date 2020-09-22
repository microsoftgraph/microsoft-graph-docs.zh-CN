---
title: windowsFirewallNetworkProfile 资源类型
description: Windows 防火墙配置文件策略。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f95258e83603f29990af120624ae91b6a389df74
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091535"
---
# <a name="windowsfirewallnetworkprofile-resource-type"></a><span data-ttu-id="c8c6f-103">windowsFirewallNetworkProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="c8c6f-103">windowsFirewallNetworkProfile resource type</span></span>

<span data-ttu-id="c8c6f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8c6f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c8c6f-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c8c6f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8c6f-106">Windows 防火墙配置文件策略。</span><span class="sxs-lookup"><span data-stu-id="c8c6f-106">Windows Firewall Profile Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="c8c6f-107">属性</span><span class="sxs-lookup"><span data-stu-id="c8c6f-107">Properties</span></span>
|<span data-ttu-id="c8c6f-108">属性</span><span class="sxs-lookup"><span data-stu-id="c8c6f-108">Property</span></span>|<span data-ttu-id="c8c6f-109">类型</span><span class="sxs-lookup"><span data-stu-id="c8c6f-109">Type</span></span>|<span data-ttu-id="c8c6f-110">说明</span><span class="sxs-lookup"><span data-stu-id="c8c6f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8c6f-111">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="c8c6f-111">firewallEnabled</span></span>|[<span data-ttu-id="c8c6f-112">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="c8c6f-112">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="c8c6f-113">将主机设备配置为允许或阻止网络配置文件的防火墙和高级安全强制实施。</span><span class="sxs-lookup"><span data-stu-id="c8c6f-113">Configures the host device to allow or block the firewall and advanced security enforcement for the network profile.</span></span> <span data-ttu-id="c8c6f-114">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="c8c6f-114">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="c8c6f-115">stealthModeBlocked</span><span class="sxs-lookup"><span data-stu-id="c8c6f-115">stealthModeBlocked</span></span>|<span data-ttu-id="c8c6f-116">布尔值</span><span class="sxs-lookup"><span data-stu-id="c8c6f-116">Boolean</span></span>|<span data-ttu-id="c8c6f-117">阻止服务器在隐藏模式下运行。</span><span class="sxs-lookup"><span data-stu-id="c8c6f-117">Prevent the server from operating in stealth mode.</span></span> <span data-ttu-id="c8c6f-118">当 StealthModeRequired 和 StealthModeBlocked 均为 true 时，StealthModeBlocked 优先。</span><span class="sxs-lookup"><span data-stu-id="c8c6f-118">When StealthModeRequired and StealthModeBlocked are both true, StealthModeBlocked takes priority.</span></span>|
|<span data-ttu-id="c8c6f-119">incomingTrafficBlocked</span><span class="sxs-lookup"><span data-stu-id="c8c6f-119">incomingTrafficBlocked</span></span>|<span data-ttu-id="c8c6f-120">布尔值</span><span class="sxs-lookup"><span data-stu-id="c8c6f-120">Boolean</span></span>|<span data-ttu-id="c8c6f-121">将防火墙配置为阻止所有传入通信，而不考虑其他策略设置。</span><span class="sxs-lookup"><span data-stu-id="c8c6f-121">Configures the firewall to block all incoming traffic regardless of other policy settings.</span></span> <span data-ttu-id="c8c6f-122">当 IncomingTrafficRequired 和 IncomingTrafficBlocked 均为 true 时，IncomingTrafficBlocked 优先。</span><span class="sxs-lookup"><span data-stu-id="c8c6f-122">When IncomingTrafficRequired and IncomingTrafficBlocked are both true, IncomingTrafficBlocked takes priority.</span></span>|
|<span data-ttu-id="c8c6f-123">unicastResponsesToMulticastBroadcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="c8c6f-123">unicastResponsesToMulticastBroadcastsBlocked</span></span>|<span data-ttu-id="c8c6f-124">布尔值</span><span class="sxs-lookup"><span data-stu-id="c8c6f-124">Boolean</span></span>|<span data-ttu-id="c8c6f-125">配置防火墙以阻止对多播广播流量的单播响应。</span><span class="sxs-lookup"><span data-stu-id="c8c6f-125">Configures the firewall to block unicast responses to multicast broadcast traffic.</span></span> <span data-ttu-id="c8c6f-126">当 UnicastResponsesToMulticastBroadcastsRequired 和 UnicastResponsesToMulticastBroadcastsBlocked 均为 true 时，UnicastResponsesToMulticastBroadcastsBlocked 优先。</span><span class="sxs-lookup"><span data-stu-id="c8c6f-126">When UnicastResponsesToMulticastBroadcastsRequired and UnicastResponsesToMulticastBroadcastsBlocked are both true, UnicastResponsesToMulticastBroadcastsBlocked takes priority.</span></span>|
|<span data-ttu-id="c8c6f-127">inboundNotificationsBlocked</span><span class="sxs-lookup"><span data-stu-id="c8c6f-127">inboundNotificationsBlocked</span></span>|<span data-ttu-id="c8c6f-128">布尔值</span><span class="sxs-lookup"><span data-stu-id="c8c6f-128">Boolean</span></span>|<span data-ttu-id="c8c6f-129">阻止阻止在某个应用程序侦听某个端口时显示通知的防火墙。</span><span class="sxs-lookup"><span data-stu-id="c8c6f-129">Prevents the firewall from displaying notifications when an application is blocked from listening on a port.</span></span> <span data-ttu-id="c8c6f-130">当 InboundNotificationsRequired 和 InboundNotificationsBlocked 均为 true 时，InboundNotificationsBlocked 优先。</span><span class="sxs-lookup"><span data-stu-id="c8c6f-130">When InboundNotificationsRequired and InboundNotificationsBlocked are both true, InboundNotificationsBlocked takes priority.</span></span>|
|<span data-ttu-id="c8c6f-131">authorizedApplicationRulesFromGroupPolicyMerged</span><span class="sxs-lookup"><span data-stu-id="c8c6f-131">authorizedApplicationRulesFromGroupPolicyMerged</span></span>|<span data-ttu-id="c8c6f-132">布尔值</span><span class="sxs-lookup"><span data-stu-id="c8c6f-132">Boolean</span></span>|<span data-ttu-id="c8c6f-133">将防火墙配置为将组策略中的已授权应用程序规则与本地存储合并，而不是忽略本地存储规则。</span><span class="sxs-lookup"><span data-stu-id="c8c6f-133">Configures the firewall to merge authorized application rules from group policy with those from local store instead of ignoring the local store rules.</span></span> <span data-ttu-id="c8c6f-134">当 AuthorizedApplicationRulesFromGroupPolicyNotMerged 和 AuthorizedApplicationRulesFromGroupPolicyMerged 均为 true 时，AuthorizedApplicationRulesFromGroupPolicyMerged 优先。</span><span class="sxs-lookup"><span data-stu-id="c8c6f-134">When AuthorizedApplicationRulesFromGroupPolicyNotMerged and AuthorizedApplicationRulesFromGroupPolicyMerged are both true, AuthorizedApplicationRulesFromGroupPolicyMerged takes priority.</span></span>|
|<span data-ttu-id="c8c6f-135">globalPortRulesFromGroupPolicyMerged</span><span class="sxs-lookup"><span data-stu-id="c8c6f-135">globalPortRulesFromGroupPolicyMerged</span></span>|<span data-ttu-id="c8c6f-136">布尔值</span><span class="sxs-lookup"><span data-stu-id="c8c6f-136">Boolean</span></span>|<span data-ttu-id="c8c6f-137">将防火墙配置为将组策略中的全局端口规则与本地存储合并，而不是忽略本地存储规则。</span><span class="sxs-lookup"><span data-stu-id="c8c6f-137">Configures the firewall to merge global port rules from group policy with those from local store instead of ignoring the local store rules.</span></span> <span data-ttu-id="c8c6f-138">当 GlobalPortRulesFromGroupPolicyNotMerged 和 GlobalPortRulesFromGroupPolicyMerged 均为 true 时，GlobalPortRulesFromGroupPolicyMerged 优先。</span><span class="sxs-lookup"><span data-stu-id="c8c6f-138">When GlobalPortRulesFromGroupPolicyNotMerged and GlobalPortRulesFromGroupPolicyMerged are both true, GlobalPortRulesFromGroupPolicyMerged takes priority.</span></span>|
|<span data-ttu-id="c8c6f-139">connectionSecurityRulesFromGroupPolicyMerged</span><span class="sxs-lookup"><span data-stu-id="c8c6f-139">connectionSecurityRulesFromGroupPolicyMerged</span></span>|<span data-ttu-id="c8c6f-140">布尔值</span><span class="sxs-lookup"><span data-stu-id="c8c6f-140">Boolean</span></span>|<span data-ttu-id="c8c6f-141">将防火墙配置为将组策略中的连接安全规则与本地存储中的连接进行合并，而不是忽略本地存储规则。</span><span class="sxs-lookup"><span data-stu-id="c8c6f-141">Configures the firewall to merge connection security rules from group policy with those from local store instead of ignoring the local store rules.</span></span> <span data-ttu-id="c8c6f-142">当 ConnectionSecurityRulesFromGroupPolicyNotMerged 和 ConnectionSecurityRulesFromGroupPolicyMerged 均为 true 时，ConnectionSecurityRulesFromGroupPolicyMerged 优先。</span><span class="sxs-lookup"><span data-stu-id="c8c6f-142">When ConnectionSecurityRulesFromGroupPolicyNotMerged and ConnectionSecurityRulesFromGroupPolicyMerged are both true, ConnectionSecurityRulesFromGroupPolicyMerged takes priority.</span></span>|
|<span data-ttu-id="c8c6f-143">outboundConnectionsBlocked</span><span class="sxs-lookup"><span data-stu-id="c8c6f-143">outboundConnectionsBlocked</span></span>|<span data-ttu-id="c8c6f-144">布尔值</span><span class="sxs-lookup"><span data-stu-id="c8c6f-144">Boolean</span></span>|<span data-ttu-id="c8c6f-145">默认情况下，将防火墙配置为阻止所有传出连接。</span><span class="sxs-lookup"><span data-stu-id="c8c6f-145">Configures the firewall to block all outgoing connections by default.</span></span> <span data-ttu-id="c8c6f-146">当 OutboundConnectionsRequired 和 OutboundConnectionsBlocked 均为 true 时，OutboundConnectionsBlocked 优先。</span><span class="sxs-lookup"><span data-stu-id="c8c6f-146">When OutboundConnectionsRequired and OutboundConnectionsBlocked are both true, OutboundConnectionsBlocked takes priority.</span></span> <span data-ttu-id="c8c6f-147">此设置将应用于 Windows 版本1809及更高版本。</span><span class="sxs-lookup"><span data-stu-id="c8c6f-147">This setting will get applied to Windows releases version 1809 and above.</span></span>|
|<span data-ttu-id="c8c6f-148">inboundConnectionsBlocked</span><span class="sxs-lookup"><span data-stu-id="c8c6f-148">inboundConnectionsBlocked</span></span>|<span data-ttu-id="c8c6f-149">布尔值</span><span class="sxs-lookup"><span data-stu-id="c8c6f-149">Boolean</span></span>|<span data-ttu-id="c8c6f-150">默认情况下，将防火墙配置为阻止所有传入连接。</span><span class="sxs-lookup"><span data-stu-id="c8c6f-150">Configures the firewall to block all incoming connections by default.</span></span> <span data-ttu-id="c8c6f-151">当 InboundConnectionsRequired 和 InboundConnectionsBlocked 均为 true 时，InboundConnectionsBlocked 优先。</span><span class="sxs-lookup"><span data-stu-id="c8c6f-151">When InboundConnectionsRequired and InboundConnectionsBlocked are both true, InboundConnectionsBlocked takes priority.</span></span>|
|<span data-ttu-id="c8c6f-152">securedPacketExemptionAllowed</span><span class="sxs-lookup"><span data-stu-id="c8c6f-152">securedPacketExemptionAllowed</span></span>|<span data-ttu-id="c8c6f-153">布尔值</span><span class="sxs-lookup"><span data-stu-id="c8c6f-153">Boolean</span></span>|<span data-ttu-id="c8c6f-154">将防火墙配置为允许主机计算机对该流量的未经请求的网络流量进行响应，即使 stealthModeBlocked 设置为 true，该流量仍受 IPSec 保护。</span><span class="sxs-lookup"><span data-stu-id="c8c6f-154">Configures the firewall to allow the host computer to respond to unsolicited network traffic of that traffic is secured by IPSec even when stealthModeBlocked is set to true.</span></span> <span data-ttu-id="c8c6f-155">当 SecuredPacketExemptionBlocked 和 SecuredPacketExemptionAllowed 均为 true 时，SecuredPacketExemptionAllowed 优先。</span><span class="sxs-lookup"><span data-stu-id="c8c6f-155">When SecuredPacketExemptionBlocked and SecuredPacketExemptionAllowed are both true, SecuredPacketExemptionAllowed takes priority.</span></span>|
|<span data-ttu-id="c8c6f-156">policyRulesFromGroupPolicyMerged</span><span class="sxs-lookup"><span data-stu-id="c8c6f-156">policyRulesFromGroupPolicyMerged</span></span>|<span data-ttu-id="c8c6f-157">布尔值</span><span class="sxs-lookup"><span data-stu-id="c8c6f-157">Boolean</span></span>|<span data-ttu-id="c8c6f-158">将防火墙配置为将组策略中的防火墙规则策略与本地存储中的防火墙规则策略相合并，而不是忽略本地存储规则。</span><span class="sxs-lookup"><span data-stu-id="c8c6f-158">Configures the firewall to merge Firewall Rule policies from group policy with those from local store instead of ignoring the local store rules.</span></span> <span data-ttu-id="c8c6f-159">当 PolicyRulesFromGroupPolicyNotMerged 和 PolicyRulesFromGroupPolicyMerged 均为 true 时，PolicyRulesFromGroupPolicyMerged 优先。</span><span class="sxs-lookup"><span data-stu-id="c8c6f-159">When PolicyRulesFromGroupPolicyNotMerged and PolicyRulesFromGroupPolicyMerged are both true, PolicyRulesFromGroupPolicyMerged takes priority.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c8c6f-160">关系</span><span class="sxs-lookup"><span data-stu-id="c8c6f-160">Relationships</span></span>
<span data-ttu-id="c8c6f-161">无</span><span class="sxs-lookup"><span data-stu-id="c8c6f-161">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c8c6f-162">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c8c6f-162">JSON Representation</span></span>
<span data-ttu-id="c8c6f-163">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c8c6f-163">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsFirewallNetworkProfile",
  "firewallEnabled": "String",
  "stealthModeBlocked": true,
  "incomingTrafficBlocked": true,
  "unicastResponsesToMulticastBroadcastsBlocked": true,
  "inboundNotificationsBlocked": true,
  "authorizedApplicationRulesFromGroupPolicyMerged": true,
  "globalPortRulesFromGroupPolicyMerged": true,
  "connectionSecurityRulesFromGroupPolicyMerged": true,
  "outboundConnectionsBlocked": true,
  "inboundConnectionsBlocked": true,
  "securedPacketExemptionAllowed": true,
  "policyRulesFromGroupPolicyMerged": true
}
```









