---
title: 更新 iosikEv2VpnConfiguration
description: 更新 iosikEv2VpnConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3c8f09a7ef8c7aa0f83b6a45482bb2cb1d030496
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448870"
---
# <a name="update-iosikev2vpnconfiguration"></a><span data-ttu-id="7b76a-103">更新 iosikEv2VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="7b76a-103">Update iosikEv2VpnConfiguration</span></span>

<span data-ttu-id="7b76a-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="7b76a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7b76a-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7b76a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7b76a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7b76a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b76a-107">更新[iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7b76a-107">Update the properties of a [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7b76a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7b76a-108">Prerequisites</span></span>
<span data-ttu-id="7b76a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7b76a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b76a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7b76a-111">Permission type</span></span>|<span data-ttu-id="7b76a-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7b76a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b76a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7b76a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7b76a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b76a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7b76a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7b76a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b76a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7b76a-116">Not supported.</span></span>|
|<span data-ttu-id="7b76a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7b76a-117">Application</span></span>|<span data-ttu-id="7b76a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b76a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b76a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7b76a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="7b76a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7b76a-120">Request headers</span></span>
|<span data-ttu-id="7b76a-121">标头</span><span class="sxs-lookup"><span data-stu-id="7b76a-121">Header</span></span>|<span data-ttu-id="7b76a-122">值</span><span class="sxs-lookup"><span data-stu-id="7b76a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7b76a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b76a-123">Authorization</span></span>|<span data-ttu-id="7b76a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7b76a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7b76a-125">接受</span><span class="sxs-lookup"><span data-stu-id="7b76a-125">Accept</span></span>|<span data-ttu-id="7b76a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7b76a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b76a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7b76a-127">Request body</span></span>
<span data-ttu-id="7b76a-128">在请求正文中，提供[iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7b76a-128">In the request body, supply a JSON representation for the [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

<span data-ttu-id="7b76a-129">下表显示创建[iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7b76a-129">The following table shows the properties that are required when you create the [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md).</span></span>

|<span data-ttu-id="7b76a-130">属性</span><span class="sxs-lookup"><span data-stu-id="7b76a-130">Property</span></span>|<span data-ttu-id="7b76a-131">类型</span><span class="sxs-lookup"><span data-stu-id="7b76a-131">Type</span></span>|<span data-ttu-id="7b76a-132">说明</span><span class="sxs-lookup"><span data-stu-id="7b76a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b76a-133">id</span><span class="sxs-lookup"><span data-stu-id="7b76a-133">id</span></span>|<span data-ttu-id="7b76a-134">字符串</span><span class="sxs-lookup"><span data-stu-id="7b76a-134">String</span></span>|<span data-ttu-id="7b76a-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7b76a-135">Key of the entity.</span></span> <span data-ttu-id="7b76a-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b76a-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b76a-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7b76a-137">lastModifiedDateTime</span></span>|<span data-ttu-id="7b76a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b76a-138">DateTimeOffset</span></span>|<span data-ttu-id="7b76a-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="7b76a-139">DateTime the object was last modified.</span></span> <span data-ttu-id="7b76a-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b76a-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b76a-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7b76a-141">roleScopeTagIds</span></span>|<span data-ttu-id="7b76a-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="7b76a-142">String collection</span></span>|<span data-ttu-id="7b76a-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="7b76a-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7b76a-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b76a-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b76a-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="7b76a-145">supportsScopeTags</span></span>|<span data-ttu-id="7b76a-146">布尔</span><span class="sxs-lookup"><span data-stu-id="7b76a-146">Boolean</span></span>|<span data-ttu-id="7b76a-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="7b76a-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="7b76a-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="7b76a-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="7b76a-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="7b76a-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="7b76a-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="7b76a-150">This property is read-only.</span></span> <span data-ttu-id="7b76a-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b76a-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b76a-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="7b76a-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="7b76a-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="7b76a-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="7b76a-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="7b76a-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="7b76a-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b76a-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b76a-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="7b76a-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="7b76a-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="7b76a-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="7b76a-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="7b76a-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="7b76a-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b76a-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b76a-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="7b76a-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="7b76a-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="7b76a-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="7b76a-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="7b76a-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="7b76a-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b76a-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b76a-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7b76a-164">createdDateTime</span></span>|<span data-ttu-id="7b76a-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b76a-165">DateTimeOffset</span></span>|<span data-ttu-id="7b76a-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="7b76a-166">DateTime the object was created.</span></span> <span data-ttu-id="7b76a-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b76a-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b76a-168">说明</span><span class="sxs-lookup"><span data-stu-id="7b76a-168">description</span></span>|<span data-ttu-id="7b76a-169">String</span><span class="sxs-lookup"><span data-stu-id="7b76a-169">String</span></span>|<span data-ttu-id="7b76a-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="7b76a-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7b76a-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b76a-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b76a-172">displayName</span><span class="sxs-lookup"><span data-stu-id="7b76a-172">displayName</span></span>|<span data-ttu-id="7b76a-173">String</span><span class="sxs-lookup"><span data-stu-id="7b76a-173">String</span></span>|<span data-ttu-id="7b76a-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="7b76a-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7b76a-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b76a-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b76a-176">version</span><span class="sxs-lookup"><span data-stu-id="7b76a-176">version</span></span>|<span data-ttu-id="7b76a-177">Int32</span><span class="sxs-lookup"><span data-stu-id="7b76a-177">Int32</span></span>|<span data-ttu-id="7b76a-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="7b76a-178">Version of the device configuration.</span></span> <span data-ttu-id="7b76a-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b76a-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b76a-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="7b76a-180">connectionName</span></span>|<span data-ttu-id="7b76a-181">String</span><span class="sxs-lookup"><span data-stu-id="7b76a-181">String</span></span>|<span data-ttu-id="7b76a-182">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="7b76a-182">Connection name displayed to the user.</span></span> <span data-ttu-id="7b76a-183">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b76a-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="7b76a-184">connectionType</span><span class="sxs-lookup"><span data-stu-id="7b76a-184">connectionType</span></span>|[<span data-ttu-id="7b76a-185">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="7b76a-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="7b76a-186">连接类型。</span><span class="sxs-lookup"><span data-stu-id="7b76a-186">Connection type.</span></span> <span data-ttu-id="7b76a-187">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="7b76a-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="7b76a-188">可取值为：`ciscoAnyConnect`、`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`customVpn`、`ciscoIPSec`、`citrix`、`ciscoAnyConnectV2`、`paloAltoGlobalProtect`、`zscalerPrivateAccess`、`f5Access2018`、`citrixSso`、`paloAltoGlobalProtectV2`、`ikEv2`、`alwaysOn`。</span><span class="sxs-lookup"><span data-stu-id="7b76a-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`.</span></span>|
|<span data-ttu-id="7b76a-189">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="7b76a-189">loginGroupOrDomain</span></span>|<span data-ttu-id="7b76a-190">String</span><span class="sxs-lookup"><span data-stu-id="7b76a-190">String</span></span>|<span data-ttu-id="7b76a-191">将连接类型设置为 Dell SonicWALL Mobile 连接时的登录组或域。</span><span class="sxs-lookup"><span data-stu-id="7b76a-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="7b76a-192">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b76a-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="7b76a-193">role</span><span class="sxs-lookup"><span data-stu-id="7b76a-193">role</span></span>|<span data-ttu-id="7b76a-194">String</span><span class="sxs-lookup"><span data-stu-id="7b76a-194">String</span></span>|<span data-ttu-id="7b76a-195">将 "连接类型" 设置为 "脉冲安全" 时的角色。</span><span class="sxs-lookup"><span data-stu-id="7b76a-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="7b76a-196">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b76a-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="7b76a-197">型</span><span class="sxs-lookup"><span data-stu-id="7b76a-197">realm</span></span>|<span data-ttu-id="7b76a-198">String</span><span class="sxs-lookup"><span data-stu-id="7b76a-198">String</span></span>|<span data-ttu-id="7b76a-199">连接类型设置为脉冲安全时的领域。</span><span class="sxs-lookup"><span data-stu-id="7b76a-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="7b76a-200">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b76a-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="7b76a-201">服务器主板</span><span class="sxs-lookup"><span data-stu-id="7b76a-201">server</span></span>|[<span data-ttu-id="7b76a-202">vpnServer</span><span class="sxs-lookup"><span data-stu-id="7b76a-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="7b76a-203">网络上的 VPN 服务器。</span><span class="sxs-lookup"><span data-stu-id="7b76a-203">VPN Server on the network.</span></span> <span data-ttu-id="7b76a-204">请确保最终用户可以访问此网络位置。</span><span class="sxs-lookup"><span data-stu-id="7b76a-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="7b76a-205">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b76a-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="7b76a-206">标识符</span><span class="sxs-lookup"><span data-stu-id="7b76a-206">identifier</span></span>|<span data-ttu-id="7b76a-207">String</span><span class="sxs-lookup"><span data-stu-id="7b76a-207">String</span></span>|<span data-ttu-id="7b76a-208">当连接类型设置为自定义 VPN 时，由 VPN 供应商提供的标识符。</span><span class="sxs-lookup"><span data-stu-id="7b76a-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="7b76a-209">例如： Cisco AnyConnect 使用从[AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)继承的 AnyConnect applevpn 的标识符。</span><span class="sxs-lookup"><span data-stu-id="7b76a-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="7b76a-210">customData</span><span class="sxs-lookup"><span data-stu-id="7b76a-210">customData</span></span>|<span data-ttu-id="7b76a-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7b76a-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="7b76a-212">将连接类型设置为自定义 VPN 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="7b76a-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="7b76a-213">使用此字段启用 Intune 不支持的功能，但在你的 VPN 解决方案中可用。</span><span class="sxs-lookup"><span data-stu-id="7b76a-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="7b76a-214">请与你的 VPN 供应商联系，了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="7b76a-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="7b76a-215">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="7b76a-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="7b76a-216">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b76a-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="7b76a-217">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="7b76a-217">customKeyValueData</span></span>|<span data-ttu-id="7b76a-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7b76a-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="7b76a-219">将连接类型设置为自定义 VPN 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="7b76a-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="7b76a-220">使用此字段启用 Intune 不支持的功能，但在你的 VPN 解决方案中可用。</span><span class="sxs-lookup"><span data-stu-id="7b76a-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="7b76a-221">请与你的 VPN 供应商联系，了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="7b76a-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="7b76a-222">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="7b76a-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="7b76a-223">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b76a-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="7b76a-224">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="7b76a-224">enableSplitTunneling</span></span>|<span data-ttu-id="7b76a-225">布尔</span><span class="sxs-lookup"><span data-stu-id="7b76a-225">Boolean</span></span>|<span data-ttu-id="7b76a-226">通过 VPN 发送所有网络流量。</span><span class="sxs-lookup"><span data-stu-id="7b76a-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="7b76a-227">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b76a-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="7b76a-228">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="7b76a-228">authenticationMethod</span></span>|[<span data-ttu-id="7b76a-229">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="7b76a-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="7b76a-230">此 VPN 连接的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="7b76a-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="7b76a-231">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="7b76a-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="7b76a-232">可取值为：`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="7b76a-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|
|<span data-ttu-id="7b76a-233">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="7b76a-233">enablePerApp</span></span>|<span data-ttu-id="7b76a-234">布尔</span><span class="sxs-lookup"><span data-stu-id="7b76a-234">Boolean</span></span>|<span data-ttu-id="7b76a-235">将此设置为 true 将创建每个应用程序 VPN 有效负载，以后可将其与可在最终用户的 iOS 设备上触发此 VPN 连接的应用程序相关联。</span><span class="sxs-lookup"><span data-stu-id="7b76a-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="7b76a-236">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b76a-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="7b76a-237">safariDomains</span><span class="sxs-lookup"><span data-stu-id="7b76a-237">safariDomains</span></span>|<span data-ttu-id="7b76a-238">String 集合</span><span class="sxs-lookup"><span data-stu-id="7b76a-238">String collection</span></span>|<span data-ttu-id="7b76a-239">启用此 VPN 每应用程序设置时的 Safari 域。</span><span class="sxs-lookup"><span data-stu-id="7b76a-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="7b76a-240">除了与此 VPN 关联的应用程序之外，此处指定的 Safari 域还将能够触发此 VPN 连接。</span><span class="sxs-lookup"><span data-stu-id="7b76a-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="7b76a-241">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b76a-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="7b76a-242">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="7b76a-242">onDemandRules</span></span>|<span data-ttu-id="7b76a-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="7b76a-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="7b76a-244">按需规则。</span><span class="sxs-lookup"><span data-stu-id="7b76a-244">On-Demand Rules.</span></span> <span data-ttu-id="7b76a-245">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="7b76a-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="7b76a-246">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b76a-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="7b76a-247">proxyServer</span><span class="sxs-lookup"><span data-stu-id="7b76a-247">proxyServer</span></span>|[<span data-ttu-id="7b76a-248">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="7b76a-248">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="7b76a-249">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="7b76a-249">Proxy Server.</span></span> <span data-ttu-id="7b76a-250">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b76a-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="7b76a-251">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="7b76a-251">optInToDeviceIdSharing</span></span>|<span data-ttu-id="7b76a-252">布尔</span><span class="sxs-lookup"><span data-stu-id="7b76a-252">Boolean</span></span>|<span data-ttu-id="7b76a-253">选择将设备的 Id 共享到第三方 vpn 客户端，以便在网络访问控制验证期间使用。</span><span class="sxs-lookup"><span data-stu-id="7b76a-253">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="7b76a-254">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b76a-254">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="7b76a-255">providerType</span><span class="sxs-lookup"><span data-stu-id="7b76a-255">providerType</span></span>|[<span data-ttu-id="7b76a-256">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="7b76a-256">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="7b76a-257">每应用 VPN 的提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="7b76a-257">Provider type for per-app VPN.</span></span> <span data-ttu-id="7b76a-258">继承自[iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="7b76a-258">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span></span> <span data-ttu-id="7b76a-259">可取值为：`notConfigured`、`appProxy`、`packetTunnel`。</span><span class="sxs-lookup"><span data-stu-id="7b76a-259">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="7b76a-260">userDomain</span><span class="sxs-lookup"><span data-stu-id="7b76a-260">userDomain</span></span>|<span data-ttu-id="7b76a-261">String</span><span class="sxs-lookup"><span data-stu-id="7b76a-261">String</span></span>|<span data-ttu-id="7b76a-262">仅 Zscaler。</span><span class="sxs-lookup"><span data-stu-id="7b76a-262">Zscaler only.</span></span> <span data-ttu-id="7b76a-263">输入一个静态域，以便在 Zscaler 应用程序中预填充 "登录" 字段。</span><span class="sxs-lookup"><span data-stu-id="7b76a-263">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="7b76a-264">如果保留为空，则将改用用户的 Azure Active Directory 域。</span><span class="sxs-lookup"><span data-stu-id="7b76a-264">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span> <span data-ttu-id="7b76a-265">继承自[iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b76a-265">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="7b76a-266">strictEnforcement</span><span class="sxs-lookup"><span data-stu-id="7b76a-266">strictEnforcement</span></span>|<span data-ttu-id="7b76a-267">布尔</span><span class="sxs-lookup"><span data-stu-id="7b76a-267">Boolean</span></span>|<span data-ttu-id="7b76a-268">仅 Zscaler。</span><span class="sxs-lookup"><span data-stu-id="7b76a-268">Zscaler only.</span></span> <span data-ttu-id="7b76a-269">阻止网络流量，直到用户登录到 Zscaler 应用程序。</span><span class="sxs-lookup"><span data-stu-id="7b76a-269">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="7b76a-270">"True" 表示阻止流量。</span><span class="sxs-lookup"><span data-stu-id="7b76a-270">"True" means traffic is blocked.</span></span> <span data-ttu-id="7b76a-271">继承自[iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b76a-271">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="7b76a-272">cloudName</span><span class="sxs-lookup"><span data-stu-id="7b76a-272">cloudName</span></span>|<span data-ttu-id="7b76a-273">String</span><span class="sxs-lookup"><span data-stu-id="7b76a-273">String</span></span>|<span data-ttu-id="7b76a-274">仅 Zscaler。</span><span class="sxs-lookup"><span data-stu-id="7b76a-274">Zscaler only.</span></span> <span data-ttu-id="7b76a-275">用户分配到的 Zscaler 云。</span><span class="sxs-lookup"><span data-stu-id="7b76a-275">Zscaler cloud which the user is assigned to.</span></span> <span data-ttu-id="7b76a-276">继承自[iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b76a-276">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="7b76a-277">excludeList</span><span class="sxs-lookup"><span data-stu-id="7b76a-277">excludeList</span></span>|<span data-ttu-id="7b76a-278">String 集合</span><span class="sxs-lookup"><span data-stu-id="7b76a-278">String collection</span></span>|<span data-ttu-id="7b76a-279">仅 Zscaler。</span><span class="sxs-lookup"><span data-stu-id="7b76a-279">Zscaler only.</span></span> <span data-ttu-id="7b76a-280">不通过 Zscaler 云发送的网络地址的列表。</span><span class="sxs-lookup"><span data-stu-id="7b76a-280">List of network addresses which are not sent through the Zscaler cloud.</span></span> <span data-ttu-id="7b76a-281">继承自[iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b76a-281">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="7b76a-282">childSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="7b76a-282">childSecurityAssociationParameters</span></span>|[<span data-ttu-id="7b76a-283">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="7b76a-283">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="7b76a-284">子安全关联参数</span><span class="sxs-lookup"><span data-stu-id="7b76a-284">Child Security Association Parameters</span></span>|
|<span data-ttu-id="7b76a-285">clientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="7b76a-285">clientAuthenticationType</span></span>|[<span data-ttu-id="7b76a-286">vpnClientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="7b76a-286">vpnClientAuthenticationType</span></span>](../resources/intune-deviceconfig-vpnclientauthenticationtype.md)|<span data-ttu-id="7b76a-287">VPN 客户端将使用的客户端身份验证的类型。</span><span class="sxs-lookup"><span data-stu-id="7b76a-287">Type of Client Authentication the VPN client will use.</span></span> <span data-ttu-id="7b76a-288">可取值为：`userAuthentication`、`deviceAuthentication`。</span><span class="sxs-lookup"><span data-stu-id="7b76a-288">Possible values are: `userAuthentication`, `deviceAuthentication`.</span></span>|
|<span data-ttu-id="7b76a-289">deadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="7b76a-289">deadPeerDetectionRate</span></span>|[<span data-ttu-id="7b76a-290">vpnDeadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="7b76a-290">vpnDeadPeerDetectionRate</span></span>](../resources/intune-deviceconfig-vpndeadpeerdetectionrate.md)|<span data-ttu-id="7b76a-291">确定检查等连接是否仍处于活动状态的频率。</span><span class="sxs-lookup"><span data-stu-id="7b76a-291">Determine how often to check if a peer connection is still active.</span></span> <span data-ttu-id="7b76a-292">.</span><span class="sxs-lookup"><span data-stu-id="7b76a-292">.</span></span> <span data-ttu-id="7b76a-293">可取值为：`medium`、`none`、`low`、`high`。</span><span class="sxs-lookup"><span data-stu-id="7b76a-293">Possible values are: `medium`, `none`, `low`, `high`.</span></span>|
|<span data-ttu-id="7b76a-294">disableMobilityAndMultihoming</span><span class="sxs-lookup"><span data-stu-id="7b76a-294">disableMobilityAndMultihoming</span></span>|<span data-ttu-id="7b76a-295">布尔</span><span class="sxs-lookup"><span data-stu-id="7b76a-295">Boolean</span></span>|<span data-ttu-id="7b76a-296">禁用 MOBIKE</span><span class="sxs-lookup"><span data-stu-id="7b76a-296">Disable MOBIKE</span></span>|
|<span data-ttu-id="7b76a-297">disableRedirect</span><span class="sxs-lookup"><span data-stu-id="7b76a-297">disableRedirect</span></span>|<span data-ttu-id="7b76a-298">布尔</span><span class="sxs-lookup"><span data-stu-id="7b76a-298">Boolean</span></span>|<span data-ttu-id="7b76a-299">禁用重定向</span><span class="sxs-lookup"><span data-stu-id="7b76a-299">Disable Redirect</span></span>|
|<span data-ttu-id="7b76a-300">enableCertificateRevocationCheck</span><span class="sxs-lookup"><span data-stu-id="7b76a-300">enableCertificateRevocationCheck</span></span>|<span data-ttu-id="7b76a-301">布尔</span><span class="sxs-lookup"><span data-stu-id="7b76a-301">Boolean</span></span>|<span data-ttu-id="7b76a-302">启用尽力吊销检查;服务器响应超时不会导致它失败</span><span class="sxs-lookup"><span data-stu-id="7b76a-302">Enables a best-effort revocation check; server response timeouts will not cause it to fail</span></span>|
|<span data-ttu-id="7b76a-303">enableEAP</span><span class="sxs-lookup"><span data-stu-id="7b76a-303">enableEAP</span></span>|<span data-ttu-id="7b76a-304">布尔</span><span class="sxs-lookup"><span data-stu-id="7b76a-304">Boolean</span></span>|<span data-ttu-id="7b76a-305">启用仅 EAP 身份验证</span><span class="sxs-lookup"><span data-stu-id="7b76a-305">Enables EAP only authentication</span></span>|
|<span data-ttu-id="7b76a-306">enablePerfectForwardSecrecy</span><span class="sxs-lookup"><span data-stu-id="7b76a-306">enablePerfectForwardSecrecy</span></span>|<span data-ttu-id="7b76a-307">布尔</span><span class="sxs-lookup"><span data-stu-id="7b76a-307">Boolean</span></span>|<span data-ttu-id="7b76a-308">启用完全向前保密（PFS）。</span><span class="sxs-lookup"><span data-stu-id="7b76a-308">Enable Perfect Forward Secrecy (PFS).</span></span>|
|<span data-ttu-id="7b76a-309">enableUseInternalSubnetAttributes</span><span class="sxs-lookup"><span data-stu-id="7b76a-309">enableUseInternalSubnetAttributes</span></span>|<span data-ttu-id="7b76a-310">布尔</span><span class="sxs-lookup"><span data-stu-id="7b76a-310">Boolean</span></span>|<span data-ttu-id="7b76a-311">启用 "使用内部子网属性"。</span><span class="sxs-lookup"><span data-stu-id="7b76a-311">Enable Use Internal Subnet Attributes.</span></span>|
|<span data-ttu-id="7b76a-312">localIdentifier</span><span class="sxs-lookup"><span data-stu-id="7b76a-312">localIdentifier</span></span>|[<span data-ttu-id="7b76a-313">vpnLocalIdentifier</span><span class="sxs-lookup"><span data-stu-id="7b76a-313">vpnLocalIdentifier</span></span>](../resources/intune-deviceconfig-vpnlocalidentifier.md)|<span data-ttu-id="7b76a-314">标识尝试通过 VPN 连接的客户端的方法。</span><span class="sxs-lookup"><span data-stu-id="7b76a-314">Method of identifying the client that is trying to connect via VPN.</span></span> <span data-ttu-id="7b76a-315">.</span><span class="sxs-lookup"><span data-stu-id="7b76a-315">.</span></span> <span data-ttu-id="7b76a-316">可取值为：`deviceFQDN`、`empty`、`clientCertificateSubjectName`。</span><span class="sxs-lookup"><span data-stu-id="7b76a-316">Possible values are: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span></span>|
|<span data-ttu-id="7b76a-317">remoteIdentifier</span><span class="sxs-lookup"><span data-stu-id="7b76a-317">remoteIdentifier</span></span>|<span data-ttu-id="7b76a-318">String</span><span class="sxs-lookup"><span data-stu-id="7b76a-318">String</span></span>|<span data-ttu-id="7b76a-319">IKEv2 服务器的地址。</span><span class="sxs-lookup"><span data-stu-id="7b76a-319">Address of the IKEv2 server.</span></span> <span data-ttu-id="7b76a-320">必须是 FQDN、UserFQDN、网络地址或 ASN1DN</span><span class="sxs-lookup"><span data-stu-id="7b76a-320">Must be a FQDN, UserFQDN, network address, or ASN1DN</span></span>|
|<span data-ttu-id="7b76a-321">securityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="7b76a-321">securityAssociationParameters</span></span>|[<span data-ttu-id="7b76a-322">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="7b76a-322">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="7b76a-323">安全关联参数</span><span class="sxs-lookup"><span data-stu-id="7b76a-323">Security Association Parameters</span></span>|
|<span data-ttu-id="7b76a-324">serverCertificateCommonName</span><span class="sxs-lookup"><span data-stu-id="7b76a-324">serverCertificateCommonName</span></span>|<span data-ttu-id="7b76a-325">String</span><span class="sxs-lookup"><span data-stu-id="7b76a-325">String</span></span>|<span data-ttu-id="7b76a-326">服务器身份验证中使用的 IKEv2 服务器证书的公用名</span><span class="sxs-lookup"><span data-stu-id="7b76a-326">Common name of the IKEv2 Server Certificate used in Server Authentication</span></span>|
|<span data-ttu-id="7b76a-327">serverCertificateIssuerCommonName</span><span class="sxs-lookup"><span data-stu-id="7b76a-327">serverCertificateIssuerCommonName</span></span>|<span data-ttu-id="7b76a-328">String</span><span class="sxs-lookup"><span data-stu-id="7b76a-328">String</span></span>|<span data-ttu-id="7b76a-329">身份验证中使用的 IKEv2 服务器证书颁发者的颁发者公用名称</span><span class="sxs-lookup"><span data-stu-id="7b76a-329">Issuer Common name of the IKEv2 Server Certificate issuer used in Authentication</span></span>|
|<span data-ttu-id="7b76a-330">serverCertificateType</span><span class="sxs-lookup"><span data-stu-id="7b76a-330">serverCertificateType</span></span>|[<span data-ttu-id="7b76a-331">vpnServerCertificateType</span><span class="sxs-lookup"><span data-stu-id="7b76a-331">vpnServerCertificateType</span></span>](../resources/intune-deviceconfig-vpnservercertificatetype.md)|<span data-ttu-id="7b76a-332">VPN 服务器将提供给 VPN 客户端进行身份验证的证书类型。</span><span class="sxs-lookup"><span data-stu-id="7b76a-332">The type of certificate the VPN server will present to the VPN client for authentication.</span></span> <span data-ttu-id="7b76a-333">可取值为：`rsa`、`ecdsa256`、`ecdsa384`、`ecdsa521`。</span><span class="sxs-lookup"><span data-stu-id="7b76a-333">Possible values are: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span></span>|
|<span data-ttu-id="7b76a-334">sharedSecret</span><span class="sxs-lookup"><span data-stu-id="7b76a-334">sharedSecret</span></span>|<span data-ttu-id="7b76a-335">String</span><span class="sxs-lookup"><span data-stu-id="7b76a-335">String</span></span>|<span data-ttu-id="7b76a-336">在选择共享密钥身份验证时使用</span><span class="sxs-lookup"><span data-stu-id="7b76a-336">Used when Shared Secret Authentication is selected</span></span>|
|<span data-ttu-id="7b76a-337">tlsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="7b76a-337">tlsMaximumVersion</span></span>|<span data-ttu-id="7b76a-338">String</span><span class="sxs-lookup"><span data-stu-id="7b76a-338">String</span></span>|<span data-ttu-id="7b76a-339">要与 EAP-TLS 身份验证一起使用的最大 TLS 版本</span><span class="sxs-lookup"><span data-stu-id="7b76a-339">The maximum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="7b76a-340">tlsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="7b76a-340">tlsMinimumVersion</span></span>|<span data-ttu-id="7b76a-341">String</span><span class="sxs-lookup"><span data-stu-id="7b76a-341">String</span></span>|<span data-ttu-id="7b76a-342">与 EAP-TLS 身份验证一起使用的最小 TLS 版本</span><span class="sxs-lookup"><span data-stu-id="7b76a-342">The minimum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="7b76a-343">allowDefaultSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="7b76a-343">allowDefaultSecurityAssociationParameters</span></span>|<span data-ttu-id="7b76a-344">布尔</span><span class="sxs-lookup"><span data-stu-id="7b76a-344">Boolean</span></span>|<span data-ttu-id="7b76a-345">允许使用安全关联参数，具体方法是将所有参数设置为设备的默认值，除非明确指定。</span><span class="sxs-lookup"><span data-stu-id="7b76a-345">Allows the use of security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="7b76a-346">allowDefaultChildSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="7b76a-346">allowDefaultChildSecurityAssociationParameters</span></span>|<span data-ttu-id="7b76a-347">布尔</span><span class="sxs-lookup"><span data-stu-id="7b76a-347">Boolean</span></span>|<span data-ttu-id="7b76a-348">允许使用子安全关联参数，具体方法是将所有参数设置为设备的默认值，除非明确指定。</span><span class="sxs-lookup"><span data-stu-id="7b76a-348">Allows the use of child security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="7b76a-349">alwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="7b76a-349">alwaysOnConfiguration</span></span>|[<span data-ttu-id="7b76a-350">appleVpnAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="7b76a-350">appleVpnAlwaysOnConfiguration</span></span>](../resources/intune-deviceconfig-applevpnalwaysonconfiguration.md)|<span data-ttu-id="7b76a-351">AlwaysOn 配置</span><span class="sxs-lookup"><span data-stu-id="7b76a-351">AlwaysOn Configuration</span></span>|
|<span data-ttu-id="7b76a-352">enableAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="7b76a-352">enableAlwaysOnConfiguration</span></span>|<span data-ttu-id="7b76a-353">布尔</span><span class="sxs-lookup"><span data-stu-id="7b76a-353">Boolean</span></span>|<span data-ttu-id="7b76a-354">确定是否始终启用 VPN</span><span class="sxs-lookup"><span data-stu-id="7b76a-354">Determines if Always on VPN is enabled</span></span>|



## <a name="response"></a><span data-ttu-id="7b76a-355">响应</span><span class="sxs-lookup"><span data-stu-id="7b76a-355">Response</span></span>
<span data-ttu-id="7b76a-356">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7b76a-356">If successful, this method returns a `200 OK` response code and an updated [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b76a-357">示例</span><span class="sxs-lookup"><span data-stu-id="7b76a-357">Example</span></span>

### <a name="request"></a><span data-ttu-id="7b76a-358">请求</span><span class="sxs-lookup"><span data-stu-id="7b76a-358">Request</span></span>
<span data-ttu-id="7b76a-359">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7b76a-359">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7b76a-360">响应</span><span class="sxs-lookup"><span data-stu-id="7b76a-360">Response</span></span>
<span data-ttu-id="7b76a-p139">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7b76a-p139">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





