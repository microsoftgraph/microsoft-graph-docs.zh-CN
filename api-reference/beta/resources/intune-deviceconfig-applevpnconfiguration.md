---
title: appleVpnConfiguration 资源类型
description: Apple VPN 配置配置文件。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 85a70322a601fd09c9b944fcfd1d07885fa8f1fd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853254"
---
# <a name="applevpnconfiguration-resource-type"></a><span data-ttu-id="7ea78-103">appleVpnConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="7ea78-103">appleVpnConfiguration resource type</span></span>

> <span data-ttu-id="7ea78-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7ea78-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7ea78-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7ea78-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7ea78-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7ea78-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7ea78-107">Apple VPN 配置配置文件。</span><span class="sxs-lookup"><span data-stu-id="7ea78-107">Apple VPN configuration profile.</span></span>

<span data-ttu-id="7ea78-108">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ea78-108">Inherits from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="7ea78-109">方法</span><span class="sxs-lookup"><span data-stu-id="7ea78-109">Methods</span></span>
|<span data-ttu-id="7ea78-110">方法</span><span class="sxs-lookup"><span data-stu-id="7ea78-110">Method</span></span>|<span data-ttu-id="7ea78-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="7ea78-111">Return Type</span></span>|<span data-ttu-id="7ea78-112">说明</span><span class="sxs-lookup"><span data-stu-id="7ea78-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7ea78-113">列表 appleVpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="7ea78-113">List appleVpnConfigurations</span></span>](../api/intune-deviceconfig-applevpnconfiguration-list.md)|<span data-ttu-id="7ea78-114">[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)集合</span><span class="sxs-lookup"><span data-stu-id="7ea78-114">[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) collection</span></span>|<span data-ttu-id="7ea78-115">列出属性和[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="7ea78-115">List properties and relationships of the [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="7ea78-116">获取 appleVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="7ea78-116">Get appleVpnConfiguration</span></span>](../api/intune-deviceconfig-applevpnconfiguration-get.md)|[<span data-ttu-id="7ea78-117">appleVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="7ea78-117">appleVpnConfiguration</span></span>](../resources/intune-deviceconfig-applevpnconfiguration.md)|<span data-ttu-id="7ea78-118">读取属性和[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="7ea78-118">Read properties and relationships of the [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7ea78-119">属性</span><span class="sxs-lookup"><span data-stu-id="7ea78-119">Properties</span></span>
|<span data-ttu-id="7ea78-120">属性</span><span class="sxs-lookup"><span data-stu-id="7ea78-120">Property</span></span>|<span data-ttu-id="7ea78-121">类型</span><span class="sxs-lookup"><span data-stu-id="7ea78-121">Type</span></span>|<span data-ttu-id="7ea78-122">说明</span><span class="sxs-lookup"><span data-stu-id="7ea78-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ea78-123">id</span><span class="sxs-lookup"><span data-stu-id="7ea78-123">id</span></span>|<span data-ttu-id="7ea78-124">String</span><span class="sxs-lookup"><span data-stu-id="7ea78-124">String</span></span>|<span data-ttu-id="7ea78-125">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7ea78-125">Key of the entity.</span></span> <span data-ttu-id="7ea78-126">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ea78-126">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7ea78-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7ea78-127">lastModifiedDateTime</span></span>|<span data-ttu-id="7ea78-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ea78-128">DateTimeOffset</span></span>|<span data-ttu-id="7ea78-129">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="7ea78-129">DateTime the object was last modified.</span></span> <span data-ttu-id="7ea78-130">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ea78-130">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7ea78-131">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7ea78-131">roleScopeTagIds</span></span>|<span data-ttu-id="7ea78-132">String 集合</span><span class="sxs-lookup"><span data-stu-id="7ea78-132">String collection</span></span>|<span data-ttu-id="7ea78-133">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="7ea78-133">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7ea78-134">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ea78-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7ea78-135">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="7ea78-135">supportsScopeTags</span></span>|<span data-ttu-id="7ea78-136">布尔</span><span class="sxs-lookup"><span data-stu-id="7ea78-136">Boolean</span></span>|<span data-ttu-id="7ea78-137">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="7ea78-137">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="7ea78-138">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="7ea78-138">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="7ea78-139">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="7ea78-139">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="7ea78-140">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="7ea78-140">This property is read-only.</span></span> <span data-ttu-id="7ea78-141">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ea78-141">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7ea78-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7ea78-142">createdDateTime</span></span>|<span data-ttu-id="7ea78-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ea78-143">DateTimeOffset</span></span>|<span data-ttu-id="7ea78-144">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="7ea78-144">DateTime the object was created.</span></span> <span data-ttu-id="7ea78-145">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ea78-145">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7ea78-146">description</span><span class="sxs-lookup"><span data-stu-id="7ea78-146">description</span></span>|<span data-ttu-id="7ea78-147">String</span><span class="sxs-lookup"><span data-stu-id="7ea78-147">String</span></span>|<span data-ttu-id="7ea78-148">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="7ea78-148">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7ea78-149">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ea78-149">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7ea78-150">displayName</span><span class="sxs-lookup"><span data-stu-id="7ea78-150">displayName</span></span>|<span data-ttu-id="7ea78-151">String</span><span class="sxs-lookup"><span data-stu-id="7ea78-151">String</span></span>|<span data-ttu-id="7ea78-152">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="7ea78-152">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7ea78-153">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ea78-153">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7ea78-154">version</span><span class="sxs-lookup"><span data-stu-id="7ea78-154">version</span></span>|<span data-ttu-id="7ea78-155">Int32</span><span class="sxs-lookup"><span data-stu-id="7ea78-155">Int32</span></span>|<span data-ttu-id="7ea78-156">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="7ea78-156">Version of the device configuration.</span></span> <span data-ttu-id="7ea78-157">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ea78-157">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7ea78-158">connectionName</span><span class="sxs-lookup"><span data-stu-id="7ea78-158">connectionName</span></span>|<span data-ttu-id="7ea78-159">字符串</span><span class="sxs-lookup"><span data-stu-id="7ea78-159">String</span></span>|<span data-ttu-id="7ea78-160">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="7ea78-160">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="7ea78-161">连接</span><span class="sxs-lookup"><span data-stu-id="7ea78-161">connectionType</span></span>|[<span data-ttu-id="7ea78-162">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="7ea78-162">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="7ea78-163">连接类型。</span><span class="sxs-lookup"><span data-stu-id="7ea78-163">Connection type.</span></span> <span data-ttu-id="7ea78-164">可能的值为： `ciscoAnyConnect`， `pulseSecure`， `f5EdgeClient`， `dellSonicWallMobileConnect`， `checkPointCapsuleVpn`， `customVpn`， `ciscoIPSec`， `citrix`， `ciscoAnyConnectV2`， `paloAltoGlobalProtect`， `zscalerPrivateAccess`， `f5Access2018`， `citrixSso`， `paloAltoGlobalProtectV2`。</span><span class="sxs-lookup"><span data-stu-id="7ea78-164">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`.</span></span>|
|<span data-ttu-id="7ea78-165">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="7ea78-165">loginGroupOrDomain</span></span>|<span data-ttu-id="7ea78-166">字符串</span><span class="sxs-lookup"><span data-stu-id="7ea78-166">String</span></span>|<span data-ttu-id="7ea78-167">登录组或域时连接类型设置为 Dell 使 SonicWALL Mobile 连接。</span><span class="sxs-lookup"><span data-stu-id="7ea78-167">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="7ea78-168">role</span><span class="sxs-lookup"><span data-stu-id="7ea78-168">role</span></span>|<span data-ttu-id="7ea78-169">字符串</span><span class="sxs-lookup"><span data-stu-id="7ea78-169">String</span></span>|<span data-ttu-id="7ea78-170">当连接类型设置为脉冲安全角色。</span><span class="sxs-lookup"><span data-stu-id="7ea78-170">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="7ea78-171">领域</span><span class="sxs-lookup"><span data-stu-id="7ea78-171">realm</span></span>|<span data-ttu-id="7ea78-172">字符串</span><span class="sxs-lookup"><span data-stu-id="7ea78-172">String</span></span>|<span data-ttu-id="7ea78-173">当连接类型设置为脉冲安全领域。</span><span class="sxs-lookup"><span data-stu-id="7ea78-173">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="7ea78-174">服务器</span><span class="sxs-lookup"><span data-stu-id="7ea78-174">server</span></span>|[<span data-ttu-id="7ea78-175">vpnServer</span><span class="sxs-lookup"><span data-stu-id="7ea78-175">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="7ea78-176">在网络上的 VPN 服务器。</span><span class="sxs-lookup"><span data-stu-id="7ea78-176">VPN Server on the network.</span></span> <span data-ttu-id="7ea78-177">请确保最终用户可以访问此网络位置。</span><span class="sxs-lookup"><span data-stu-id="7ea78-177">Make sure end users can access this network location.</span></span>|
|<span data-ttu-id="7ea78-178">标识符</span><span class="sxs-lookup"><span data-stu-id="7ea78-178">identifier</span></span>|<span data-ttu-id="7ea78-179">字符串</span><span class="sxs-lookup"><span data-stu-id="7ea78-179">String</span></span>|<span data-ttu-id="7ea78-180">当连接类型设置为自定义 VPN VPN 供应商提供的标识符。</span><span class="sxs-lookup"><span data-stu-id="7ea78-180">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="7ea78-181">例如： Cisco AnyConnect 使用的窗体 com.cisco.anyconnect.applevpn.plugin 标识符</span><span class="sxs-lookup"><span data-stu-id="7ea78-181">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin</span></span>|
|<span data-ttu-id="7ea78-182">customData</span><span class="sxs-lookup"><span data-stu-id="7ea78-182">customData</span></span>|<span data-ttu-id="7ea78-183">[keyValue](../resources/intune-deviceconfig-keyvalue.md)集合</span><span class="sxs-lookup"><span data-stu-id="7ea78-183">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="7ea78-184">当设置为自定义 VPN 连接类型的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="7ea78-184">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="7ea78-185">使用此字段启用不支持 Intune，但在 VPN 解决方案中可用的功能。</span><span class="sxs-lookup"><span data-stu-id="7ea78-185">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="7ea78-186">了解如何添加这些键/值对 VPN 供应商联系。</span><span class="sxs-lookup"><span data-stu-id="7ea78-186">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="7ea78-187">此集合可以包含最多 25 元素。</span><span class="sxs-lookup"><span data-stu-id="7ea78-187">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="7ea78-188">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="7ea78-188">customKeyValueData</span></span>|<span data-ttu-id="7ea78-189">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7ea78-189">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="7ea78-190">当设置为自定义 VPN 连接类型的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="7ea78-190">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="7ea78-191">使用此字段启用不支持 Intune，但在 VPN 解决方案中可用的功能。</span><span class="sxs-lookup"><span data-stu-id="7ea78-191">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="7ea78-192">了解如何添加这些键/值对 VPN 供应商联系。</span><span class="sxs-lookup"><span data-stu-id="7ea78-192">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="7ea78-193">此集合可以包含最多 25 元素。</span><span class="sxs-lookup"><span data-stu-id="7ea78-193">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="7ea78-194">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="7ea78-194">enableSplitTunneling</span></span>|<span data-ttu-id="7ea78-195">布尔</span><span class="sxs-lookup"><span data-stu-id="7ea78-195">Boolean</span></span>|<span data-ttu-id="7ea78-196">将发送所有网络流量通过 VPN。</span><span class="sxs-lookup"><span data-stu-id="7ea78-196">Send all network traffic through VPN.</span></span>|
|<span data-ttu-id="7ea78-197">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="7ea78-197">authenticationMethod</span></span>|[<span data-ttu-id="7ea78-198">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="7ea78-198">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="7ea78-199">此 VPN 连接的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="7ea78-199">Authentication method for this VPN connection.</span></span> <span data-ttu-id="7ea78-200">可取值为：`certificate`、`usernameAndPassword`。</span><span class="sxs-lookup"><span data-stu-id="7ea78-200">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="7ea78-201">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="7ea78-201">enablePerApp</span></span>|<span data-ttu-id="7ea78-202">布尔</span><span class="sxs-lookup"><span data-stu-id="7ea78-202">Boolean</span></span>|<span data-ttu-id="7ea78-203">将此值设置为 true 时，创建更高版本可以是与可触发本 VPN 连接最终用户的 iOS 设备上的应用程序关联的每个应用程序 VPN 负载。</span><span class="sxs-lookup"><span data-stu-id="7ea78-203">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span>|
|<span data-ttu-id="7ea78-204">safariDomains</span><span class="sxs-lookup"><span data-stu-id="7ea78-204">safariDomains</span></span>|<span data-ttu-id="7ea78-205">String 集合</span><span class="sxs-lookup"><span data-stu-id="7ea78-205">String collection</span></span>|<span data-ttu-id="7ea78-206">Safari 域时启用此 VPN 每应用程序设置。</span><span class="sxs-lookup"><span data-stu-id="7ea78-206">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="7ea78-207">与此 VPN 关联的应用程序，除了 Safari 域指定此处还将能够触发本 VPN 连接。</span><span class="sxs-lookup"><span data-stu-id="7ea78-207">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span>|
|<span data-ttu-id="7ea78-208">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="7ea78-208">onDemandRules</span></span>|<span data-ttu-id="7ea78-209">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="7ea78-209">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="7ea78-210">按需规则。</span><span class="sxs-lookup"><span data-stu-id="7ea78-210">On-Demand Rules.</span></span> <span data-ttu-id="7ea78-211">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="7ea78-211">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="7ea78-212">代理服务器</span><span class="sxs-lookup"><span data-stu-id="7ea78-212">proxyServer</span></span>|[<span data-ttu-id="7ea78-213">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="7ea78-213">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="7ea78-214">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="7ea78-214">Proxy Server.</span></span>|
|<span data-ttu-id="7ea78-215">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="7ea78-215">optInToDeviceIdSharing</span></span>|<span data-ttu-id="7ea78-216">布尔</span><span class="sxs-lookup"><span data-stu-id="7ea78-216">Boolean</span></span>|<span data-ttu-id="7ea78-217">加入到共享网络访问控制验证过程中的第三方 vpn 客户端使用的设备的 Id。</span><span class="sxs-lookup"><span data-stu-id="7ea78-217">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7ea78-218">Relationships</span><span class="sxs-lookup"><span data-stu-id="7ea78-218">Relationships</span></span>
|<span data-ttu-id="7ea78-219">关系</span><span class="sxs-lookup"><span data-stu-id="7ea78-219">Relationship</span></span>|<span data-ttu-id="7ea78-220">类型</span><span class="sxs-lookup"><span data-stu-id="7ea78-220">Type</span></span>|<span data-ttu-id="7ea78-221">Description</span><span class="sxs-lookup"><span data-stu-id="7ea78-221">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ea78-222">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="7ea78-222">groupAssignments</span></span>|<span data-ttu-id="7ea78-223">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="7ea78-223">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="7ea78-224">设备配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="7ea78-224">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="7ea78-225">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ea78-225">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7ea78-226">assignments</span><span class="sxs-lookup"><span data-stu-id="7ea78-226">assignments</span></span>|<span data-ttu-id="7ea78-227">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7ea78-227">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="7ea78-228">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="7ea78-228">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="7ea78-229">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ea78-229">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7ea78-230">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="7ea78-230">deviceStatuses</span></span>|<span data-ttu-id="7ea78-231">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7ea78-231">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="7ea78-232">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="7ea78-232">Device configuration installation status by device.</span></span> <span data-ttu-id="7ea78-233">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ea78-233">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7ea78-234">userStatuses</span><span class="sxs-lookup"><span data-stu-id="7ea78-234">userStatuses</span></span>|<span data-ttu-id="7ea78-235">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7ea78-235">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="7ea78-236">用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="7ea78-236">Device configuration installation status by user.</span></span> <span data-ttu-id="7ea78-237">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ea78-237">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7ea78-238">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="7ea78-238">deviceStatusOverview</span></span>|[<span data-ttu-id="7ea78-239">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="7ea78-239">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="7ea78-240">设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ea78-240">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7ea78-241">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="7ea78-241">userStatusOverview</span></span>|[<span data-ttu-id="7ea78-242">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="7ea78-242">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="7ea78-243">设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ea78-243">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7ea78-244">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="7ea78-244">deviceSettingStateSummaries</span></span>|<span data-ttu-id="7ea78-245">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7ea78-245">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="7ea78-246">设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ea78-246">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7ea78-247">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7ea78-247">JSON Representation</span></span>
<span data-ttu-id="7ea78-248">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7ea78-248">Here is a JSON representation of the resource.</span></span>
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





