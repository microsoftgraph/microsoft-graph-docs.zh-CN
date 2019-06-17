---
title: appleVpnConfiguration 资源类型
description: Apple VPN 配置文件。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 57f3e7416dc984cf39b67638557aecf5a92a48a7
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34987675"
---
# <a name="applevpnconfiguration-resource-type"></a><span data-ttu-id="88d81-103">appleVpnConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="88d81-103">appleVpnConfiguration resource type</span></span>

> <span data-ttu-id="88d81-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="88d81-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88d81-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="88d81-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88d81-106">Apple VPN 配置文件。</span><span class="sxs-lookup"><span data-stu-id="88d81-106">Apple VPN configuration profile.</span></span>


<span data-ttu-id="88d81-107">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88d81-107">Inherits from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="88d81-108">方法</span><span class="sxs-lookup"><span data-stu-id="88d81-108">Methods</span></span>
|<span data-ttu-id="88d81-109">方法</span><span class="sxs-lookup"><span data-stu-id="88d81-109">Method</span></span>|<span data-ttu-id="88d81-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="88d81-110">Return Type</span></span>|<span data-ttu-id="88d81-111">说明</span><span class="sxs-lookup"><span data-stu-id="88d81-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="88d81-112">列出 appleVpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="88d81-112">List appleVpnConfigurations</span></span>](../api/intune-deviceconfig-applevpnconfiguration-list.md)|<span data-ttu-id="88d81-113">[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)集合</span><span class="sxs-lookup"><span data-stu-id="88d81-113">[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) collection</span></span>|<span data-ttu-id="88d81-114">列出[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="88d81-114">List properties and relationships of the [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="88d81-115">获取 appleVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="88d81-115">Get appleVpnConfiguration</span></span>](../api/intune-deviceconfig-applevpnconfiguration-get.md)|[<span data-ttu-id="88d81-116">appleVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="88d81-116">appleVpnConfiguration</span></span>](../resources/intune-deviceconfig-applevpnconfiguration.md)|<span data-ttu-id="88d81-117">读取[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="88d81-117">Read properties and relationships of the [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="88d81-118">属性</span><span class="sxs-lookup"><span data-stu-id="88d81-118">Properties</span></span>
|<span data-ttu-id="88d81-119">属性</span><span class="sxs-lookup"><span data-stu-id="88d81-119">Property</span></span>|<span data-ttu-id="88d81-120">类型</span><span class="sxs-lookup"><span data-stu-id="88d81-120">Type</span></span>|<span data-ttu-id="88d81-121">说明</span><span class="sxs-lookup"><span data-stu-id="88d81-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88d81-122">id</span><span class="sxs-lookup"><span data-stu-id="88d81-122">id</span></span>|<span data-ttu-id="88d81-123">字符串</span><span class="sxs-lookup"><span data-stu-id="88d81-123">String</span></span>|<span data-ttu-id="88d81-124">实体的键。</span><span class="sxs-lookup"><span data-stu-id="88d81-124">Key of the entity.</span></span> <span data-ttu-id="88d81-125">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88d81-125">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88d81-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="88d81-126">lastModifiedDateTime</span></span>|<span data-ttu-id="88d81-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88d81-127">DateTimeOffset</span></span>|<span data-ttu-id="88d81-128">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="88d81-128">DateTime the object was last modified.</span></span> <span data-ttu-id="88d81-129">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88d81-129">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88d81-130">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="88d81-130">roleScopeTagIds</span></span>|<span data-ttu-id="88d81-131">String collection</span><span class="sxs-lookup"><span data-stu-id="88d81-131">String collection</span></span>|<span data-ttu-id="88d81-132">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="88d81-132">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="88d81-133">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88d81-133">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88d81-134">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="88d81-134">supportsScopeTags</span></span>|<span data-ttu-id="88d81-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="88d81-135">Boolean</span></span>|<span data-ttu-id="88d81-136">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="88d81-136">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="88d81-137">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="88d81-137">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="88d81-138">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="88d81-138">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="88d81-139">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="88d81-139">This property is read-only.</span></span> <span data-ttu-id="88d81-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88d81-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88d81-141">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="88d81-141">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="88d81-142">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="88d81-142">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="88d81-143">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="88d81-143">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="88d81-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88d81-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88d81-145">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="88d81-145">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="88d81-146">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="88d81-146">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="88d81-147">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="88d81-147">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="88d81-148">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88d81-148">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88d81-149">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="88d81-149">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="88d81-150">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="88d81-150">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="88d81-151">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="88d81-151">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="88d81-152">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88d81-152">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88d81-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="88d81-153">createdDateTime</span></span>|<span data-ttu-id="88d81-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88d81-154">DateTimeOffset</span></span>|<span data-ttu-id="88d81-155">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="88d81-155">DateTime the object was created.</span></span> <span data-ttu-id="88d81-156">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88d81-156">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88d81-157">说明</span><span class="sxs-lookup"><span data-stu-id="88d81-157">description</span></span>|<span data-ttu-id="88d81-158">String</span><span class="sxs-lookup"><span data-stu-id="88d81-158">String</span></span>|<span data-ttu-id="88d81-159">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="88d81-159">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="88d81-160">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88d81-160">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88d81-161">displayName</span><span class="sxs-lookup"><span data-stu-id="88d81-161">displayName</span></span>|<span data-ttu-id="88d81-162">String</span><span class="sxs-lookup"><span data-stu-id="88d81-162">String</span></span>|<span data-ttu-id="88d81-163">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="88d81-163">Admin provided name of the device configuration.</span></span> <span data-ttu-id="88d81-164">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88d81-164">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88d81-165">version</span><span class="sxs-lookup"><span data-stu-id="88d81-165">version</span></span>|<span data-ttu-id="88d81-166">Int32</span><span class="sxs-lookup"><span data-stu-id="88d81-166">Int32</span></span>|<span data-ttu-id="88d81-167">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="88d81-167">Version of the device configuration.</span></span> <span data-ttu-id="88d81-168">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88d81-168">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88d81-169">connectionName</span><span class="sxs-lookup"><span data-stu-id="88d81-169">connectionName</span></span>|<span data-ttu-id="88d81-170">String</span><span class="sxs-lookup"><span data-stu-id="88d81-170">String</span></span>|<span data-ttu-id="88d81-171">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="88d81-171">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="88d81-172">connectionType</span><span class="sxs-lookup"><span data-stu-id="88d81-172">connectionType</span></span>|[<span data-ttu-id="88d81-173">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="88d81-173">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="88d81-174">连接类型。</span><span class="sxs-lookup"><span data-stu-id="88d81-174">Connection type.</span></span> <span data-ttu-id="88d81-175">可能的值为`ciscoAnyConnect`: `pulseSecure`、 `f5EdgeClient`、 `dellSonicWallMobileConnect` `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `ciscoAnyConnectV2` `ikEv2`、、 `zscalerPrivateAccess`、、、、、、、、、、。 `paloAltoGlobalProtect` `f5Access2018` `citrixSso` `paloAltoGlobalProtectV2`</span><span class="sxs-lookup"><span data-stu-id="88d81-175">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`.</span></span>|
|<span data-ttu-id="88d81-176">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="88d81-176">loginGroupOrDomain</span></span>|<span data-ttu-id="88d81-177">String</span><span class="sxs-lookup"><span data-stu-id="88d81-177">String</span></span>|<span data-ttu-id="88d81-178">将连接类型设置为 Dell SonicWALL Mobile 连接时的登录组或域。</span><span class="sxs-lookup"><span data-stu-id="88d81-178">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="88d81-179">role</span><span class="sxs-lookup"><span data-stu-id="88d81-179">role</span></span>|<span data-ttu-id="88d81-180">String</span><span class="sxs-lookup"><span data-stu-id="88d81-180">String</span></span>|<span data-ttu-id="88d81-181">将 "连接类型" 设置为 "脉冲安全" 时的角色。</span><span class="sxs-lookup"><span data-stu-id="88d81-181">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="88d81-182">型</span><span class="sxs-lookup"><span data-stu-id="88d81-182">realm</span></span>|<span data-ttu-id="88d81-183">String</span><span class="sxs-lookup"><span data-stu-id="88d81-183">String</span></span>|<span data-ttu-id="88d81-184">连接类型设置为脉冲安全时的领域。</span><span class="sxs-lookup"><span data-stu-id="88d81-184">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="88d81-185">服务器主板</span><span class="sxs-lookup"><span data-stu-id="88d81-185">server</span></span>|[<span data-ttu-id="88d81-186">vpnServer</span><span class="sxs-lookup"><span data-stu-id="88d81-186">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="88d81-187">网络上的 VPN 服务器。</span><span class="sxs-lookup"><span data-stu-id="88d81-187">VPN Server on the network.</span></span> <span data-ttu-id="88d81-188">请确保最终用户可以访问此网络位置。</span><span class="sxs-lookup"><span data-stu-id="88d81-188">Make sure end users can access this network location.</span></span>|
|<span data-ttu-id="88d81-189">标识符</span><span class="sxs-lookup"><span data-stu-id="88d81-189">identifier</span></span>|<span data-ttu-id="88d81-190">String</span><span class="sxs-lookup"><span data-stu-id="88d81-190">String</span></span>|<span data-ttu-id="88d81-191">当连接类型设置为自定义 VPN 时, 由 VPN 供应商提供的标识符。</span><span class="sxs-lookup"><span data-stu-id="88d81-191">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="88d81-192">例如: Cisco AnyConnect 使用 AnyConnect 形式的标识符。 applevpn 的标识符</span><span class="sxs-lookup"><span data-stu-id="88d81-192">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin</span></span>|
|<span data-ttu-id="88d81-193">customData</span><span class="sxs-lookup"><span data-stu-id="88d81-193">customData</span></span>|<span data-ttu-id="88d81-194">[keyValue](../resources/intune-deviceconfig-keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="88d81-194">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="88d81-195">将连接类型设置为自定义 VPN 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="88d81-195">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="88d81-196">使用此字段启用 Intune 不支持的功能, 但在你的 VPN 解决方案中可用。</span><span class="sxs-lookup"><span data-stu-id="88d81-196">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="88d81-197">请与你的 VPN 供应商联系, 了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="88d81-197">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="88d81-198">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="88d81-198">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="88d81-199">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="88d81-199">customKeyValueData</span></span>|<span data-ttu-id="88d81-200">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="88d81-200">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="88d81-201">将连接类型设置为自定义 VPN 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="88d81-201">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="88d81-202">使用此字段启用 Intune 不支持的功能, 但在你的 VPN 解决方案中可用。</span><span class="sxs-lookup"><span data-stu-id="88d81-202">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="88d81-203">请与你的 VPN 供应商联系, 了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="88d81-203">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="88d81-204">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="88d81-204">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="88d81-205">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="88d81-205">enableSplitTunneling</span></span>|<span data-ttu-id="88d81-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="88d81-206">Boolean</span></span>|<span data-ttu-id="88d81-207">通过 VPN 发送所有网络流量。</span><span class="sxs-lookup"><span data-stu-id="88d81-207">Send all network traffic through VPN.</span></span>|
|<span data-ttu-id="88d81-208">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="88d81-208">authenticationMethod</span></span>|[<span data-ttu-id="88d81-209">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="88d81-209">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="88d81-210">此 VPN 连接的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="88d81-210">Authentication method for this VPN connection.</span></span> <span data-ttu-id="88d81-211">可取值为：`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="88d81-211">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|
|<span data-ttu-id="88d81-212">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="88d81-212">enablePerApp</span></span>|<span data-ttu-id="88d81-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="88d81-213">Boolean</span></span>|<span data-ttu-id="88d81-214">将此设置为 true 将创建每个应用程序 VPN 有效负载, 以后可将其与可在最终用户的 iOS 设备上触发此 VPN 连接的应用程序相关联。</span><span class="sxs-lookup"><span data-stu-id="88d81-214">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span>|
|<span data-ttu-id="88d81-215">safariDomains</span><span class="sxs-lookup"><span data-stu-id="88d81-215">safariDomains</span></span>|<span data-ttu-id="88d81-216">String collection</span><span class="sxs-lookup"><span data-stu-id="88d81-216">String collection</span></span>|<span data-ttu-id="88d81-217">启用此 VPN 每应用程序设置时的 Safari 域。</span><span class="sxs-lookup"><span data-stu-id="88d81-217">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="88d81-218">除了与此 VPN 关联的应用程序之外, 此处指定的 Safari 域还将能够触发此 VPN 连接。</span><span class="sxs-lookup"><span data-stu-id="88d81-218">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span>|
|<span data-ttu-id="88d81-219">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="88d81-219">onDemandRules</span></span>|<span data-ttu-id="88d81-220">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="88d81-220">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="88d81-221">按需规则。</span><span class="sxs-lookup"><span data-stu-id="88d81-221">On-Demand Rules.</span></span> <span data-ttu-id="88d81-222">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="88d81-222">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="88d81-223">proxyServer</span><span class="sxs-lookup"><span data-stu-id="88d81-223">proxyServer</span></span>|[<span data-ttu-id="88d81-224">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="88d81-224">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="88d81-225">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="88d81-225">Proxy Server.</span></span>|
|<span data-ttu-id="88d81-226">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="88d81-226">optInToDeviceIdSharing</span></span>|<span data-ttu-id="88d81-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="88d81-227">Boolean</span></span>|<span data-ttu-id="88d81-228">选择将设备的 Id 共享到第三方 vpn 客户端, 以便在网络访问控制验证期间使用。</span><span class="sxs-lookup"><span data-stu-id="88d81-228">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="88d81-229">关系</span><span class="sxs-lookup"><span data-stu-id="88d81-229">Relationships</span></span>
|<span data-ttu-id="88d81-230">关系</span><span class="sxs-lookup"><span data-stu-id="88d81-230">Relationship</span></span>|<span data-ttu-id="88d81-231">类型</span><span class="sxs-lookup"><span data-stu-id="88d81-231">Type</span></span>|<span data-ttu-id="88d81-232">说明</span><span class="sxs-lookup"><span data-stu-id="88d81-232">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88d81-233">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="88d81-233">groupAssignments</span></span>|<span data-ttu-id="88d81-234">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="88d81-234">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="88d81-235">设备配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="88d81-235">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="88d81-236">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88d81-236">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88d81-237">assignments</span><span class="sxs-lookup"><span data-stu-id="88d81-237">assignments</span></span>|<span data-ttu-id="88d81-238">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="88d81-238">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="88d81-239">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="88d81-239">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="88d81-240">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88d81-240">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88d81-241">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="88d81-241">deviceStatuses</span></span>|<span data-ttu-id="88d81-242">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="88d81-242">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="88d81-243">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="88d81-243">Device configuration installation status by device.</span></span> <span data-ttu-id="88d81-244">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88d81-244">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88d81-245">userStatuses</span><span class="sxs-lookup"><span data-stu-id="88d81-245">userStatuses</span></span>|<span data-ttu-id="88d81-246">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="88d81-246">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="88d81-247">按用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="88d81-247">Device configuration installation status by user.</span></span> <span data-ttu-id="88d81-248">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88d81-248">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88d81-249">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="88d81-249">deviceStatusOverview</span></span>|[<span data-ttu-id="88d81-250">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="88d81-250">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="88d81-251">设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88d81-251">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88d81-252">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="88d81-252">userStatusOverview</span></span>|[<span data-ttu-id="88d81-253">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="88d81-253">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="88d81-254">设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88d81-254">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88d81-255">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="88d81-255">deviceSettingStateSummaries</span></span>|<span data-ttu-id="88d81-256">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="88d81-256">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="88d81-257">设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88d81-257">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="88d81-258">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="88d81-258">JSON Representation</span></span>
<span data-ttu-id="88d81-259">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="88d81-259">Here is a JSON representation of the resource.</span></span>
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
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "String"
    ],
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "String",
    "maxOSVersion": "String",
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "String",
    "name": "String",
    "ruleType": "String"
  },
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





