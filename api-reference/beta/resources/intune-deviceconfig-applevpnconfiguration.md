---
title: appleVpnConfiguration 资源类型
description: Apple VPN 配置文件。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3f367badce65cfabc2523aaa0c06794188d5000b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33947699"
---
# <a name="applevpnconfiguration-resource-type"></a><span data-ttu-id="a6081-103">appleVpnConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="a6081-103">appleVpnConfiguration resource type</span></span>

> <span data-ttu-id="a6081-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a6081-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6081-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a6081-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6081-106">Apple VPN 配置文件。</span><span class="sxs-lookup"><span data-stu-id="a6081-106">Apple VPN configuration profile.</span></span>


<span data-ttu-id="a6081-107">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6081-107">Inherits from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="a6081-108">方法</span><span class="sxs-lookup"><span data-stu-id="a6081-108">Methods</span></span>
|<span data-ttu-id="a6081-109">方法</span><span class="sxs-lookup"><span data-stu-id="a6081-109">Method</span></span>|<span data-ttu-id="a6081-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="a6081-110">Return Type</span></span>|<span data-ttu-id="a6081-111">说明</span><span class="sxs-lookup"><span data-stu-id="a6081-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a6081-112">列出 appleVpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="a6081-112">List appleVpnConfigurations</span></span>](../api/intune-deviceconfig-applevpnconfiguration-list.md)|<span data-ttu-id="a6081-113">[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)集合</span><span class="sxs-lookup"><span data-stu-id="a6081-113">[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) collection</span></span>|<span data-ttu-id="a6081-114">列出[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a6081-114">List properties and relationships of the [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="a6081-115">获取 appleVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="a6081-115">Get appleVpnConfiguration</span></span>](../api/intune-deviceconfig-applevpnconfiguration-get.md)|[<span data-ttu-id="a6081-116">appleVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="a6081-116">appleVpnConfiguration</span></span>](../resources/intune-deviceconfig-applevpnconfiguration.md)|<span data-ttu-id="a6081-117">读取[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a6081-117">Read properties and relationships of the [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a6081-118">属性</span><span class="sxs-lookup"><span data-stu-id="a6081-118">Properties</span></span>
|<span data-ttu-id="a6081-119">属性</span><span class="sxs-lookup"><span data-stu-id="a6081-119">Property</span></span>|<span data-ttu-id="a6081-120">类型</span><span class="sxs-lookup"><span data-stu-id="a6081-120">Type</span></span>|<span data-ttu-id="a6081-121">说明</span><span class="sxs-lookup"><span data-stu-id="a6081-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6081-122">id</span><span class="sxs-lookup"><span data-stu-id="a6081-122">id</span></span>|<span data-ttu-id="a6081-123">字符串</span><span class="sxs-lookup"><span data-stu-id="a6081-123">String</span></span>|<span data-ttu-id="a6081-124">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a6081-124">Key of the entity.</span></span> <span data-ttu-id="a6081-125">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6081-125">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6081-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a6081-126">lastModifiedDateTime</span></span>|<span data-ttu-id="a6081-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6081-127">DateTimeOffset</span></span>|<span data-ttu-id="a6081-128">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a6081-128">DateTime the object was last modified.</span></span> <span data-ttu-id="a6081-129">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6081-129">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6081-130">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a6081-130">roleScopeTagIds</span></span>|<span data-ttu-id="a6081-131">String collection</span><span class="sxs-lookup"><span data-stu-id="a6081-131">String collection</span></span>|<span data-ttu-id="a6081-132">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="a6081-132">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a6081-133">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6081-133">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6081-134">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a6081-134">supportsScopeTags</span></span>|<span data-ttu-id="a6081-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="a6081-135">Boolean</span></span>|<span data-ttu-id="a6081-136">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="a6081-136">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a6081-137">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="a6081-137">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a6081-138">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="a6081-138">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a6081-139">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="a6081-139">This property is read-only.</span></span> <span data-ttu-id="a6081-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6081-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6081-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a6081-141">createdDateTime</span></span>|<span data-ttu-id="a6081-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6081-142">DateTimeOffset</span></span>|<span data-ttu-id="a6081-143">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a6081-143">DateTime the object was created.</span></span> <span data-ttu-id="a6081-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6081-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6081-145">说明</span><span class="sxs-lookup"><span data-stu-id="a6081-145">description</span></span>|<span data-ttu-id="a6081-146">String</span><span class="sxs-lookup"><span data-stu-id="a6081-146">String</span></span>|<span data-ttu-id="a6081-147">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="a6081-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a6081-148">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6081-148">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6081-149">displayName</span><span class="sxs-lookup"><span data-stu-id="a6081-149">displayName</span></span>|<span data-ttu-id="a6081-150">String</span><span class="sxs-lookup"><span data-stu-id="a6081-150">String</span></span>|<span data-ttu-id="a6081-151">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="a6081-151">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a6081-152">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6081-152">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6081-153">version</span><span class="sxs-lookup"><span data-stu-id="a6081-153">version</span></span>|<span data-ttu-id="a6081-154">Int32</span><span class="sxs-lookup"><span data-stu-id="a6081-154">Int32</span></span>|<span data-ttu-id="a6081-155">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="a6081-155">Version of the device configuration.</span></span> <span data-ttu-id="a6081-156">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6081-156">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6081-157">connectionName</span><span class="sxs-lookup"><span data-stu-id="a6081-157">connectionName</span></span>|<span data-ttu-id="a6081-158">String</span><span class="sxs-lookup"><span data-stu-id="a6081-158">String</span></span>|<span data-ttu-id="a6081-159">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="a6081-159">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="a6081-160">connectionType</span><span class="sxs-lookup"><span data-stu-id="a6081-160">connectionType</span></span>|[<span data-ttu-id="a6081-161">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="a6081-161">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="a6081-162">连接类型。</span><span class="sxs-lookup"><span data-stu-id="a6081-162">Connection type.</span></span> <span data-ttu-id="a6081-163">可能的值为`ciscoAnyConnect`: `pulseSecure`、 `f5EdgeClient`、 `dellSonicWallMobileConnect` `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `paloAltoGlobalProtectV2`、、、、、、、、、、、。 `ciscoAnyConnectV2` `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso`</span><span class="sxs-lookup"><span data-stu-id="a6081-163">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`.</span></span>|
|<span data-ttu-id="a6081-164">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="a6081-164">loginGroupOrDomain</span></span>|<span data-ttu-id="a6081-165">String</span><span class="sxs-lookup"><span data-stu-id="a6081-165">String</span></span>|<span data-ttu-id="a6081-166">将连接类型设置为 Dell SonicWALL Mobile 连接时的登录组或域。</span><span class="sxs-lookup"><span data-stu-id="a6081-166">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="a6081-167">role</span><span class="sxs-lookup"><span data-stu-id="a6081-167">role</span></span>|<span data-ttu-id="a6081-168">String</span><span class="sxs-lookup"><span data-stu-id="a6081-168">String</span></span>|<span data-ttu-id="a6081-169">将 "连接类型" 设置为 "脉冲安全" 时的角色。</span><span class="sxs-lookup"><span data-stu-id="a6081-169">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="a6081-170">型</span><span class="sxs-lookup"><span data-stu-id="a6081-170">realm</span></span>|<span data-ttu-id="a6081-171">String</span><span class="sxs-lookup"><span data-stu-id="a6081-171">String</span></span>|<span data-ttu-id="a6081-172">连接类型设置为脉冲安全时的领域。</span><span class="sxs-lookup"><span data-stu-id="a6081-172">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="a6081-173">服务器主板</span><span class="sxs-lookup"><span data-stu-id="a6081-173">server</span></span>|[<span data-ttu-id="a6081-174">vpnServer</span><span class="sxs-lookup"><span data-stu-id="a6081-174">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="a6081-175">网络上的 VPN 服务器。</span><span class="sxs-lookup"><span data-stu-id="a6081-175">VPN Server on the network.</span></span> <span data-ttu-id="a6081-176">请确保最终用户可以访问此网络位置。</span><span class="sxs-lookup"><span data-stu-id="a6081-176">Make sure end users can access this network location.</span></span>|
|<span data-ttu-id="a6081-177">标识符</span><span class="sxs-lookup"><span data-stu-id="a6081-177">identifier</span></span>|<span data-ttu-id="a6081-178">String</span><span class="sxs-lookup"><span data-stu-id="a6081-178">String</span></span>|<span data-ttu-id="a6081-179">当连接类型设置为自定义 VPN 时, 由 VPN 供应商提供的标识符。</span><span class="sxs-lookup"><span data-stu-id="a6081-179">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="a6081-180">例如: Cisco AnyConnect 使用 AnyConnect 形式的标识符。 applevpn 的标识符</span><span class="sxs-lookup"><span data-stu-id="a6081-180">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin</span></span>|
|<span data-ttu-id="a6081-181">customData</span><span class="sxs-lookup"><span data-stu-id="a6081-181">customData</span></span>|<span data-ttu-id="a6081-182">[keyValue](../resources/intune-deviceconfig-keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a6081-182">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="a6081-183">将连接类型设置为自定义 VPN 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="a6081-183">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="a6081-184">使用此字段启用 Intune 不支持的功能, 但在你的 VPN 解决方案中可用。</span><span class="sxs-lookup"><span data-stu-id="a6081-184">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="a6081-185">请与你的 VPN 供应商联系, 了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="a6081-185">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="a6081-186">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="a6081-186">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="a6081-187">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="a6081-187">customKeyValueData</span></span>|<span data-ttu-id="a6081-188">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a6081-188">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="a6081-189">将连接类型设置为自定义 VPN 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="a6081-189">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="a6081-190">使用此字段启用 Intune 不支持的功能, 但在你的 VPN 解决方案中可用。</span><span class="sxs-lookup"><span data-stu-id="a6081-190">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="a6081-191">请与你的 VPN 供应商联系, 了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="a6081-191">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="a6081-192">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="a6081-192">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="a6081-193">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="a6081-193">enableSplitTunneling</span></span>|<span data-ttu-id="a6081-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="a6081-194">Boolean</span></span>|<span data-ttu-id="a6081-195">通过 VPN 发送所有网络流量。</span><span class="sxs-lookup"><span data-stu-id="a6081-195">Send all network traffic through VPN.</span></span>|
|<span data-ttu-id="a6081-196">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a6081-196">authenticationMethod</span></span>|[<span data-ttu-id="a6081-197">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a6081-197">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="a6081-198">此 VPN 连接的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="a6081-198">Authentication method for this VPN connection.</span></span> <span data-ttu-id="a6081-199">可取值为：`certificate`、`usernameAndPassword`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="a6081-199">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="a6081-200">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="a6081-200">enablePerApp</span></span>|<span data-ttu-id="a6081-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="a6081-201">Boolean</span></span>|<span data-ttu-id="a6081-202">将此设置为 true 将创建每个应用程序 VPN 有效负载, 以后可将其与可在最终用户的 iOS 设备上触发此 VPN 连接的应用程序相关联。</span><span class="sxs-lookup"><span data-stu-id="a6081-202">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span>|
|<span data-ttu-id="a6081-203">safariDomains</span><span class="sxs-lookup"><span data-stu-id="a6081-203">safariDomains</span></span>|<span data-ttu-id="a6081-204">String collection</span><span class="sxs-lookup"><span data-stu-id="a6081-204">String collection</span></span>|<span data-ttu-id="a6081-205">启用此 VPN 每应用程序设置时的 Safari 域。</span><span class="sxs-lookup"><span data-stu-id="a6081-205">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="a6081-206">除了与此 VPN 关联的应用程序之外, 此处指定的 Safari 域还将能够触发此 VPN 连接。</span><span class="sxs-lookup"><span data-stu-id="a6081-206">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span>|
|<span data-ttu-id="a6081-207">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="a6081-207">onDemandRules</span></span>|<span data-ttu-id="a6081-208">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="a6081-208">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="a6081-209">按需规则。</span><span class="sxs-lookup"><span data-stu-id="a6081-209">On-Demand Rules.</span></span> <span data-ttu-id="a6081-210">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="a6081-210">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="a6081-211">proxyServer</span><span class="sxs-lookup"><span data-stu-id="a6081-211">proxyServer</span></span>|[<span data-ttu-id="a6081-212">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="a6081-212">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="a6081-213">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="a6081-213">Proxy Server.</span></span>|
|<span data-ttu-id="a6081-214">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="a6081-214">optInToDeviceIdSharing</span></span>|<span data-ttu-id="a6081-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="a6081-215">Boolean</span></span>|<span data-ttu-id="a6081-216">选择将设备的 Id 共享到第三方 vpn 客户端, 以便在网络访问控制验证期间使用。</span><span class="sxs-lookup"><span data-stu-id="a6081-216">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a6081-217">关系</span><span class="sxs-lookup"><span data-stu-id="a6081-217">Relationships</span></span>
|<span data-ttu-id="a6081-218">关系</span><span class="sxs-lookup"><span data-stu-id="a6081-218">Relationship</span></span>|<span data-ttu-id="a6081-219">类型</span><span class="sxs-lookup"><span data-stu-id="a6081-219">Type</span></span>|<span data-ttu-id="a6081-220">说明</span><span class="sxs-lookup"><span data-stu-id="a6081-220">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6081-221">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="a6081-221">groupAssignments</span></span>|<span data-ttu-id="a6081-222">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="a6081-222">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="a6081-223">设备配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="a6081-223">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="a6081-224">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6081-224">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6081-225">assignments</span><span class="sxs-lookup"><span data-stu-id="a6081-225">assignments</span></span>|<span data-ttu-id="a6081-226">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a6081-226">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="a6081-227">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="a6081-227">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="a6081-228">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6081-228">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6081-229">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="a6081-229">deviceStatuses</span></span>|<span data-ttu-id="a6081-230">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a6081-230">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="a6081-231">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="a6081-231">Device configuration installation status by device.</span></span> <span data-ttu-id="a6081-232">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6081-232">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6081-233">userStatuses</span><span class="sxs-lookup"><span data-stu-id="a6081-233">userStatuses</span></span>|<span data-ttu-id="a6081-234">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a6081-234">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="a6081-235">按用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="a6081-235">Device configuration installation status by user.</span></span> <span data-ttu-id="a6081-236">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6081-236">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6081-237">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="a6081-237">deviceStatusOverview</span></span>|[<span data-ttu-id="a6081-238">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="a6081-238">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="a6081-239">设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6081-239">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6081-240">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="a6081-240">userStatusOverview</span></span>|[<span data-ttu-id="a6081-241">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="a6081-241">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="a6081-242">设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6081-242">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6081-243">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="a6081-243">deviceSettingStateSummaries</span></span>|<span data-ttu-id="a6081-244">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a6081-244">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="a6081-245">设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6081-245">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a6081-246">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a6081-246">JSON Representation</span></span>
<span data-ttu-id="a6081-247">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a6081-247">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.appleVpnConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appleVpnConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "connectionName": "String",
  "connectionType": "String",
  "loginGroupOrDomain": "String",
  "role": "String",
  "realm": "String",
  "server": {
    "@odata.type": "microsoft.graph.vpnServer",
    "description": "String",
    "address": "String",
    "isDefaultServer": true
  },
  "identifier": "String",
  "customData": [
    {
      "@odata.type": "microsoft.graph.keyValue",
      "key": "String",
      "value": "String"
    }
  ],
  "customKeyValueData": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "enableSplitTunneling": true,
  "authenticationMethod": "String",
  "enablePerApp": true,
  "safariDomains": [
    "String"
  ],
  "onDemandRules": [
    {
      "@odata.type": "microsoft.graph.vpnOnDemandRule",
      "ssids": [
        "String"
      ],
      "dnsSearchDomains": [
        "String"
      ],
      "probeUrl": "String",
      "action": "String",
      "domainAction": "String",
      "domains": [
        "String"
      ],
      "probeRequiredUrl": "String"
    }
  ],
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "String",
    "address": "String",
    "port": 1024
  },
  "optInToDeviceIdSharing": true
}
```




