---
title: windowsFirewallRule 资源类型
description: 通过 Windows 防火墙控制流量的规则。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dbf322718bd3b95e27583350bf840cc05f2e6ca0
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944059"
---
# <a name="windowsfirewallrule-resource-type"></a><span data-ttu-id="b1bd0-103">windowsFirewallRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="b1bd0-103">windowsFirewallRule resource type</span></span>

> <span data-ttu-id="b1bd0-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b1bd0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1bd0-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b1bd0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1bd0-106">通过 Windows 防火墙控制流量的规则。</span><span class="sxs-lookup"><span data-stu-id="b1bd0-106">A rule controlling traffic through the Windows Firewall.</span></span>

## <a name="properties"></a><span data-ttu-id="b1bd0-107">属性</span><span class="sxs-lookup"><span data-stu-id="b1bd0-107">Properties</span></span>
|<span data-ttu-id="b1bd0-108">属性</span><span class="sxs-lookup"><span data-stu-id="b1bd0-108">Property</span></span>|<span data-ttu-id="b1bd0-109">类型</span><span class="sxs-lookup"><span data-stu-id="b1bd0-109">Type</span></span>|<span data-ttu-id="b1bd0-110">说明</span><span class="sxs-lookup"><span data-stu-id="b1bd0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1bd0-111">displayName</span><span class="sxs-lookup"><span data-stu-id="b1bd0-111">displayName</span></span>|<span data-ttu-id="b1bd0-112">String</span><span class="sxs-lookup"><span data-stu-id="b1bd0-112">String</span></span>|<span data-ttu-id="b1bd0-113">规则的显示名称。</span><span class="sxs-lookup"><span data-stu-id="b1bd0-113">The display name of the rule.</span></span> <span data-ttu-id="b1bd0-114">不需要是唯一的。</span><span class="sxs-lookup"><span data-stu-id="b1bd0-114">Does not need to be unique.</span></span>|
|<span data-ttu-id="b1bd0-115">说明</span><span class="sxs-lookup"><span data-stu-id="b1bd0-115">description</span></span>|<span data-ttu-id="b1bd0-116">String</span><span class="sxs-lookup"><span data-stu-id="b1bd0-116">String</span></span>|<span data-ttu-id="b1bd0-117">规则的说明。</span><span class="sxs-lookup"><span data-stu-id="b1bd0-117">The description of the rule.</span></span>|
|<span data-ttu-id="b1bd0-118">packageFamilyName</span><span class="sxs-lookup"><span data-stu-id="b1bd0-118">packageFamilyName</span></span>|<span data-ttu-id="b1bd0-119">String</span><span class="sxs-lookup"><span data-stu-id="b1bd0-119">String</span></span>|<span data-ttu-id="b1bd0-120">受防火墙规则影响的 Microsoft Store 应用程序的程序包系列名称。</span><span class="sxs-lookup"><span data-stu-id="b1bd0-120">The package family name of a Microsoft Store application that's affected by the firewall rule.</span></span>|
|<span data-ttu-id="b1bd0-121">路径</span><span class="sxs-lookup"><span data-stu-id="b1bd0-121">filePath</span></span>|<span data-ttu-id="b1bd0-122">String</span><span class="sxs-lookup"><span data-stu-id="b1bd0-122">String</span></span>|<span data-ttu-id="b1bd0-123">受防火墙规则影响的应用程序的完整文件路径。</span><span class="sxs-lookup"><span data-stu-id="b1bd0-123">The full file path of an app that's affected by the firewall rule.</span></span>|
|<span data-ttu-id="b1bd0-124">serviceName</span><span class="sxs-lookup"><span data-stu-id="b1bd0-124">serviceName</span></span>|<span data-ttu-id="b1bd0-125">String</span><span class="sxs-lookup"><span data-stu-id="b1bd0-125">String</span></span>|<span data-ttu-id="b1bd0-126">当服务 (而不是应用程序) 发送或接收通信时使用的名称。</span><span class="sxs-lookup"><span data-stu-id="b1bd0-126">The name used in cases when a service, not an application, is sending or receiving traffic.</span></span>|
|<span data-ttu-id="b1bd0-127">协议</span><span class="sxs-lookup"><span data-stu-id="b1bd0-127">protocol</span></span>|<span data-ttu-id="b1bd0-128">Int32</span><span class="sxs-lookup"><span data-stu-id="b1bd0-128">Int32</span></span>|<span data-ttu-id="b1bd0-129">0-255 表示 IP 协议 (TCP = 6, UDP = 17) 的数字。</span><span class="sxs-lookup"><span data-stu-id="b1bd0-129">0-255 number representing the IP protocol (TCP = 6, UDP = 17).</span></span> <span data-ttu-id="b1bd0-130">如果未指定, 则默认值为 All。</span><span class="sxs-lookup"><span data-stu-id="b1bd0-130">If not specified, the default is All.</span></span> <span data-ttu-id="b1bd0-131">有效值为0至255</span><span class="sxs-lookup"><span data-stu-id="b1bd0-131">Valid values 0 to 255</span></span>|
|<span data-ttu-id="b1bd0-132">localPortRanges</span><span class="sxs-lookup"><span data-stu-id="b1bd0-132">localPortRanges</span></span>|<span data-ttu-id="b1bd0-133">String collection</span><span class="sxs-lookup"><span data-stu-id="b1bd0-133">String collection</span></span>|<span data-ttu-id="b1bd0-134">本地端口范围的列表。</span><span class="sxs-lookup"><span data-stu-id="b1bd0-134">List of local port ranges.</span></span> <span data-ttu-id="b1bd0-135">例如, "100-120", "200", "300-320"。</span><span class="sxs-lookup"><span data-stu-id="b1bd0-135">For example, "100-120", "200", "300-320".</span></span> <span data-ttu-id="b1bd0-136">如果未指定, 则默认值为 All。</span><span class="sxs-lookup"><span data-stu-id="b1bd0-136">If not specified, the default is All.</span></span>|
|<span data-ttu-id="b1bd0-137">remotePortRanges</span><span class="sxs-lookup"><span data-stu-id="b1bd0-137">remotePortRanges</span></span>|<span data-ttu-id="b1bd0-138">String collection</span><span class="sxs-lookup"><span data-stu-id="b1bd0-138">String collection</span></span>|<span data-ttu-id="b1bd0-139">远程端口范围的列表。</span><span class="sxs-lookup"><span data-stu-id="b1bd0-139">List of remote port ranges.</span></span> <span data-ttu-id="b1bd0-140">例如, "100-120", "200", "300-320"。</span><span class="sxs-lookup"><span data-stu-id="b1bd0-140">For example, "100-120", "200", "300-320".</span></span> <span data-ttu-id="b1bd0-141">如果未指定, 则默认值为 All。</span><span class="sxs-lookup"><span data-stu-id="b1bd0-141">If not specified, the default is All.</span></span>|
|<span data-ttu-id="b1bd0-142">localAddressRanges</span><span class="sxs-lookup"><span data-stu-id="b1bd0-142">localAddressRanges</span></span>|<span data-ttu-id="b1bd0-143">String collection</span><span class="sxs-lookup"><span data-stu-id="b1bd0-143">String collection</span></span>|<span data-ttu-id="b1bd0-144">规则所涵盖的本地地址的列表。</span><span class="sxs-lookup"><span data-stu-id="b1bd0-144">List of local addresses covered by the rule.</span></span> <span data-ttu-id="b1bd0-145">有效令牌包括:</span><span class="sxs-lookup"><span data-stu-id="b1bd0-145">Valid tokens include:</span></span>
- <span data-ttu-id="b1bd0-146">"\*" 表示任何本地地址。</span><span class="sxs-lookup"><span data-stu-id="b1bd0-146">"\*" indicates any local address.</span></span> <span data-ttu-id="b1bd0-147">如果存在此标记, 则必须是包含的唯一标记。</span><span class="sxs-lookup"><span data-stu-id="b1bd0-147">If present, this must be the only token included.</span></span>
- <span data-ttu-id="b1bd0-148">可以使用子网掩码或网络前缀表示法指定子网。</span><span class="sxs-lookup"><span data-stu-id="b1bd0-148">A subnet can be specified using either the subnet mask or network prefix notation.</span></span> <span data-ttu-id="b1bd0-149">如果不指定子网掩码和网络前缀, 则子网掩码默认为255.255.255.255。</span><span class="sxs-lookup"><span data-stu-id="b1bd0-149">If neither a subnet mask nor a network prefix is specified, the subnet mask defaults to 255.255.255.255.</span></span>
- <span data-ttu-id="b1bd0-150">有效的 IPv6 地址。</span><span class="sxs-lookup"><span data-stu-id="b1bd0-150">A valid IPv6 address.</span></span>
- <span data-ttu-id="b1bd0-151">不包含空格的 IPv4 地址范围, 格式为 "起始地址-结束地址"。</span><span class="sxs-lookup"><span data-stu-id="b1bd0-151">An IPv4 address range in the format of "start address - end address" with no spaces included.</span></span>
- <span data-ttu-id="b1bd0-152">不包含空格的 IPv6 地址范围, 格式为 "起始地址-结束地址"。</span><span class="sxs-lookup"><span data-stu-id="b1bd0-152">An IPv6 address range in the format of "start address - end address" with no spaces included.</span></span>
<span data-ttu-id="b1bd0-153">默认值为任意地址。 || remoteAddressRanges |字符串集合 |指定规则所涵盖的远程地址的令牌列表。</span><span class="sxs-lookup"><span data-stu-id="b1bd0-153">Default is any address.| |remoteAddressRanges|String collection|List of tokens specifying the remote addresses covered by the rule.</span></span> <span data-ttu-id="b1bd0-154">标记不区分大小写。</span><span class="sxs-lookup"><span data-stu-id="b1bd0-154">Tokens are case insensitive.</span></span> <span data-ttu-id="b1bd0-155">有效令牌包括:</span><span class="sxs-lookup"><span data-stu-id="b1bd0-155">Valid tokens include:</span></span>
- <span data-ttu-id="b1bd0-156">"\*" 表示任何远程地址。</span><span class="sxs-lookup"><span data-stu-id="b1bd0-156">"\*" indicates any remote address.</span></span> <span data-ttu-id="b1bd0-157">如果存在此标记, 则必须是包含的唯一标记。</span><span class="sxs-lookup"><span data-stu-id="b1bd0-157">If present, this must be the only token included.</span></span>
- <span data-ttu-id="b1bd0-158">"Defaultgateway"</span><span class="sxs-lookup"><span data-stu-id="b1bd0-158">"Defaultgateway"</span></span>
- <span data-ttu-id="b1bd0-159">LDHCP</span><span class="sxs-lookup"><span data-stu-id="b1bd0-159">"DHCP"</span></span>
- <span data-ttu-id="b1bd0-160">DN</span><span class="sxs-lookup"><span data-stu-id="b1bd0-160">"DNS"</span></span>
- <span data-ttu-id="b1bd0-161">首选</span><span class="sxs-lookup"><span data-stu-id="b1bd0-161">"WINS"</span></span>
- <span data-ttu-id="b1bd0-162">"Intranet" (在 Windows 版本 1809 + 上受支持)</span><span class="sxs-lookup"><span data-stu-id="b1bd0-162">"Intranet" (supported on Windows versions 1809+)</span></span>
- <span data-ttu-id="b1bd0-163">"RmtIntranet" (在 Windows 版本 1809 + 上受支持)</span><span class="sxs-lookup"><span data-stu-id="b1bd0-163">"RmtIntranet" (supported on Windows versions 1809+)</span></span>
- <span data-ttu-id="b1bd0-164">"Internet" (在 Windows 版本 1809 + 上受支持)</span><span class="sxs-lookup"><span data-stu-id="b1bd0-164">"Internet" (supported on Windows versions 1809+)</span></span>
- <span data-ttu-id="b1bd0-165">"Ply2Renders" (在 Windows 版本 1809 + 上受支持)</span><span class="sxs-lookup"><span data-stu-id="b1bd0-165">"Ply2Renders" (supported on Windows versions 1809+)</span></span>
- <span data-ttu-id="b1bd0-166">"LocalSubnet" 指示本地子网上的任何本地地址。</span><span class="sxs-lookup"><span data-stu-id="b1bd0-166">"LocalSubnet" indicates any local address on the local subnet.</span></span>
- <span data-ttu-id="b1bd0-167">可以使用子网掩码或网络前缀表示法指定子网。</span><span class="sxs-lookup"><span data-stu-id="b1bd0-167">A subnet can be specified using either the subnet mask or network prefix notation.</span></span> <span data-ttu-id="b1bd0-168">如果不指定子网掩码和网络前缀, 则子网掩码默认为255.255.255.255。</span><span class="sxs-lookup"><span data-stu-id="b1bd0-168">If neither a subnet mask nor a network prefix is specified, the subnet mask defaults to 255.255.255.255.</span></span>
- <span data-ttu-id="b1bd0-169">有效的 IPv6 地址。</span><span class="sxs-lookup"><span data-stu-id="b1bd0-169">A valid IPv6 address.</span></span>
- <span data-ttu-id="b1bd0-170">不包含空格的 IPv4 地址范围, 格式为 "起始地址-结束地址"。</span><span class="sxs-lookup"><span data-stu-id="b1bd0-170">An IPv4 address range in the format of "start address - end address" with no spaces included.</span></span>
- <span data-ttu-id="b1bd0-171">不包含空格的 IPv6 地址范围, 格式为 "起始地址-结束地址"。</span><span class="sxs-lookup"><span data-stu-id="b1bd0-171">An IPv6 address range in the format of "start address - end address" with no spaces included.</span></span>
<span data-ttu-id="b1bd0-172">默认值为任意地址。 || profileTypes |[windowsFirewallRuleNetworkProfileTypes](../resources/intune-deviceconfig-windowsfirewallrulenetworkprofiletypes.md)|指定规则所属的配置文件。</span><span class="sxs-lookup"><span data-stu-id="b1bd0-172">Default is any address.| |profileTypes|[windowsFirewallRuleNetworkProfileTypes](../resources/intune-deviceconfig-windowsfirewallrulenetworkprofiletypes.md)|Specifies the profiles to which the rule belongs.</span></span> <span data-ttu-id="b1bd0-173">如果未指定, 则默认值为 All。</span><span class="sxs-lookup"><span data-stu-id="b1bd0-173">If not specified, the default is All.</span></span> <span data-ttu-id="b1bd0-174">可能的值为`notConfigured`: `domain`、 `private`、 `public`、。 || 操作 |[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|规则强制执行的操作。</span><span class="sxs-lookup"><span data-stu-id="b1bd0-174">Possible values are: `notConfigured`, `domain`, `private`, `public`.| |action|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|The action the rule enforces.</span></span> <span data-ttu-id="b1bd0-175">如果未指定, 则允许使用默认值。</span><span class="sxs-lookup"><span data-stu-id="b1bd0-175">If not specified, the default is Allowed.</span></span> <span data-ttu-id="b1bd0-176">可能的值为`notConfigured`: `blocked`、 `allowed`、。 || trafficDirection |[windowsFirewallRuleTrafficDirectionType](../resources/intune-deviceconfig-windowsfirewallruletrafficdirectiontype.md)|启用了规则的流量方向。</span><span class="sxs-lookup"><span data-stu-id="b1bd0-176">Possible values are: `notConfigured`, `blocked`, `allowed`.| |trafficDirection|[windowsFirewallRuleTrafficDirectionType](../resources/intune-deviceconfig-windowsfirewallruletrafficdirectiontype.md)|The traffic direction that the rule is enabled for.</span></span> <span data-ttu-id="b1bd0-177">如果未指定, 则默认值为 Out。可能的值为`notConfigured`: `out`、 `in`、。 || interfaceTypes |[windowsFirewallRuleInterfaceTypes](../resources/intune-deviceconfig-windowsfirewallruleinterfacetypes.md)|规则的接口类型。</span><span class="sxs-lookup"><span data-stu-id="b1bd0-177">If not specified, the default is Out. Possible values are: `notConfigured`, `out`, `in`.| |interfaceTypes|[windowsFirewallRuleInterfaceTypes](../resources/intune-deviceconfig-windowsfirewallruleinterfacetypes.md)|The interface types of the rule.</span></span> <span data-ttu-id="b1bd0-178">可能的值为`notConfigured`: `remoteAccess`、 `wireless`、 `lan`、。 || localUserAuthorizations |String |指定应用程序容器的授权本地用户的列表。</span><span class="sxs-lookup"><span data-stu-id="b1bd0-178">Possible values are: `notConfigured`, `remoteAccess`, `wireless`, `lan`.| |localUserAuthorizations|String|Specifies the list of authorized local users for the app container.</span></span> <span data-ttu-id="b1bd0-179">这是安全描述符定义语言 (SDDL) 格式的字符串。 |</span><span class="sxs-lookup"><span data-stu-id="b1bd0-179">This is a string in Security Descriptor Definition Language (SDDL) format.|</span></span>

## <a name="relationships"></a><span data-ttu-id="b1bd0-180">关系</span><span class="sxs-lookup"><span data-stu-id="b1bd0-180">Relationships</span></span>
<span data-ttu-id="b1bd0-181">无</span><span class="sxs-lookup"><span data-stu-id="b1bd0-181">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b1bd0-182">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b1bd0-182">JSON Representation</span></span>
<span data-ttu-id="b1bd0-183">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b1bd0-183">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsFirewallRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsFirewallRule",
  "displayName": "String",
  "description": "String",
  "packageFamilyName": "String",
  "filePath": "String",
  "serviceName": "String",
  "protocol": 1024,
  "localPortRanges": [
    "String"
  ],
  "remotePortRanges": [
    "String"
  ],
  "localAddressRanges": [
    "String"
  ],
  "remoteAddressRanges": [
    "String"
  ],
  "profileTypes": "String",
  "action": "String",
  "trafficDirection": "String",
  "interfaceTypes": "String",
  "localUserAuthorizations": "String"
}
```




