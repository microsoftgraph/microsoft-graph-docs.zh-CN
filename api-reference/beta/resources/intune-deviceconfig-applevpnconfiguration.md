---
title: appleVpnConfiguration 资源类型
description: Apple VPN 配置文件。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 52f99c4037dd0b3884f57f628bdbf6e883ccd49a
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/18/2020
ms.locfileid: "46790446"
---
# <a name="applevpnconfiguration-resource-type"></a><span data-ttu-id="0fa59-103">appleVpnConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="0fa59-103">appleVpnConfiguration resource type</span></span>

<span data-ttu-id="0fa59-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0fa59-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0fa59-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0fa59-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0fa59-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0fa59-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0fa59-107">Apple VPN 配置文件。</span><span class="sxs-lookup"><span data-stu-id="0fa59-107">Apple VPN configuration profile.</span></span>


<span data-ttu-id="0fa59-108">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0fa59-108">Inherits from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="0fa59-109">方法</span><span class="sxs-lookup"><span data-stu-id="0fa59-109">Methods</span></span>
|<span data-ttu-id="0fa59-110">方法</span><span class="sxs-lookup"><span data-stu-id="0fa59-110">Method</span></span>|<span data-ttu-id="0fa59-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="0fa59-111">Return Type</span></span>|<span data-ttu-id="0fa59-112">说明</span><span class="sxs-lookup"><span data-stu-id="0fa59-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0fa59-113">列出 appleVpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="0fa59-113">List appleVpnConfigurations</span></span>](../api/intune-deviceconfig-applevpnconfiguration-list.md)|<span data-ttu-id="0fa59-114">[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0fa59-114">[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) collection</span></span>|<span data-ttu-id="0fa59-115">列出 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0fa59-115">List properties and relationships of the [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="0fa59-116">获取 appleVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="0fa59-116">Get appleVpnConfiguration</span></span>](../api/intune-deviceconfig-applevpnconfiguration-get.md)|[<span data-ttu-id="0fa59-117">appleVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="0fa59-117">appleVpnConfiguration</span></span>](../resources/intune-deviceconfig-applevpnconfiguration.md)|<span data-ttu-id="0fa59-118">读取 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0fa59-118">Read properties and relationships of the [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0fa59-119">属性</span><span class="sxs-lookup"><span data-stu-id="0fa59-119">Properties</span></span>
|<span data-ttu-id="0fa59-120">属性</span><span class="sxs-lookup"><span data-stu-id="0fa59-120">Property</span></span>|<span data-ttu-id="0fa59-121">类型</span><span class="sxs-lookup"><span data-stu-id="0fa59-121">Type</span></span>|<span data-ttu-id="0fa59-122">说明</span><span class="sxs-lookup"><span data-stu-id="0fa59-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0fa59-123">id</span><span class="sxs-lookup"><span data-stu-id="0fa59-123">id</span></span>|<span data-ttu-id="0fa59-124">String</span><span class="sxs-lookup"><span data-stu-id="0fa59-124">String</span></span>|<span data-ttu-id="0fa59-125">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0fa59-125">Key of the entity.</span></span> <span data-ttu-id="0fa59-126">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0fa59-126">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0fa59-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0fa59-127">lastModifiedDateTime</span></span>|<span data-ttu-id="0fa59-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0fa59-128">DateTimeOffset</span></span>|<span data-ttu-id="0fa59-129">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0fa59-129">DateTime the object was last modified.</span></span> <span data-ttu-id="0fa59-130">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0fa59-130">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0fa59-131">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0fa59-131">roleScopeTagIds</span></span>|<span data-ttu-id="0fa59-132">字符串集合</span><span class="sxs-lookup"><span data-stu-id="0fa59-132">String collection</span></span>|<span data-ttu-id="0fa59-133">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="0fa59-133">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0fa59-134">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0fa59-134">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0fa59-135">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0fa59-135">supportsScopeTags</span></span>|<span data-ttu-id="0fa59-136">布尔值</span><span class="sxs-lookup"><span data-stu-id="0fa59-136">Boolean</span></span>|<span data-ttu-id="0fa59-137">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="0fa59-137">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0fa59-138">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="0fa59-138">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0fa59-139">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="0fa59-139">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0fa59-140">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="0fa59-140">This property is read-only.</span></span> <span data-ttu-id="0fa59-141">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0fa59-141">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0fa59-142">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0fa59-142">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="0fa59-143">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0fa59-143">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="0fa59-144">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="0fa59-144">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="0fa59-145">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0fa59-145">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0fa59-146">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0fa59-146">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="0fa59-147">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0fa59-147">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="0fa59-148">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="0fa59-148">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="0fa59-149">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0fa59-149">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0fa59-150">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0fa59-150">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="0fa59-151">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0fa59-151">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="0fa59-152">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="0fa59-152">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="0fa59-153">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0fa59-153">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0fa59-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0fa59-154">createdDateTime</span></span>|<span data-ttu-id="0fa59-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0fa59-155">DateTimeOffset</span></span>|<span data-ttu-id="0fa59-156">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0fa59-156">DateTime the object was created.</span></span> <span data-ttu-id="0fa59-157">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0fa59-157">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0fa59-158">description</span><span class="sxs-lookup"><span data-stu-id="0fa59-158">description</span></span>|<span data-ttu-id="0fa59-159">String</span><span class="sxs-lookup"><span data-stu-id="0fa59-159">String</span></span>|<span data-ttu-id="0fa59-160">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="0fa59-160">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0fa59-161">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0fa59-161">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0fa59-162">displayName</span><span class="sxs-lookup"><span data-stu-id="0fa59-162">displayName</span></span>|<span data-ttu-id="0fa59-163">String</span><span class="sxs-lookup"><span data-stu-id="0fa59-163">String</span></span>|<span data-ttu-id="0fa59-164">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="0fa59-164">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0fa59-165">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0fa59-165">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0fa59-166">version</span><span class="sxs-lookup"><span data-stu-id="0fa59-166">version</span></span>|<span data-ttu-id="0fa59-167">Int32</span><span class="sxs-lookup"><span data-stu-id="0fa59-167">Int32</span></span>|<span data-ttu-id="0fa59-168">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="0fa59-168">Version of the device configuration.</span></span> <span data-ttu-id="0fa59-169">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0fa59-169">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0fa59-170">connectionName</span><span class="sxs-lookup"><span data-stu-id="0fa59-170">connectionName</span></span>|<span data-ttu-id="0fa59-171">String</span><span class="sxs-lookup"><span data-stu-id="0fa59-171">String</span></span>|<span data-ttu-id="0fa59-172">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="0fa59-172">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="0fa59-173">connectionType</span><span class="sxs-lookup"><span data-stu-id="0fa59-173">connectionType</span></span>|[<span data-ttu-id="0fa59-174">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="0fa59-174">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="0fa59-175">连接类型。</span><span class="sxs-lookup"><span data-stu-id="0fa59-175">Connection type.</span></span> <span data-ttu-id="0fa59-176">可能的值为：、、、、、、、、、、、、、、、、、、 `ciscoAnyConnect` `pulseSecure` `f5EdgeClient` `dellSonicWallMobileConnect` `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `ciscoAnyConnectV2` `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso` `paloAltoGlobalProtectV2` `ikEv2` `alwaysOn` `microsoftTunnel` `netMotionMobility` 。</span><span class="sxs-lookup"><span data-stu-id="0fa59-176">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`, `microsoftTunnel`, `netMotionMobility`.</span></span>|
|<span data-ttu-id="0fa59-177">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="0fa59-177">loginGroupOrDomain</span></span>|<span data-ttu-id="0fa59-178">String</span><span class="sxs-lookup"><span data-stu-id="0fa59-178">String</span></span>|<span data-ttu-id="0fa59-179">将连接类型设置为 Dell SonicWALL Mobile 连接时的登录组或域。</span><span class="sxs-lookup"><span data-stu-id="0fa59-179">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="0fa59-180">role</span><span class="sxs-lookup"><span data-stu-id="0fa59-180">role</span></span>|<span data-ttu-id="0fa59-181">String</span><span class="sxs-lookup"><span data-stu-id="0fa59-181">String</span></span>|<span data-ttu-id="0fa59-182">将 "连接类型" 设置为 "脉冲安全" 时的角色。</span><span class="sxs-lookup"><span data-stu-id="0fa59-182">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="0fa59-183">型</span><span class="sxs-lookup"><span data-stu-id="0fa59-183">realm</span></span>|<span data-ttu-id="0fa59-184">String</span><span class="sxs-lookup"><span data-stu-id="0fa59-184">String</span></span>|<span data-ttu-id="0fa59-185">连接类型设置为脉冲安全时的领域。</span><span class="sxs-lookup"><span data-stu-id="0fa59-185">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="0fa59-186">服务器主板</span><span class="sxs-lookup"><span data-stu-id="0fa59-186">server</span></span>|[<span data-ttu-id="0fa59-187">vpnServer</span><span class="sxs-lookup"><span data-stu-id="0fa59-187">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="0fa59-188">网络上的 VPN 服务器。</span><span class="sxs-lookup"><span data-stu-id="0fa59-188">VPN Server on the network.</span></span> <span data-ttu-id="0fa59-189">请确保最终用户可以访问此网络位置。</span><span class="sxs-lookup"><span data-stu-id="0fa59-189">Make sure end users can access this network location.</span></span>|
|<span data-ttu-id="0fa59-190">标识符</span><span class="sxs-lookup"><span data-stu-id="0fa59-190">identifier</span></span>|<span data-ttu-id="0fa59-191">String</span><span class="sxs-lookup"><span data-stu-id="0fa59-191">String</span></span>|<span data-ttu-id="0fa59-192">当连接类型设置为自定义 VPN 时，由 VPN 供应商提供的标识符。</span><span class="sxs-lookup"><span data-stu-id="0fa59-192">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="0fa59-193">例如： Cisco AnyConnect 使用 AnyConnect 形式的标识符。 applevpn 的标识符</span><span class="sxs-lookup"><span data-stu-id="0fa59-193">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin</span></span>|
|<span data-ttu-id="0fa59-194">customData</span><span class="sxs-lookup"><span data-stu-id="0fa59-194">customData</span></span>|<span data-ttu-id="0fa59-195">[keyValue](../resources/intune-deviceconfig-keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0fa59-195">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="0fa59-196">将连接类型设置为自定义 VPN 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="0fa59-196">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="0fa59-197">使用此字段启用 Intune 不支持的功能，但在你的 VPN 解决方案中可用。</span><span class="sxs-lookup"><span data-stu-id="0fa59-197">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="0fa59-198">请与你的 VPN 供应商联系，了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="0fa59-198">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="0fa59-199">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="0fa59-199">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="0fa59-200">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="0fa59-200">customKeyValueData</span></span>|<span data-ttu-id="0fa59-201">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0fa59-201">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="0fa59-202">将连接类型设置为自定义 VPN 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="0fa59-202">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="0fa59-203">使用此字段启用 Intune 不支持的功能，但在你的 VPN 解决方案中可用。</span><span class="sxs-lookup"><span data-stu-id="0fa59-203">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="0fa59-204">请与你的 VPN 供应商联系，了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="0fa59-204">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="0fa59-205">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="0fa59-205">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="0fa59-206">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="0fa59-206">enableSplitTunneling</span></span>|<span data-ttu-id="0fa59-207">布尔值</span><span class="sxs-lookup"><span data-stu-id="0fa59-207">Boolean</span></span>|<span data-ttu-id="0fa59-208">通过 VPN 发送所有网络流量。</span><span class="sxs-lookup"><span data-stu-id="0fa59-208">Send all network traffic through VPN.</span></span>|
|<span data-ttu-id="0fa59-209">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0fa59-209">authenticationMethod</span></span>|[<span data-ttu-id="0fa59-210">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0fa59-210">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="0fa59-211">此 VPN 连接的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="0fa59-211">Authentication method for this VPN connection.</span></span> <span data-ttu-id="0fa59-212">可取值为：`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential`、`azureAD`。</span><span class="sxs-lookup"><span data-stu-id="0fa59-212">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="0fa59-213">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="0fa59-213">enablePerApp</span></span>|<span data-ttu-id="0fa59-214">布尔值</span><span class="sxs-lookup"><span data-stu-id="0fa59-214">Boolean</span></span>|<span data-ttu-id="0fa59-215">将此设置为 true 将创建每个应用程序 VPN 有效负载，以后可将其与可在最终用户的 iOS 设备上触发此 VPN 连接的应用程序相关联。</span><span class="sxs-lookup"><span data-stu-id="0fa59-215">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span>|
|<span data-ttu-id="0fa59-216">safariDomains</span><span class="sxs-lookup"><span data-stu-id="0fa59-216">safariDomains</span></span>|<span data-ttu-id="0fa59-217">字符串集合</span><span class="sxs-lookup"><span data-stu-id="0fa59-217">String collection</span></span>|<span data-ttu-id="0fa59-218">启用此 VPN 每应用程序设置时的 Safari 域。</span><span class="sxs-lookup"><span data-stu-id="0fa59-218">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="0fa59-219">除了与此 VPN 关联的应用程序之外，此处指定的 Safari 域还将能够触发此 VPN 连接。</span><span class="sxs-lookup"><span data-stu-id="0fa59-219">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span>|
|<span data-ttu-id="0fa59-220">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="0fa59-220">onDemandRules</span></span>|<span data-ttu-id="0fa59-221">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0fa59-221">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="0fa59-222">按需规则。</span><span class="sxs-lookup"><span data-stu-id="0fa59-222">On-Demand Rules.</span></span> <span data-ttu-id="0fa59-223">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="0fa59-223">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="0fa59-224">providerType</span><span class="sxs-lookup"><span data-stu-id="0fa59-224">providerType</span></span>|[<span data-ttu-id="0fa59-225">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="0fa59-225">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="0fa59-226">每应用 VPN 的提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="0fa59-226">Provider type for per-app VPN.</span></span> <span data-ttu-id="0fa59-227">可取值为：`notConfigured`、`appProxy`、`packetTunnel`。</span><span class="sxs-lookup"><span data-stu-id="0fa59-227">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="0fa59-228">proxyServer</span><span class="sxs-lookup"><span data-stu-id="0fa59-228">proxyServer</span></span>|[<span data-ttu-id="0fa59-229">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="0fa59-229">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="0fa59-230">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="0fa59-230">Proxy Server.</span></span>|
|<span data-ttu-id="0fa59-231">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="0fa59-231">optInToDeviceIdSharing</span></span>|<span data-ttu-id="0fa59-232">布尔值</span><span class="sxs-lookup"><span data-stu-id="0fa59-232">Boolean</span></span>|<span data-ttu-id="0fa59-233">选择将设备的 Id 共享到第三方 vpn 客户端，以便在网络访问控制验证期间使用。</span><span class="sxs-lookup"><span data-stu-id="0fa59-233">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0fa59-234">关系</span><span class="sxs-lookup"><span data-stu-id="0fa59-234">Relationships</span></span>
|<span data-ttu-id="0fa59-235">关系</span><span class="sxs-lookup"><span data-stu-id="0fa59-235">Relationship</span></span>|<span data-ttu-id="0fa59-236">类型</span><span class="sxs-lookup"><span data-stu-id="0fa59-236">Type</span></span>|<span data-ttu-id="0fa59-237">说明</span><span class="sxs-lookup"><span data-stu-id="0fa59-237">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0fa59-238">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="0fa59-238">groupAssignments</span></span>|<span data-ttu-id="0fa59-239">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0fa59-239">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="0fa59-240">设备配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="0fa59-240">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="0fa59-241">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0fa59-241">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0fa59-242">assignments</span><span class="sxs-lookup"><span data-stu-id="0fa59-242">assignments</span></span>|<span data-ttu-id="0fa59-243">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0fa59-243">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="0fa59-244">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="0fa59-244">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="0fa59-245">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0fa59-245">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0fa59-246">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="0fa59-246">deviceStatuses</span></span>|<span data-ttu-id="0fa59-247">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0fa59-247">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="0fa59-248">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="0fa59-248">Device configuration installation status by device.</span></span> <span data-ttu-id="0fa59-249">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0fa59-249">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0fa59-250">userStatuses</span><span class="sxs-lookup"><span data-stu-id="0fa59-250">userStatuses</span></span>|<span data-ttu-id="0fa59-251">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0fa59-251">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="0fa59-252">按用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="0fa59-252">Device configuration installation status by user.</span></span> <span data-ttu-id="0fa59-253">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0fa59-253">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0fa59-254">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="0fa59-254">deviceStatusOverview</span></span>|[<span data-ttu-id="0fa59-255">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="0fa59-255">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="0fa59-256">设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0fa59-256">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0fa59-257">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="0fa59-257">userStatusOverview</span></span>|[<span data-ttu-id="0fa59-258">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="0fa59-258">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="0fa59-259">设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0fa59-259">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0fa59-260">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="0fa59-260">deviceSettingStateSummaries</span></span>|<span data-ttu-id="0fa59-261">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0fa59-261">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="0fa59-262">设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0fa59-262">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0fa59-263">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0fa59-263">JSON Representation</span></span>
<span data-ttu-id="0fa59-264">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0fa59-264">Here is a JSON representation of the resource.</span></span>
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
  "providerType": "String",
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "String",
    "address": "String",
    "port": 1024
  },
  "optInToDeviceIdSharing": true
}
```



