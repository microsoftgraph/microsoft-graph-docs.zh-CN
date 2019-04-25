---
title: appleVpnConfiguration 资源类型
description: Apple VPN 配置文件。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d63fa3f8a93551be9c3180d4f8d6c7119838efd8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562305"
---
# <a name="applevpnconfiguration-resource-type"></a><span data-ttu-id="5ed8d-103">appleVpnConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="5ed8d-103">appleVpnConfiguration resource type</span></span>

> <span data-ttu-id="5ed8d-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5ed8d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5ed8d-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5ed8d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ed8d-106">Apple VPN 配置文件。</span><span class="sxs-lookup"><span data-stu-id="5ed8d-106">Apple VPN configuration profile.</span></span>


<span data-ttu-id="5ed8d-107">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ed8d-107">Inherits from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="5ed8d-108">方法</span><span class="sxs-lookup"><span data-stu-id="5ed8d-108">Methods</span></span>
|<span data-ttu-id="5ed8d-109">方法</span><span class="sxs-lookup"><span data-stu-id="5ed8d-109">Method</span></span>|<span data-ttu-id="5ed8d-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="5ed8d-110">Return Type</span></span>|<span data-ttu-id="5ed8d-111">说明</span><span class="sxs-lookup"><span data-stu-id="5ed8d-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5ed8d-112">列出 appleVpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="5ed8d-112">List appleVpnConfigurations</span></span>](../api/intune-deviceconfig-applevpnconfiguration-list.md)|<span data-ttu-id="5ed8d-113">[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)集合</span><span class="sxs-lookup"><span data-stu-id="5ed8d-113">[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) collection</span></span>|<span data-ttu-id="5ed8d-114">列出[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5ed8d-114">List properties and relationships of the [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="5ed8d-115">获取 appleVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="5ed8d-115">Get appleVpnConfiguration</span></span>](../api/intune-deviceconfig-applevpnconfiguration-get.md)|[<span data-ttu-id="5ed8d-116">appleVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="5ed8d-116">appleVpnConfiguration</span></span>](../resources/intune-deviceconfig-applevpnconfiguration.md)|<span data-ttu-id="5ed8d-117">读取[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5ed8d-117">Read properties and relationships of the [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5ed8d-118">属性</span><span class="sxs-lookup"><span data-stu-id="5ed8d-118">Properties</span></span>
|<span data-ttu-id="5ed8d-119">属性</span><span class="sxs-lookup"><span data-stu-id="5ed8d-119">Property</span></span>|<span data-ttu-id="5ed8d-120">类型</span><span class="sxs-lookup"><span data-stu-id="5ed8d-120">Type</span></span>|<span data-ttu-id="5ed8d-121">说明</span><span class="sxs-lookup"><span data-stu-id="5ed8d-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ed8d-122">id</span><span class="sxs-lookup"><span data-stu-id="5ed8d-122">id</span></span>|<span data-ttu-id="5ed8d-123">字符串</span><span class="sxs-lookup"><span data-stu-id="5ed8d-123">String</span></span>|<span data-ttu-id="5ed8d-124">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5ed8d-124">Key of the entity.</span></span> <span data-ttu-id="5ed8d-125">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ed8d-125">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ed8d-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5ed8d-126">lastModifiedDateTime</span></span>|<span data-ttu-id="5ed8d-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ed8d-127">DateTimeOffset</span></span>|<span data-ttu-id="5ed8d-128">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="5ed8d-128">DateTime the object was last modified.</span></span> <span data-ttu-id="5ed8d-129">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ed8d-129">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ed8d-130">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5ed8d-130">roleScopeTagIds</span></span>|<span data-ttu-id="5ed8d-131">String collection</span><span class="sxs-lookup"><span data-stu-id="5ed8d-131">String collection</span></span>|<span data-ttu-id="5ed8d-132">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="5ed8d-132">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5ed8d-133">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ed8d-133">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ed8d-134">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="5ed8d-134">supportsScopeTags</span></span>|<span data-ttu-id="5ed8d-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ed8d-135">Boolean</span></span>|<span data-ttu-id="5ed8d-136">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="5ed8d-136">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5ed8d-137">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="5ed8d-137">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5ed8d-138">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="5ed8d-138">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5ed8d-139">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ed8d-139">This property is read-only.</span></span> <span data-ttu-id="5ed8d-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ed8d-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ed8d-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5ed8d-141">createdDateTime</span></span>|<span data-ttu-id="5ed8d-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ed8d-142">DateTimeOffset</span></span>|<span data-ttu-id="5ed8d-143">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="5ed8d-143">DateTime the object was created.</span></span> <span data-ttu-id="5ed8d-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ed8d-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ed8d-145">说明</span><span class="sxs-lookup"><span data-stu-id="5ed8d-145">description</span></span>|<span data-ttu-id="5ed8d-146">String</span><span class="sxs-lookup"><span data-stu-id="5ed8d-146">String</span></span>|<span data-ttu-id="5ed8d-147">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="5ed8d-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5ed8d-148">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ed8d-148">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ed8d-149">displayName</span><span class="sxs-lookup"><span data-stu-id="5ed8d-149">displayName</span></span>|<span data-ttu-id="5ed8d-150">String</span><span class="sxs-lookup"><span data-stu-id="5ed8d-150">String</span></span>|<span data-ttu-id="5ed8d-151">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="5ed8d-151">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5ed8d-152">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ed8d-152">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ed8d-153">version</span><span class="sxs-lookup"><span data-stu-id="5ed8d-153">version</span></span>|<span data-ttu-id="5ed8d-154">Int32</span><span class="sxs-lookup"><span data-stu-id="5ed8d-154">Int32</span></span>|<span data-ttu-id="5ed8d-155">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="5ed8d-155">Version of the device configuration.</span></span> <span data-ttu-id="5ed8d-156">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ed8d-156">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ed8d-157">connectionName</span><span class="sxs-lookup"><span data-stu-id="5ed8d-157">connectionName</span></span>|<span data-ttu-id="5ed8d-158">String</span><span class="sxs-lookup"><span data-stu-id="5ed8d-158">String</span></span>|<span data-ttu-id="5ed8d-159">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="5ed8d-159">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="5ed8d-160">connectionType</span><span class="sxs-lookup"><span data-stu-id="5ed8d-160">connectionType</span></span>|[<span data-ttu-id="5ed8d-161">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="5ed8d-161">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="5ed8d-162">连接类型。</span><span class="sxs-lookup"><span data-stu-id="5ed8d-162">Connection type.</span></span> <span data-ttu-id="5ed8d-163">可能的值为`ciscoAnyConnect`: `pulseSecure`、 `f5EdgeClient`、 `dellSonicWallMobileConnect` `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `paloAltoGlobalProtectV2`、、、、、、、、、、、。 `ciscoAnyConnectV2` `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso`</span><span class="sxs-lookup"><span data-stu-id="5ed8d-163">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`.</span></span>|
|<span data-ttu-id="5ed8d-164">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="5ed8d-164">loginGroupOrDomain</span></span>|<span data-ttu-id="5ed8d-165">String</span><span class="sxs-lookup"><span data-stu-id="5ed8d-165">String</span></span>|<span data-ttu-id="5ed8d-166">将连接类型设置为 Dell SonicWALL Mobile 连接时的登录组或域。</span><span class="sxs-lookup"><span data-stu-id="5ed8d-166">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="5ed8d-167">role</span><span class="sxs-lookup"><span data-stu-id="5ed8d-167">role</span></span>|<span data-ttu-id="5ed8d-168">String</span><span class="sxs-lookup"><span data-stu-id="5ed8d-168">String</span></span>|<span data-ttu-id="5ed8d-169">将 "连接类型" 设置为 "脉冲安全" 时的角色。</span><span class="sxs-lookup"><span data-stu-id="5ed8d-169">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="5ed8d-170">型</span><span class="sxs-lookup"><span data-stu-id="5ed8d-170">realm</span></span>|<span data-ttu-id="5ed8d-171">String</span><span class="sxs-lookup"><span data-stu-id="5ed8d-171">String</span></span>|<span data-ttu-id="5ed8d-172">连接类型设置为脉冲安全时的领域。</span><span class="sxs-lookup"><span data-stu-id="5ed8d-172">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="5ed8d-173">服务器主板</span><span class="sxs-lookup"><span data-stu-id="5ed8d-173">server</span></span>|[<span data-ttu-id="5ed8d-174">vpnServer</span><span class="sxs-lookup"><span data-stu-id="5ed8d-174">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="5ed8d-175">网络上的 VPN 服务器。</span><span class="sxs-lookup"><span data-stu-id="5ed8d-175">VPN Server on the network.</span></span> <span data-ttu-id="5ed8d-176">请确保最终用户可以访问此网络位置。</span><span class="sxs-lookup"><span data-stu-id="5ed8d-176">Make sure end users can access this network location.</span></span>|
|<span data-ttu-id="5ed8d-177">标识符</span><span class="sxs-lookup"><span data-stu-id="5ed8d-177">identifier</span></span>|<span data-ttu-id="5ed8d-178">String</span><span class="sxs-lookup"><span data-stu-id="5ed8d-178">String</span></span>|<span data-ttu-id="5ed8d-179">当连接类型设置为自定义 vpn 时, 由 VPN 供应商提供的标识符。</span><span class="sxs-lookup"><span data-stu-id="5ed8d-179">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="5ed8d-180">例如: Cisco AnyConnect 使用 AnyConnect 形式的标识符。 applevpn 的标识符</span><span class="sxs-lookup"><span data-stu-id="5ed8d-180">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin</span></span>|
|<span data-ttu-id="5ed8d-181">customData</span><span class="sxs-lookup"><span data-stu-id="5ed8d-181">customData</span></span>|<span data-ttu-id="5ed8d-182">[keyValue](../resources/intune-deviceconfig-keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5ed8d-182">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="5ed8d-183">将连接类型设置为自定义 VPN 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="5ed8d-183">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="5ed8d-184">使用此字段启用 Intune 不支持的功能, 但在你的 VPN 解决方案中可用。</span><span class="sxs-lookup"><span data-stu-id="5ed8d-184">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="5ed8d-185">请与你的 VPN 供应商联系, 了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="5ed8d-185">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="5ed8d-186">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="5ed8d-186">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="5ed8d-187">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="5ed8d-187">customKeyValueData</span></span>|<span data-ttu-id="5ed8d-188">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5ed8d-188">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="5ed8d-189">将连接类型设置为自定义 VPN 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="5ed8d-189">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="5ed8d-190">使用此字段启用 Intune 不支持的功能, 但在你的 VPN 解决方案中可用。</span><span class="sxs-lookup"><span data-stu-id="5ed8d-190">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="5ed8d-191">请与你的 VPN 供应商联系, 了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="5ed8d-191">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="5ed8d-192">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="5ed8d-192">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="5ed8d-193">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="5ed8d-193">enableSplitTunneling</span></span>|<span data-ttu-id="5ed8d-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ed8d-194">Boolean</span></span>|<span data-ttu-id="5ed8d-195">通过 VPN 发送所有网络流量。</span><span class="sxs-lookup"><span data-stu-id="5ed8d-195">Send all network traffic through VPN.</span></span>|
|<span data-ttu-id="5ed8d-196">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="5ed8d-196">authenticationMethod</span></span>|[<span data-ttu-id="5ed8d-197">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="5ed8d-197">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="5ed8d-198">此 VPN 连接的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="5ed8d-198">Authentication method for this VPN connection.</span></span> <span data-ttu-id="5ed8d-199">可取值为：`certificate`、`usernameAndPassword`。</span><span class="sxs-lookup"><span data-stu-id="5ed8d-199">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="5ed8d-200">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="5ed8d-200">enablePerApp</span></span>|<span data-ttu-id="5ed8d-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ed8d-201">Boolean</span></span>|<span data-ttu-id="5ed8d-202">将此设置为 true 将创建每个应用程序 VPN 有效负载, 以后可将其与可在最终用户的 iOS 设备上触发此 VPN 连接的应用程序相关联。</span><span class="sxs-lookup"><span data-stu-id="5ed8d-202">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span>|
|<span data-ttu-id="5ed8d-203">safariDomains</span><span class="sxs-lookup"><span data-stu-id="5ed8d-203">safariDomains</span></span>|<span data-ttu-id="5ed8d-204">String collection</span><span class="sxs-lookup"><span data-stu-id="5ed8d-204">String collection</span></span>|<span data-ttu-id="5ed8d-205">启用此 VPN 每应用程序设置时的 Safari 域。</span><span class="sxs-lookup"><span data-stu-id="5ed8d-205">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="5ed8d-206">除了与此 vpn 关联的应用程序之外, 此处指定的 Safari 域还将能够触发此 vpn 连接。</span><span class="sxs-lookup"><span data-stu-id="5ed8d-206">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span>|
|<span data-ttu-id="5ed8d-207">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="5ed8d-207">onDemandRules</span></span>|<span data-ttu-id="5ed8d-208">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="5ed8d-208">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="5ed8d-209">按需规则。</span><span class="sxs-lookup"><span data-stu-id="5ed8d-209">On-Demand Rules.</span></span> <span data-ttu-id="5ed8d-210">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="5ed8d-210">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="5ed8d-211">proxyServer</span><span class="sxs-lookup"><span data-stu-id="5ed8d-211">proxyServer</span></span>|[<span data-ttu-id="5ed8d-212">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="5ed8d-212">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="5ed8d-213">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="5ed8d-213">Proxy Server.</span></span>|
|<span data-ttu-id="5ed8d-214">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="5ed8d-214">optInToDeviceIdSharing</span></span>|<span data-ttu-id="5ed8d-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ed8d-215">Boolean</span></span>|<span data-ttu-id="5ed8d-216">选择将设备的 Id 共享到第三方 vpn 客户端, 以便在网络访问控制验证期间使用。</span><span class="sxs-lookup"><span data-stu-id="5ed8d-216">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5ed8d-217">关系</span><span class="sxs-lookup"><span data-stu-id="5ed8d-217">Relationships</span></span>
|<span data-ttu-id="5ed8d-218">关系</span><span class="sxs-lookup"><span data-stu-id="5ed8d-218">Relationship</span></span>|<span data-ttu-id="5ed8d-219">类型</span><span class="sxs-lookup"><span data-stu-id="5ed8d-219">Type</span></span>|<span data-ttu-id="5ed8d-220">说明</span><span class="sxs-lookup"><span data-stu-id="5ed8d-220">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ed8d-221">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="5ed8d-221">groupAssignments</span></span>|<span data-ttu-id="5ed8d-222">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="5ed8d-222">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="5ed8d-223">设备配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="5ed8d-223">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="5ed8d-224">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ed8d-224">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ed8d-225">assignments</span><span class="sxs-lookup"><span data-stu-id="5ed8d-225">assignments</span></span>|<span data-ttu-id="5ed8d-226">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5ed8d-226">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="5ed8d-227">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="5ed8d-227">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="5ed8d-228">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ed8d-228">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ed8d-229">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="5ed8d-229">deviceStatuses</span></span>|<span data-ttu-id="5ed8d-230">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5ed8d-230">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="5ed8d-231">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="5ed8d-231">Device configuration installation status by device.</span></span> <span data-ttu-id="5ed8d-232">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ed8d-232">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ed8d-233">userStatuses</span><span class="sxs-lookup"><span data-stu-id="5ed8d-233">userStatuses</span></span>|<span data-ttu-id="5ed8d-234">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5ed8d-234">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="5ed8d-235">按用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="5ed8d-235">Device configuration installation status by user.</span></span> <span data-ttu-id="5ed8d-236">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ed8d-236">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ed8d-237">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="5ed8d-237">deviceStatusOverview</span></span>|[<span data-ttu-id="5ed8d-238">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="5ed8d-238">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="5ed8d-239">设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ed8d-239">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ed8d-240">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="5ed8d-240">userStatusOverview</span></span>|[<span data-ttu-id="5ed8d-241">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="5ed8d-241">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="5ed8d-242">设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ed8d-242">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ed8d-243">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="5ed8d-243">deviceSettingStateSummaries</span></span>|<span data-ttu-id="5ed8d-244">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5ed8d-244">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="5ed8d-245">设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ed8d-245">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5ed8d-246">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5ed8d-246">JSON Representation</span></span>
<span data-ttu-id="5ed8d-247">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5ed8d-247">Here is a JSON representation of the resource.</span></span>
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





