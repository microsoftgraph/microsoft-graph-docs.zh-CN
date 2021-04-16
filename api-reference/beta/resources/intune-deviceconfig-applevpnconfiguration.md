---
title: appleVpnConfiguration 资源类型
description: Apple VPN 配置文件。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 50cecd3f7653c461371c4e938a0b296de3567628
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51864520"
---
# <a name="applevpnconfiguration-resource-type"></a><span data-ttu-id="c94db-103">appleVpnConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="c94db-103">appleVpnConfiguration resource type</span></span>

<span data-ttu-id="c94db-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c94db-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c94db-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c94db-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c94db-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c94db-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c94db-107">Apple VPN 配置文件。</span><span class="sxs-lookup"><span data-stu-id="c94db-107">Apple VPN configuration profile.</span></span>


<span data-ttu-id="c94db-108">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c94db-108">Inherits from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="c94db-109">方法</span><span class="sxs-lookup"><span data-stu-id="c94db-109">Methods</span></span>
|<span data-ttu-id="c94db-110">方法</span><span class="sxs-lookup"><span data-stu-id="c94db-110">Method</span></span>|<span data-ttu-id="c94db-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="c94db-111">Return Type</span></span>|<span data-ttu-id="c94db-112">说明</span><span class="sxs-lookup"><span data-stu-id="c94db-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c94db-113">列出 appleVpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="c94db-113">List appleVpnConfigurations</span></span>](../api/intune-deviceconfig-applevpnconfiguration-list.md)|<span data-ttu-id="c94db-114">[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c94db-114">[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) collection</span></span>|<span data-ttu-id="c94db-115">列出 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c94db-115">List properties and relationships of the [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="c94db-116">获取 appleVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="c94db-116">Get appleVpnConfiguration</span></span>](../api/intune-deviceconfig-applevpnconfiguration-get.md)|[<span data-ttu-id="c94db-117">appleVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="c94db-117">appleVpnConfiguration</span></span>](../resources/intune-deviceconfig-applevpnconfiguration.md)|<span data-ttu-id="c94db-118">读取 [appleVpnConfiguration 对象的属性和](../resources/intune-deviceconfig-applevpnconfiguration.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="c94db-118">Read properties and relationships of the [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c94db-119">属性</span><span class="sxs-lookup"><span data-stu-id="c94db-119">Properties</span></span>
|<span data-ttu-id="c94db-120">属性</span><span class="sxs-lookup"><span data-stu-id="c94db-120">Property</span></span>|<span data-ttu-id="c94db-121">类型</span><span class="sxs-lookup"><span data-stu-id="c94db-121">Type</span></span>|<span data-ttu-id="c94db-122">说明</span><span class="sxs-lookup"><span data-stu-id="c94db-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c94db-123">id</span><span class="sxs-lookup"><span data-stu-id="c94db-123">id</span></span>|<span data-ttu-id="c94db-124">String</span><span class="sxs-lookup"><span data-stu-id="c94db-124">String</span></span>|<span data-ttu-id="c94db-125">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c94db-125">Key of the entity.</span></span> <span data-ttu-id="c94db-126">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c94db-126">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c94db-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c94db-127">lastModifiedDateTime</span></span>|<span data-ttu-id="c94db-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c94db-128">DateTimeOffset</span></span>|<span data-ttu-id="c94db-129">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c94db-129">DateTime the object was last modified.</span></span> <span data-ttu-id="c94db-130">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c94db-130">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c94db-131">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c94db-131">roleScopeTagIds</span></span>|<span data-ttu-id="c94db-132">String 集合</span><span class="sxs-lookup"><span data-stu-id="c94db-132">String collection</span></span>|<span data-ttu-id="c94db-133">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="c94db-133">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c94db-134">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c94db-134">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c94db-135">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c94db-135">supportsScopeTags</span></span>|<span data-ttu-id="c94db-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="c94db-136">Boolean</span></span>|<span data-ttu-id="c94db-137">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="c94db-137">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c94db-138">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="c94db-138">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c94db-139">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="c94db-139">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c94db-140">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c94db-140">This property is read-only.</span></span> <span data-ttu-id="c94db-141">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c94db-141">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c94db-142">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c94db-142">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="c94db-143">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c94db-143">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="c94db-144">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="c94db-144">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="c94db-145">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c94db-145">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c94db-146">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c94db-146">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="c94db-147">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c94db-147">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="c94db-148">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="c94db-148">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="c94db-149">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c94db-149">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c94db-150">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c94db-150">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="c94db-151">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c94db-151">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="c94db-152">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="c94db-152">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="c94db-153">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c94db-153">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c94db-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c94db-154">createdDateTime</span></span>|<span data-ttu-id="c94db-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c94db-155">DateTimeOffset</span></span>|<span data-ttu-id="c94db-156">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c94db-156">DateTime the object was created.</span></span> <span data-ttu-id="c94db-157">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c94db-157">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c94db-158">说明</span><span class="sxs-lookup"><span data-stu-id="c94db-158">description</span></span>|<span data-ttu-id="c94db-159">String</span><span class="sxs-lookup"><span data-stu-id="c94db-159">String</span></span>|<span data-ttu-id="c94db-160">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="c94db-160">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c94db-161">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c94db-161">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c94db-162">displayName</span><span class="sxs-lookup"><span data-stu-id="c94db-162">displayName</span></span>|<span data-ttu-id="c94db-163">String</span><span class="sxs-lookup"><span data-stu-id="c94db-163">String</span></span>|<span data-ttu-id="c94db-164">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="c94db-164">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c94db-165">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c94db-165">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c94db-166">version</span><span class="sxs-lookup"><span data-stu-id="c94db-166">version</span></span>|<span data-ttu-id="c94db-167">Int32</span><span class="sxs-lookup"><span data-stu-id="c94db-167">Int32</span></span>|<span data-ttu-id="c94db-168">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="c94db-168">Version of the device configuration.</span></span> <span data-ttu-id="c94db-169">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c94db-169">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c94db-170">connectionName</span><span class="sxs-lookup"><span data-stu-id="c94db-170">connectionName</span></span>|<span data-ttu-id="c94db-171">String</span><span class="sxs-lookup"><span data-stu-id="c94db-171">String</span></span>|<span data-ttu-id="c94db-172">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="c94db-172">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="c94db-173">connectionType</span><span class="sxs-lookup"><span data-stu-id="c94db-173">connectionType</span></span>|[<span data-ttu-id="c94db-174">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="c94db-174">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="c94db-175">连接类型。</span><span class="sxs-lookup"><span data-stu-id="c94db-175">Connection type.</span></span> <span data-ttu-id="c94db-176">可能的值是 `ciscoAnyConnect` `pulseSecure` `f5EdgeClient` ：、、、、、、、、 `dellSonicWallMobileConnect` `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `ciscoAnyConnectV2` `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso` `paloAltoGlobalProtectV2` `ikEv2` `alwaysOn` `microsoftTunnel` `netMotionMobility` `microsoftProtect` 。</span><span class="sxs-lookup"><span data-stu-id="c94db-176">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`, `microsoftTunnel`, `netMotionMobility`, `microsoftProtect`.</span></span>|
|<span data-ttu-id="c94db-177">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="c94db-177">loginGroupOrDomain</span></span>|<span data-ttu-id="c94db-178">String</span><span class="sxs-lookup"><span data-stu-id="c94db-178">String</span></span>|<span data-ttu-id="c94db-179">连接类型设置为 Dell SonicWALL 移动连接时登录组或域。</span><span class="sxs-lookup"><span data-stu-id="c94db-179">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="c94db-180">role</span><span class="sxs-lookup"><span data-stu-id="c94db-180">role</span></span>|<span data-ttu-id="c94db-181">String</span><span class="sxs-lookup"><span data-stu-id="c94db-181">String</span></span>|<span data-ttu-id="c94db-182">将连接类型设置为 Pulse Secure 时的角色。</span><span class="sxs-lookup"><span data-stu-id="c94db-182">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="c94db-183">realm</span><span class="sxs-lookup"><span data-stu-id="c94db-183">realm</span></span>|<span data-ttu-id="c94db-184">String</span><span class="sxs-lookup"><span data-stu-id="c94db-184">String</span></span>|<span data-ttu-id="c94db-185">将连接类型设置为 Pulse Secure 时的领域。</span><span class="sxs-lookup"><span data-stu-id="c94db-185">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="c94db-186">server</span><span class="sxs-lookup"><span data-stu-id="c94db-186">server</span></span>|[<span data-ttu-id="c94db-187">vpnServer</span><span class="sxs-lookup"><span data-stu-id="c94db-187">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="c94db-188">VPN 服务器。</span><span class="sxs-lookup"><span data-stu-id="c94db-188">VPN Server on the network.</span></span> <span data-ttu-id="c94db-189">确保最终用户可以访问此网络位置。</span><span class="sxs-lookup"><span data-stu-id="c94db-189">Make sure end users can access this network location.</span></span>|
|<span data-ttu-id="c94db-190">标识符</span><span class="sxs-lookup"><span data-stu-id="c94db-190">identifier</span></span>|<span data-ttu-id="c94db-191">String</span><span class="sxs-lookup"><span data-stu-id="c94db-191">String</span></span>|<span data-ttu-id="c94db-192">连接类型设置为自定义 VPN 时 VPN 供应商提供的标识符。</span><span class="sxs-lookup"><span data-stu-id="c94db-192">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="c94db-193">例如：Cisco AnyConnect 使用 com.cisco.anyconnect.applevpn.plugin 形式的标识符</span><span class="sxs-lookup"><span data-stu-id="c94db-193">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin</span></span>|
|<span data-ttu-id="c94db-194">customData</span><span class="sxs-lookup"><span data-stu-id="c94db-194">customData</span></span>|<span data-ttu-id="c94db-195">[keyValue](../resources/intune-deviceconfig-keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c94db-195">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="c94db-196">连接类型设置为自定义 VPN 时自定义数据。</span><span class="sxs-lookup"><span data-stu-id="c94db-196">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="c94db-197">使用此字段启用 Intune 不支持但在 VPN 解决方案中提供的功能。</span><span class="sxs-lookup"><span data-stu-id="c94db-197">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="c94db-198">请联系 VPN 供应商，了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="c94db-198">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="c94db-199">此集合最多可包含 25 个元素。</span><span class="sxs-lookup"><span data-stu-id="c94db-199">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="c94db-200">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="c94db-200">customKeyValueData</span></span>|<span data-ttu-id="c94db-201">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c94db-201">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="c94db-202">连接类型设置为自定义 VPN 时自定义数据。</span><span class="sxs-lookup"><span data-stu-id="c94db-202">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="c94db-203">使用此字段启用 Intune 不支持但在 VPN 解决方案中提供的功能。</span><span class="sxs-lookup"><span data-stu-id="c94db-203">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="c94db-204">请联系 VPN 供应商，了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="c94db-204">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="c94db-205">此集合最多可包含 25 个元素。</span><span class="sxs-lookup"><span data-stu-id="c94db-205">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="c94db-206">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="c94db-206">enableSplitTunneling</span></span>|<span data-ttu-id="c94db-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="c94db-207">Boolean</span></span>|<span data-ttu-id="c94db-208">通过 VPN 发送所有网络流量。</span><span class="sxs-lookup"><span data-stu-id="c94db-208">Send all network traffic through VPN.</span></span>|
|<span data-ttu-id="c94db-209">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c94db-209">authenticationMethod</span></span>|[<span data-ttu-id="c94db-210">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c94db-210">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="c94db-211">此 VPN 连接的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="c94db-211">Authentication method for this VPN connection.</span></span> <span data-ttu-id="c94db-212">可取值为：`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential`、`azureAD`。</span><span class="sxs-lookup"><span data-stu-id="c94db-212">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="c94db-213">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="c94db-213">enablePerApp</span></span>|<span data-ttu-id="c94db-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="c94db-214">Boolean</span></span>|<span data-ttu-id="c94db-215">如果设置为 true，Per-App VPN 有效负载，稍后可关联到可在最终用户的 iOS 设备上触发此 VPN 连接的应用。</span><span class="sxs-lookup"><span data-stu-id="c94db-215">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span>|
|<span data-ttu-id="c94db-216">safariDomains</span><span class="sxs-lookup"><span data-stu-id="c94db-216">safariDomains</span></span>|<span data-ttu-id="c94db-217">String 集合</span><span class="sxs-lookup"><span data-stu-id="c94db-217">String collection</span></span>|<span data-ttu-id="c94db-218">启用"每个应用此 VPN"设置时，Safari 域。</span><span class="sxs-lookup"><span data-stu-id="c94db-218">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="c94db-219">除了与此 VPN 关联的应用之外，此处指定的 Safari 域还将能够触发此 VPN 连接。</span><span class="sxs-lookup"><span data-stu-id="c94db-219">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span>|
|<span data-ttu-id="c94db-220">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="c94db-220">onDemandRules</span></span>|<span data-ttu-id="c94db-221">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c94db-221">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="c94db-222">按需规则。</span><span class="sxs-lookup"><span data-stu-id="c94db-222">On-Demand Rules.</span></span> <span data-ttu-id="c94db-223">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="c94db-223">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="c94db-224">providerType</span><span class="sxs-lookup"><span data-stu-id="c94db-224">providerType</span></span>|[<span data-ttu-id="c94db-225">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="c94db-225">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="c94db-226">每个应用 VPN 的提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="c94db-226">Provider type for per-app VPN.</span></span> <span data-ttu-id="c94db-227">可取值为：`notConfigured`、`appProxy`、`packetTunnel`。</span><span class="sxs-lookup"><span data-stu-id="c94db-227">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="c94db-228">associatedDomains</span><span class="sxs-lookup"><span data-stu-id="c94db-228">associatedDomains</span></span>|<span data-ttu-id="c94db-229">String 集合</span><span class="sxs-lookup"><span data-stu-id="c94db-229">String collection</span></span>|<span data-ttu-id="c94db-230">关联的域</span><span class="sxs-lookup"><span data-stu-id="c94db-230">Associated Domains</span></span>|
|<span data-ttu-id="c94db-231">excludedDomains</span><span class="sxs-lookup"><span data-stu-id="c94db-231">excludedDomains</span></span>|<span data-ttu-id="c94db-232">String 集合</span><span class="sxs-lookup"><span data-stu-id="c94db-232">String collection</span></span>|<span data-ttu-id="c94db-233">通过公共 Internet 而不是 VPN 访问的域，即使已激活每应用 VPN 也是如此</span><span class="sxs-lookup"><span data-stu-id="c94db-233">Domains that are accessed through the public internet instead of through VPN, even when per-app VPN is activated</span></span>|
|<span data-ttu-id="c94db-234">disableOnDemandUserOverride</span><span class="sxs-lookup"><span data-stu-id="c94db-234">disableOnDemandUserOverride</span></span>|<span data-ttu-id="c94db-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="c94db-235">Boolean</span></span>|<span data-ttu-id="c94db-236">切换以阻止用户在"设置"应用中禁用自动 VPN</span><span class="sxs-lookup"><span data-stu-id="c94db-236">Toggle to prevent user from disabling automatic VPN in the Settings app</span></span>|
|<span data-ttu-id="c94db-237">disconnectOnIdle</span><span class="sxs-lookup"><span data-stu-id="c94db-237">disconnectOnIdle</span></span>|<span data-ttu-id="c94db-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="c94db-238">Boolean</span></span>|<span data-ttu-id="c94db-239">在按需连接空闲后是否断开连接</span><span class="sxs-lookup"><span data-stu-id="c94db-239">Whether to disconnect after on-demand connection idles</span></span>|
|<span data-ttu-id="c94db-240">disconnectOnIdleTimerInSeconds</span><span class="sxs-lookup"><span data-stu-id="c94db-240">disconnectOnIdleTimerInSeconds</span></span>|<span data-ttu-id="c94db-241">Int32</span><span class="sxs-lookup"><span data-stu-id="c94db-241">Int32</span></span>|<span data-ttu-id="c94db-242">断开按需连接之前要等待的时间长度（秒）。</span><span class="sxs-lookup"><span data-stu-id="c94db-242">The length of time in seconds to wait before disconnecting an on-demand connection.</span></span> <span data-ttu-id="c94db-243">有效值为 0 到 65535</span><span class="sxs-lookup"><span data-stu-id="c94db-243">Valid values 0 to 65535</span></span>|
|<span data-ttu-id="c94db-244">proxyServer</span><span class="sxs-lookup"><span data-stu-id="c94db-244">proxyServer</span></span>|[<span data-ttu-id="c94db-245">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="c94db-245">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="c94db-246">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="c94db-246">Proxy Server.</span></span>|
|<span data-ttu-id="c94db-247">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="c94db-247">optInToDeviceIdSharing</span></span>|<span data-ttu-id="c94db-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="c94db-248">Boolean</span></span>|<span data-ttu-id="c94db-249">Opt-In将设备 ID 共享给第三方 vpn 客户端，以在网络访问控制验证期间使用。</span><span class="sxs-lookup"><span data-stu-id="c94db-249">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c94db-250">关系</span><span class="sxs-lookup"><span data-stu-id="c94db-250">Relationships</span></span>
|<span data-ttu-id="c94db-251">关系</span><span class="sxs-lookup"><span data-stu-id="c94db-251">Relationship</span></span>|<span data-ttu-id="c94db-252">类型</span><span class="sxs-lookup"><span data-stu-id="c94db-252">Type</span></span>|<span data-ttu-id="c94db-253">说明</span><span class="sxs-lookup"><span data-stu-id="c94db-253">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c94db-254">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="c94db-254">groupAssignments</span></span>|<span data-ttu-id="c94db-255">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c94db-255">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="c94db-256">设备配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="c94db-256">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="c94db-257">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c94db-257">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c94db-258">assignments</span><span class="sxs-lookup"><span data-stu-id="c94db-258">assignments</span></span>|<span data-ttu-id="c94db-259">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c94db-259">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="c94db-260">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="c94db-260">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="c94db-261">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c94db-261">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c94db-262">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="c94db-262">deviceStatuses</span></span>|<span data-ttu-id="c94db-263">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c94db-263">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="c94db-264">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="c94db-264">Device configuration installation status by device.</span></span> <span data-ttu-id="c94db-265">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c94db-265">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c94db-266">userStatuses</span><span class="sxs-lookup"><span data-stu-id="c94db-266">userStatuses</span></span>|<span data-ttu-id="c94db-267">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c94db-267">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="c94db-268">用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="c94db-268">Device configuration installation status by user.</span></span> <span data-ttu-id="c94db-269">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c94db-269">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c94db-270">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="c94db-270">deviceStatusOverview</span></span>|[<span data-ttu-id="c94db-271">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="c94db-271">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="c94db-272">设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c94db-272">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c94db-273">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="c94db-273">userStatusOverview</span></span>|[<span data-ttu-id="c94db-274">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="c94db-274">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="c94db-275">设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c94db-275">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c94db-276">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="c94db-276">deviceSettingStateSummaries</span></span>|<span data-ttu-id="c94db-277">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c94db-277">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="c94db-278">设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c94db-278">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c94db-279">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c94db-279">JSON Representation</span></span>
<span data-ttu-id="c94db-280">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c94db-280">Here is a JSON representation of the resource.</span></span>
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
  "associatedDomains": [
    "String"
  ],
  "excludedDomains": [
    "String"
  ],
  "disableOnDemandUserOverride": true,
  "disconnectOnIdle": true,
  "disconnectOnIdleTimerInSeconds": 1024,
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "String",
    "address": "String",
    "port": 1024
  },
  "optInToDeviceIdSharing": true
}
```




