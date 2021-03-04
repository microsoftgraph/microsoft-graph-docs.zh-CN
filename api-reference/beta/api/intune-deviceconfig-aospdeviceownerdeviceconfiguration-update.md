---
title: 更新 aospDeviceOwnerDeviceConfiguration
description: 更新 aospDeviceOwnerDeviceConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 812aa9a8b3c71cc406365a5170e371aee1cedd84
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445964"
---
# <a name="update-aospdeviceownerdeviceconfiguration"></a><span data-ttu-id="a31d8-103">更新 aospDeviceOwnerDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="a31d8-103">Update aospDeviceOwnerDeviceConfiguration</span></span>

<span data-ttu-id="a31d8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a31d8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a31d8-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a31d8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a31d8-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a31d8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a31d8-107">更新 [aospDeviceOwnerDeviceConfiguration 对象](../resources/intune-deviceconfig-aospdeviceownerdeviceconfiguration.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="a31d8-107">Update the properties of a [aospDeviceOwnerDeviceConfiguration](../resources/intune-deviceconfig-aospdeviceownerdeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a31d8-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a31d8-108">Prerequisites</span></span>
<span data-ttu-id="a31d8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a31d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a31d8-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a31d8-111">Permission type</span></span>|<span data-ttu-id="a31d8-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a31d8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a31d8-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a31d8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a31d8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a31d8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a31d8-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a31d8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a31d8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a31d8-116">Not supported.</span></span>|
|<span data-ttu-id="a31d8-117">Application</span><span class="sxs-lookup"><span data-stu-id="a31d8-117">Application</span></span>|<span data-ttu-id="a31d8-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a31d8-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a31d8-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a31d8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a31d8-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a31d8-120">Request headers</span></span>
|<span data-ttu-id="a31d8-121">标头</span><span class="sxs-lookup"><span data-stu-id="a31d8-121">Header</span></span>|<span data-ttu-id="a31d8-122">值</span><span class="sxs-lookup"><span data-stu-id="a31d8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a31d8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a31d8-123">Authorization</span></span>|<span data-ttu-id="a31d8-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a31d8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a31d8-125">接受</span><span class="sxs-lookup"><span data-stu-id="a31d8-125">Accept</span></span>|<span data-ttu-id="a31d8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a31d8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a31d8-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a31d8-127">Request body</span></span>
<span data-ttu-id="a31d8-128">在请求正文中，提供 [aospDeviceOwnerDeviceConfiguration](../resources/intune-deviceconfig-aospdeviceownerdeviceconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a31d8-128">In the request body, supply a JSON representation for the [aospDeviceOwnerDeviceConfiguration](../resources/intune-deviceconfig-aospdeviceownerdeviceconfiguration.md) object.</span></span>

<span data-ttu-id="a31d8-129">下表显示创建 [aospDeviceOwnerDeviceConfiguration 时所需的属性](../resources/intune-deviceconfig-aospdeviceownerdeviceconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="a31d8-129">The following table shows the properties that are required when you create the [aospDeviceOwnerDeviceConfiguration](../resources/intune-deviceconfig-aospdeviceownerdeviceconfiguration.md).</span></span>

|<span data-ttu-id="a31d8-130">属性</span><span class="sxs-lookup"><span data-stu-id="a31d8-130">Property</span></span>|<span data-ttu-id="a31d8-131">类型</span><span class="sxs-lookup"><span data-stu-id="a31d8-131">Type</span></span>|<span data-ttu-id="a31d8-132">说明</span><span class="sxs-lookup"><span data-stu-id="a31d8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a31d8-133">id</span><span class="sxs-lookup"><span data-stu-id="a31d8-133">id</span></span>|<span data-ttu-id="a31d8-134">String</span><span class="sxs-lookup"><span data-stu-id="a31d8-134">String</span></span>|<span data-ttu-id="a31d8-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a31d8-135">Key of the entity.</span></span> <span data-ttu-id="a31d8-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a31d8-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a31d8-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a31d8-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a31d8-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a31d8-138">DateTimeOffset</span></span>|<span data-ttu-id="a31d8-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a31d8-139">DateTime the object was last modified.</span></span> <span data-ttu-id="a31d8-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a31d8-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a31d8-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a31d8-141">roleScopeTagIds</span></span>|<span data-ttu-id="a31d8-142">字符串集合</span><span class="sxs-lookup"><span data-stu-id="a31d8-142">String collection</span></span>|<span data-ttu-id="a31d8-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="a31d8-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a31d8-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a31d8-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a31d8-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a31d8-145">supportsScopeTags</span></span>|<span data-ttu-id="a31d8-146">布尔</span><span class="sxs-lookup"><span data-stu-id="a31d8-146">Boolean</span></span>|<span data-ttu-id="a31d8-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="a31d8-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a31d8-148">当此值为 false 且实体对范围用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="a31d8-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a31d8-149">对于在 Silverlight 中创建的旧策略，会发生此情况，可通过在 Azure 门户中删除和重新创建策略来解决此问题。</span><span class="sxs-lookup"><span data-stu-id="a31d8-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a31d8-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="a31d8-150">This property is read-only.</span></span> <span data-ttu-id="a31d8-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a31d8-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a31d8-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a31d8-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="a31d8-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a31d8-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="a31d8-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="a31d8-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="a31d8-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a31d8-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a31d8-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a31d8-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="a31d8-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a31d8-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="a31d8-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="a31d8-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="a31d8-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a31d8-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a31d8-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a31d8-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="a31d8-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a31d8-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="a31d8-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="a31d8-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="a31d8-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a31d8-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a31d8-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a31d8-164">createdDateTime</span></span>|<span data-ttu-id="a31d8-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a31d8-165">DateTimeOffset</span></span>|<span data-ttu-id="a31d8-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a31d8-166">DateTime the object was created.</span></span> <span data-ttu-id="a31d8-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a31d8-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a31d8-168">说明</span><span class="sxs-lookup"><span data-stu-id="a31d8-168">description</span></span>|<span data-ttu-id="a31d8-169">String</span><span class="sxs-lookup"><span data-stu-id="a31d8-169">String</span></span>|<span data-ttu-id="a31d8-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="a31d8-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a31d8-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a31d8-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a31d8-172">displayName</span><span class="sxs-lookup"><span data-stu-id="a31d8-172">displayName</span></span>|<span data-ttu-id="a31d8-173">String</span><span class="sxs-lookup"><span data-stu-id="a31d8-173">String</span></span>|<span data-ttu-id="a31d8-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="a31d8-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a31d8-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a31d8-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a31d8-176">version</span><span class="sxs-lookup"><span data-stu-id="a31d8-176">version</span></span>|<span data-ttu-id="a31d8-177">Int32</span><span class="sxs-lookup"><span data-stu-id="a31d8-177">Int32</span></span>|<span data-ttu-id="a31d8-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="a31d8-178">Version of the device configuration.</span></span> <span data-ttu-id="a31d8-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a31d8-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a31d8-180">appsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="a31d8-180">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="a31d8-181">布尔</span><span class="sxs-lookup"><span data-stu-id="a31d8-181">Boolean</span></span>|<span data-ttu-id="a31d8-182">指示是否允许用户启用未知源设置。</span><span class="sxs-lookup"><span data-stu-id="a31d8-182">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="a31d8-183">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="a31d8-183">bluetoothBlocked</span></span>|<span data-ttu-id="a31d8-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="a31d8-184">Boolean</span></span>|<span data-ttu-id="a31d8-185">指示是否禁用蓝牙的使用。</span><span class="sxs-lookup"><span data-stu-id="a31d8-185">Indicates whether or not to disable the use of bluetooth.</span></span> <span data-ttu-id="a31d8-186">设置为 true 时，无法在设备上启用蓝牙。</span><span class="sxs-lookup"><span data-stu-id="a31d8-186">When set to true, bluetooth cannot be enabled on the device.</span></span>|
|<span data-ttu-id="a31d8-187">bluetoothBlockConfiguration</span><span class="sxs-lookup"><span data-stu-id="a31d8-187">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="a31d8-188">布尔</span><span class="sxs-lookup"><span data-stu-id="a31d8-188">Boolean</span></span>|<span data-ttu-id="a31d8-189">指示是否阻止用户配置蓝牙。</span><span class="sxs-lookup"><span data-stu-id="a31d8-189">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="a31d8-190">bluetoothBlockContactSharing</span><span class="sxs-lookup"><span data-stu-id="a31d8-190">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="a31d8-191">布尔</span><span class="sxs-lookup"><span data-stu-id="a31d8-191">Boolean</span></span>|<span data-ttu-id="a31d8-192">指示是否阻止用户通过蓝牙共享联系人。</span><span class="sxs-lookup"><span data-stu-id="a31d8-192">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="a31d8-193">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="a31d8-193">cameraBlocked</span></span>|<span data-ttu-id="a31d8-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="a31d8-194">Boolean</span></span>|<span data-ttu-id="a31d8-195">指示是否禁用相机的使用。</span><span class="sxs-lookup"><span data-stu-id="a31d8-195">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="a31d8-196">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="a31d8-196">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="a31d8-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="a31d8-197">Boolean</span></span>|<span data-ttu-id="a31d8-198">指示是否阻止 Wi-Fi 网络共享。</span><span class="sxs-lookup"><span data-stu-id="a31d8-198">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="a31d8-199">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="a31d8-199">factoryResetBlocked</span></span>|<span data-ttu-id="a31d8-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="a31d8-200">Boolean</span></span>|<span data-ttu-id="a31d8-201">指示是否已禁用设置中的出厂设置重置选项。</span><span class="sxs-lookup"><span data-stu-id="a31d8-201">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="a31d8-202">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="a31d8-202">passwordMinimumLength</span></span>|<span data-ttu-id="a31d8-203">Int32</span><span class="sxs-lookup"><span data-stu-id="a31d8-203">Int32</span></span>|<span data-ttu-id="a31d8-204">指示设备上所需的密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="a31d8-204">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="a31d8-205">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="a31d8-205">Valid values 4 to 16</span></span>|
|<span data-ttu-id="a31d8-206">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="a31d8-206">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="a31d8-207">Int32</span><span class="sxs-lookup"><span data-stu-id="a31d8-207">Int32</span></span>|<span data-ttu-id="a31d8-208">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="a31d8-208">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="a31d8-209">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="a31d8-209">passwordRequiredType</span></span>|[<span data-ttu-id="a31d8-210">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="a31d8-210">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="a31d8-211">指示设备上所需的最低密码质量。</span><span class="sxs-lookup"><span data-stu-id="a31d8-211">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="a31d8-212">可取值为：`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`customPassword`。</span><span class="sxs-lookup"><span data-stu-id="a31d8-212">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|
|<span data-ttu-id="a31d8-213">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="a31d8-213">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="a31d8-214">Int32</span><span class="sxs-lookup"><span data-stu-id="a31d8-214">Int32</span></span>|<span data-ttu-id="a31d8-215">指示擦除设备之前，用户可以输入错误密码次数。</span><span class="sxs-lookup"><span data-stu-id="a31d8-215">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="a31d8-216">有效值为 4 至 11</span><span class="sxs-lookup"><span data-stu-id="a31d8-216">Valid values 4 to 11</span></span>|
|<span data-ttu-id="a31d8-217">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="a31d8-217">screenCaptureBlocked</span></span>|<span data-ttu-id="a31d8-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="a31d8-218">Boolean</span></span>|<span data-ttu-id="a31d8-219">指示是否禁用屏幕截图功能。</span><span class="sxs-lookup"><span data-stu-id="a31d8-219">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="a31d8-220">securityAllowDebuggingFeatures</span><span class="sxs-lookup"><span data-stu-id="a31d8-220">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="a31d8-221">布尔</span><span class="sxs-lookup"><span data-stu-id="a31d8-221">Boolean</span></span>|<span data-ttu-id="a31d8-222">指示是否阻止用户在设备上启用调试功能。</span><span class="sxs-lookup"><span data-stu-id="a31d8-222">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="a31d8-223">storageAllowUsb</span><span class="sxs-lookup"><span data-stu-id="a31d8-223">storageAllowUsb</span></span>|<span data-ttu-id="a31d8-224">布尔</span><span class="sxs-lookup"><span data-stu-id="a31d8-224">Boolean</span></span>|<span data-ttu-id="a31d8-225">指示是否阻止 USB 存储。</span><span class="sxs-lookup"><span data-stu-id="a31d8-225">Indicates whether or not to block USB storage.</span></span>|
|<span data-ttu-id="a31d8-226">storageBlockExternalMedia</span><span class="sxs-lookup"><span data-stu-id="a31d8-226">storageBlockExternalMedia</span></span>|<span data-ttu-id="a31d8-227">布尔</span><span class="sxs-lookup"><span data-stu-id="a31d8-227">Boolean</span></span>|<span data-ttu-id="a31d8-228">指示是否阻止外部媒体。</span><span class="sxs-lookup"><span data-stu-id="a31d8-228">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="a31d8-229">storageBlockUsbFileTransfer</span><span class="sxs-lookup"><span data-stu-id="a31d8-229">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="a31d8-230">布尔</span><span class="sxs-lookup"><span data-stu-id="a31d8-230">Boolean</span></span>|<span data-ttu-id="a31d8-231">指示是否阻止 USB 文件传输。</span><span class="sxs-lookup"><span data-stu-id="a31d8-231">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="a31d8-232">backupBlocked</span><span class="sxs-lookup"><span data-stu-id="a31d8-232">backupBlocked</span></span>|<span data-ttu-id="a31d8-233">布尔</span><span class="sxs-lookup"><span data-stu-id="a31d8-233">Boolean</span></span>|<span data-ttu-id="a31d8-234">指示是否阻止备份服务。</span><span class="sxs-lookup"><span data-stu-id="a31d8-234">Indicates whether or not to block backup service.</span></span>|
|<span data-ttu-id="a31d8-235">wifiBlockEditConfigurations</span><span class="sxs-lookup"><span data-stu-id="a31d8-235">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="a31d8-236">布尔</span><span class="sxs-lookup"><span data-stu-id="a31d8-236">Boolean</span></span>|<span data-ttu-id="a31d8-237">指示是否阻止用户编辑 wifi 连接设置。</span><span class="sxs-lookup"><span data-stu-id="a31d8-237">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|



## <a name="response"></a><span data-ttu-id="a31d8-238">响应</span><span class="sxs-lookup"><span data-stu-id="a31d8-238">Response</span></span>
<span data-ttu-id="a31d8-239">如果成功，此方法在响应正文中返回响应代码和更新的 `200 OK` [aospDeviceOwnerDeviceConfiguration](../resources/intune-deviceconfig-aospdeviceownerdeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a31d8-239">If successful, this method returns a `200 OK` response code and an updated [aospDeviceOwnerDeviceConfiguration](../resources/intune-deviceconfig-aospdeviceownerdeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a31d8-240">示例</span><span class="sxs-lookup"><span data-stu-id="a31d8-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="a31d8-241">请求</span><span class="sxs-lookup"><span data-stu-id="a31d8-241">Request</span></span>
<span data-ttu-id="a31d8-242">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a31d8-242">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1721

{
  "@odata.type": "#microsoft.graph.aospDeviceOwnerDeviceConfiguration",
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
  "appsAllowInstallFromUnknownSources": true,
  "bluetoothBlocked": true,
  "bluetoothBlockConfiguration": true,
  "bluetoothBlockContactSharing": true,
  "cameraBlocked": true,
  "cellularBlockWiFiTethering": true,
  "factoryResetBlocked": true,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordRequiredType": "required",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "screenCaptureBlocked": true,
  "securityAllowDebuggingFeatures": true,
  "storageAllowUsb": true,
  "storageBlockExternalMedia": true,
  "storageBlockUsbFileTransfer": true,
  "backupBlocked": true,
  "wifiBlockEditConfigurations": true
}
```

### <a name="response"></a><span data-ttu-id="a31d8-243">响应</span><span class="sxs-lookup"><span data-stu-id="a31d8-243">Response</span></span>
<span data-ttu-id="a31d8-p117">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a31d8-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1893

{
  "@odata.type": "#microsoft.graph.aospDeviceOwnerDeviceConfiguration",
  "id": "c9e83a69-3a69-c9e8-693a-e8c9693ae8c9",
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
  "appsAllowInstallFromUnknownSources": true,
  "bluetoothBlocked": true,
  "bluetoothBlockConfiguration": true,
  "bluetoothBlockContactSharing": true,
  "cameraBlocked": true,
  "cellularBlockWiFiTethering": true,
  "factoryResetBlocked": true,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordRequiredType": "required",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "screenCaptureBlocked": true,
  "securityAllowDebuggingFeatures": true,
  "storageAllowUsb": true,
  "storageBlockExternalMedia": true,
  "storageBlockUsbFileTransfer": true,
  "backupBlocked": true,
  "wifiBlockEditConfigurations": true
}
```




