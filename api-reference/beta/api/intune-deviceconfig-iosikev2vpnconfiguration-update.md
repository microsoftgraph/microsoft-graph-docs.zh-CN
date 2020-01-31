---
title: 更新 iosikEv2VpnConfiguration
description: 更新 iosikEv2VpnConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bc54a9306df5c8d03bbd4fd9db969a1380cba4da
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/31/2020
ms.locfileid: "41635893"
---
# <a name="update-iosikev2vpnconfiguration"></a><span data-ttu-id="0ad46-103">更新 iosikEv2VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="0ad46-103">Update iosikEv2VpnConfiguration</span></span>

> <span data-ttu-id="0ad46-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0ad46-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ad46-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0ad46-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ad46-106">更新[iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0ad46-106">Update the properties of a [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0ad46-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="0ad46-107">Prerequisites</span></span>
<span data-ttu-id="0ad46-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0ad46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ad46-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0ad46-110">Permission type</span></span>|<span data-ttu-id="0ad46-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0ad46-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ad46-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0ad46-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0ad46-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ad46-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0ad46-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0ad46-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ad46-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0ad46-115">Not supported.</span></span>|
|<span data-ttu-id="0ad46-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0ad46-116">Application</span></span>|<span data-ttu-id="0ad46-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ad46-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ad46-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0ad46-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="0ad46-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0ad46-119">Request headers</span></span>
|<span data-ttu-id="0ad46-120">标头</span><span class="sxs-lookup"><span data-stu-id="0ad46-120">Header</span></span>|<span data-ttu-id="0ad46-121">值</span><span class="sxs-lookup"><span data-stu-id="0ad46-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ad46-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ad46-122">Authorization</span></span>|<span data-ttu-id="0ad46-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0ad46-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ad46-124">接受</span><span class="sxs-lookup"><span data-stu-id="0ad46-124">Accept</span></span>|<span data-ttu-id="0ad46-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0ad46-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ad46-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0ad46-126">Request body</span></span>
<span data-ttu-id="0ad46-127">在请求正文中，提供[iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0ad46-127">In the request body, supply a JSON representation for the [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

<span data-ttu-id="0ad46-128">下表显示创建[iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0ad46-128">The following table shows the properties that are required when you create the [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md).</span></span>

|<span data-ttu-id="0ad46-129">属性</span><span class="sxs-lookup"><span data-stu-id="0ad46-129">Property</span></span>|<span data-ttu-id="0ad46-130">类型</span><span class="sxs-lookup"><span data-stu-id="0ad46-130">Type</span></span>|<span data-ttu-id="0ad46-131">Description</span><span class="sxs-lookup"><span data-stu-id="0ad46-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ad46-132">id</span><span class="sxs-lookup"><span data-stu-id="0ad46-132">id</span></span>|<span data-ttu-id="0ad46-133">字符串</span><span class="sxs-lookup"><span data-stu-id="0ad46-133">String</span></span>|<span data-ttu-id="0ad46-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0ad46-134">Key of the entity.</span></span> <span data-ttu-id="0ad46-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ad46-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ad46-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0ad46-136">lastModifiedDateTime</span></span>|<span data-ttu-id="0ad46-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ad46-137">DateTimeOffset</span></span>|<span data-ttu-id="0ad46-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0ad46-138">DateTime the object was last modified.</span></span> <span data-ttu-id="0ad46-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ad46-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ad46-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0ad46-140">roleScopeTagIds</span></span>|<span data-ttu-id="0ad46-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="0ad46-141">String collection</span></span>|<span data-ttu-id="0ad46-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="0ad46-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0ad46-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ad46-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ad46-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0ad46-144">supportsScopeTags</span></span>|<span data-ttu-id="0ad46-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ad46-145">Boolean</span></span>|<span data-ttu-id="0ad46-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="0ad46-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0ad46-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="0ad46-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0ad46-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="0ad46-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0ad46-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="0ad46-149">This property is read-only.</span></span> <span data-ttu-id="0ad46-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ad46-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ad46-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0ad46-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="0ad46-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0ad46-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="0ad46-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="0ad46-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="0ad46-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ad46-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ad46-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0ad46-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="0ad46-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0ad46-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="0ad46-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="0ad46-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="0ad46-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ad46-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ad46-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0ad46-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="0ad46-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0ad46-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="0ad46-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="0ad46-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="0ad46-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ad46-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ad46-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0ad46-163">createdDateTime</span></span>|<span data-ttu-id="0ad46-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ad46-164">DateTimeOffset</span></span>|<span data-ttu-id="0ad46-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0ad46-165">DateTime the object was created.</span></span> <span data-ttu-id="0ad46-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ad46-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ad46-167">说明</span><span class="sxs-lookup"><span data-stu-id="0ad46-167">description</span></span>|<span data-ttu-id="0ad46-168">String</span><span class="sxs-lookup"><span data-stu-id="0ad46-168">String</span></span>|<span data-ttu-id="0ad46-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="0ad46-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0ad46-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ad46-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ad46-171">displayName</span><span class="sxs-lookup"><span data-stu-id="0ad46-171">displayName</span></span>|<span data-ttu-id="0ad46-172">String</span><span class="sxs-lookup"><span data-stu-id="0ad46-172">String</span></span>|<span data-ttu-id="0ad46-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="0ad46-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0ad46-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ad46-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ad46-175">version</span><span class="sxs-lookup"><span data-stu-id="0ad46-175">version</span></span>|<span data-ttu-id="0ad46-176">Int32</span><span class="sxs-lookup"><span data-stu-id="0ad46-176">Int32</span></span>|<span data-ttu-id="0ad46-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="0ad46-177">Version of the device configuration.</span></span> <span data-ttu-id="0ad46-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ad46-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ad46-179">connectionName</span><span class="sxs-lookup"><span data-stu-id="0ad46-179">connectionName</span></span>|<span data-ttu-id="0ad46-180">字符串</span><span class="sxs-lookup"><span data-stu-id="0ad46-180">String</span></span>|<span data-ttu-id="0ad46-181">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="0ad46-181">Connection name displayed to the user.</span></span> <span data-ttu-id="0ad46-182">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ad46-182">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0ad46-183">connectionType</span><span class="sxs-lookup"><span data-stu-id="0ad46-183">connectionType</span></span>|[<span data-ttu-id="0ad46-184">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="0ad46-184">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="0ad46-185">连接类型。</span><span class="sxs-lookup"><span data-stu-id="0ad46-185">Connection type.</span></span> <span data-ttu-id="0ad46-186">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="0ad46-186">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="0ad46-187">可取值为：`ciscoAnyConnect`、`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`customVpn`、`ciscoIPSec`、`citrix`、`ciscoAnyConnectV2`、`paloAltoGlobalProtect`、`zscalerPrivateAccess`、`f5Access2018`、`citrixSso`、`paloAltoGlobalProtectV2`、`ikEv2`、`alwaysOn`。</span><span class="sxs-lookup"><span data-stu-id="0ad46-187">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`.</span></span>|
|<span data-ttu-id="0ad46-188">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="0ad46-188">loginGroupOrDomain</span></span>|<span data-ttu-id="0ad46-189">字符串</span><span class="sxs-lookup"><span data-stu-id="0ad46-189">String</span></span>|<span data-ttu-id="0ad46-190">将连接类型设置为 Dell SonicWALL Mobile 连接时的登录组或域。</span><span class="sxs-lookup"><span data-stu-id="0ad46-190">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="0ad46-191">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ad46-191">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0ad46-192">role</span><span class="sxs-lookup"><span data-stu-id="0ad46-192">role</span></span>|<span data-ttu-id="0ad46-193">字符串</span><span class="sxs-lookup"><span data-stu-id="0ad46-193">String</span></span>|<span data-ttu-id="0ad46-194">将 "连接类型" 设置为 "脉冲安全" 时的角色。</span><span class="sxs-lookup"><span data-stu-id="0ad46-194">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="0ad46-195">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ad46-195">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0ad46-196">型</span><span class="sxs-lookup"><span data-stu-id="0ad46-196">realm</span></span>|<span data-ttu-id="0ad46-197">字符串</span><span class="sxs-lookup"><span data-stu-id="0ad46-197">String</span></span>|<span data-ttu-id="0ad46-198">连接类型设置为脉冲安全时的领域。</span><span class="sxs-lookup"><span data-stu-id="0ad46-198">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="0ad46-199">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ad46-199">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0ad46-200">服务器主板</span><span class="sxs-lookup"><span data-stu-id="0ad46-200">server</span></span>|[<span data-ttu-id="0ad46-201">vpnServer</span><span class="sxs-lookup"><span data-stu-id="0ad46-201">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="0ad46-202">网络上的 VPN 服务器。</span><span class="sxs-lookup"><span data-stu-id="0ad46-202">VPN Server on the network.</span></span> <span data-ttu-id="0ad46-203">请确保最终用户可以访问此网络位置。</span><span class="sxs-lookup"><span data-stu-id="0ad46-203">Make sure end users can access this network location.</span></span> <span data-ttu-id="0ad46-204">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ad46-204">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0ad46-205">标识符</span><span class="sxs-lookup"><span data-stu-id="0ad46-205">identifier</span></span>|<span data-ttu-id="0ad46-206">字符串</span><span class="sxs-lookup"><span data-stu-id="0ad46-206">String</span></span>|<span data-ttu-id="0ad46-207">当连接类型设置为自定义 VPN 时，由 VPN 供应商提供的标识符。</span><span class="sxs-lookup"><span data-stu-id="0ad46-207">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="0ad46-208">例如： Cisco AnyConnect 使用从[AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)继承的 AnyConnect applevpn 的标识符。</span><span class="sxs-lookup"><span data-stu-id="0ad46-208">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0ad46-209">customData</span><span class="sxs-lookup"><span data-stu-id="0ad46-209">customData</span></span>|<span data-ttu-id="0ad46-210">[keyValue](../resources/intune-deviceconfig-keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0ad46-210">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="0ad46-211">将连接类型设置为自定义 VPN 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="0ad46-211">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="0ad46-212">使用此字段启用 Intune 不支持的功能，但在你的 VPN 解决方案中可用。</span><span class="sxs-lookup"><span data-stu-id="0ad46-212">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="0ad46-213">请与你的 VPN 供应商联系，了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="0ad46-213">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="0ad46-214">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="0ad46-214">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="0ad46-215">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ad46-215">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0ad46-216">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="0ad46-216">customKeyValueData</span></span>|<span data-ttu-id="0ad46-217">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0ad46-217">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="0ad46-218">将连接类型设置为自定义 VPN 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="0ad46-218">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="0ad46-219">使用此字段启用 Intune 不支持的功能，但在你的 VPN 解决方案中可用。</span><span class="sxs-lookup"><span data-stu-id="0ad46-219">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="0ad46-220">请与你的 VPN 供应商联系，了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="0ad46-220">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="0ad46-221">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="0ad46-221">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="0ad46-222">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ad46-222">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0ad46-223">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="0ad46-223">enableSplitTunneling</span></span>|<span data-ttu-id="0ad46-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ad46-224">Boolean</span></span>|<span data-ttu-id="0ad46-225">通过 VPN 发送所有网络流量。</span><span class="sxs-lookup"><span data-stu-id="0ad46-225">Send all network traffic through VPN.</span></span> <span data-ttu-id="0ad46-226">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ad46-226">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0ad46-227">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0ad46-227">authenticationMethod</span></span>|[<span data-ttu-id="0ad46-228">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0ad46-228">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="0ad46-229">此 VPN 连接的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="0ad46-229">Authentication method for this VPN connection.</span></span> <span data-ttu-id="0ad46-230">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="0ad46-230">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="0ad46-231">可取值为：`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="0ad46-231">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|
|<span data-ttu-id="0ad46-232">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="0ad46-232">enablePerApp</span></span>|<span data-ttu-id="0ad46-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ad46-233">Boolean</span></span>|<span data-ttu-id="0ad46-234">将此设置为 true 将创建每个应用程序 VPN 有效负载，以后可将其与可在最终用户的 iOS 设备上触发此 VPN 连接的应用程序相关联。</span><span class="sxs-lookup"><span data-stu-id="0ad46-234">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="0ad46-235">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ad46-235">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0ad46-236">safariDomains</span><span class="sxs-lookup"><span data-stu-id="0ad46-236">safariDomains</span></span>|<span data-ttu-id="0ad46-237">String 集合</span><span class="sxs-lookup"><span data-stu-id="0ad46-237">String collection</span></span>|<span data-ttu-id="0ad46-238">启用此 VPN 每应用程序设置时的 Safari 域。</span><span class="sxs-lookup"><span data-stu-id="0ad46-238">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="0ad46-239">除了与此 VPN 关联的应用程序之外，此处指定的 Safari 域还将能够触发此 VPN 连接。</span><span class="sxs-lookup"><span data-stu-id="0ad46-239">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="0ad46-240">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ad46-240">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0ad46-241">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="0ad46-241">onDemandRules</span></span>|<span data-ttu-id="0ad46-242">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="0ad46-242">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="0ad46-243">按需规则。</span><span class="sxs-lookup"><span data-stu-id="0ad46-243">On-Demand Rules.</span></span> <span data-ttu-id="0ad46-244">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="0ad46-244">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="0ad46-245">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ad46-245">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0ad46-246">proxyServer</span><span class="sxs-lookup"><span data-stu-id="0ad46-246">proxyServer</span></span>|[<span data-ttu-id="0ad46-247">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="0ad46-247">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="0ad46-248">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="0ad46-248">Proxy Server.</span></span> <span data-ttu-id="0ad46-249">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ad46-249">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0ad46-250">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="0ad46-250">optInToDeviceIdSharing</span></span>|<span data-ttu-id="0ad46-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ad46-251">Boolean</span></span>|<span data-ttu-id="0ad46-252">选择将设备的 Id 共享到第三方 vpn 客户端，以便在网络访问控制验证期间使用。</span><span class="sxs-lookup"><span data-stu-id="0ad46-252">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="0ad46-253">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ad46-253">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0ad46-254">providerType</span><span class="sxs-lookup"><span data-stu-id="0ad46-254">providerType</span></span>|[<span data-ttu-id="0ad46-255">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="0ad46-255">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="0ad46-256">每应用 VPN 的提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="0ad46-256">Provider type for per-app VPN.</span></span> <span data-ttu-id="0ad46-257">继承自[iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="0ad46-257">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span></span> <span data-ttu-id="0ad46-258">可取值为：`notConfigured`、`appProxy`、`packetTunnel`。</span><span class="sxs-lookup"><span data-stu-id="0ad46-258">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="0ad46-259">userDomain</span><span class="sxs-lookup"><span data-stu-id="0ad46-259">userDomain</span></span>|<span data-ttu-id="0ad46-260">字符串</span><span class="sxs-lookup"><span data-stu-id="0ad46-260">String</span></span>|<span data-ttu-id="0ad46-261">仅 Zscaler。</span><span class="sxs-lookup"><span data-stu-id="0ad46-261">Zscaler only.</span></span> <span data-ttu-id="0ad46-262">输入一个静态域，以便在 Zscaler 应用程序中预填充 "登录" 字段。</span><span class="sxs-lookup"><span data-stu-id="0ad46-262">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="0ad46-263">如果保留为空，则将改用用户的 Azure Active Directory 域。</span><span class="sxs-lookup"><span data-stu-id="0ad46-263">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span> <span data-ttu-id="0ad46-264">继承自[iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ad46-264">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="0ad46-265">strictEnforcement</span><span class="sxs-lookup"><span data-stu-id="0ad46-265">strictEnforcement</span></span>|<span data-ttu-id="0ad46-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ad46-266">Boolean</span></span>|<span data-ttu-id="0ad46-267">仅 Zscaler。</span><span class="sxs-lookup"><span data-stu-id="0ad46-267">Zscaler only.</span></span> <span data-ttu-id="0ad46-268">阻止网络流量，直到用户登录到 Zscaler 应用程序。</span><span class="sxs-lookup"><span data-stu-id="0ad46-268">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="0ad46-269">"True" 表示阻止流量。</span><span class="sxs-lookup"><span data-stu-id="0ad46-269">"True" means traffic is blocked.</span></span> <span data-ttu-id="0ad46-270">继承自[iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ad46-270">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="0ad46-271">cloudName</span><span class="sxs-lookup"><span data-stu-id="0ad46-271">cloudName</span></span>|<span data-ttu-id="0ad46-272">字符串</span><span class="sxs-lookup"><span data-stu-id="0ad46-272">String</span></span>|<span data-ttu-id="0ad46-273">仅 Zscaler。</span><span class="sxs-lookup"><span data-stu-id="0ad46-273">Zscaler only.</span></span> <span data-ttu-id="0ad46-274">用户分配到的 Zscaler 云。</span><span class="sxs-lookup"><span data-stu-id="0ad46-274">Zscaler cloud which the user is assigned to.</span></span> <span data-ttu-id="0ad46-275">继承自[iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ad46-275">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="0ad46-276">excludeList</span><span class="sxs-lookup"><span data-stu-id="0ad46-276">excludeList</span></span>|<span data-ttu-id="0ad46-277">String 集合</span><span class="sxs-lookup"><span data-stu-id="0ad46-277">String collection</span></span>|<span data-ttu-id="0ad46-278">仅 Zscaler。</span><span class="sxs-lookup"><span data-stu-id="0ad46-278">Zscaler only.</span></span> <span data-ttu-id="0ad46-279">不通过 Zscaler 云发送的网络地址的列表。</span><span class="sxs-lookup"><span data-stu-id="0ad46-279">List of network addresses which are not sent through the Zscaler cloud.</span></span> <span data-ttu-id="0ad46-280">继承自[iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ad46-280">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="0ad46-281">childSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="0ad46-281">childSecurityAssociationParameters</span></span>|[<span data-ttu-id="0ad46-282">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="0ad46-282">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="0ad46-283">子安全关联参数</span><span class="sxs-lookup"><span data-stu-id="0ad46-283">Child Security Association Parameters</span></span>|
|<span data-ttu-id="0ad46-284">clientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="0ad46-284">clientAuthenticationType</span></span>|[<span data-ttu-id="0ad46-285">vpnClientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="0ad46-285">vpnClientAuthenticationType</span></span>](../resources/intune-deviceconfig-vpnclientauthenticationtype.md)|<span data-ttu-id="0ad46-286">VPN 客户端将使用的客户端身份验证的类型。</span><span class="sxs-lookup"><span data-stu-id="0ad46-286">Type of Client Authentication the VPN client will use.</span></span> <span data-ttu-id="0ad46-287">可取值为：`userAuthentication`、`deviceAuthentication`。</span><span class="sxs-lookup"><span data-stu-id="0ad46-287">Possible values are: `userAuthentication`, `deviceAuthentication`.</span></span>|
|<span data-ttu-id="0ad46-288">deadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="0ad46-288">deadPeerDetectionRate</span></span>|[<span data-ttu-id="0ad46-289">vpnDeadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="0ad46-289">vpnDeadPeerDetectionRate</span></span>](../resources/intune-deviceconfig-vpndeadpeerdetectionrate.md)|<span data-ttu-id="0ad46-290">确定检查等连接是否仍处于活动状态的频率。</span><span class="sxs-lookup"><span data-stu-id="0ad46-290">Determine how often to check if a peer connection is still active.</span></span> <span data-ttu-id="0ad46-291">.</span><span class="sxs-lookup"><span data-stu-id="0ad46-291">.</span></span> <span data-ttu-id="0ad46-292">可取值为：`medium`、`none`、`low`、`high`。</span><span class="sxs-lookup"><span data-stu-id="0ad46-292">Possible values are: `medium`, `none`, `low`, `high`.</span></span>|
|<span data-ttu-id="0ad46-293">disableMobilityAndMultihoming</span><span class="sxs-lookup"><span data-stu-id="0ad46-293">disableMobilityAndMultihoming</span></span>|<span data-ttu-id="0ad46-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ad46-294">Boolean</span></span>|<span data-ttu-id="0ad46-295">禁用 MOBIKE</span><span class="sxs-lookup"><span data-stu-id="0ad46-295">Disable MOBIKE</span></span>|
|<span data-ttu-id="0ad46-296">disableRedirect</span><span class="sxs-lookup"><span data-stu-id="0ad46-296">disableRedirect</span></span>|<span data-ttu-id="0ad46-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ad46-297">Boolean</span></span>|<span data-ttu-id="0ad46-298">禁用重定向</span><span class="sxs-lookup"><span data-stu-id="0ad46-298">Disable Redirect</span></span>|
|<span data-ttu-id="0ad46-299">enableCertificateRevocationCheck</span><span class="sxs-lookup"><span data-stu-id="0ad46-299">enableCertificateRevocationCheck</span></span>|<span data-ttu-id="0ad46-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ad46-300">Boolean</span></span>|<span data-ttu-id="0ad46-301">启用尽力吊销检查;服务器响应超时不会导致它失败</span><span class="sxs-lookup"><span data-stu-id="0ad46-301">Enables a best-effort revocation check; server response timeouts will not cause it to fail</span></span>|
|<span data-ttu-id="0ad46-302">enableEAP</span><span class="sxs-lookup"><span data-stu-id="0ad46-302">enableEAP</span></span>|<span data-ttu-id="0ad46-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ad46-303">Boolean</span></span>|<span data-ttu-id="0ad46-304">启用仅 EAP 身份验证</span><span class="sxs-lookup"><span data-stu-id="0ad46-304">Enables EAP only authentication</span></span>|
|<span data-ttu-id="0ad46-305">enablePerfectForwardSecrecy</span><span class="sxs-lookup"><span data-stu-id="0ad46-305">enablePerfectForwardSecrecy</span></span>|<span data-ttu-id="0ad46-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ad46-306">Boolean</span></span>|<span data-ttu-id="0ad46-307">启用完全向前保密（PFS）。</span><span class="sxs-lookup"><span data-stu-id="0ad46-307">Enable Perfect Forward Secrecy (PFS).</span></span>|
|<span data-ttu-id="0ad46-308">enableUseInternalSubnetAttributes</span><span class="sxs-lookup"><span data-stu-id="0ad46-308">enableUseInternalSubnetAttributes</span></span>|<span data-ttu-id="0ad46-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ad46-309">Boolean</span></span>|<span data-ttu-id="0ad46-310">启用 "使用内部子网属性"。</span><span class="sxs-lookup"><span data-stu-id="0ad46-310">Enable Use Internal Subnet Attributes.</span></span>|
|<span data-ttu-id="0ad46-311">localIdentifier</span><span class="sxs-lookup"><span data-stu-id="0ad46-311">localIdentifier</span></span>|[<span data-ttu-id="0ad46-312">vpnLocalIdentifier</span><span class="sxs-lookup"><span data-stu-id="0ad46-312">vpnLocalIdentifier</span></span>](../resources/intune-deviceconfig-vpnlocalidentifier.md)|<span data-ttu-id="0ad46-313">标识尝试通过 VPN 连接的客户端的方法。</span><span class="sxs-lookup"><span data-stu-id="0ad46-313">Method of identifying the client that is trying to connect via VPN.</span></span> <span data-ttu-id="0ad46-314">.</span><span class="sxs-lookup"><span data-stu-id="0ad46-314">.</span></span> <span data-ttu-id="0ad46-315">可取值为：`deviceFQDN`、`empty`、`clientCertificateSubjectName`。</span><span class="sxs-lookup"><span data-stu-id="0ad46-315">Possible values are: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span></span>|
|<span data-ttu-id="0ad46-316">remoteIdentifier</span><span class="sxs-lookup"><span data-stu-id="0ad46-316">remoteIdentifier</span></span>|<span data-ttu-id="0ad46-317">字符串</span><span class="sxs-lookup"><span data-stu-id="0ad46-317">String</span></span>|<span data-ttu-id="0ad46-318">IKEv2 服务器的地址。</span><span class="sxs-lookup"><span data-stu-id="0ad46-318">Address of the IKEv2 server.</span></span> <span data-ttu-id="0ad46-319">必须是 FQDN、UserFQDN、网络地址或 ASN1DN</span><span class="sxs-lookup"><span data-stu-id="0ad46-319">Must be a FQDN, UserFQDN, network address, or ASN1DN</span></span>|
|<span data-ttu-id="0ad46-320">securityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="0ad46-320">securityAssociationParameters</span></span>|[<span data-ttu-id="0ad46-321">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="0ad46-321">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="0ad46-322">安全关联参数</span><span class="sxs-lookup"><span data-stu-id="0ad46-322">Security Association Parameters</span></span>|
|<span data-ttu-id="0ad46-323">serverCertificateCommonName</span><span class="sxs-lookup"><span data-stu-id="0ad46-323">serverCertificateCommonName</span></span>|<span data-ttu-id="0ad46-324">字符串</span><span class="sxs-lookup"><span data-stu-id="0ad46-324">String</span></span>|<span data-ttu-id="0ad46-325">服务器身份验证中使用的 IKEv2 服务器证书的公用名</span><span class="sxs-lookup"><span data-stu-id="0ad46-325">Common name of the IKEv2 Server Certificate used in Server Authentication</span></span>|
|<span data-ttu-id="0ad46-326">serverCertificateIssuerCommonName</span><span class="sxs-lookup"><span data-stu-id="0ad46-326">serverCertificateIssuerCommonName</span></span>|<span data-ttu-id="0ad46-327">字符串</span><span class="sxs-lookup"><span data-stu-id="0ad46-327">String</span></span>|<span data-ttu-id="0ad46-328">身份验证中使用的 IKEv2 服务器证书颁发者的颁发者公用名称</span><span class="sxs-lookup"><span data-stu-id="0ad46-328">Issuer Common name of the IKEv2 Server Certificate issuer used in Authentication</span></span>|
|<span data-ttu-id="0ad46-329">serverCertificateType</span><span class="sxs-lookup"><span data-stu-id="0ad46-329">serverCertificateType</span></span>|[<span data-ttu-id="0ad46-330">vpnServerCertificateType</span><span class="sxs-lookup"><span data-stu-id="0ad46-330">vpnServerCertificateType</span></span>](../resources/intune-deviceconfig-vpnservercertificatetype.md)|<span data-ttu-id="0ad46-331">VPN 服务器将提供给 VPN 客户端进行身份验证的证书类型。</span><span class="sxs-lookup"><span data-stu-id="0ad46-331">The type of certificate the VPN server will present to the VPN client for authentication.</span></span> <span data-ttu-id="0ad46-332">可取值为：`rsa`、`ecdsa256`、`ecdsa384`、`ecdsa521`。</span><span class="sxs-lookup"><span data-stu-id="0ad46-332">Possible values are: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span></span>|
|<span data-ttu-id="0ad46-333">sharedSecret</span><span class="sxs-lookup"><span data-stu-id="0ad46-333">sharedSecret</span></span>|<span data-ttu-id="0ad46-334">字符串</span><span class="sxs-lookup"><span data-stu-id="0ad46-334">String</span></span>|<span data-ttu-id="0ad46-335">在选择共享密钥身份验证时使用</span><span class="sxs-lookup"><span data-stu-id="0ad46-335">Used when Shared Secret Authentication is selected</span></span>|
|<span data-ttu-id="0ad46-336">tlsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="0ad46-336">tlsMaximumVersion</span></span>|<span data-ttu-id="0ad46-337">字符串</span><span class="sxs-lookup"><span data-stu-id="0ad46-337">String</span></span>|<span data-ttu-id="0ad46-338">要与 EAP-TLS 身份验证一起使用的最大 TLS 版本</span><span class="sxs-lookup"><span data-stu-id="0ad46-338">The maximum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="0ad46-339">tlsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="0ad46-339">tlsMinimumVersion</span></span>|<span data-ttu-id="0ad46-340">字符串</span><span class="sxs-lookup"><span data-stu-id="0ad46-340">String</span></span>|<span data-ttu-id="0ad46-341">与 EAP-TLS 身份验证一起使用的最小 TLS 版本</span><span class="sxs-lookup"><span data-stu-id="0ad46-341">The minimum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="0ad46-342">allowDefaultSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="0ad46-342">allowDefaultSecurityAssociationParameters</span></span>|<span data-ttu-id="0ad46-343">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ad46-343">Boolean</span></span>|<span data-ttu-id="0ad46-344">允许使用安全关联参数，具体方法是将所有参数设置为设备的默认值，除非明确指定。</span><span class="sxs-lookup"><span data-stu-id="0ad46-344">Allows the use of security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="0ad46-345">allowDefaultChildSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="0ad46-345">allowDefaultChildSecurityAssociationParameters</span></span>|<span data-ttu-id="0ad46-346">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ad46-346">Boolean</span></span>|<span data-ttu-id="0ad46-347">允许使用子安全关联参数，具体方法是将所有参数设置为设备的默认值，除非明确指定。</span><span class="sxs-lookup"><span data-stu-id="0ad46-347">Allows the use of child security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="0ad46-348">alwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="0ad46-348">alwaysOnConfiguration</span></span>|[<span data-ttu-id="0ad46-349">appleVpnAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="0ad46-349">appleVpnAlwaysOnConfiguration</span></span>](../resources/intune-deviceconfig-applevpnalwaysonconfiguration.md)|<span data-ttu-id="0ad46-350">AlwaysOn 配置</span><span class="sxs-lookup"><span data-stu-id="0ad46-350">AlwaysOn Configuration</span></span>|
|<span data-ttu-id="0ad46-351">enableAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="0ad46-351">enableAlwaysOnConfiguration</span></span>|<span data-ttu-id="0ad46-352">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ad46-352">Boolean</span></span>|<span data-ttu-id="0ad46-353">确定是否始终启用 VPN</span><span class="sxs-lookup"><span data-stu-id="0ad46-353">Determines if Always on VPN is enabled</span></span>|



## <a name="response"></a><span data-ttu-id="0ad46-354">响应</span><span class="sxs-lookup"><span data-stu-id="0ad46-354">Response</span></span>
<span data-ttu-id="0ad46-355">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0ad46-355">If successful, this method returns a `200 OK` response code and an updated [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ad46-356">示例</span><span class="sxs-lookup"><span data-stu-id="0ad46-356">Example</span></span>

### <a name="request"></a><span data-ttu-id="0ad46-357">请求</span><span class="sxs-lookup"><span data-stu-id="0ad46-357">Request</span></span>
<span data-ttu-id="0ad46-358">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0ad46-358">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 4984

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
  "allowDefaultChildSecurityAssociationParameters": true,
  "alwaysOnConfiguration": {
    "@odata.type": "microsoft.graph.appleVpnAlwaysOnConfiguration",
    "tunnelConfiguration": "cellular",
    "userToggleEnabled": true,
    "voicemailExceptionAction": "allowTrafficOutside",
    "airPrintExceptionAction": "allowTrafficOutside",
    "cellularExceptionAction": "allowTrafficOutside",
    "allowAllCaptiveNetworkPlugins": true,
    "allowedCaptiveNetworkPlugins": {
      "@odata.type": "microsoft.graph.specifiedCaptiveNetworkPlugins",
      "allowedBundleIdentifiers": [
        "Allowed Bundle Identifiers value"
      ]
    },
    "allowCaptiveWebSheet": true,
    "natKeepAliveIntervalInSeconds": 13,
    "natKeepAliveOffloadEnable": true
  },
  "enableAlwaysOnConfiguration": true
}
```

### <a name="response"></a><span data-ttu-id="0ad46-359">响应</span><span class="sxs-lookup"><span data-stu-id="0ad46-359">Response</span></span>
<span data-ttu-id="0ad46-p139">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0ad46-p139">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 5156

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
  "allowDefaultChildSecurityAssociationParameters": true,
  "alwaysOnConfiguration": {
    "@odata.type": "microsoft.graph.appleVpnAlwaysOnConfiguration",
    "tunnelConfiguration": "cellular",
    "userToggleEnabled": true,
    "voicemailExceptionAction": "allowTrafficOutside",
    "airPrintExceptionAction": "allowTrafficOutside",
    "cellularExceptionAction": "allowTrafficOutside",
    "allowAllCaptiveNetworkPlugins": true,
    "allowedCaptiveNetworkPlugins": {
      "@odata.type": "microsoft.graph.specifiedCaptiveNetworkPlugins",
      "allowedBundleIdentifiers": [
        "Allowed Bundle Identifiers value"
      ]
    },
    "allowCaptiveWebSheet": true,
    "natKeepAliveIntervalInSeconds": 13,
    "natKeepAliveOffloadEnable": true
  },
  "enableAlwaysOnConfiguration": true
}
```





