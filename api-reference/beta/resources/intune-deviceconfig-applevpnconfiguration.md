---
title: appleVpnConfiguration 资源类型
description: Apple VPN 配置文件。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 595dee75c4c3f46e0befc16d914c988c7c1b6666
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48076034"
---
# <a name="applevpnconfiguration-resource-type"></a><span data-ttu-id="890c9-103">appleVpnConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="890c9-103">appleVpnConfiguration resource type</span></span>

<span data-ttu-id="890c9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="890c9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="890c9-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="890c9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="890c9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="890c9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="890c9-107">Apple VPN 配置文件。</span><span class="sxs-lookup"><span data-stu-id="890c9-107">Apple VPN configuration profile.</span></span>


<span data-ttu-id="890c9-108">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="890c9-108">Inherits from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="890c9-109">方法</span><span class="sxs-lookup"><span data-stu-id="890c9-109">Methods</span></span>
|<span data-ttu-id="890c9-110">方法</span><span class="sxs-lookup"><span data-stu-id="890c9-110">Method</span></span>|<span data-ttu-id="890c9-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="890c9-111">Return Type</span></span>|<span data-ttu-id="890c9-112">说明</span><span class="sxs-lookup"><span data-stu-id="890c9-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="890c9-113">列出 appleVpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="890c9-113">List appleVpnConfigurations</span></span>](../api/intune-deviceconfig-applevpnconfiguration-list.md)|<span data-ttu-id="890c9-114">[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="890c9-114">[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) collection</span></span>|<span data-ttu-id="890c9-115">列出 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="890c9-115">List properties and relationships of the [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="890c9-116">获取 appleVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="890c9-116">Get appleVpnConfiguration</span></span>](../api/intune-deviceconfig-applevpnconfiguration-get.md)|[<span data-ttu-id="890c9-117">appleVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="890c9-117">appleVpnConfiguration</span></span>](../resources/intune-deviceconfig-applevpnconfiguration.md)|<span data-ttu-id="890c9-118">读取 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="890c9-118">Read properties and relationships of the [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="890c9-119">属性</span><span class="sxs-lookup"><span data-stu-id="890c9-119">Properties</span></span>
|<span data-ttu-id="890c9-120">属性</span><span class="sxs-lookup"><span data-stu-id="890c9-120">Property</span></span>|<span data-ttu-id="890c9-121">类型</span><span class="sxs-lookup"><span data-stu-id="890c9-121">Type</span></span>|<span data-ttu-id="890c9-122">说明</span><span class="sxs-lookup"><span data-stu-id="890c9-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="890c9-123">id</span><span class="sxs-lookup"><span data-stu-id="890c9-123">id</span></span>|<span data-ttu-id="890c9-124">String</span><span class="sxs-lookup"><span data-stu-id="890c9-124">String</span></span>|<span data-ttu-id="890c9-125">实体的键。</span><span class="sxs-lookup"><span data-stu-id="890c9-125">Key of the entity.</span></span> <span data-ttu-id="890c9-126">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="890c9-126">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="890c9-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="890c9-127">lastModifiedDateTime</span></span>|<span data-ttu-id="890c9-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="890c9-128">DateTimeOffset</span></span>|<span data-ttu-id="890c9-129">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="890c9-129">DateTime the object was last modified.</span></span> <span data-ttu-id="890c9-130">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="890c9-130">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="890c9-131">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="890c9-131">roleScopeTagIds</span></span>|<span data-ttu-id="890c9-132">String 集合</span><span class="sxs-lookup"><span data-stu-id="890c9-132">String collection</span></span>|<span data-ttu-id="890c9-133">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="890c9-133">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="890c9-134">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="890c9-134">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="890c9-135">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="890c9-135">supportsScopeTags</span></span>|<span data-ttu-id="890c9-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="890c9-136">Boolean</span></span>|<span data-ttu-id="890c9-137">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="890c9-137">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="890c9-138">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="890c9-138">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="890c9-139">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="890c9-139">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="890c9-140">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="890c9-140">This property is read-only.</span></span> <span data-ttu-id="890c9-141">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="890c9-141">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="890c9-142">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="890c9-142">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="890c9-143">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="890c9-143">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="890c9-144">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="890c9-144">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="890c9-145">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="890c9-145">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="890c9-146">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="890c9-146">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="890c9-147">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="890c9-147">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="890c9-148">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="890c9-148">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="890c9-149">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="890c9-149">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="890c9-150">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="890c9-150">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="890c9-151">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="890c9-151">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="890c9-152">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="890c9-152">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="890c9-153">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="890c9-153">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="890c9-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="890c9-154">createdDateTime</span></span>|<span data-ttu-id="890c9-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="890c9-155">DateTimeOffset</span></span>|<span data-ttu-id="890c9-156">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="890c9-156">DateTime the object was created.</span></span> <span data-ttu-id="890c9-157">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="890c9-157">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="890c9-158">说明</span><span class="sxs-lookup"><span data-stu-id="890c9-158">description</span></span>|<span data-ttu-id="890c9-159">String</span><span class="sxs-lookup"><span data-stu-id="890c9-159">String</span></span>|<span data-ttu-id="890c9-160">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="890c9-160">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="890c9-161">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="890c9-161">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="890c9-162">displayName</span><span class="sxs-lookup"><span data-stu-id="890c9-162">displayName</span></span>|<span data-ttu-id="890c9-163">String</span><span class="sxs-lookup"><span data-stu-id="890c9-163">String</span></span>|<span data-ttu-id="890c9-164">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="890c9-164">Admin provided name of the device configuration.</span></span> <span data-ttu-id="890c9-165">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="890c9-165">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="890c9-166">version</span><span class="sxs-lookup"><span data-stu-id="890c9-166">version</span></span>|<span data-ttu-id="890c9-167">Int32</span><span class="sxs-lookup"><span data-stu-id="890c9-167">Int32</span></span>|<span data-ttu-id="890c9-168">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="890c9-168">Version of the device configuration.</span></span> <span data-ttu-id="890c9-169">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="890c9-169">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="890c9-170">connectionName</span><span class="sxs-lookup"><span data-stu-id="890c9-170">connectionName</span></span>|<span data-ttu-id="890c9-171">String</span><span class="sxs-lookup"><span data-stu-id="890c9-171">String</span></span>|<span data-ttu-id="890c9-172">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="890c9-172">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="890c9-173">connectionType</span><span class="sxs-lookup"><span data-stu-id="890c9-173">connectionType</span></span>|[<span data-ttu-id="890c9-174">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="890c9-174">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="890c9-175">连接类型。</span><span class="sxs-lookup"><span data-stu-id="890c9-175">Connection type.</span></span> <span data-ttu-id="890c9-176">可能的值为：、、、、、、、、、、、、、、、、、、 `ciscoAnyConnect` `pulseSecure` `f5EdgeClient` `dellSonicWallMobileConnect` `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `ciscoAnyConnectV2` `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso` `paloAltoGlobalProtectV2` `ikEv2` `alwaysOn` `microsoftTunnel` `netMotionMobility` 。</span><span class="sxs-lookup"><span data-stu-id="890c9-176">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`, `microsoftTunnel`, `netMotionMobility`.</span></span>|
|<span data-ttu-id="890c9-177">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="890c9-177">loginGroupOrDomain</span></span>|<span data-ttu-id="890c9-178">String</span><span class="sxs-lookup"><span data-stu-id="890c9-178">String</span></span>|<span data-ttu-id="890c9-179">将连接类型设置为 Dell SonicWALL Mobile 连接时的登录组或域。</span><span class="sxs-lookup"><span data-stu-id="890c9-179">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="890c9-180">role</span><span class="sxs-lookup"><span data-stu-id="890c9-180">role</span></span>|<span data-ttu-id="890c9-181">String</span><span class="sxs-lookup"><span data-stu-id="890c9-181">String</span></span>|<span data-ttu-id="890c9-182">将 "连接类型" 设置为 "脉冲安全" 时的角色。</span><span class="sxs-lookup"><span data-stu-id="890c9-182">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="890c9-183">型</span><span class="sxs-lookup"><span data-stu-id="890c9-183">realm</span></span>|<span data-ttu-id="890c9-184">String</span><span class="sxs-lookup"><span data-stu-id="890c9-184">String</span></span>|<span data-ttu-id="890c9-185">连接类型设置为脉冲安全时的领域。</span><span class="sxs-lookup"><span data-stu-id="890c9-185">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="890c9-186">服务器主板</span><span class="sxs-lookup"><span data-stu-id="890c9-186">server</span></span>|[<span data-ttu-id="890c9-187">vpnServer</span><span class="sxs-lookup"><span data-stu-id="890c9-187">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="890c9-188">网络上的 VPN 服务器。</span><span class="sxs-lookup"><span data-stu-id="890c9-188">VPN Server on the network.</span></span> <span data-ttu-id="890c9-189">请确保最终用户可以访问此网络位置。</span><span class="sxs-lookup"><span data-stu-id="890c9-189">Make sure end users can access this network location.</span></span>|
|<span data-ttu-id="890c9-190">标识符</span><span class="sxs-lookup"><span data-stu-id="890c9-190">identifier</span></span>|<span data-ttu-id="890c9-191">String</span><span class="sxs-lookup"><span data-stu-id="890c9-191">String</span></span>|<span data-ttu-id="890c9-192">当连接类型设置为自定义 VPN 时，由 VPN 供应商提供的标识符。</span><span class="sxs-lookup"><span data-stu-id="890c9-192">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="890c9-193">例如： Cisco AnyConnect 使用 AnyConnect 形式的标识符。 applevpn 的标识符</span><span class="sxs-lookup"><span data-stu-id="890c9-193">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin</span></span>|
|<span data-ttu-id="890c9-194">customData</span><span class="sxs-lookup"><span data-stu-id="890c9-194">customData</span></span>|<span data-ttu-id="890c9-195">[keyValue](../resources/intune-deviceconfig-keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="890c9-195">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="890c9-196">将连接类型设置为自定义 VPN 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="890c9-196">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="890c9-197">使用此字段启用 Intune 不支持的功能，但在你的 VPN 解决方案中可用。</span><span class="sxs-lookup"><span data-stu-id="890c9-197">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="890c9-198">请与你的 VPN 供应商联系，了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="890c9-198">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="890c9-199">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="890c9-199">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="890c9-200">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="890c9-200">customKeyValueData</span></span>|<span data-ttu-id="890c9-201">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="890c9-201">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="890c9-202">将连接类型设置为自定义 VPN 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="890c9-202">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="890c9-203">使用此字段启用 Intune 不支持的功能，但在你的 VPN 解决方案中可用。</span><span class="sxs-lookup"><span data-stu-id="890c9-203">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="890c9-204">请与你的 VPN 供应商联系，了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="890c9-204">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="890c9-205">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="890c9-205">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="890c9-206">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="890c9-206">enableSplitTunneling</span></span>|<span data-ttu-id="890c9-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="890c9-207">Boolean</span></span>|<span data-ttu-id="890c9-208">通过 VPN 发送所有网络流量。</span><span class="sxs-lookup"><span data-stu-id="890c9-208">Send all network traffic through VPN.</span></span>|
|<span data-ttu-id="890c9-209">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="890c9-209">authenticationMethod</span></span>|[<span data-ttu-id="890c9-210">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="890c9-210">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="890c9-211">此 VPN 连接的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="890c9-211">Authentication method for this VPN connection.</span></span> <span data-ttu-id="890c9-212">可取值为：`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential`、`azureAD`。</span><span class="sxs-lookup"><span data-stu-id="890c9-212">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="890c9-213">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="890c9-213">enablePerApp</span></span>|<span data-ttu-id="890c9-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="890c9-214">Boolean</span></span>|<span data-ttu-id="890c9-215">将此设置为 true 将创建每个应用程序 VPN 有效负载，以后可将其与可在最终用户的 iOS 设备上触发此 VPN 连接的应用程序相关联。</span><span class="sxs-lookup"><span data-stu-id="890c9-215">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span>|
|<span data-ttu-id="890c9-216">safariDomains</span><span class="sxs-lookup"><span data-stu-id="890c9-216">safariDomains</span></span>|<span data-ttu-id="890c9-217">String 集合</span><span class="sxs-lookup"><span data-stu-id="890c9-217">String collection</span></span>|<span data-ttu-id="890c9-218">启用此 VPN 每应用程序设置时的 Safari 域。</span><span class="sxs-lookup"><span data-stu-id="890c9-218">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="890c9-219">除了与此 VPN 关联的应用程序之外，此处指定的 Safari 域还将能够触发此 VPN 连接。</span><span class="sxs-lookup"><span data-stu-id="890c9-219">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span>|
|<span data-ttu-id="890c9-220">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="890c9-220">onDemandRules</span></span>|<span data-ttu-id="890c9-221">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="890c9-221">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="890c9-222">按需规则。</span><span class="sxs-lookup"><span data-stu-id="890c9-222">On-Demand Rules.</span></span> <span data-ttu-id="890c9-223">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="890c9-223">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="890c9-224">providerType</span><span class="sxs-lookup"><span data-stu-id="890c9-224">providerType</span></span>|[<span data-ttu-id="890c9-225">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="890c9-225">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="890c9-226">每应用 VPN 的提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="890c9-226">Provider type for per-app VPN.</span></span> <span data-ttu-id="890c9-227">可取值为：`notConfigured`、`appProxy`、`packetTunnel`。</span><span class="sxs-lookup"><span data-stu-id="890c9-227">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="890c9-228">excludedDomains</span><span class="sxs-lookup"><span data-stu-id="890c9-228">excludedDomains</span></span>|<span data-ttu-id="890c9-229">String 集合</span><span class="sxs-lookup"><span data-stu-id="890c9-229">String collection</span></span>|<span data-ttu-id="890c9-230">通过公用 internet 而不是通过 VPN 访问的域，即使已激活每个应用 VPN 也是如此</span><span class="sxs-lookup"><span data-stu-id="890c9-230">Domains that are accessed through the public internet instead of through VPN, even when per-app VPN is activated</span></span>|
|<span data-ttu-id="890c9-231">disableOnDemandUserOverride</span><span class="sxs-lookup"><span data-stu-id="890c9-231">disableOnDemandUserOverride</span></span>|<span data-ttu-id="890c9-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="890c9-232">Boolean</span></span>|<span data-ttu-id="890c9-233">切换以防止用户在 "设置" 应用中禁用自动 VPN</span><span class="sxs-lookup"><span data-stu-id="890c9-233">Toggle to prevent user from disabling automatic VPN in the Settings app</span></span>|
|<span data-ttu-id="890c9-234">proxyServer</span><span class="sxs-lookup"><span data-stu-id="890c9-234">proxyServer</span></span>|[<span data-ttu-id="890c9-235">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="890c9-235">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="890c9-236">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="890c9-236">Proxy Server.</span></span>|
|<span data-ttu-id="890c9-237">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="890c9-237">optInToDeviceIdSharing</span></span>|<span data-ttu-id="890c9-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="890c9-238">Boolean</span></span>|<span data-ttu-id="890c9-239">选择将设备的 Id 共享到第三方 vpn 客户端，以便在网络访问控制验证期间使用。</span><span class="sxs-lookup"><span data-stu-id="890c9-239">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="890c9-240">关系</span><span class="sxs-lookup"><span data-stu-id="890c9-240">Relationships</span></span>
|<span data-ttu-id="890c9-241">关系</span><span class="sxs-lookup"><span data-stu-id="890c9-241">Relationship</span></span>|<span data-ttu-id="890c9-242">类型</span><span class="sxs-lookup"><span data-stu-id="890c9-242">Type</span></span>|<span data-ttu-id="890c9-243">说明</span><span class="sxs-lookup"><span data-stu-id="890c9-243">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="890c9-244">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="890c9-244">groupAssignments</span></span>|<span data-ttu-id="890c9-245">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="890c9-245">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="890c9-246">设备配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="890c9-246">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="890c9-247">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="890c9-247">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="890c9-248">assignments</span><span class="sxs-lookup"><span data-stu-id="890c9-248">assignments</span></span>|<span data-ttu-id="890c9-249">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="890c9-249">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="890c9-250">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="890c9-250">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="890c9-251">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="890c9-251">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="890c9-252">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="890c9-252">deviceStatuses</span></span>|<span data-ttu-id="890c9-253">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="890c9-253">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="890c9-254">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="890c9-254">Device configuration installation status by device.</span></span> <span data-ttu-id="890c9-255">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="890c9-255">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="890c9-256">userStatuses</span><span class="sxs-lookup"><span data-stu-id="890c9-256">userStatuses</span></span>|<span data-ttu-id="890c9-257">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="890c9-257">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="890c9-258">按用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="890c9-258">Device configuration installation status by user.</span></span> <span data-ttu-id="890c9-259">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="890c9-259">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="890c9-260">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="890c9-260">deviceStatusOverview</span></span>|[<span data-ttu-id="890c9-261">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="890c9-261">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="890c9-262">设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="890c9-262">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="890c9-263">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="890c9-263">userStatusOverview</span></span>|[<span data-ttu-id="890c9-264">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="890c9-264">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="890c9-265">设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="890c9-265">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="890c9-266">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="890c9-266">deviceSettingStateSummaries</span></span>|<span data-ttu-id="890c9-267">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="890c9-267">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="890c9-268">设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="890c9-268">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="890c9-269">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="890c9-269">JSON Representation</span></span>
<span data-ttu-id="890c9-270">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="890c9-270">Here is a JSON representation of the resource.</span></span>
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






