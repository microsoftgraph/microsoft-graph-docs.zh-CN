---
title: appleVpnConfiguration 资源类型
description: Apple VPN 配置文件。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c9f526e256a5ec8ecd4e364b4e017508a999ea17
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163299"
---
# <a name="applevpnconfiguration-resource-type"></a><span data-ttu-id="3ea02-103">appleVpnConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="3ea02-103">appleVpnConfiguration resource type</span></span>

> <span data-ttu-id="3ea02-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3ea02-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ea02-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3ea02-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ea02-106">Apple VPN 配置文件。</span><span class="sxs-lookup"><span data-stu-id="3ea02-106">Apple VPN configuration profile.</span></span>


<span data-ttu-id="3ea02-107">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3ea02-107">Inherits from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="3ea02-108">方法</span><span class="sxs-lookup"><span data-stu-id="3ea02-108">Methods</span></span>
|<span data-ttu-id="3ea02-109">方法</span><span class="sxs-lookup"><span data-stu-id="3ea02-109">Method</span></span>|<span data-ttu-id="3ea02-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="3ea02-110">Return Type</span></span>|<span data-ttu-id="3ea02-111">说明</span><span class="sxs-lookup"><span data-stu-id="3ea02-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3ea02-112">列出 appleVpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="3ea02-112">List appleVpnConfigurations</span></span>](../api/intune-deviceconfig-applevpnconfiguration-list.md)|<span data-ttu-id="3ea02-113">[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)集合</span><span class="sxs-lookup"><span data-stu-id="3ea02-113">[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) collection</span></span>|<span data-ttu-id="3ea02-114">列出[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3ea02-114">List properties and relationships of the [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="3ea02-115">获取 appleVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="3ea02-115">Get appleVpnConfiguration</span></span>](../api/intune-deviceconfig-applevpnconfiguration-get.md)|[<span data-ttu-id="3ea02-116">appleVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="3ea02-116">appleVpnConfiguration</span></span>](../resources/intune-deviceconfig-applevpnconfiguration.md)|<span data-ttu-id="3ea02-117">读取[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3ea02-117">Read properties and relationships of the [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3ea02-118">属性</span><span class="sxs-lookup"><span data-stu-id="3ea02-118">Properties</span></span>
|<span data-ttu-id="3ea02-119">属性</span><span class="sxs-lookup"><span data-stu-id="3ea02-119">Property</span></span>|<span data-ttu-id="3ea02-120">类型</span><span class="sxs-lookup"><span data-stu-id="3ea02-120">Type</span></span>|<span data-ttu-id="3ea02-121">说明</span><span class="sxs-lookup"><span data-stu-id="3ea02-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ea02-122">id</span><span class="sxs-lookup"><span data-stu-id="3ea02-122">id</span></span>|<span data-ttu-id="3ea02-123">String</span><span class="sxs-lookup"><span data-stu-id="3ea02-123">String</span></span>|<span data-ttu-id="3ea02-124">实体的键。</span><span class="sxs-lookup"><span data-stu-id="3ea02-124">Key of the entity.</span></span> <span data-ttu-id="3ea02-125">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3ea02-125">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3ea02-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3ea02-126">lastModifiedDateTime</span></span>|<span data-ttu-id="3ea02-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ea02-127">DateTimeOffset</span></span>|<span data-ttu-id="3ea02-128">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="3ea02-128">DateTime the object was last modified.</span></span> <span data-ttu-id="3ea02-129">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3ea02-129">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3ea02-130">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3ea02-130">roleScopeTagIds</span></span>|<span data-ttu-id="3ea02-131">String collection</span><span class="sxs-lookup"><span data-stu-id="3ea02-131">String collection</span></span>|<span data-ttu-id="3ea02-132">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="3ea02-132">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3ea02-133">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3ea02-133">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3ea02-134">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3ea02-134">supportsScopeTags</span></span>|<span data-ttu-id="3ea02-135">布尔</span><span class="sxs-lookup"><span data-stu-id="3ea02-135">Boolean</span></span>|<span data-ttu-id="3ea02-136">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="3ea02-136">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3ea02-137">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="3ea02-137">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3ea02-138">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="3ea02-138">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3ea02-139">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="3ea02-139">This property is read-only.</span></span> <span data-ttu-id="3ea02-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3ea02-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3ea02-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3ea02-141">createdDateTime</span></span>|<span data-ttu-id="3ea02-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ea02-142">DateTimeOffset</span></span>|<span data-ttu-id="3ea02-143">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="3ea02-143">DateTime the object was created.</span></span> <span data-ttu-id="3ea02-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3ea02-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3ea02-145">description</span><span class="sxs-lookup"><span data-stu-id="3ea02-145">description</span></span>|<span data-ttu-id="3ea02-146">String</span><span class="sxs-lookup"><span data-stu-id="3ea02-146">String</span></span>|<span data-ttu-id="3ea02-147">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="3ea02-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3ea02-148">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3ea02-148">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3ea02-149">displayName</span><span class="sxs-lookup"><span data-stu-id="3ea02-149">displayName</span></span>|<span data-ttu-id="3ea02-150">String</span><span class="sxs-lookup"><span data-stu-id="3ea02-150">String</span></span>|<span data-ttu-id="3ea02-151">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="3ea02-151">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3ea02-152">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3ea02-152">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3ea02-153">version</span><span class="sxs-lookup"><span data-stu-id="3ea02-153">version</span></span>|<span data-ttu-id="3ea02-154">Int32</span><span class="sxs-lookup"><span data-stu-id="3ea02-154">Int32</span></span>|<span data-ttu-id="3ea02-155">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="3ea02-155">Version of the device configuration.</span></span> <span data-ttu-id="3ea02-156">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3ea02-156">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3ea02-157">connectionName</span><span class="sxs-lookup"><span data-stu-id="3ea02-157">connectionName</span></span>|<span data-ttu-id="3ea02-158">字符串</span><span class="sxs-lookup"><span data-stu-id="3ea02-158">String</span></span>|<span data-ttu-id="3ea02-159">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="3ea02-159">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="3ea02-160">connectionType</span><span class="sxs-lookup"><span data-stu-id="3ea02-160">connectionType</span></span>|[<span data-ttu-id="3ea02-161">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="3ea02-161">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="3ea02-162">连接类型。</span><span class="sxs-lookup"><span data-stu-id="3ea02-162">Connection type.</span></span> <span data-ttu-id="3ea02-163">可能的值为`ciscoAnyConnect`: `pulseSecure`、 `f5EdgeClient`、 `dellSonicWallMobileConnect` `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `paloAltoGlobalProtectV2`、、、、、、、、、、、。 `ciscoAnyConnectV2` `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso`</span><span class="sxs-lookup"><span data-stu-id="3ea02-163">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`.</span></span>|
|<span data-ttu-id="3ea02-164">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="3ea02-164">loginGroupOrDomain</span></span>|<span data-ttu-id="3ea02-165">字符串</span><span class="sxs-lookup"><span data-stu-id="3ea02-165">String</span></span>|<span data-ttu-id="3ea02-166">将连接类型设置为 Dell SonicWALL Mobile 连接时的登录组或域。</span><span class="sxs-lookup"><span data-stu-id="3ea02-166">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="3ea02-167">role</span><span class="sxs-lookup"><span data-stu-id="3ea02-167">role</span></span>|<span data-ttu-id="3ea02-168">字符串</span><span class="sxs-lookup"><span data-stu-id="3ea02-168">String</span></span>|<span data-ttu-id="3ea02-169">将 "连接类型" 设置为 "脉冲安全" 时的角色。</span><span class="sxs-lookup"><span data-stu-id="3ea02-169">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="3ea02-170">领域</span><span class="sxs-lookup"><span data-stu-id="3ea02-170">realm</span></span>|<span data-ttu-id="3ea02-171">字符串</span><span class="sxs-lookup"><span data-stu-id="3ea02-171">String</span></span>|<span data-ttu-id="3ea02-172">连接类型设置为脉冲安全时的领域。</span><span class="sxs-lookup"><span data-stu-id="3ea02-172">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="3ea02-173">服务器主板</span><span class="sxs-lookup"><span data-stu-id="3ea02-173">server</span></span>|[<span data-ttu-id="3ea02-174">vpnServer</span><span class="sxs-lookup"><span data-stu-id="3ea02-174">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="3ea02-175">网络上的 VPN 服务器。</span><span class="sxs-lookup"><span data-stu-id="3ea02-175">VPN Server on the network.</span></span> <span data-ttu-id="3ea02-176">请确保最终用户可以访问此网络位置。</span><span class="sxs-lookup"><span data-stu-id="3ea02-176">Make sure end users can access this network location.</span></span>|
|<span data-ttu-id="3ea02-177">标识符</span><span class="sxs-lookup"><span data-stu-id="3ea02-177">identifier</span></span>|<span data-ttu-id="3ea02-178">字符串</span><span class="sxs-lookup"><span data-stu-id="3ea02-178">String</span></span>|<span data-ttu-id="3ea02-179">当连接类型设置为自定义 vpn 时, 由 VPN 供应商提供的标识符。</span><span class="sxs-lookup"><span data-stu-id="3ea02-179">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="3ea02-180">例如: Cisco AnyConnect 使用 AnyConnect 形式的标识符。 applevpn 的标识符</span><span class="sxs-lookup"><span data-stu-id="3ea02-180">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin</span></span>|
|<span data-ttu-id="3ea02-181">customData</span><span class="sxs-lookup"><span data-stu-id="3ea02-181">customData</span></span>|<span data-ttu-id="3ea02-182">[keyValue](../resources/intune-deviceconfig-keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3ea02-182">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="3ea02-183">将连接类型设置为自定义 VPN 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="3ea02-183">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="3ea02-184">使用此字段启用 Intune 不支持的功能, 但在你的 VPN 解决方案中可用。</span><span class="sxs-lookup"><span data-stu-id="3ea02-184">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="3ea02-185">请与你的 VPN 供应商联系, 了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="3ea02-185">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="3ea02-186">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="3ea02-186">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="3ea02-187">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="3ea02-187">customKeyValueData</span></span>|<span data-ttu-id="3ea02-188">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3ea02-188">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="3ea02-189">将连接类型设置为自定义 VPN 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="3ea02-189">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="3ea02-190">使用此字段启用 Intune 不支持的功能, 但在你的 VPN 解决方案中可用。</span><span class="sxs-lookup"><span data-stu-id="3ea02-190">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="3ea02-191">请与你的 VPN 供应商联系, 了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="3ea02-191">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="3ea02-192">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="3ea02-192">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="3ea02-193">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="3ea02-193">enableSplitTunneling</span></span>|<span data-ttu-id="3ea02-194">布尔</span><span class="sxs-lookup"><span data-stu-id="3ea02-194">Boolean</span></span>|<span data-ttu-id="3ea02-195">通过 VPN 发送所有网络流量。</span><span class="sxs-lookup"><span data-stu-id="3ea02-195">Send all network traffic through VPN.</span></span>|
|<span data-ttu-id="3ea02-196">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="3ea02-196">authenticationMethod</span></span>|[<span data-ttu-id="3ea02-197">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="3ea02-197">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="3ea02-198">此 VPN 连接的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="3ea02-198">Authentication method for this VPN connection.</span></span> <span data-ttu-id="3ea02-199">可取值为：`certificate`、`usernameAndPassword`。</span><span class="sxs-lookup"><span data-stu-id="3ea02-199">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="3ea02-200">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="3ea02-200">enablePerApp</span></span>|<span data-ttu-id="3ea02-201">布尔</span><span class="sxs-lookup"><span data-stu-id="3ea02-201">Boolean</span></span>|<span data-ttu-id="3ea02-202">将此设置为 true 将创建每个应用程序 VPN 有效负载, 以后可将其与可在最终用户的 iOS 设备上触发此 VPN 连接的应用程序相关联。</span><span class="sxs-lookup"><span data-stu-id="3ea02-202">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span>|
|<span data-ttu-id="3ea02-203">safariDomains</span><span class="sxs-lookup"><span data-stu-id="3ea02-203">safariDomains</span></span>|<span data-ttu-id="3ea02-204">String collection</span><span class="sxs-lookup"><span data-stu-id="3ea02-204">String collection</span></span>|<span data-ttu-id="3ea02-205">启用此 VPN 每应用程序设置时的 Safari 域。</span><span class="sxs-lookup"><span data-stu-id="3ea02-205">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="3ea02-206">除了与此 vpn 关联的应用程序之外, 此处指定的 Safari 域还将能够触发此 vpn 连接。</span><span class="sxs-lookup"><span data-stu-id="3ea02-206">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span>|
|<span data-ttu-id="3ea02-207">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="3ea02-207">onDemandRules</span></span>|<span data-ttu-id="3ea02-208">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="3ea02-208">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="3ea02-209">按需规则。</span><span class="sxs-lookup"><span data-stu-id="3ea02-209">On-Demand Rules.</span></span> <span data-ttu-id="3ea02-210">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="3ea02-210">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="3ea02-211">proxyServer</span><span class="sxs-lookup"><span data-stu-id="3ea02-211">proxyServer</span></span>|[<span data-ttu-id="3ea02-212">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="3ea02-212">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="3ea02-213">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="3ea02-213">Proxy Server.</span></span>|
|<span data-ttu-id="3ea02-214">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="3ea02-214">optInToDeviceIdSharing</span></span>|<span data-ttu-id="3ea02-215">布尔</span><span class="sxs-lookup"><span data-stu-id="3ea02-215">Boolean</span></span>|<span data-ttu-id="3ea02-216">选择将设备的 Id 共享到第三方 vpn 客户端, 以便在网络访问控制验证期间使用。</span><span class="sxs-lookup"><span data-stu-id="3ea02-216">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3ea02-217">关系</span><span class="sxs-lookup"><span data-stu-id="3ea02-217">Relationships</span></span>
|<span data-ttu-id="3ea02-218">关系</span><span class="sxs-lookup"><span data-stu-id="3ea02-218">Relationship</span></span>|<span data-ttu-id="3ea02-219">类型</span><span class="sxs-lookup"><span data-stu-id="3ea02-219">Type</span></span>|<span data-ttu-id="3ea02-220">说明</span><span class="sxs-lookup"><span data-stu-id="3ea02-220">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ea02-221">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="3ea02-221">groupAssignments</span></span>|<span data-ttu-id="3ea02-222">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="3ea02-222">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="3ea02-223">设备配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="3ea02-223">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="3ea02-224">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3ea02-224">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3ea02-225">assignments</span><span class="sxs-lookup"><span data-stu-id="3ea02-225">assignments</span></span>|<span data-ttu-id="3ea02-226">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3ea02-226">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="3ea02-227">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="3ea02-227">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="3ea02-228">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3ea02-228">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3ea02-229">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="3ea02-229">deviceStatuses</span></span>|<span data-ttu-id="3ea02-230">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3ea02-230">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="3ea02-231">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="3ea02-231">Device configuration installation status by device.</span></span> <span data-ttu-id="3ea02-232">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3ea02-232">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3ea02-233">userStatuses</span><span class="sxs-lookup"><span data-stu-id="3ea02-233">userStatuses</span></span>|<span data-ttu-id="3ea02-234">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3ea02-234">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="3ea02-235">按用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="3ea02-235">Device configuration installation status by user.</span></span> <span data-ttu-id="3ea02-236">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3ea02-236">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3ea02-237">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="3ea02-237">deviceStatusOverview</span></span>|[<span data-ttu-id="3ea02-238">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="3ea02-238">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="3ea02-239">设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3ea02-239">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3ea02-240">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="3ea02-240">userStatusOverview</span></span>|[<span data-ttu-id="3ea02-241">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="3ea02-241">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="3ea02-242">设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3ea02-242">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3ea02-243">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="3ea02-243">deviceSettingStateSummaries</span></span>|<span data-ttu-id="3ea02-244">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3ea02-244">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="3ea02-245">设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3ea02-245">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3ea02-246">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3ea02-246">JSON Representation</span></span>
<span data-ttu-id="3ea02-247">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3ea02-247">Here is a JSON representation of the resource.</span></span>
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




