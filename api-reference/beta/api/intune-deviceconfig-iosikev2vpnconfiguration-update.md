---
title: 更新 iosikEv2VpnConfiguration
description: 更新 iosikEv2VpnConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 265a124431e2c1e01cce1d87360717926b319150
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123083"
---
# <a name="update-iosikev2vpnconfiguration"></a><span data-ttu-id="f26fc-103">更新 iosikEv2VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="f26fc-103">Update iosikEv2VpnConfiguration</span></span>

<span data-ttu-id="f26fc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f26fc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f26fc-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f26fc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f26fc-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f26fc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f26fc-107">更新[iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f26fc-107">Update the properties of a [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f26fc-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f26fc-108">Prerequisites</span></span>
<span data-ttu-id="f26fc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f26fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f26fc-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f26fc-111">Permission type</span></span>|<span data-ttu-id="f26fc-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f26fc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f26fc-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f26fc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f26fc-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f26fc-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f26fc-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f26fc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f26fc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f26fc-116">Not supported.</span></span>|
|<span data-ttu-id="f26fc-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f26fc-117">Application</span></span>|<span data-ttu-id="f26fc-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f26fc-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f26fc-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f26fc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f26fc-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f26fc-120">Request headers</span></span>
|<span data-ttu-id="f26fc-121">标头</span><span class="sxs-lookup"><span data-stu-id="f26fc-121">Header</span></span>|<span data-ttu-id="f26fc-122">值</span><span class="sxs-lookup"><span data-stu-id="f26fc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f26fc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f26fc-123">Authorization</span></span>|<span data-ttu-id="f26fc-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f26fc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f26fc-125">接受</span><span class="sxs-lookup"><span data-stu-id="f26fc-125">Accept</span></span>|<span data-ttu-id="f26fc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f26fc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f26fc-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f26fc-127">Request body</span></span>
<span data-ttu-id="f26fc-128">在请求正文中，提供[iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f26fc-128">In the request body, supply a JSON representation for the [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

<span data-ttu-id="f26fc-129">下表显示创建[iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f26fc-129">The following table shows the properties that are required when you create the [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md).</span></span>

|<span data-ttu-id="f26fc-130">属性</span><span class="sxs-lookup"><span data-stu-id="f26fc-130">Property</span></span>|<span data-ttu-id="f26fc-131">类型</span><span class="sxs-lookup"><span data-stu-id="f26fc-131">Type</span></span>|<span data-ttu-id="f26fc-132">说明</span><span class="sxs-lookup"><span data-stu-id="f26fc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f26fc-133">id</span><span class="sxs-lookup"><span data-stu-id="f26fc-133">id</span></span>|<span data-ttu-id="f26fc-134">字符串</span><span class="sxs-lookup"><span data-stu-id="f26fc-134">String</span></span>|<span data-ttu-id="f26fc-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f26fc-135">Key of the entity.</span></span> <span data-ttu-id="f26fc-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f26fc-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f26fc-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f26fc-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f26fc-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f26fc-138">DateTimeOffset</span></span>|<span data-ttu-id="f26fc-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f26fc-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f26fc-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f26fc-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f26fc-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f26fc-141">roleScopeTagIds</span></span>|<span data-ttu-id="f26fc-142">String collection</span><span class="sxs-lookup"><span data-stu-id="f26fc-142">String collection</span></span>|<span data-ttu-id="f26fc-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="f26fc-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f26fc-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f26fc-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f26fc-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f26fc-145">supportsScopeTags</span></span>|<span data-ttu-id="f26fc-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="f26fc-146">Boolean</span></span>|<span data-ttu-id="f26fc-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="f26fc-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f26fc-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="f26fc-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f26fc-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="f26fc-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f26fc-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="f26fc-150">This property is read-only.</span></span> <span data-ttu-id="f26fc-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f26fc-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f26fc-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f26fc-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="f26fc-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f26fc-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="f26fc-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="f26fc-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="f26fc-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f26fc-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f26fc-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f26fc-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="f26fc-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f26fc-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="f26fc-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="f26fc-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="f26fc-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f26fc-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f26fc-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f26fc-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="f26fc-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f26fc-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="f26fc-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="f26fc-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="f26fc-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f26fc-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f26fc-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f26fc-164">createdDateTime</span></span>|<span data-ttu-id="f26fc-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f26fc-165">DateTimeOffset</span></span>|<span data-ttu-id="f26fc-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f26fc-166">DateTime the object was created.</span></span> <span data-ttu-id="f26fc-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f26fc-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f26fc-168">说明</span><span class="sxs-lookup"><span data-stu-id="f26fc-168">description</span></span>|<span data-ttu-id="f26fc-169">String</span><span class="sxs-lookup"><span data-stu-id="f26fc-169">String</span></span>|<span data-ttu-id="f26fc-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="f26fc-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f26fc-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f26fc-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f26fc-172">displayName</span><span class="sxs-lookup"><span data-stu-id="f26fc-172">displayName</span></span>|<span data-ttu-id="f26fc-173">String</span><span class="sxs-lookup"><span data-stu-id="f26fc-173">String</span></span>|<span data-ttu-id="f26fc-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="f26fc-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f26fc-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f26fc-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f26fc-176">version</span><span class="sxs-lookup"><span data-stu-id="f26fc-176">version</span></span>|<span data-ttu-id="f26fc-177">Int32</span><span class="sxs-lookup"><span data-stu-id="f26fc-177">Int32</span></span>|<span data-ttu-id="f26fc-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="f26fc-178">Version of the device configuration.</span></span> <span data-ttu-id="f26fc-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f26fc-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f26fc-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="f26fc-180">connectionName</span></span>|<span data-ttu-id="f26fc-181">String</span><span class="sxs-lookup"><span data-stu-id="f26fc-181">String</span></span>|<span data-ttu-id="f26fc-182">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="f26fc-182">Connection name displayed to the user.</span></span> <span data-ttu-id="f26fc-183">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f26fc-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f26fc-184">connectionType</span><span class="sxs-lookup"><span data-stu-id="f26fc-184">connectionType</span></span>|[<span data-ttu-id="f26fc-185">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="f26fc-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="f26fc-186">连接类型。</span><span class="sxs-lookup"><span data-stu-id="f26fc-186">Connection type.</span></span> <span data-ttu-id="f26fc-187">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="f26fc-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="f26fc-188">可能的值是：、、、、、、、、、、、、、、、、 `ciscoAnyConnect` `pulseSecure` `f5EdgeClient` `dellSonicWallMobileConnect` `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `ciscoAnyConnectV2` `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso` `paloAltoGlobalProtectV2` `ikEv2` `alwaysOn` `microsoftTunnel` 。</span><span class="sxs-lookup"><span data-stu-id="f26fc-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`, `microsoftTunnel`.</span></span>|
|<span data-ttu-id="f26fc-189">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="f26fc-189">loginGroupOrDomain</span></span>|<span data-ttu-id="f26fc-190">String</span><span class="sxs-lookup"><span data-stu-id="f26fc-190">String</span></span>|<span data-ttu-id="f26fc-191">将连接类型设置为 Dell SonicWALL Mobile 连接时的登录组或域。</span><span class="sxs-lookup"><span data-stu-id="f26fc-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="f26fc-192">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f26fc-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f26fc-193">role</span><span class="sxs-lookup"><span data-stu-id="f26fc-193">role</span></span>|<span data-ttu-id="f26fc-194">String</span><span class="sxs-lookup"><span data-stu-id="f26fc-194">String</span></span>|<span data-ttu-id="f26fc-195">将 "连接类型" 设置为 "脉冲安全" 时的角色。</span><span class="sxs-lookup"><span data-stu-id="f26fc-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="f26fc-196">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f26fc-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f26fc-197">型</span><span class="sxs-lookup"><span data-stu-id="f26fc-197">realm</span></span>|<span data-ttu-id="f26fc-198">String</span><span class="sxs-lookup"><span data-stu-id="f26fc-198">String</span></span>|<span data-ttu-id="f26fc-199">连接类型设置为脉冲安全时的领域。</span><span class="sxs-lookup"><span data-stu-id="f26fc-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="f26fc-200">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f26fc-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f26fc-201">服务器主板</span><span class="sxs-lookup"><span data-stu-id="f26fc-201">server</span></span>|[<span data-ttu-id="f26fc-202">vpnServer</span><span class="sxs-lookup"><span data-stu-id="f26fc-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="f26fc-203">网络上的 VPN 服务器。</span><span class="sxs-lookup"><span data-stu-id="f26fc-203">VPN Server on the network.</span></span> <span data-ttu-id="f26fc-204">请确保最终用户可以访问此网络位置。</span><span class="sxs-lookup"><span data-stu-id="f26fc-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="f26fc-205">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f26fc-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f26fc-206">标识符</span><span class="sxs-lookup"><span data-stu-id="f26fc-206">identifier</span></span>|<span data-ttu-id="f26fc-207">String</span><span class="sxs-lookup"><span data-stu-id="f26fc-207">String</span></span>|<span data-ttu-id="f26fc-208">当连接类型设置为自定义 VPN 时，由 VPN 供应商提供的标识符。</span><span class="sxs-lookup"><span data-stu-id="f26fc-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="f26fc-209">例如： Cisco AnyConnect 使用从[AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)继承的 AnyConnect applevpn 的标识符。</span><span class="sxs-lookup"><span data-stu-id="f26fc-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f26fc-210">customData</span><span class="sxs-lookup"><span data-stu-id="f26fc-210">customData</span></span>|<span data-ttu-id="f26fc-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f26fc-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="f26fc-212">将连接类型设置为自定义 VPN 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="f26fc-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="f26fc-213">使用此字段启用 Intune 不支持的功能，但在你的 VPN 解决方案中可用。</span><span class="sxs-lookup"><span data-stu-id="f26fc-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="f26fc-214">请与你的 VPN 供应商联系，了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="f26fc-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="f26fc-215">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="f26fc-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="f26fc-216">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f26fc-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f26fc-217">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="f26fc-217">customKeyValueData</span></span>|<span data-ttu-id="f26fc-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f26fc-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="f26fc-219">将连接类型设置为自定义 VPN 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="f26fc-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="f26fc-220">使用此字段启用 Intune 不支持的功能，但在你的 VPN 解决方案中可用。</span><span class="sxs-lookup"><span data-stu-id="f26fc-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="f26fc-221">请与你的 VPN 供应商联系，了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="f26fc-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="f26fc-222">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="f26fc-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="f26fc-223">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f26fc-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f26fc-224">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="f26fc-224">enableSplitTunneling</span></span>|<span data-ttu-id="f26fc-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="f26fc-225">Boolean</span></span>|<span data-ttu-id="f26fc-226">通过 VPN 发送所有网络流量。</span><span class="sxs-lookup"><span data-stu-id="f26fc-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="f26fc-227">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f26fc-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f26fc-228">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f26fc-228">authenticationMethod</span></span>|[<span data-ttu-id="f26fc-229">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f26fc-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="f26fc-230">此 VPN 连接的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="f26fc-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="f26fc-231">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="f26fc-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="f26fc-232">可取值为：`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential`、`azureAD`。</span><span class="sxs-lookup"><span data-stu-id="f26fc-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="f26fc-233">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="f26fc-233">enablePerApp</span></span>|<span data-ttu-id="f26fc-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="f26fc-234">Boolean</span></span>|<span data-ttu-id="f26fc-235">将此设置为 true 将创建每个应用程序 VPN 有效负载，以后可将其与可在最终用户的 iOS 设备上触发此 VPN 连接的应用程序相关联。</span><span class="sxs-lookup"><span data-stu-id="f26fc-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="f26fc-236">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f26fc-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f26fc-237">safariDomains</span><span class="sxs-lookup"><span data-stu-id="f26fc-237">safariDomains</span></span>|<span data-ttu-id="f26fc-238">String collection</span><span class="sxs-lookup"><span data-stu-id="f26fc-238">String collection</span></span>|<span data-ttu-id="f26fc-239">启用此 VPN 每应用程序设置时的 Safari 域。</span><span class="sxs-lookup"><span data-stu-id="f26fc-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="f26fc-240">除了与此 VPN 关联的应用程序之外，此处指定的 Safari 域还将能够触发此 VPN 连接。</span><span class="sxs-lookup"><span data-stu-id="f26fc-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="f26fc-241">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f26fc-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f26fc-242">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="f26fc-242">onDemandRules</span></span>|<span data-ttu-id="f26fc-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="f26fc-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="f26fc-244">按需规则。</span><span class="sxs-lookup"><span data-stu-id="f26fc-244">On-Demand Rules.</span></span> <span data-ttu-id="f26fc-245">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="f26fc-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="f26fc-246">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f26fc-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f26fc-247">proxyServer</span><span class="sxs-lookup"><span data-stu-id="f26fc-247">proxyServer</span></span>|[<span data-ttu-id="f26fc-248">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="f26fc-248">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="f26fc-249">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="f26fc-249">Proxy Server.</span></span> <span data-ttu-id="f26fc-250">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f26fc-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f26fc-251">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="f26fc-251">optInToDeviceIdSharing</span></span>|<span data-ttu-id="f26fc-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="f26fc-252">Boolean</span></span>|<span data-ttu-id="f26fc-253">选择将设备的 Id 共享到第三方 vpn 客户端，以便在网络访问控制验证期间使用。</span><span class="sxs-lookup"><span data-stu-id="f26fc-253">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="f26fc-254">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f26fc-254">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f26fc-255">providerType</span><span class="sxs-lookup"><span data-stu-id="f26fc-255">providerType</span></span>|[<span data-ttu-id="f26fc-256">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="f26fc-256">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="f26fc-257">每应用 VPN 的提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="f26fc-257">Provider type for per-app VPN.</span></span> <span data-ttu-id="f26fc-258">继承自[iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="f26fc-258">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span></span> <span data-ttu-id="f26fc-259">可取值为：`notConfigured`、`appProxy`、`packetTunnel`。</span><span class="sxs-lookup"><span data-stu-id="f26fc-259">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="f26fc-260">userDomain</span><span class="sxs-lookup"><span data-stu-id="f26fc-260">userDomain</span></span>|<span data-ttu-id="f26fc-261">String</span><span class="sxs-lookup"><span data-stu-id="f26fc-261">String</span></span>|<span data-ttu-id="f26fc-262">仅 Zscaler。</span><span class="sxs-lookup"><span data-stu-id="f26fc-262">Zscaler only.</span></span> <span data-ttu-id="f26fc-263">输入一个静态域，以便在 Zscaler 应用程序中预填充 "登录" 字段。</span><span class="sxs-lookup"><span data-stu-id="f26fc-263">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="f26fc-264">如果保留为空，则将改用用户的 Azure Active Directory 域。</span><span class="sxs-lookup"><span data-stu-id="f26fc-264">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span> <span data-ttu-id="f26fc-265">继承自[iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f26fc-265">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="f26fc-266">strictEnforcement</span><span class="sxs-lookup"><span data-stu-id="f26fc-266">strictEnforcement</span></span>|<span data-ttu-id="f26fc-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="f26fc-267">Boolean</span></span>|<span data-ttu-id="f26fc-268">仅 Zscaler。</span><span class="sxs-lookup"><span data-stu-id="f26fc-268">Zscaler only.</span></span> <span data-ttu-id="f26fc-269">阻止网络流量，直到用户登录到 Zscaler 应用程序。</span><span class="sxs-lookup"><span data-stu-id="f26fc-269">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="f26fc-270">"True" 表示阻止流量。</span><span class="sxs-lookup"><span data-stu-id="f26fc-270">"True" means traffic is blocked.</span></span> <span data-ttu-id="f26fc-271">继承自[iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f26fc-271">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="f26fc-272">cloudName</span><span class="sxs-lookup"><span data-stu-id="f26fc-272">cloudName</span></span>|<span data-ttu-id="f26fc-273">String</span><span class="sxs-lookup"><span data-stu-id="f26fc-273">String</span></span>|<span data-ttu-id="f26fc-274">仅 Zscaler。</span><span class="sxs-lookup"><span data-stu-id="f26fc-274">Zscaler only.</span></span> <span data-ttu-id="f26fc-275">用户分配到的 Zscaler 云。</span><span class="sxs-lookup"><span data-stu-id="f26fc-275">Zscaler cloud which the user is assigned to.</span></span> <span data-ttu-id="f26fc-276">继承自[iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f26fc-276">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="f26fc-277">excludeList</span><span class="sxs-lookup"><span data-stu-id="f26fc-277">excludeList</span></span>|<span data-ttu-id="f26fc-278">String collection</span><span class="sxs-lookup"><span data-stu-id="f26fc-278">String collection</span></span>|<span data-ttu-id="f26fc-279">仅 Zscaler。</span><span class="sxs-lookup"><span data-stu-id="f26fc-279">Zscaler only.</span></span> <span data-ttu-id="f26fc-280">不通过 Zscaler 云发送的网络地址的列表。</span><span class="sxs-lookup"><span data-stu-id="f26fc-280">List of network addresses which are not sent through the Zscaler cloud.</span></span> <span data-ttu-id="f26fc-281">继承自[iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f26fc-281">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="f26fc-282">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="f26fc-282">targetedMobileApps</span></span>|<span data-ttu-id="f26fc-283">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f26fc-283">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="f26fc-284">目标移动应用。</span><span class="sxs-lookup"><span data-stu-id="f26fc-284">Targeted mobile apps.</span></span> <span data-ttu-id="f26fc-285">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="f26fc-285">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="f26fc-286">继承自[iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f26fc-286">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="f26fc-287">childSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="f26fc-287">childSecurityAssociationParameters</span></span>|[<span data-ttu-id="f26fc-288">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="f26fc-288">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="f26fc-289">子安全关联参数</span><span class="sxs-lookup"><span data-stu-id="f26fc-289">Child Security Association Parameters</span></span>|
|<span data-ttu-id="f26fc-290">clientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="f26fc-290">clientAuthenticationType</span></span>|[<span data-ttu-id="f26fc-291">vpnClientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="f26fc-291">vpnClientAuthenticationType</span></span>](../resources/intune-deviceconfig-vpnclientauthenticationtype.md)|<span data-ttu-id="f26fc-292">VPN 客户端将使用的客户端身份验证的类型。</span><span class="sxs-lookup"><span data-stu-id="f26fc-292">Type of Client Authentication the VPN client will use.</span></span> <span data-ttu-id="f26fc-293">可取值为：`userAuthentication`、`deviceAuthentication`。</span><span class="sxs-lookup"><span data-stu-id="f26fc-293">Possible values are: `userAuthentication`, `deviceAuthentication`.</span></span>|
|<span data-ttu-id="f26fc-294">deadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="f26fc-294">deadPeerDetectionRate</span></span>|[<span data-ttu-id="f26fc-295">vpnDeadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="f26fc-295">vpnDeadPeerDetectionRate</span></span>](../resources/intune-deviceconfig-vpndeadpeerdetectionrate.md)|<span data-ttu-id="f26fc-296">确定检查等连接是否仍处于活动状态的频率。</span><span class="sxs-lookup"><span data-stu-id="f26fc-296">Determine how often to check if a peer connection is still active.</span></span> <span data-ttu-id="f26fc-297">.</span><span class="sxs-lookup"><span data-stu-id="f26fc-297">.</span></span> <span data-ttu-id="f26fc-298">可取值为：`medium`、`none`、`low`、`high`。</span><span class="sxs-lookup"><span data-stu-id="f26fc-298">Possible values are: `medium`, `none`, `low`, `high`.</span></span>|
|<span data-ttu-id="f26fc-299">disableMobilityAndMultihoming</span><span class="sxs-lookup"><span data-stu-id="f26fc-299">disableMobilityAndMultihoming</span></span>|<span data-ttu-id="f26fc-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="f26fc-300">Boolean</span></span>|<span data-ttu-id="f26fc-301">禁用 MOBIKE</span><span class="sxs-lookup"><span data-stu-id="f26fc-301">Disable MOBIKE</span></span>|
|<span data-ttu-id="f26fc-302">disableRedirect</span><span class="sxs-lookup"><span data-stu-id="f26fc-302">disableRedirect</span></span>|<span data-ttu-id="f26fc-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="f26fc-303">Boolean</span></span>|<span data-ttu-id="f26fc-304">禁用重定向</span><span class="sxs-lookup"><span data-stu-id="f26fc-304">Disable Redirect</span></span>|
|<span data-ttu-id="f26fc-305">enableCertificateRevocationCheck</span><span class="sxs-lookup"><span data-stu-id="f26fc-305">enableCertificateRevocationCheck</span></span>|<span data-ttu-id="f26fc-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="f26fc-306">Boolean</span></span>|<span data-ttu-id="f26fc-307">启用尽力吊销检查;服务器响应超时不会导致它失败</span><span class="sxs-lookup"><span data-stu-id="f26fc-307">Enables a best-effort revocation check; server response timeouts will not cause it to fail</span></span>|
|<span data-ttu-id="f26fc-308">enableEAP</span><span class="sxs-lookup"><span data-stu-id="f26fc-308">enableEAP</span></span>|<span data-ttu-id="f26fc-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="f26fc-309">Boolean</span></span>|<span data-ttu-id="f26fc-310">启用仅 EAP 身份验证</span><span class="sxs-lookup"><span data-stu-id="f26fc-310">Enables EAP only authentication</span></span>|
|<span data-ttu-id="f26fc-311">enablePerfectForwardSecrecy</span><span class="sxs-lookup"><span data-stu-id="f26fc-311">enablePerfectForwardSecrecy</span></span>|<span data-ttu-id="f26fc-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="f26fc-312">Boolean</span></span>|<span data-ttu-id="f26fc-313">启用完全向前保密 (PFS) 。</span><span class="sxs-lookup"><span data-stu-id="f26fc-313">Enable Perfect Forward Secrecy (PFS).</span></span>|
|<span data-ttu-id="f26fc-314">enableUseInternalSubnetAttributes</span><span class="sxs-lookup"><span data-stu-id="f26fc-314">enableUseInternalSubnetAttributes</span></span>|<span data-ttu-id="f26fc-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="f26fc-315">Boolean</span></span>|<span data-ttu-id="f26fc-316">启用 "使用内部子网属性"。</span><span class="sxs-lookup"><span data-stu-id="f26fc-316">Enable Use Internal Subnet Attributes.</span></span>|
|<span data-ttu-id="f26fc-317">localIdentifier</span><span class="sxs-lookup"><span data-stu-id="f26fc-317">localIdentifier</span></span>|[<span data-ttu-id="f26fc-318">vpnLocalIdentifier</span><span class="sxs-lookup"><span data-stu-id="f26fc-318">vpnLocalIdentifier</span></span>](../resources/intune-deviceconfig-vpnlocalidentifier.md)|<span data-ttu-id="f26fc-319">标识尝试通过 VPN 连接的客户端的方法。</span><span class="sxs-lookup"><span data-stu-id="f26fc-319">Method of identifying the client that is trying to connect via VPN.</span></span> <span data-ttu-id="f26fc-320">.</span><span class="sxs-lookup"><span data-stu-id="f26fc-320">.</span></span> <span data-ttu-id="f26fc-321">可取值为：`deviceFQDN`、`empty`、`clientCertificateSubjectName`。</span><span class="sxs-lookup"><span data-stu-id="f26fc-321">Possible values are: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span></span>|
|<span data-ttu-id="f26fc-322">remoteIdentifier</span><span class="sxs-lookup"><span data-stu-id="f26fc-322">remoteIdentifier</span></span>|<span data-ttu-id="f26fc-323">String</span><span class="sxs-lookup"><span data-stu-id="f26fc-323">String</span></span>|<span data-ttu-id="f26fc-324">IKEv2 服务器的地址。</span><span class="sxs-lookup"><span data-stu-id="f26fc-324">Address of the IKEv2 server.</span></span> <span data-ttu-id="f26fc-325">必须是 FQDN、UserFQDN、网络地址或 ASN1DN</span><span class="sxs-lookup"><span data-stu-id="f26fc-325">Must be a FQDN, UserFQDN, network address, or ASN1DN</span></span>|
|<span data-ttu-id="f26fc-326">securityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="f26fc-326">securityAssociationParameters</span></span>|[<span data-ttu-id="f26fc-327">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="f26fc-327">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="f26fc-328">安全关联参数</span><span class="sxs-lookup"><span data-stu-id="f26fc-328">Security Association Parameters</span></span>|
|<span data-ttu-id="f26fc-329">serverCertificateCommonName</span><span class="sxs-lookup"><span data-stu-id="f26fc-329">serverCertificateCommonName</span></span>|<span data-ttu-id="f26fc-330">String</span><span class="sxs-lookup"><span data-stu-id="f26fc-330">String</span></span>|<span data-ttu-id="f26fc-331">服务器身份验证中使用的 IKEv2 服务器证书的公用名</span><span class="sxs-lookup"><span data-stu-id="f26fc-331">Common name of the IKEv2 Server Certificate used in Server Authentication</span></span>|
|<span data-ttu-id="f26fc-332">serverCertificateIssuerCommonName</span><span class="sxs-lookup"><span data-stu-id="f26fc-332">serverCertificateIssuerCommonName</span></span>|<span data-ttu-id="f26fc-333">String</span><span class="sxs-lookup"><span data-stu-id="f26fc-333">String</span></span>|<span data-ttu-id="f26fc-334">身份验证中使用的 IKEv2 服务器证书颁发者的颁发者公用名称</span><span class="sxs-lookup"><span data-stu-id="f26fc-334">Issuer Common name of the IKEv2 Server Certificate issuer used in Authentication</span></span>|
|<span data-ttu-id="f26fc-335">serverCertificateType</span><span class="sxs-lookup"><span data-stu-id="f26fc-335">serverCertificateType</span></span>|[<span data-ttu-id="f26fc-336">vpnServerCertificateType</span><span class="sxs-lookup"><span data-stu-id="f26fc-336">vpnServerCertificateType</span></span>](../resources/intune-deviceconfig-vpnservercertificatetype.md)|<span data-ttu-id="f26fc-337">VPN 服务器将提供给 VPN 客户端进行身份验证的证书类型。</span><span class="sxs-lookup"><span data-stu-id="f26fc-337">The type of certificate the VPN server will present to the VPN client for authentication.</span></span> <span data-ttu-id="f26fc-338">可取值为：`rsa`、`ecdsa256`、`ecdsa384`、`ecdsa521`。</span><span class="sxs-lookup"><span data-stu-id="f26fc-338">Possible values are: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span></span>|
|<span data-ttu-id="f26fc-339">sharedSecret</span><span class="sxs-lookup"><span data-stu-id="f26fc-339">sharedSecret</span></span>|<span data-ttu-id="f26fc-340">String</span><span class="sxs-lookup"><span data-stu-id="f26fc-340">String</span></span>|<span data-ttu-id="f26fc-341">在选择共享密钥身份验证时使用</span><span class="sxs-lookup"><span data-stu-id="f26fc-341">Used when Shared Secret Authentication is selected</span></span>|
|<span data-ttu-id="f26fc-342">tlsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="f26fc-342">tlsMaximumVersion</span></span>|<span data-ttu-id="f26fc-343">String</span><span class="sxs-lookup"><span data-stu-id="f26fc-343">String</span></span>|<span data-ttu-id="f26fc-344">要与 EAP-TLS 身份验证一起使用的最大 TLS 版本</span><span class="sxs-lookup"><span data-stu-id="f26fc-344">The maximum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="f26fc-345">tlsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="f26fc-345">tlsMinimumVersion</span></span>|<span data-ttu-id="f26fc-346">String</span><span class="sxs-lookup"><span data-stu-id="f26fc-346">String</span></span>|<span data-ttu-id="f26fc-347">与 EAP-TLS 身份验证一起使用的最小 TLS 版本</span><span class="sxs-lookup"><span data-stu-id="f26fc-347">The minimum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="f26fc-348">allowDefaultSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="f26fc-348">allowDefaultSecurityAssociationParameters</span></span>|<span data-ttu-id="f26fc-349">Boolean</span><span class="sxs-lookup"><span data-stu-id="f26fc-349">Boolean</span></span>|<span data-ttu-id="f26fc-350">允许使用安全关联参数，具体方法是将所有参数设置为设备的默认值，除非明确指定。</span><span class="sxs-lookup"><span data-stu-id="f26fc-350">Allows the use of security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="f26fc-351">allowDefaultChildSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="f26fc-351">allowDefaultChildSecurityAssociationParameters</span></span>|<span data-ttu-id="f26fc-352">Boolean</span><span class="sxs-lookup"><span data-stu-id="f26fc-352">Boolean</span></span>|<span data-ttu-id="f26fc-353">允许使用子安全关联参数，具体方法是将所有参数设置为设备的默认值，除非明确指定。</span><span class="sxs-lookup"><span data-stu-id="f26fc-353">Allows the use of child security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="f26fc-354">alwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="f26fc-354">alwaysOnConfiguration</span></span>|[<span data-ttu-id="f26fc-355">appleVpnAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="f26fc-355">appleVpnAlwaysOnConfiguration</span></span>](../resources/intune-deviceconfig-applevpnalwaysonconfiguration.md)|<span data-ttu-id="f26fc-356">AlwaysOn 配置</span><span class="sxs-lookup"><span data-stu-id="f26fc-356">AlwaysOn Configuration</span></span>|
|<span data-ttu-id="f26fc-357">enableAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="f26fc-357">enableAlwaysOnConfiguration</span></span>|<span data-ttu-id="f26fc-358">Boolean</span><span class="sxs-lookup"><span data-stu-id="f26fc-358">Boolean</span></span>|<span data-ttu-id="f26fc-359">确定是否始终启用 VPN</span><span class="sxs-lookup"><span data-stu-id="f26fc-359">Determines if Always on VPN is enabled</span></span>|



## <a name="response"></a><span data-ttu-id="f26fc-360">响应</span><span class="sxs-lookup"><span data-stu-id="f26fc-360">Response</span></span>
<span data-ttu-id="f26fc-361">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的[iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f26fc-361">If successful, this method returns a `200 OK` response code and an updated [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f26fc-362">示例</span><span class="sxs-lookup"><span data-stu-id="f26fc-362">Example</span></span>

### <a name="request"></a><span data-ttu-id="f26fc-363">请求</span><span class="sxs-lookup"><span data-stu-id="f26fc-363">Request</span></span>
<span data-ttu-id="f26fc-364">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f26fc-364">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 5241

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
  "targetedMobileApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
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

### <a name="response"></a><span data-ttu-id="f26fc-365">响应</span><span class="sxs-lookup"><span data-stu-id="f26fc-365">Response</span></span>
<span data-ttu-id="f26fc-p140">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f26fc-p140">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 5413

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
  "targetedMobileApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
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



