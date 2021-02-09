---
title: appleVpnConfiguration 资源类型
description: Apple VPN 配置文件。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8f3f37e5a55e7fd251188505dcdab551ee8e04e8
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158756"
---
# <a name="applevpnconfiguration-resource-type"></a><span data-ttu-id="c7fe3-103">appleVpnConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="c7fe3-103">appleVpnConfiguration resource type</span></span>

<span data-ttu-id="c7fe3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7fe3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c7fe3-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c7fe3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7fe3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c7fe3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7fe3-107">Apple VPN 配置文件。</span><span class="sxs-lookup"><span data-stu-id="c7fe3-107">Apple VPN configuration profile.</span></span>


<span data-ttu-id="c7fe3-108">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c7fe3-108">Inherits from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="c7fe3-109">方法</span><span class="sxs-lookup"><span data-stu-id="c7fe3-109">Methods</span></span>
|<span data-ttu-id="c7fe3-110">方法</span><span class="sxs-lookup"><span data-stu-id="c7fe3-110">Method</span></span>|<span data-ttu-id="c7fe3-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="c7fe3-111">Return Type</span></span>|<span data-ttu-id="c7fe3-112">说明</span><span class="sxs-lookup"><span data-stu-id="c7fe3-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c7fe3-113">列出 appleVpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="c7fe3-113">List appleVpnConfigurations</span></span>](../api/intune-deviceconfig-applevpnconfiguration-list.md)|<span data-ttu-id="c7fe3-114">[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c7fe3-114">[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) collection</span></span>|<span data-ttu-id="c7fe3-115">列出 [appleVpnConfiguration 对象的属性和](../resources/intune-deviceconfig-applevpnconfiguration.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="c7fe3-115">List properties and relationships of the [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="c7fe3-116">获取 appleVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="c7fe3-116">Get appleVpnConfiguration</span></span>](../api/intune-deviceconfig-applevpnconfiguration-get.md)|[<span data-ttu-id="c7fe3-117">appleVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="c7fe3-117">appleVpnConfiguration</span></span>](../resources/intune-deviceconfig-applevpnconfiguration.md)|<span data-ttu-id="c7fe3-118">读取 [appleVpnConfiguration 对象的属性和](../resources/intune-deviceconfig-applevpnconfiguration.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="c7fe3-118">Read properties and relationships of the [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c7fe3-119">属性</span><span class="sxs-lookup"><span data-stu-id="c7fe3-119">Properties</span></span>
|<span data-ttu-id="c7fe3-120">属性</span><span class="sxs-lookup"><span data-stu-id="c7fe3-120">Property</span></span>|<span data-ttu-id="c7fe3-121">类型</span><span class="sxs-lookup"><span data-stu-id="c7fe3-121">Type</span></span>|<span data-ttu-id="c7fe3-122">说明</span><span class="sxs-lookup"><span data-stu-id="c7fe3-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7fe3-123">id</span><span class="sxs-lookup"><span data-stu-id="c7fe3-123">id</span></span>|<span data-ttu-id="c7fe3-124">String</span><span class="sxs-lookup"><span data-stu-id="c7fe3-124">String</span></span>|<span data-ttu-id="c7fe3-125">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c7fe3-125">Key of the entity.</span></span> <span data-ttu-id="c7fe3-126">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c7fe3-126">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7fe3-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c7fe3-127">lastModifiedDateTime</span></span>|<span data-ttu-id="c7fe3-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7fe3-128">DateTimeOffset</span></span>|<span data-ttu-id="c7fe3-129">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c7fe3-129">DateTime the object was last modified.</span></span> <span data-ttu-id="c7fe3-130">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c7fe3-130">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7fe3-131">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c7fe3-131">roleScopeTagIds</span></span>|<span data-ttu-id="c7fe3-132">字符串集合</span><span class="sxs-lookup"><span data-stu-id="c7fe3-132">String collection</span></span>|<span data-ttu-id="c7fe3-133">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="c7fe3-133">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c7fe3-134">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c7fe3-134">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7fe3-135">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c7fe3-135">supportsScopeTags</span></span>|<span data-ttu-id="c7fe3-136">布尔</span><span class="sxs-lookup"><span data-stu-id="c7fe3-136">Boolean</span></span>|<span data-ttu-id="c7fe3-137">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="c7fe3-137">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c7fe3-138">如果此值为 false 且实体对范围用户不可见，则不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="c7fe3-138">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c7fe3-139">这适用于在 Silverlight 中创建的旧策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="c7fe3-139">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c7fe3-140">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c7fe3-140">This property is read-only.</span></span> <span data-ttu-id="c7fe3-141">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c7fe3-141">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7fe3-142">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c7fe3-142">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="c7fe3-143">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c7fe3-143">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="c7fe3-144">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="c7fe3-144">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="c7fe3-145">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c7fe3-145">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7fe3-146">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c7fe3-146">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="c7fe3-147">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c7fe3-147">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="c7fe3-148">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="c7fe3-148">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="c7fe3-149">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c7fe3-149">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7fe3-150">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c7fe3-150">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="c7fe3-151">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c7fe3-151">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="c7fe3-152">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="c7fe3-152">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="c7fe3-153">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c7fe3-153">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7fe3-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c7fe3-154">createdDateTime</span></span>|<span data-ttu-id="c7fe3-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7fe3-155">DateTimeOffset</span></span>|<span data-ttu-id="c7fe3-156">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c7fe3-156">DateTime the object was created.</span></span> <span data-ttu-id="c7fe3-157">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c7fe3-157">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7fe3-158">说明</span><span class="sxs-lookup"><span data-stu-id="c7fe3-158">description</span></span>|<span data-ttu-id="c7fe3-159">String</span><span class="sxs-lookup"><span data-stu-id="c7fe3-159">String</span></span>|<span data-ttu-id="c7fe3-160">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="c7fe3-160">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c7fe3-161">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c7fe3-161">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7fe3-162">displayName</span><span class="sxs-lookup"><span data-stu-id="c7fe3-162">displayName</span></span>|<span data-ttu-id="c7fe3-163">String</span><span class="sxs-lookup"><span data-stu-id="c7fe3-163">String</span></span>|<span data-ttu-id="c7fe3-164">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="c7fe3-164">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c7fe3-165">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c7fe3-165">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7fe3-166">version</span><span class="sxs-lookup"><span data-stu-id="c7fe3-166">version</span></span>|<span data-ttu-id="c7fe3-167">Int32</span><span class="sxs-lookup"><span data-stu-id="c7fe3-167">Int32</span></span>|<span data-ttu-id="c7fe3-168">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="c7fe3-168">Version of the device configuration.</span></span> <span data-ttu-id="c7fe3-169">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c7fe3-169">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7fe3-170">connectionName</span><span class="sxs-lookup"><span data-stu-id="c7fe3-170">connectionName</span></span>|<span data-ttu-id="c7fe3-171">String</span><span class="sxs-lookup"><span data-stu-id="c7fe3-171">String</span></span>|<span data-ttu-id="c7fe3-172">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="c7fe3-172">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="c7fe3-173">connectionType</span><span class="sxs-lookup"><span data-stu-id="c7fe3-173">connectionType</span></span>|[<span data-ttu-id="c7fe3-174">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="c7fe3-174">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="c7fe3-175">连接类型。</span><span class="sxs-lookup"><span data-stu-id="c7fe3-175">Connection type.</span></span> <span data-ttu-id="c7fe3-176">可能的值是： `ciscoAnyConnect` ， ， ， ， ， ， ， ， `pulseSecure` ， `f5EdgeClient` `dellSonicWallMobileConnect` `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `ciscoAnyConnectV2` `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso` `paloAltoGlobalProtectV2` `ikEv2` `alwaysOn` `microsoftTunnel` `netMotionMobility` `microsoftProtect` 。</span><span class="sxs-lookup"><span data-stu-id="c7fe3-176">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`, `microsoftTunnel`, `netMotionMobility`, `microsoftProtect`.</span></span>|
|<span data-ttu-id="c7fe3-177">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="c7fe3-177">loginGroupOrDomain</span></span>|<span data-ttu-id="c7fe3-178">String</span><span class="sxs-lookup"><span data-stu-id="c7fe3-178">String</span></span>|<span data-ttu-id="c7fe3-179">连接类型设置为 Dell SonicWALL Mobile Connection 时登录组或域。</span><span class="sxs-lookup"><span data-stu-id="c7fe3-179">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="c7fe3-180">role</span><span class="sxs-lookup"><span data-stu-id="c7fe3-180">role</span></span>|<span data-ttu-id="c7fe3-181">String</span><span class="sxs-lookup"><span data-stu-id="c7fe3-181">String</span></span>|<span data-ttu-id="c7fe3-182">将连接类型设置为"脉冲安全"时的角色。</span><span class="sxs-lookup"><span data-stu-id="c7fe3-182">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="c7fe3-183">realm</span><span class="sxs-lookup"><span data-stu-id="c7fe3-183">realm</span></span>|<span data-ttu-id="c7fe3-184">String</span><span class="sxs-lookup"><span data-stu-id="c7fe3-184">String</span></span>|<span data-ttu-id="c7fe3-185">连接类型设置为"脉冲安全"时的领域。</span><span class="sxs-lookup"><span data-stu-id="c7fe3-185">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="c7fe3-186">server</span><span class="sxs-lookup"><span data-stu-id="c7fe3-186">server</span></span>|[<span data-ttu-id="c7fe3-187">vpnServer</span><span class="sxs-lookup"><span data-stu-id="c7fe3-187">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="c7fe3-188">网络 VPN 服务器。</span><span class="sxs-lookup"><span data-stu-id="c7fe3-188">VPN Server on the network.</span></span> <span data-ttu-id="c7fe3-189">确保最终用户可以访问此网络位置。</span><span class="sxs-lookup"><span data-stu-id="c7fe3-189">Make sure end users can access this network location.</span></span>|
|<span data-ttu-id="c7fe3-190">标识符</span><span class="sxs-lookup"><span data-stu-id="c7fe3-190">identifier</span></span>|<span data-ttu-id="c7fe3-191">String</span><span class="sxs-lookup"><span data-stu-id="c7fe3-191">String</span></span>|<span data-ttu-id="c7fe3-192">连接类型设置为自定义 VPN 时 VPN 供应商提供的标识符。</span><span class="sxs-lookup"><span data-stu-id="c7fe3-192">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="c7fe3-193">例如：Cisco AnyConnect 使用窗体 com.cisco.anyconnect.applevpn.plugin 的标识符</span><span class="sxs-lookup"><span data-stu-id="c7fe3-193">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin</span></span>|
|<span data-ttu-id="c7fe3-194">customData</span><span class="sxs-lookup"><span data-stu-id="c7fe3-194">customData</span></span>|<span data-ttu-id="c7fe3-195">[keyValue](../resources/intune-deviceconfig-keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c7fe3-195">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="c7fe3-196">连接类型设置为自定义 VPN 时自定义数据。</span><span class="sxs-lookup"><span data-stu-id="c7fe3-196">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="c7fe3-197">使用此字段启用 Intune 不支持但在 VPN 解决方案中提供的功能。</span><span class="sxs-lookup"><span data-stu-id="c7fe3-197">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="c7fe3-198">请联系 VPN 供应商，了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="c7fe3-198">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="c7fe3-199">此集合最多可包含 25 个元素。</span><span class="sxs-lookup"><span data-stu-id="c7fe3-199">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="c7fe3-200">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="c7fe3-200">customKeyValueData</span></span>|<span data-ttu-id="c7fe3-201">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c7fe3-201">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="c7fe3-202">连接类型设置为自定义 VPN 时自定义数据。</span><span class="sxs-lookup"><span data-stu-id="c7fe3-202">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="c7fe3-203">使用此字段启用 Intune 不支持但在 VPN 解决方案中提供的功能。</span><span class="sxs-lookup"><span data-stu-id="c7fe3-203">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="c7fe3-204">请联系 VPN 供应商，了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="c7fe3-204">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="c7fe3-205">此集合最多可包含 25 个元素。</span><span class="sxs-lookup"><span data-stu-id="c7fe3-205">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="c7fe3-206">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="c7fe3-206">enableSplitTunneling</span></span>|<span data-ttu-id="c7fe3-207">布尔</span><span class="sxs-lookup"><span data-stu-id="c7fe3-207">Boolean</span></span>|<span data-ttu-id="c7fe3-208">通过 VPN 发送所有网络流量。</span><span class="sxs-lookup"><span data-stu-id="c7fe3-208">Send all network traffic through VPN.</span></span>|
|<span data-ttu-id="c7fe3-209">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c7fe3-209">authenticationMethod</span></span>|[<span data-ttu-id="c7fe3-210">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c7fe3-210">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="c7fe3-211">此 VPN 连接的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="c7fe3-211">Authentication method for this VPN connection.</span></span> <span data-ttu-id="c7fe3-212">可取值为：`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential`、`azureAD`。</span><span class="sxs-lookup"><span data-stu-id="c7fe3-212">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="c7fe3-213">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="c7fe3-213">enablePerApp</span></span>|<span data-ttu-id="c7fe3-214">布尔</span><span class="sxs-lookup"><span data-stu-id="c7fe3-214">Boolean</span></span>|<span data-ttu-id="c7fe3-215">如果设置为 true，Per-App VPN 负载，稍后可以与在最终用户的 iOS 设备上触发此 VPN 连接的应用关联。</span><span class="sxs-lookup"><span data-stu-id="c7fe3-215">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span>|
|<span data-ttu-id="c7fe3-216">safariDomains</span><span class="sxs-lookup"><span data-stu-id="c7fe3-216">safariDomains</span></span>|<span data-ttu-id="c7fe3-217">字符串集合</span><span class="sxs-lookup"><span data-stu-id="c7fe3-217">String collection</span></span>|<span data-ttu-id="c7fe3-218">启用此 VPN（每个应用）设置时，Safari 域。</span><span class="sxs-lookup"><span data-stu-id="c7fe3-218">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="c7fe3-219">除了与此 VPN 关联的应用之外，此处指定的 Safari 域还将能够触发此 VPN 连接。</span><span class="sxs-lookup"><span data-stu-id="c7fe3-219">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span>|
|<span data-ttu-id="c7fe3-220">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="c7fe3-220">onDemandRules</span></span>|<span data-ttu-id="c7fe3-221">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c7fe3-221">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="c7fe3-222">按需规则。</span><span class="sxs-lookup"><span data-stu-id="c7fe3-222">On-Demand Rules.</span></span> <span data-ttu-id="c7fe3-223">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="c7fe3-223">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="c7fe3-224">providerType</span><span class="sxs-lookup"><span data-stu-id="c7fe3-224">providerType</span></span>|[<span data-ttu-id="c7fe3-225">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="c7fe3-225">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="c7fe3-226">每个应用 VPN 的提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="c7fe3-226">Provider type for per-app VPN.</span></span> <span data-ttu-id="c7fe3-227">可取值为：`notConfigured`、`appProxy`、`packetTunnel`。</span><span class="sxs-lookup"><span data-stu-id="c7fe3-227">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="c7fe3-228">associatedDomains</span><span class="sxs-lookup"><span data-stu-id="c7fe3-228">associatedDomains</span></span>|<span data-ttu-id="c7fe3-229">字符串集合</span><span class="sxs-lookup"><span data-stu-id="c7fe3-229">String collection</span></span>|<span data-ttu-id="c7fe3-230">关联域</span><span class="sxs-lookup"><span data-stu-id="c7fe3-230">Associated Domains</span></span>|
|<span data-ttu-id="c7fe3-231">excludedDomains</span><span class="sxs-lookup"><span data-stu-id="c7fe3-231">excludedDomains</span></span>|<span data-ttu-id="c7fe3-232">字符串集合</span><span class="sxs-lookup"><span data-stu-id="c7fe3-232">String collection</span></span>|<span data-ttu-id="c7fe3-233">通过公共 Internet 而不是 VPN 访问的域，即使已激活每应用 VPN 也是如此</span><span class="sxs-lookup"><span data-stu-id="c7fe3-233">Domains that are accessed through the public internet instead of through VPN, even when per-app VPN is activated</span></span>|
|<span data-ttu-id="c7fe3-234">disableOnDemandUserOverride</span><span class="sxs-lookup"><span data-stu-id="c7fe3-234">disableOnDemandUserOverride</span></span>|<span data-ttu-id="c7fe3-235">布尔</span><span class="sxs-lookup"><span data-stu-id="c7fe3-235">Boolean</span></span>|<span data-ttu-id="c7fe3-236">切换以阻止用户在"设置"应用中禁用自动 VPN</span><span class="sxs-lookup"><span data-stu-id="c7fe3-236">Toggle to prevent user from disabling automatic VPN in the Settings app</span></span>|
|<span data-ttu-id="c7fe3-237">proxyServer</span><span class="sxs-lookup"><span data-stu-id="c7fe3-237">proxyServer</span></span>|[<span data-ttu-id="c7fe3-238">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="c7fe3-238">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="c7fe3-239">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="c7fe3-239">Proxy Server.</span></span>|
|<span data-ttu-id="c7fe3-240">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="c7fe3-240">optInToDeviceIdSharing</span></span>|<span data-ttu-id="c7fe3-241">布尔</span><span class="sxs-lookup"><span data-stu-id="c7fe3-241">Boolean</span></span>|<span data-ttu-id="c7fe3-242">Opt-In将设备 ID 共享给第三方 vpn 客户端，以在网络访问控制验证期间使用。</span><span class="sxs-lookup"><span data-stu-id="c7fe3-242">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7fe3-243">关系</span><span class="sxs-lookup"><span data-stu-id="c7fe3-243">Relationships</span></span>
|<span data-ttu-id="c7fe3-244">关系</span><span class="sxs-lookup"><span data-stu-id="c7fe3-244">Relationship</span></span>|<span data-ttu-id="c7fe3-245">类型</span><span class="sxs-lookup"><span data-stu-id="c7fe3-245">Type</span></span>|<span data-ttu-id="c7fe3-246">说明</span><span class="sxs-lookup"><span data-stu-id="c7fe3-246">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7fe3-247">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="c7fe3-247">groupAssignments</span></span>|<span data-ttu-id="c7fe3-248">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c7fe3-248">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="c7fe3-249">设备配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="c7fe3-249">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="c7fe3-250">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c7fe3-250">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7fe3-251">assignments</span><span class="sxs-lookup"><span data-stu-id="c7fe3-251">assignments</span></span>|<span data-ttu-id="c7fe3-252">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c7fe3-252">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="c7fe3-253">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="c7fe3-253">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="c7fe3-254">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c7fe3-254">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7fe3-255">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="c7fe3-255">deviceStatuses</span></span>|<span data-ttu-id="c7fe3-256">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c7fe3-256">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="c7fe3-257">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="c7fe3-257">Device configuration installation status by device.</span></span> <span data-ttu-id="c7fe3-258">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c7fe3-258">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7fe3-259">userStatuses</span><span class="sxs-lookup"><span data-stu-id="c7fe3-259">userStatuses</span></span>|<span data-ttu-id="c7fe3-260">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c7fe3-260">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="c7fe3-261">用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="c7fe3-261">Device configuration installation status by user.</span></span> <span data-ttu-id="c7fe3-262">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c7fe3-262">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7fe3-263">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="c7fe3-263">deviceStatusOverview</span></span>|[<span data-ttu-id="c7fe3-264">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="c7fe3-264">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="c7fe3-265">设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c7fe3-265">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7fe3-266">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="c7fe3-266">userStatusOverview</span></span>|[<span data-ttu-id="c7fe3-267">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="c7fe3-267">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="c7fe3-268">设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c7fe3-268">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7fe3-269">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="c7fe3-269">deviceSettingStateSummaries</span></span>|<span data-ttu-id="c7fe3-270">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c7fe3-270">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="c7fe3-271">设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c7fe3-271">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c7fe3-272">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c7fe3-272">JSON Representation</span></span>
<span data-ttu-id="c7fe3-273">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c7fe3-273">Here is a JSON representation of the resource.</span></span>
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
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "String",
    "address": "String",
    "port": 1024
  },
  "optInToDeviceIdSharing": true
}
```




