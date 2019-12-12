---
title: 更新 iosikEv2VpnConfiguration
description: 更新 iosikEv2VpnConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0171dc8904a8a92a82f4a65aded3f62837dbcd61
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39948828"
---
# <a name="update-iosikev2vpnconfiguration"></a><span data-ttu-id="2491c-103">更新 iosikEv2VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="2491c-103">Update iosikEv2VpnConfiguration</span></span>

> <span data-ttu-id="2491c-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2491c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2491c-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2491c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2491c-106">更新[iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2491c-106">Update the properties of a [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2491c-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="2491c-107">Prerequisites</span></span>
<span data-ttu-id="2491c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2491c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2491c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2491c-110">Permission type</span></span>|<span data-ttu-id="2491c-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2491c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2491c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2491c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2491c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2491c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2491c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2491c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2491c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2491c-115">Not supported.</span></span>|
|<span data-ttu-id="2491c-116">Application</span><span class="sxs-lookup"><span data-stu-id="2491c-116">Application</span></span>|<span data-ttu-id="2491c-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2491c-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2491c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2491c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2491c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2491c-119">Request headers</span></span>
|<span data-ttu-id="2491c-120">标头</span><span class="sxs-lookup"><span data-stu-id="2491c-120">Header</span></span>|<span data-ttu-id="2491c-121">值</span><span class="sxs-lookup"><span data-stu-id="2491c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2491c-122">授权</span><span class="sxs-lookup"><span data-stu-id="2491c-122">Authorization</span></span>|<span data-ttu-id="2491c-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2491c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2491c-124">接受</span><span class="sxs-lookup"><span data-stu-id="2491c-124">Accept</span></span>|<span data-ttu-id="2491c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2491c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2491c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2491c-126">Request body</span></span>
<span data-ttu-id="2491c-127">在请求正文中，提供[iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2491c-127">In the request body, supply a JSON representation for the [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

<span data-ttu-id="2491c-128">下表显示创建[iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2491c-128">The following table shows the properties that are required when you create the [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md).</span></span>

|<span data-ttu-id="2491c-129">属性</span><span class="sxs-lookup"><span data-stu-id="2491c-129">Property</span></span>|<span data-ttu-id="2491c-130">类型</span><span class="sxs-lookup"><span data-stu-id="2491c-130">Type</span></span>|<span data-ttu-id="2491c-131">说明</span><span class="sxs-lookup"><span data-stu-id="2491c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2491c-132">id</span><span class="sxs-lookup"><span data-stu-id="2491c-132">id</span></span>|<span data-ttu-id="2491c-133">字符串</span><span class="sxs-lookup"><span data-stu-id="2491c-133">String</span></span>|<span data-ttu-id="2491c-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2491c-134">Key of the entity.</span></span> <span data-ttu-id="2491c-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2491c-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2491c-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2491c-136">lastModifiedDateTime</span></span>|<span data-ttu-id="2491c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2491c-137">DateTimeOffset</span></span>|<span data-ttu-id="2491c-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2491c-138">DateTime the object was last modified.</span></span> <span data-ttu-id="2491c-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2491c-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2491c-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2491c-140">roleScopeTagIds</span></span>|<span data-ttu-id="2491c-141">String collection</span><span class="sxs-lookup"><span data-stu-id="2491c-141">String collection</span></span>|<span data-ttu-id="2491c-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="2491c-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2491c-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2491c-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2491c-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="2491c-144">supportsScopeTags</span></span>|<span data-ttu-id="2491c-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="2491c-145">Boolean</span></span>|<span data-ttu-id="2491c-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="2491c-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2491c-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="2491c-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2491c-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="2491c-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2491c-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="2491c-149">This property is read-only.</span></span> <span data-ttu-id="2491c-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2491c-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2491c-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2491c-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="2491c-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2491c-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="2491c-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="2491c-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="2491c-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2491c-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2491c-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2491c-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="2491c-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2491c-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="2491c-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="2491c-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="2491c-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2491c-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2491c-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="2491c-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="2491c-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="2491c-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="2491c-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="2491c-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="2491c-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2491c-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2491c-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2491c-163">createdDateTime</span></span>|<span data-ttu-id="2491c-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2491c-164">DateTimeOffset</span></span>|<span data-ttu-id="2491c-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2491c-165">DateTime the object was created.</span></span> <span data-ttu-id="2491c-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2491c-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2491c-167">说明</span><span class="sxs-lookup"><span data-stu-id="2491c-167">description</span></span>|<span data-ttu-id="2491c-168">String</span><span class="sxs-lookup"><span data-stu-id="2491c-168">String</span></span>|<span data-ttu-id="2491c-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="2491c-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2491c-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2491c-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2491c-171">displayName</span><span class="sxs-lookup"><span data-stu-id="2491c-171">displayName</span></span>|<span data-ttu-id="2491c-172">String</span><span class="sxs-lookup"><span data-stu-id="2491c-172">String</span></span>|<span data-ttu-id="2491c-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="2491c-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2491c-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2491c-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2491c-175">version</span><span class="sxs-lookup"><span data-stu-id="2491c-175">version</span></span>|<span data-ttu-id="2491c-176">Int32</span><span class="sxs-lookup"><span data-stu-id="2491c-176">Int32</span></span>|<span data-ttu-id="2491c-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="2491c-177">Version of the device configuration.</span></span> <span data-ttu-id="2491c-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2491c-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2491c-179">connectionName</span><span class="sxs-lookup"><span data-stu-id="2491c-179">connectionName</span></span>|<span data-ttu-id="2491c-180">字符串</span><span class="sxs-lookup"><span data-stu-id="2491c-180">String</span></span>|<span data-ttu-id="2491c-181">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="2491c-181">Connection name displayed to the user.</span></span> <span data-ttu-id="2491c-182">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2491c-182">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2491c-183">connectionType</span><span class="sxs-lookup"><span data-stu-id="2491c-183">connectionType</span></span>|[<span data-ttu-id="2491c-184">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="2491c-184">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="2491c-185">连接类型。</span><span class="sxs-lookup"><span data-stu-id="2491c-185">Connection type.</span></span> <span data-ttu-id="2491c-186">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="2491c-186">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="2491c-187">可能的值为`ciscoAnyConnect`： `pulseSecure`、 `f5EdgeClient`、 `dellSonicWallMobileConnect` `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `ciscoAnyConnectV2` `ikEv2`、、 `zscalerPrivateAccess`、、、、、、、、、、。 `paloAltoGlobalProtect` `f5Access2018` `citrixSso` `paloAltoGlobalProtectV2`</span><span class="sxs-lookup"><span data-stu-id="2491c-187">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`.</span></span>|
|<span data-ttu-id="2491c-188">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="2491c-188">loginGroupOrDomain</span></span>|<span data-ttu-id="2491c-189">字符串</span><span class="sxs-lookup"><span data-stu-id="2491c-189">String</span></span>|<span data-ttu-id="2491c-190">将连接类型设置为 Dell SonicWALL Mobile 连接时的登录组或域。</span><span class="sxs-lookup"><span data-stu-id="2491c-190">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="2491c-191">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2491c-191">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2491c-192">role</span><span class="sxs-lookup"><span data-stu-id="2491c-192">role</span></span>|<span data-ttu-id="2491c-193">字符串</span><span class="sxs-lookup"><span data-stu-id="2491c-193">String</span></span>|<span data-ttu-id="2491c-194">将 "连接类型" 设置为 "脉冲安全" 时的角色。</span><span class="sxs-lookup"><span data-stu-id="2491c-194">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="2491c-195">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2491c-195">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2491c-196">型</span><span class="sxs-lookup"><span data-stu-id="2491c-196">realm</span></span>|<span data-ttu-id="2491c-197">字符串</span><span class="sxs-lookup"><span data-stu-id="2491c-197">String</span></span>|<span data-ttu-id="2491c-198">连接类型设置为脉冲安全时的领域。</span><span class="sxs-lookup"><span data-stu-id="2491c-198">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="2491c-199">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2491c-199">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2491c-200">服务器主板</span><span class="sxs-lookup"><span data-stu-id="2491c-200">server</span></span>|[<span data-ttu-id="2491c-201">vpnServer</span><span class="sxs-lookup"><span data-stu-id="2491c-201">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="2491c-202">网络上的 VPN 服务器。</span><span class="sxs-lookup"><span data-stu-id="2491c-202">VPN Server on the network.</span></span> <span data-ttu-id="2491c-203">请确保最终用户可以访问此网络位置。</span><span class="sxs-lookup"><span data-stu-id="2491c-203">Make sure end users can access this network location.</span></span> <span data-ttu-id="2491c-204">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2491c-204">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2491c-205">标识符</span><span class="sxs-lookup"><span data-stu-id="2491c-205">identifier</span></span>|<span data-ttu-id="2491c-206">字符串</span><span class="sxs-lookup"><span data-stu-id="2491c-206">String</span></span>|<span data-ttu-id="2491c-207">当连接类型设置为自定义 VPN 时，由 VPN 供应商提供的标识符。</span><span class="sxs-lookup"><span data-stu-id="2491c-207">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="2491c-208">例如： Cisco AnyConnect 使用从[AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)继承的 AnyConnect applevpn 的标识符。</span><span class="sxs-lookup"><span data-stu-id="2491c-208">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2491c-209">customData</span><span class="sxs-lookup"><span data-stu-id="2491c-209">customData</span></span>|<span data-ttu-id="2491c-210">[keyValue](../resources/intune-deviceconfig-keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2491c-210">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="2491c-211">将连接类型设置为自定义 VPN 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="2491c-211">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="2491c-212">使用此字段启用 Intune 不支持的功能，但在你的 VPN 解决方案中可用。</span><span class="sxs-lookup"><span data-stu-id="2491c-212">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="2491c-213">请与你的 VPN 供应商联系，了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="2491c-213">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="2491c-214">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="2491c-214">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="2491c-215">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2491c-215">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2491c-216">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="2491c-216">customKeyValueData</span></span>|<span data-ttu-id="2491c-217">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2491c-217">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="2491c-218">将连接类型设置为自定义 VPN 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="2491c-218">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="2491c-219">使用此字段启用 Intune 不支持的功能，但在你的 VPN 解决方案中可用。</span><span class="sxs-lookup"><span data-stu-id="2491c-219">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="2491c-220">请与你的 VPN 供应商联系，了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="2491c-220">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="2491c-221">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="2491c-221">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="2491c-222">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2491c-222">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2491c-223">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="2491c-223">enableSplitTunneling</span></span>|<span data-ttu-id="2491c-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="2491c-224">Boolean</span></span>|<span data-ttu-id="2491c-225">通过 VPN 发送所有网络流量。</span><span class="sxs-lookup"><span data-stu-id="2491c-225">Send all network traffic through VPN.</span></span> <span data-ttu-id="2491c-226">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2491c-226">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2491c-227">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="2491c-227">authenticationMethod</span></span>|[<span data-ttu-id="2491c-228">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="2491c-228">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="2491c-229">此 VPN 连接的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="2491c-229">Authentication method for this VPN connection.</span></span> <span data-ttu-id="2491c-230">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="2491c-230">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="2491c-231">可取值为：`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="2491c-231">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|
|<span data-ttu-id="2491c-232">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="2491c-232">enablePerApp</span></span>|<span data-ttu-id="2491c-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="2491c-233">Boolean</span></span>|<span data-ttu-id="2491c-234">将此设置为 true 将创建每个应用程序 VPN 有效负载，以后可将其与可在最终用户的 iOS 设备上触发此 VPN 连接的应用程序相关联。</span><span class="sxs-lookup"><span data-stu-id="2491c-234">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="2491c-235">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2491c-235">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2491c-236">safariDomains</span><span class="sxs-lookup"><span data-stu-id="2491c-236">safariDomains</span></span>|<span data-ttu-id="2491c-237">String collection</span><span class="sxs-lookup"><span data-stu-id="2491c-237">String collection</span></span>|<span data-ttu-id="2491c-238">启用此 VPN 每应用程序设置时的 Safari 域。</span><span class="sxs-lookup"><span data-stu-id="2491c-238">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="2491c-239">除了与此 VPN 关联的应用程序之外，此处指定的 Safari 域还将能够触发此 VPN 连接。</span><span class="sxs-lookup"><span data-stu-id="2491c-239">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="2491c-240">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2491c-240">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2491c-241">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="2491c-241">onDemandRules</span></span>|<span data-ttu-id="2491c-242">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="2491c-242">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="2491c-243">按需规则。</span><span class="sxs-lookup"><span data-stu-id="2491c-243">On-Demand Rules.</span></span> <span data-ttu-id="2491c-244">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="2491c-244">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="2491c-245">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2491c-245">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2491c-246">proxyServer</span><span class="sxs-lookup"><span data-stu-id="2491c-246">proxyServer</span></span>|[<span data-ttu-id="2491c-247">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="2491c-247">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="2491c-248">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="2491c-248">Proxy Server.</span></span> <span data-ttu-id="2491c-249">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2491c-249">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2491c-250">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="2491c-250">optInToDeviceIdSharing</span></span>|<span data-ttu-id="2491c-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="2491c-251">Boolean</span></span>|<span data-ttu-id="2491c-252">选择将设备的 Id 共享到第三方 vpn 客户端，以便在网络访问控制验证期间使用。</span><span class="sxs-lookup"><span data-stu-id="2491c-252">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="2491c-253">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2491c-253">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2491c-254">providerType</span><span class="sxs-lookup"><span data-stu-id="2491c-254">providerType</span></span>|[<span data-ttu-id="2491c-255">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="2491c-255">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="2491c-256">每应用 VPN 的提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="2491c-256">Provider type for per-app VPN.</span></span> <span data-ttu-id="2491c-257">继承自[iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="2491c-257">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span></span> <span data-ttu-id="2491c-258">可取值为：`notConfigured`、`appProxy`、`packetTunnel`。</span><span class="sxs-lookup"><span data-stu-id="2491c-258">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="2491c-259">userDomain</span><span class="sxs-lookup"><span data-stu-id="2491c-259">userDomain</span></span>|<span data-ttu-id="2491c-260">字符串</span><span class="sxs-lookup"><span data-stu-id="2491c-260">String</span></span>|<span data-ttu-id="2491c-261">仅 Zscaler。</span><span class="sxs-lookup"><span data-stu-id="2491c-261">Zscaler only.</span></span> <span data-ttu-id="2491c-262">输入一个静态域，以便在 Zscaler 应用程序中预填充 "登录" 字段。</span><span class="sxs-lookup"><span data-stu-id="2491c-262">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="2491c-263">如果保留为空，则将改用用户的 Azure Active Directory 域。</span><span class="sxs-lookup"><span data-stu-id="2491c-263">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span> <span data-ttu-id="2491c-264">继承自[iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2491c-264">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="2491c-265">strictEnforcement</span><span class="sxs-lookup"><span data-stu-id="2491c-265">strictEnforcement</span></span>|<span data-ttu-id="2491c-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="2491c-266">Boolean</span></span>|<span data-ttu-id="2491c-267">仅 Zscaler。</span><span class="sxs-lookup"><span data-stu-id="2491c-267">Zscaler only.</span></span> <span data-ttu-id="2491c-268">阻止网络流量，直到用户登录到 Zscaler 应用程序。</span><span class="sxs-lookup"><span data-stu-id="2491c-268">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="2491c-269">"True" 表示阻止流量。</span><span class="sxs-lookup"><span data-stu-id="2491c-269">"True" means traffic is blocked.</span></span> <span data-ttu-id="2491c-270">继承自[iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2491c-270">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="2491c-271">cloudName</span><span class="sxs-lookup"><span data-stu-id="2491c-271">cloudName</span></span>|<span data-ttu-id="2491c-272">字符串</span><span class="sxs-lookup"><span data-stu-id="2491c-272">String</span></span>|<span data-ttu-id="2491c-273">仅 Zscaler。</span><span class="sxs-lookup"><span data-stu-id="2491c-273">Zscaler only.</span></span> <span data-ttu-id="2491c-274">用户分配到的 Zscaler 云。</span><span class="sxs-lookup"><span data-stu-id="2491c-274">Zscaler cloud which the user is assigned to.</span></span> <span data-ttu-id="2491c-275">继承自[iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2491c-275">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="2491c-276">excludeList</span><span class="sxs-lookup"><span data-stu-id="2491c-276">excludeList</span></span>|<span data-ttu-id="2491c-277">String collection</span><span class="sxs-lookup"><span data-stu-id="2491c-277">String collection</span></span>|<span data-ttu-id="2491c-278">仅 Zscaler。</span><span class="sxs-lookup"><span data-stu-id="2491c-278">Zscaler only.</span></span> <span data-ttu-id="2491c-279">不通过 Zscaler 云发送的网络地址的列表。</span><span class="sxs-lookup"><span data-stu-id="2491c-279">List of network addresses which are not sent through the Zscaler cloud.</span></span> <span data-ttu-id="2491c-280">继承自[iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2491c-280">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="2491c-281">childSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="2491c-281">childSecurityAssociationParameters</span></span>|[<span data-ttu-id="2491c-282">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="2491c-282">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="2491c-283">子安全关联参数</span><span class="sxs-lookup"><span data-stu-id="2491c-283">Child Security Association Parameters</span></span>|
|<span data-ttu-id="2491c-284">clientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="2491c-284">clientAuthenticationType</span></span>|[<span data-ttu-id="2491c-285">vpnClientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="2491c-285">vpnClientAuthenticationType</span></span>](../resources/intune-deviceconfig-vpnclientauthenticationtype.md)|<span data-ttu-id="2491c-286">VPN 客户端将使用的客户端身份验证的类型。</span><span class="sxs-lookup"><span data-stu-id="2491c-286">Type of Client Authentication the VPN client will use.</span></span> <span data-ttu-id="2491c-287">可取值为：`userAuthentication`、`deviceAuthentication`。</span><span class="sxs-lookup"><span data-stu-id="2491c-287">Possible values are: `userAuthentication`, `deviceAuthentication`.</span></span>|
|<span data-ttu-id="2491c-288">deadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="2491c-288">deadPeerDetectionRate</span></span>|[<span data-ttu-id="2491c-289">vpnDeadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="2491c-289">vpnDeadPeerDetectionRate</span></span>](../resources/intune-deviceconfig-vpndeadpeerdetectionrate.md)|<span data-ttu-id="2491c-290">确定检查等连接是否仍处于活动状态的频率。</span><span class="sxs-lookup"><span data-stu-id="2491c-290">Determine how often to check if a peer connection is still active.</span></span> <span data-ttu-id="2491c-291">.</span><span class="sxs-lookup"><span data-stu-id="2491c-291"></span></span> <span data-ttu-id="2491c-292">可取值为：`medium`、`none`、`low`、`high`。</span><span class="sxs-lookup"><span data-stu-id="2491c-292">Possible values are: `medium`, `none`, `low`, `high`.</span></span>|
|<span data-ttu-id="2491c-293">disableMobilityAndMultihoming</span><span class="sxs-lookup"><span data-stu-id="2491c-293">disableMobilityAndMultihoming</span></span>|<span data-ttu-id="2491c-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="2491c-294">Boolean</span></span>|<span data-ttu-id="2491c-295">禁用 MOBIKE</span><span class="sxs-lookup"><span data-stu-id="2491c-295">Disable MOBIKE</span></span>|
|<span data-ttu-id="2491c-296">disableRedirect</span><span class="sxs-lookup"><span data-stu-id="2491c-296">disableRedirect</span></span>|<span data-ttu-id="2491c-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="2491c-297">Boolean</span></span>|<span data-ttu-id="2491c-298">禁用重定向</span><span class="sxs-lookup"><span data-stu-id="2491c-298">Disable Redirect</span></span>|
|<span data-ttu-id="2491c-299">enableCertificateRevocationCheck</span><span class="sxs-lookup"><span data-stu-id="2491c-299">enableCertificateRevocationCheck</span></span>|<span data-ttu-id="2491c-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="2491c-300">Boolean</span></span>|<span data-ttu-id="2491c-301">启用尽力吊销检查;服务器响应超时不会导致它失败</span><span class="sxs-lookup"><span data-stu-id="2491c-301">Enables a best-effort revocation check; server response timeouts will not cause it to fail</span></span>|
|<span data-ttu-id="2491c-302">enableEAP</span><span class="sxs-lookup"><span data-stu-id="2491c-302">enableEAP</span></span>|<span data-ttu-id="2491c-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="2491c-303">Boolean</span></span>|<span data-ttu-id="2491c-304">启用仅 EAP 身份验证</span><span class="sxs-lookup"><span data-stu-id="2491c-304">Enables EAP only authentication</span></span>|
|<span data-ttu-id="2491c-305">enablePerfectForwardSecrecy</span><span class="sxs-lookup"><span data-stu-id="2491c-305">enablePerfectForwardSecrecy</span></span>|<span data-ttu-id="2491c-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="2491c-306">Boolean</span></span>|<span data-ttu-id="2491c-307">启用完全向前保密（PFS）。</span><span class="sxs-lookup"><span data-stu-id="2491c-307">Enable Perfect Forward Secrecy (PFS).</span></span>|
|<span data-ttu-id="2491c-308">enableUseInternalSubnetAttributes</span><span class="sxs-lookup"><span data-stu-id="2491c-308">enableUseInternalSubnetAttributes</span></span>|<span data-ttu-id="2491c-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="2491c-309">Boolean</span></span>|<span data-ttu-id="2491c-310">启用 "使用内部子网属性"。</span><span class="sxs-lookup"><span data-stu-id="2491c-310">Enable Use Internal Subnet Attributes.</span></span>|
|<span data-ttu-id="2491c-311">localIdentifier</span><span class="sxs-lookup"><span data-stu-id="2491c-311">localIdentifier</span></span>|[<span data-ttu-id="2491c-312">vpnLocalIdentifier</span><span class="sxs-lookup"><span data-stu-id="2491c-312">vpnLocalIdentifier</span></span>](../resources/intune-deviceconfig-vpnlocalidentifier.md)|<span data-ttu-id="2491c-313">标识尝试通过 VPN 连接的客户端的方法。</span><span class="sxs-lookup"><span data-stu-id="2491c-313">Method of identifying the client that is trying to connect via VPN.</span></span> <span data-ttu-id="2491c-314">.</span><span class="sxs-lookup"><span data-stu-id="2491c-314"></span></span> <span data-ttu-id="2491c-315">可取值为：`deviceFQDN`、`empty`、`clientCertificateSubjectName`。</span><span class="sxs-lookup"><span data-stu-id="2491c-315">Possible values are: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span></span>|
|<span data-ttu-id="2491c-316">remoteIdentifier</span><span class="sxs-lookup"><span data-stu-id="2491c-316">remoteIdentifier</span></span>|<span data-ttu-id="2491c-317">字符串</span><span class="sxs-lookup"><span data-stu-id="2491c-317">String</span></span>|<span data-ttu-id="2491c-318">IKEv2 服务器的地址。</span><span class="sxs-lookup"><span data-stu-id="2491c-318">Address of the IKEv2 server.</span></span> <span data-ttu-id="2491c-319">必须是 FQDN、UserFQDN、网络地址或 ASN1DN</span><span class="sxs-lookup"><span data-stu-id="2491c-319">Must be a FQDN, UserFQDN, network address, or ASN1DN</span></span>|
|<span data-ttu-id="2491c-320">securityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="2491c-320">securityAssociationParameters</span></span>|[<span data-ttu-id="2491c-321">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="2491c-321">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="2491c-322">安全关联参数</span><span class="sxs-lookup"><span data-stu-id="2491c-322">Security Association Parameters</span></span>|
|<span data-ttu-id="2491c-323">serverCertificateCommonName</span><span class="sxs-lookup"><span data-stu-id="2491c-323">serverCertificateCommonName</span></span>|<span data-ttu-id="2491c-324">字符串</span><span class="sxs-lookup"><span data-stu-id="2491c-324">String</span></span>|<span data-ttu-id="2491c-325">服务器身份验证中使用的 IKEv2 服务器证书的公用名</span><span class="sxs-lookup"><span data-stu-id="2491c-325">Common name of the IKEv2 Server Certificate used in Server Authentication</span></span>|
|<span data-ttu-id="2491c-326">serverCertificateIssuerCommonName</span><span class="sxs-lookup"><span data-stu-id="2491c-326">serverCertificateIssuerCommonName</span></span>|<span data-ttu-id="2491c-327">字符串</span><span class="sxs-lookup"><span data-stu-id="2491c-327">String</span></span>|<span data-ttu-id="2491c-328">身份验证中使用的 IKEv2 服务器证书颁发者的颁发者公用名称</span><span class="sxs-lookup"><span data-stu-id="2491c-328">Issuer Common name of the IKEv2 Server Certificate issuer used in Authentication</span></span>|
|<span data-ttu-id="2491c-329">serverCertificateType</span><span class="sxs-lookup"><span data-stu-id="2491c-329">serverCertificateType</span></span>|[<span data-ttu-id="2491c-330">vpnServerCertificateType</span><span class="sxs-lookup"><span data-stu-id="2491c-330">vpnServerCertificateType</span></span>](../resources/intune-deviceconfig-vpnservercertificatetype.md)|<span data-ttu-id="2491c-331">VPN 服务器将提供给 VPN 客户端进行身份验证的证书类型。</span><span class="sxs-lookup"><span data-stu-id="2491c-331">The type of certificate the VPN server will present to the VPN client for authentication.</span></span> <span data-ttu-id="2491c-332">可取值为：`rsa`、`ecdsa256`、`ecdsa384`、`ecdsa521`。</span><span class="sxs-lookup"><span data-stu-id="2491c-332">Possible values are: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span></span>|
|<span data-ttu-id="2491c-333">sharedSecret</span><span class="sxs-lookup"><span data-stu-id="2491c-333">sharedSecret</span></span>|<span data-ttu-id="2491c-334">字符串</span><span class="sxs-lookup"><span data-stu-id="2491c-334">String</span></span>|<span data-ttu-id="2491c-335">在选择共享密钥身份验证时使用</span><span class="sxs-lookup"><span data-stu-id="2491c-335">Used when Shared Secret Authentication is selected</span></span>|
|<span data-ttu-id="2491c-336">tlsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="2491c-336">tlsMaximumVersion</span></span>|<span data-ttu-id="2491c-337">字符串</span><span class="sxs-lookup"><span data-stu-id="2491c-337">String</span></span>|<span data-ttu-id="2491c-338">要与 EAP-TLS 身份验证一起使用的最大 TLS 版本</span><span class="sxs-lookup"><span data-stu-id="2491c-338">The maximum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="2491c-339">tlsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="2491c-339">tlsMinimumVersion</span></span>|<span data-ttu-id="2491c-340">字符串</span><span class="sxs-lookup"><span data-stu-id="2491c-340">String</span></span>|<span data-ttu-id="2491c-341">与 EAP-TLS 身份验证一起使用的最小 TLS 版本</span><span class="sxs-lookup"><span data-stu-id="2491c-341">The minimum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="2491c-342">allowDefaultSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="2491c-342">allowDefaultSecurityAssociationParameters</span></span>|<span data-ttu-id="2491c-343">Boolean</span><span class="sxs-lookup"><span data-stu-id="2491c-343">Boolean</span></span>|<span data-ttu-id="2491c-344">允许使用安全关联参数，具体方法是将所有参数设置为设备的默认值，除非明确指定。</span><span class="sxs-lookup"><span data-stu-id="2491c-344">Allows the use of security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="2491c-345">allowDefaultChildSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="2491c-345">allowDefaultChildSecurityAssociationParameters</span></span>|<span data-ttu-id="2491c-346">Boolean</span><span class="sxs-lookup"><span data-stu-id="2491c-346">Boolean</span></span>|<span data-ttu-id="2491c-347">允许使用子安全关联参数，具体方法是将所有参数设置为设备的默认值，除非明确指定。</span><span class="sxs-lookup"><span data-stu-id="2491c-347">Allows the use of child security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|



## <a name="response"></a><span data-ttu-id="2491c-348">响应</span><span class="sxs-lookup"><span data-stu-id="2491c-348">Response</span></span>
<span data-ttu-id="2491c-349">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2491c-349">If successful, this method returns a `200 OK` response code and an updated [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2491c-350">示例</span><span class="sxs-lookup"><span data-stu-id="2491c-350">Example</span></span>

### <a name="request"></a><span data-ttu-id="2491c-351">请求</span><span class="sxs-lookup"><span data-stu-id="2491c-351">Request</span></span>
<span data-ttu-id="2491c-352">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2491c-352">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 4232

{
  "@odata.type": "#microsoft.graph.iosikEv2VpnConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "connectionName": "Connection Name value",
  "connectionType": "pulseSecure",
  "loginGroupOrDomain": "Login Group Or Domain value",
  "role": "Role value",
  "realm": "Realm value",
  "server": {
    "@odata.type": "microsoft.graph.vpnServer",
    "description": "Description value",
    "address": "Address value",
    "isDefaultServer": true
  },
  "identifier": "Identifier value",
  "customData": [
    {
      "@odata.type": "microsoft.graph.keyValue",
      "key": "Key value",
      "value": "Value value"
    }
  ],
  "customKeyValueData": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "enableSplitTunneling": true,
  "authenticationMethod": "usernameAndPassword",
  "enablePerApp": true,
  "safariDomains": [
    "Safari Domains value"
  ],
  "onDemandRules": [
    {
      "@odata.type": "microsoft.graph.vpnOnDemandRule",
      "ssids": [
        "Ssids value"
      ],
      "dnsSearchDomains": [
        "Dns Search Domains value"
      ],
      "probeUrl": "https://example.com/probeUrl/",
      "action": "evaluateConnection",
      "domainAction": "neverConnect",
      "domains": [
        "Domains value"
      ],
      "probeRequiredUrl": "https://example.com/probeRequiredUrl/"
    }
  ],
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4
  },
  "optInToDeviceIdSharing": true,
  "providerType": "appProxy",
  "userDomain": "User Domain value",
  "strictEnforcement": true,
  "cloudName": "Cloud Name value",
  "excludeList": [
    "Exclude List value"
  ],
  "childSecurityAssociationParameters": {
    "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters",
    "securityEncryptionAlgorithm": "des",
    "securityIntegrityAlgorithm": "sha1_96",
    "securityDiffieHellmanGroup": 10,
    "lifetimeInMinutes": 1
  },
  "clientAuthenticationType": "deviceAuthentication",
  "deadPeerDetectionRate": "none",
  "disableMobilityAndMultihoming": true,
  "disableRedirect": true,
  "enableCertificateRevocationCheck": true,
  "enableEAP": true,
  "enablePerfectForwardSecrecy": true,
  "enableUseInternalSubnetAttributes": true,
  "localIdentifier": "empty",
  "remoteIdentifier": "Remote Identifier value",
  "securityAssociationParameters": {
    "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters",
    "securityEncryptionAlgorithm": "des",
    "securityIntegrityAlgorithm": "sha1_96",
    "securityDiffieHellmanGroup": 10,
    "lifetimeInMinutes": 1
  },
  "serverCertificateCommonName": "Server Certificate Common Name value",
  "serverCertificateIssuerCommonName": "Server Certificate Issuer Common Name value",
  "serverCertificateType": "ecdsa256",
  "sharedSecret": "Shared Secret value",
  "tlsMaximumVersion": "Tls Maximum Version value",
  "tlsMinimumVersion": "Tls Minimum Version value",
  "allowDefaultSecurityAssociationParameters": true,
  "allowDefaultChildSecurityAssociationParameters": true
}
```

### <a name="response"></a><span data-ttu-id="2491c-353">响应</span><span class="sxs-lookup"><span data-stu-id="2491c-353">Response</span></span>
<span data-ttu-id="2491c-p139">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2491c-p139">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4404

{
  "@odata.type": "#microsoft.graph.iosikEv2VpnConfiguration",
  "id": "b87b0327-0327-b87b-2703-7bb827037bb8",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "connectionName": "Connection Name value",
  "connectionType": "pulseSecure",
  "loginGroupOrDomain": "Login Group Or Domain value",
  "role": "Role value",
  "realm": "Realm value",
  "server": {
    "@odata.type": "microsoft.graph.vpnServer",
    "description": "Description value",
    "address": "Address value",
    "isDefaultServer": true
  },
  "identifier": "Identifier value",
  "customData": [
    {
      "@odata.type": "microsoft.graph.keyValue",
      "key": "Key value",
      "value": "Value value"
    }
  ],
  "customKeyValueData": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "enableSplitTunneling": true,
  "authenticationMethod": "usernameAndPassword",
  "enablePerApp": true,
  "safariDomains": [
    "Safari Domains value"
  ],
  "onDemandRules": [
    {
      "@odata.type": "microsoft.graph.vpnOnDemandRule",
      "ssids": [
        "Ssids value"
      ],
      "dnsSearchDomains": [
        "Dns Search Domains value"
      ],
      "probeUrl": "https://example.com/probeUrl/",
      "action": "evaluateConnection",
      "domainAction": "neverConnect",
      "domains": [
        "Domains value"
      ],
      "probeRequiredUrl": "https://example.com/probeRequiredUrl/"
    }
  ],
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4
  },
  "optInToDeviceIdSharing": true,
  "providerType": "appProxy",
  "userDomain": "User Domain value",
  "strictEnforcement": true,
  "cloudName": "Cloud Name value",
  "excludeList": [
    "Exclude List value"
  ],
  "childSecurityAssociationParameters": {
    "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters",
    "securityEncryptionAlgorithm": "des",
    "securityIntegrityAlgorithm": "sha1_96",
    "securityDiffieHellmanGroup": 10,
    "lifetimeInMinutes": 1
  },
  "clientAuthenticationType": "deviceAuthentication",
  "deadPeerDetectionRate": "none",
  "disableMobilityAndMultihoming": true,
  "disableRedirect": true,
  "enableCertificateRevocationCheck": true,
  "enableEAP": true,
  "enablePerfectForwardSecrecy": true,
  "enableUseInternalSubnetAttributes": true,
  "localIdentifier": "empty",
  "remoteIdentifier": "Remote Identifier value",
  "securityAssociationParameters": {
    "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters",
    "securityEncryptionAlgorithm": "des",
    "securityIntegrityAlgorithm": "sha1_96",
    "securityDiffieHellmanGroup": 10,
    "lifetimeInMinutes": 1
  },
  "serverCertificateCommonName": "Server Certificate Common Name value",
  "serverCertificateIssuerCommonName": "Server Certificate Issuer Common Name value",
  "serverCertificateType": "ecdsa256",
  "sharedSecret": "Shared Secret value",
  "tlsMaximumVersion": "Tls Maximum Version value",
  "tlsMinimumVersion": "Tls Minimum Version value",
  "allowDefaultSecurityAssociationParameters": true,
  "allowDefaultChildSecurityAssociationParameters": true
}
```





