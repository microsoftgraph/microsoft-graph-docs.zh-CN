---
title: appleVpnConfiguration 资源类型
description: Apple VPN 配置文件。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: af50edfb0c098ed2fffabb7b736d8e0ab4dcb871
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333980"
---
# <a name="applevpnconfiguration-resource-type"></a><span data-ttu-id="6337d-103">appleVpnConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="6337d-103">appleVpnConfiguration resource type</span></span>

> <span data-ttu-id="6337d-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6337d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6337d-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6337d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6337d-106">Apple VPN 配置文件。</span><span class="sxs-lookup"><span data-stu-id="6337d-106">Apple VPN configuration profile.</span></span>


<span data-ttu-id="6337d-107">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6337d-107">Inherits from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="6337d-108">方法</span><span class="sxs-lookup"><span data-stu-id="6337d-108">Methods</span></span>
|<span data-ttu-id="6337d-109">方法</span><span class="sxs-lookup"><span data-stu-id="6337d-109">Method</span></span>|<span data-ttu-id="6337d-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="6337d-110">Return Type</span></span>|<span data-ttu-id="6337d-111">说明</span><span class="sxs-lookup"><span data-stu-id="6337d-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6337d-112">列出 appleVpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="6337d-112">List appleVpnConfigurations</span></span>](../api/intune-deviceconfig-applevpnconfiguration-list.md)|<span data-ttu-id="6337d-113">[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)集合</span><span class="sxs-lookup"><span data-stu-id="6337d-113">[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) collection</span></span>|<span data-ttu-id="6337d-114">列出[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6337d-114">List properties and relationships of the [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="6337d-115">获取 appleVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="6337d-115">Get appleVpnConfiguration</span></span>](../api/intune-deviceconfig-applevpnconfiguration-get.md)|[<span data-ttu-id="6337d-116">appleVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="6337d-116">appleVpnConfiguration</span></span>](../resources/intune-deviceconfig-applevpnconfiguration.md)|<span data-ttu-id="6337d-117">读取[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6337d-117">Read properties and relationships of the [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6337d-118">属性</span><span class="sxs-lookup"><span data-stu-id="6337d-118">Properties</span></span>
|<span data-ttu-id="6337d-119">属性</span><span class="sxs-lookup"><span data-stu-id="6337d-119">Property</span></span>|<span data-ttu-id="6337d-120">类型</span><span class="sxs-lookup"><span data-stu-id="6337d-120">Type</span></span>|<span data-ttu-id="6337d-121">说明</span><span class="sxs-lookup"><span data-stu-id="6337d-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6337d-122">id</span><span class="sxs-lookup"><span data-stu-id="6337d-122">id</span></span>|<span data-ttu-id="6337d-123">字符串</span><span class="sxs-lookup"><span data-stu-id="6337d-123">String</span></span>|<span data-ttu-id="6337d-124">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6337d-124">Key of the entity.</span></span> <span data-ttu-id="6337d-125">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6337d-125">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6337d-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6337d-126">lastModifiedDateTime</span></span>|<span data-ttu-id="6337d-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6337d-127">DateTimeOffset</span></span>|<span data-ttu-id="6337d-128">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6337d-128">DateTime the object was last modified.</span></span> <span data-ttu-id="6337d-129">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6337d-129">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6337d-130">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6337d-130">roleScopeTagIds</span></span>|<span data-ttu-id="6337d-131">String collection</span><span class="sxs-lookup"><span data-stu-id="6337d-131">String collection</span></span>|<span data-ttu-id="6337d-132">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="6337d-132">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6337d-133">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6337d-133">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6337d-134">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6337d-134">supportsScopeTags</span></span>|<span data-ttu-id="6337d-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="6337d-135">Boolean</span></span>|<span data-ttu-id="6337d-136">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="6337d-136">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6337d-137">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="6337d-137">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6337d-138">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="6337d-138">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6337d-139">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6337d-139">This property is read-only.</span></span> <span data-ttu-id="6337d-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6337d-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6337d-141">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6337d-141">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="6337d-142">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6337d-142">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="6337d-143">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="6337d-143">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="6337d-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6337d-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6337d-145">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6337d-145">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="6337d-146">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6337d-146">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="6337d-147">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="6337d-147">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="6337d-148">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6337d-148">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6337d-149">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6337d-149">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="6337d-150">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6337d-150">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="6337d-151">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="6337d-151">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="6337d-152">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6337d-152">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6337d-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6337d-153">createdDateTime</span></span>|<span data-ttu-id="6337d-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6337d-154">DateTimeOffset</span></span>|<span data-ttu-id="6337d-155">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6337d-155">DateTime the object was created.</span></span> <span data-ttu-id="6337d-156">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6337d-156">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6337d-157">说明</span><span class="sxs-lookup"><span data-stu-id="6337d-157">description</span></span>|<span data-ttu-id="6337d-158">String</span><span class="sxs-lookup"><span data-stu-id="6337d-158">String</span></span>|<span data-ttu-id="6337d-159">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="6337d-159">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6337d-160">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6337d-160">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6337d-161">displayName</span><span class="sxs-lookup"><span data-stu-id="6337d-161">displayName</span></span>|<span data-ttu-id="6337d-162">String</span><span class="sxs-lookup"><span data-stu-id="6337d-162">String</span></span>|<span data-ttu-id="6337d-163">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="6337d-163">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6337d-164">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6337d-164">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6337d-165">version</span><span class="sxs-lookup"><span data-stu-id="6337d-165">version</span></span>|<span data-ttu-id="6337d-166">Int32</span><span class="sxs-lookup"><span data-stu-id="6337d-166">Int32</span></span>|<span data-ttu-id="6337d-167">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="6337d-167">Version of the device configuration.</span></span> <span data-ttu-id="6337d-168">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6337d-168">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6337d-169">connectionName</span><span class="sxs-lookup"><span data-stu-id="6337d-169">connectionName</span></span>|<span data-ttu-id="6337d-170">String</span><span class="sxs-lookup"><span data-stu-id="6337d-170">String</span></span>|<span data-ttu-id="6337d-171">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="6337d-171">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="6337d-172">connectionType</span><span class="sxs-lookup"><span data-stu-id="6337d-172">connectionType</span></span>|[<span data-ttu-id="6337d-173">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="6337d-173">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="6337d-174">连接类型。</span><span class="sxs-lookup"><span data-stu-id="6337d-174">Connection type.</span></span> <span data-ttu-id="6337d-175">可能的值为`ciscoAnyConnect`: `pulseSecure`、 `f5EdgeClient`、 `dellSonicWallMobileConnect` `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `ciscoAnyConnectV2` `ikEv2`、、 `zscalerPrivateAccess`、、、、、、、、、、。 `paloAltoGlobalProtect` `f5Access2018` `citrixSso` `paloAltoGlobalProtectV2`</span><span class="sxs-lookup"><span data-stu-id="6337d-175">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`.</span></span>|
|<span data-ttu-id="6337d-176">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="6337d-176">loginGroupOrDomain</span></span>|<span data-ttu-id="6337d-177">String</span><span class="sxs-lookup"><span data-stu-id="6337d-177">String</span></span>|<span data-ttu-id="6337d-178">将连接类型设置为 Dell SonicWALL Mobile 连接时的登录组或域。</span><span class="sxs-lookup"><span data-stu-id="6337d-178">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="6337d-179">role</span><span class="sxs-lookup"><span data-stu-id="6337d-179">role</span></span>|<span data-ttu-id="6337d-180">String</span><span class="sxs-lookup"><span data-stu-id="6337d-180">String</span></span>|<span data-ttu-id="6337d-181">将 "连接类型" 设置为 "脉冲安全" 时的角色。</span><span class="sxs-lookup"><span data-stu-id="6337d-181">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="6337d-182">型</span><span class="sxs-lookup"><span data-stu-id="6337d-182">realm</span></span>|<span data-ttu-id="6337d-183">String</span><span class="sxs-lookup"><span data-stu-id="6337d-183">String</span></span>|<span data-ttu-id="6337d-184">连接类型设置为脉冲安全时的领域。</span><span class="sxs-lookup"><span data-stu-id="6337d-184">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="6337d-185">服务器主板</span><span class="sxs-lookup"><span data-stu-id="6337d-185">server</span></span>|[<span data-ttu-id="6337d-186">vpnServer</span><span class="sxs-lookup"><span data-stu-id="6337d-186">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="6337d-187">网络上的 VPN 服务器。</span><span class="sxs-lookup"><span data-stu-id="6337d-187">VPN Server on the network.</span></span> <span data-ttu-id="6337d-188">请确保最终用户可以访问此网络位置。</span><span class="sxs-lookup"><span data-stu-id="6337d-188">Make sure end users can access this network location.</span></span>|
|<span data-ttu-id="6337d-189">标识符</span><span class="sxs-lookup"><span data-stu-id="6337d-189">identifier</span></span>|<span data-ttu-id="6337d-190">String</span><span class="sxs-lookup"><span data-stu-id="6337d-190">String</span></span>|<span data-ttu-id="6337d-191">当连接类型设置为自定义 VPN 时, 由 VPN 供应商提供的标识符。</span><span class="sxs-lookup"><span data-stu-id="6337d-191">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="6337d-192">例如: Cisco AnyConnect 使用 AnyConnect 形式的标识符。 applevpn 的标识符</span><span class="sxs-lookup"><span data-stu-id="6337d-192">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin</span></span>|
|<span data-ttu-id="6337d-193">customData</span><span class="sxs-lookup"><span data-stu-id="6337d-193">customData</span></span>|<span data-ttu-id="6337d-194">[keyValue](../resources/intune-deviceconfig-keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6337d-194">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="6337d-195">将连接类型设置为自定义 VPN 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="6337d-195">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="6337d-196">使用此字段启用 Intune 不支持的功能, 但在你的 VPN 解决方案中可用。</span><span class="sxs-lookup"><span data-stu-id="6337d-196">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="6337d-197">请与你的 VPN 供应商联系, 了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="6337d-197">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="6337d-198">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="6337d-198">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="6337d-199">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="6337d-199">customKeyValueData</span></span>|<span data-ttu-id="6337d-200">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6337d-200">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="6337d-201">将连接类型设置为自定义 VPN 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="6337d-201">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="6337d-202">使用此字段启用 Intune 不支持的功能, 但在你的 VPN 解决方案中可用。</span><span class="sxs-lookup"><span data-stu-id="6337d-202">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="6337d-203">请与你的 VPN 供应商联系, 了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="6337d-203">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="6337d-204">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="6337d-204">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="6337d-205">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="6337d-205">enableSplitTunneling</span></span>|<span data-ttu-id="6337d-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="6337d-206">Boolean</span></span>|<span data-ttu-id="6337d-207">通过 VPN 发送所有网络流量。</span><span class="sxs-lookup"><span data-stu-id="6337d-207">Send all network traffic through VPN.</span></span>|
|<span data-ttu-id="6337d-208">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6337d-208">authenticationMethod</span></span>|[<span data-ttu-id="6337d-209">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6337d-209">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="6337d-210">此 VPN 连接的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="6337d-210">Authentication method for this VPN connection.</span></span> <span data-ttu-id="6337d-211">可取值为：`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="6337d-211">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|
|<span data-ttu-id="6337d-212">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="6337d-212">enablePerApp</span></span>|<span data-ttu-id="6337d-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="6337d-213">Boolean</span></span>|<span data-ttu-id="6337d-214">将此设置为 true 将创建每个应用程序 VPN 有效负载, 以后可将其与可在最终用户的 iOS 设备上触发此 VPN 连接的应用程序相关联。</span><span class="sxs-lookup"><span data-stu-id="6337d-214">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span>|
|<span data-ttu-id="6337d-215">safariDomains</span><span class="sxs-lookup"><span data-stu-id="6337d-215">safariDomains</span></span>|<span data-ttu-id="6337d-216">String collection</span><span class="sxs-lookup"><span data-stu-id="6337d-216">String collection</span></span>|<span data-ttu-id="6337d-217">启用此 VPN 每应用程序设置时的 Safari 域。</span><span class="sxs-lookup"><span data-stu-id="6337d-217">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="6337d-218">除了与此 VPN 关联的应用程序之外, 此处指定的 Safari 域还将能够触发此 VPN 连接。</span><span class="sxs-lookup"><span data-stu-id="6337d-218">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span>|
|<span data-ttu-id="6337d-219">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="6337d-219">onDemandRules</span></span>|<span data-ttu-id="6337d-220">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="6337d-220">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="6337d-221">按需规则。</span><span class="sxs-lookup"><span data-stu-id="6337d-221">On-Demand Rules.</span></span> <span data-ttu-id="6337d-222">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="6337d-222">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="6337d-223">proxyServer</span><span class="sxs-lookup"><span data-stu-id="6337d-223">proxyServer</span></span>|[<span data-ttu-id="6337d-224">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="6337d-224">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="6337d-225">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="6337d-225">Proxy Server.</span></span>|
|<span data-ttu-id="6337d-226">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="6337d-226">optInToDeviceIdSharing</span></span>|<span data-ttu-id="6337d-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="6337d-227">Boolean</span></span>|<span data-ttu-id="6337d-228">选择将设备的 Id 共享到第三方 vpn 客户端, 以便在网络访问控制验证期间使用。</span><span class="sxs-lookup"><span data-stu-id="6337d-228">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6337d-229">关系</span><span class="sxs-lookup"><span data-stu-id="6337d-229">Relationships</span></span>
|<span data-ttu-id="6337d-230">关系</span><span class="sxs-lookup"><span data-stu-id="6337d-230">Relationship</span></span>|<span data-ttu-id="6337d-231">类型</span><span class="sxs-lookup"><span data-stu-id="6337d-231">Type</span></span>|<span data-ttu-id="6337d-232">说明</span><span class="sxs-lookup"><span data-stu-id="6337d-232">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6337d-233">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="6337d-233">groupAssignments</span></span>|<span data-ttu-id="6337d-234">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="6337d-234">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="6337d-235">设备配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="6337d-235">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="6337d-236">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6337d-236">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6337d-237">assignments</span><span class="sxs-lookup"><span data-stu-id="6337d-237">assignments</span></span>|<span data-ttu-id="6337d-238">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6337d-238">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="6337d-239">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="6337d-239">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="6337d-240">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6337d-240">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6337d-241">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="6337d-241">deviceStatuses</span></span>|<span data-ttu-id="6337d-242">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6337d-242">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="6337d-243">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="6337d-243">Device configuration installation status by device.</span></span> <span data-ttu-id="6337d-244">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6337d-244">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6337d-245">userStatuses</span><span class="sxs-lookup"><span data-stu-id="6337d-245">userStatuses</span></span>|<span data-ttu-id="6337d-246">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6337d-246">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="6337d-247">按用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="6337d-247">Device configuration installation status by user.</span></span> <span data-ttu-id="6337d-248">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6337d-248">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6337d-249">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="6337d-249">deviceStatusOverview</span></span>|[<span data-ttu-id="6337d-250">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="6337d-250">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="6337d-251">设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6337d-251">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6337d-252">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="6337d-252">userStatusOverview</span></span>|[<span data-ttu-id="6337d-253">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="6337d-253">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="6337d-254">设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6337d-254">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6337d-255">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="6337d-255">deviceSettingStateSummaries</span></span>|<span data-ttu-id="6337d-256">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6337d-256">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="6337d-257">设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6337d-257">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6337d-258">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6337d-258">JSON Representation</span></span>
<span data-ttu-id="6337d-259">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6337d-259">Here is a JSON representation of the resource.</span></span>
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



