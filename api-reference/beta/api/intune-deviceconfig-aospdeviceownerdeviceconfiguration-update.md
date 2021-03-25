---
title: 更新 aospDeviceOwnerDeviceConfiguration
description: 更新 aospDeviceOwnerDeviceConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f32f9a6bbd7265260bf937b4d7dde6a06ca516fc
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51155916"
---
# <a name="update-aospdeviceownerdeviceconfiguration"></a><span data-ttu-id="14563-103">更新 aospDeviceOwnerDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="14563-103">Update aospDeviceOwnerDeviceConfiguration</span></span>

<span data-ttu-id="14563-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14563-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="14563-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="14563-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14563-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="14563-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14563-107">更新 [aospDeviceOwnerDeviceConfiguration 对象](../resources/intune-deviceconfig-aospdeviceownerdeviceconfiguration.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="14563-107">Update the properties of a [aospDeviceOwnerDeviceConfiguration](../resources/intune-deviceconfig-aospdeviceownerdeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="14563-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="14563-108">Prerequisites</span></span>
<span data-ttu-id="14563-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="14563-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14563-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="14563-111">Permission type</span></span>|<span data-ttu-id="14563-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="14563-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14563-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="14563-113">Delegated (work or school account)</span></span>|<span data-ttu-id="14563-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14563-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="14563-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="14563-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14563-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="14563-116">Not supported.</span></span>|
|<span data-ttu-id="14563-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="14563-117">Application</span></span>|<span data-ttu-id="14563-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14563-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="14563-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="14563-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="14563-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="14563-120">Request headers</span></span>
|<span data-ttu-id="14563-121">标头</span><span class="sxs-lookup"><span data-stu-id="14563-121">Header</span></span>|<span data-ttu-id="14563-122">值</span><span class="sxs-lookup"><span data-stu-id="14563-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="14563-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="14563-123">Authorization</span></span>|<span data-ttu-id="14563-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="14563-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="14563-125">接受</span><span class="sxs-lookup"><span data-stu-id="14563-125">Accept</span></span>|<span data-ttu-id="14563-126">application/json</span><span class="sxs-lookup"><span data-stu-id="14563-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="14563-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="14563-127">Request body</span></span>
<span data-ttu-id="14563-128">在请求正文中，提供 [aospDeviceOwnerDeviceConfiguration](../resources/intune-deviceconfig-aospdeviceownerdeviceconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="14563-128">In the request body, supply a JSON representation for the [aospDeviceOwnerDeviceConfiguration](../resources/intune-deviceconfig-aospdeviceownerdeviceconfiguration.md) object.</span></span>

<span data-ttu-id="14563-129">下表显示创建 [aospDeviceOwnerDeviceConfiguration 时所需的属性](../resources/intune-deviceconfig-aospdeviceownerdeviceconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="14563-129">The following table shows the properties that are required when you create the [aospDeviceOwnerDeviceConfiguration](../resources/intune-deviceconfig-aospdeviceownerdeviceconfiguration.md).</span></span>

|<span data-ttu-id="14563-130">属性</span><span class="sxs-lookup"><span data-stu-id="14563-130">Property</span></span>|<span data-ttu-id="14563-131">类型</span><span class="sxs-lookup"><span data-stu-id="14563-131">Type</span></span>|<span data-ttu-id="14563-132">说明</span><span class="sxs-lookup"><span data-stu-id="14563-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14563-133">id</span><span class="sxs-lookup"><span data-stu-id="14563-133">id</span></span>|<span data-ttu-id="14563-134">String</span><span class="sxs-lookup"><span data-stu-id="14563-134">String</span></span>|<span data-ttu-id="14563-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="14563-135">Key of the entity.</span></span> <span data-ttu-id="14563-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="14563-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14563-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="14563-137">lastModifiedDateTime</span></span>|<span data-ttu-id="14563-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14563-138">DateTimeOffset</span></span>|<span data-ttu-id="14563-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="14563-139">DateTime the object was last modified.</span></span> <span data-ttu-id="14563-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="14563-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14563-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="14563-141">roleScopeTagIds</span></span>|<span data-ttu-id="14563-142">String collection</span><span class="sxs-lookup"><span data-stu-id="14563-142">String collection</span></span>|<span data-ttu-id="14563-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="14563-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="14563-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="14563-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14563-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="14563-145">supportsScopeTags</span></span>|<span data-ttu-id="14563-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="14563-146">Boolean</span></span>|<span data-ttu-id="14563-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="14563-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="14563-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="14563-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="14563-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="14563-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="14563-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="14563-150">This property is read-only.</span></span> <span data-ttu-id="14563-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="14563-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14563-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="14563-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="14563-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="14563-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="14563-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="14563-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="14563-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="14563-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14563-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="14563-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="14563-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="14563-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="14563-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="14563-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="14563-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="14563-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14563-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="14563-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="14563-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="14563-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="14563-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="14563-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="14563-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="14563-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14563-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="14563-164">createdDateTime</span></span>|<span data-ttu-id="14563-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14563-165">DateTimeOffset</span></span>|<span data-ttu-id="14563-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="14563-166">DateTime the object was created.</span></span> <span data-ttu-id="14563-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="14563-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14563-168">说明</span><span class="sxs-lookup"><span data-stu-id="14563-168">description</span></span>|<span data-ttu-id="14563-169">String</span><span class="sxs-lookup"><span data-stu-id="14563-169">String</span></span>|<span data-ttu-id="14563-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="14563-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="14563-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="14563-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14563-172">displayName</span><span class="sxs-lookup"><span data-stu-id="14563-172">displayName</span></span>|<span data-ttu-id="14563-173">String</span><span class="sxs-lookup"><span data-stu-id="14563-173">String</span></span>|<span data-ttu-id="14563-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="14563-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="14563-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="14563-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14563-176">version</span><span class="sxs-lookup"><span data-stu-id="14563-176">version</span></span>|<span data-ttu-id="14563-177">Int32</span><span class="sxs-lookup"><span data-stu-id="14563-177">Int32</span></span>|<span data-ttu-id="14563-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="14563-178">Version of the device configuration.</span></span> <span data-ttu-id="14563-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="14563-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14563-180">appsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="14563-180">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="14563-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="14563-181">Boolean</span></span>|<span data-ttu-id="14563-182">指示是否允许用户启用未知源设置。</span><span class="sxs-lookup"><span data-stu-id="14563-182">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="14563-183">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="14563-183">bluetoothBlocked</span></span>|<span data-ttu-id="14563-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="14563-184">Boolean</span></span>|<span data-ttu-id="14563-185">指示是否禁用蓝牙的使用。</span><span class="sxs-lookup"><span data-stu-id="14563-185">Indicates whether or not to disable the use of bluetooth.</span></span> <span data-ttu-id="14563-186">设置为 true 时，无法在设备上启用蓝牙。</span><span class="sxs-lookup"><span data-stu-id="14563-186">When set to true, bluetooth cannot be enabled on the device.</span></span>|
|<span data-ttu-id="14563-187">bluetoothBlockConfiguration</span><span class="sxs-lookup"><span data-stu-id="14563-187">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="14563-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="14563-188">Boolean</span></span>|<span data-ttu-id="14563-189">指示是否阻止用户配置蓝牙。</span><span class="sxs-lookup"><span data-stu-id="14563-189">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="14563-190">bluetoothBlockContactSharing</span><span class="sxs-lookup"><span data-stu-id="14563-190">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="14563-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="14563-191">Boolean</span></span>|<span data-ttu-id="14563-192">指示是否阻止用户通过蓝牙共享联系人。</span><span class="sxs-lookup"><span data-stu-id="14563-192">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="14563-193">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="14563-193">cameraBlocked</span></span>|<span data-ttu-id="14563-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="14563-194">Boolean</span></span>|<span data-ttu-id="14563-195">指示是否禁用相机的使用。</span><span class="sxs-lookup"><span data-stu-id="14563-195">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="14563-196">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="14563-196">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="14563-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="14563-197">Boolean</span></span>|<span data-ttu-id="14563-198">指示是否阻止 Wi-Fi 网络共享。</span><span class="sxs-lookup"><span data-stu-id="14563-198">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="14563-199">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="14563-199">factoryResetBlocked</span></span>|<span data-ttu-id="14563-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="14563-200">Boolean</span></span>|<span data-ttu-id="14563-201">指示设置中的恢复出厂设置选项是否已禁用。</span><span class="sxs-lookup"><span data-stu-id="14563-201">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="14563-202">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="14563-202">passwordMinimumLength</span></span>|<span data-ttu-id="14563-203">Int32</span><span class="sxs-lookup"><span data-stu-id="14563-203">Int32</span></span>|<span data-ttu-id="14563-204">指示设备上所需的密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="14563-204">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="14563-205">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="14563-205">Valid values 4 to 16</span></span>|
|<span data-ttu-id="14563-206">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="14563-206">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="14563-207">Int32</span><span class="sxs-lookup"><span data-stu-id="14563-207">Int32</span></span>|<span data-ttu-id="14563-208">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="14563-208">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="14563-209">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="14563-209">passwordRequiredType</span></span>|[<span data-ttu-id="14563-210">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="14563-210">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="14563-211">指示设备上所需的最低密码质量。</span><span class="sxs-lookup"><span data-stu-id="14563-211">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="14563-212">可取值为：`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`customPassword`。</span><span class="sxs-lookup"><span data-stu-id="14563-212">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|
|<span data-ttu-id="14563-213">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="14563-213">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="14563-214">Int32</span><span class="sxs-lookup"><span data-stu-id="14563-214">Int32</span></span>|<span data-ttu-id="14563-215">指示擦除设备之前用户可以输入错误密码次数。</span><span class="sxs-lookup"><span data-stu-id="14563-215">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="14563-216">有效值为 4 至 11</span><span class="sxs-lookup"><span data-stu-id="14563-216">Valid values 4 to 11</span></span>|
|<span data-ttu-id="14563-217">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="14563-217">screenCaptureBlocked</span></span>|<span data-ttu-id="14563-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="14563-218">Boolean</span></span>|<span data-ttu-id="14563-219">指示是否禁用屏幕截图功能。</span><span class="sxs-lookup"><span data-stu-id="14563-219">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="14563-220">securityAllowDebuggingFeatures</span><span class="sxs-lookup"><span data-stu-id="14563-220">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="14563-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="14563-221">Boolean</span></span>|<span data-ttu-id="14563-222">指示是否阻止用户在设备上启用调试功能。</span><span class="sxs-lookup"><span data-stu-id="14563-222">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="14563-223">storageAllowUsb</span><span class="sxs-lookup"><span data-stu-id="14563-223">storageAllowUsb</span></span>|<span data-ttu-id="14563-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="14563-224">Boolean</span></span>|<span data-ttu-id="14563-225">指示是否阻止 USB 存储。</span><span class="sxs-lookup"><span data-stu-id="14563-225">Indicates whether or not to block USB storage.</span></span>|
|<span data-ttu-id="14563-226">storageBlockExternalMedia</span><span class="sxs-lookup"><span data-stu-id="14563-226">storageBlockExternalMedia</span></span>|<span data-ttu-id="14563-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="14563-227">Boolean</span></span>|<span data-ttu-id="14563-228">指示是否阻止外部媒体。</span><span class="sxs-lookup"><span data-stu-id="14563-228">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="14563-229">storageBlockUsbFileTransfer</span><span class="sxs-lookup"><span data-stu-id="14563-229">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="14563-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="14563-230">Boolean</span></span>|<span data-ttu-id="14563-231">指示是否阻止 USB 文件传输。</span><span class="sxs-lookup"><span data-stu-id="14563-231">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="14563-232">backupBlocked</span><span class="sxs-lookup"><span data-stu-id="14563-232">backupBlocked</span></span>|<span data-ttu-id="14563-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="14563-233">Boolean</span></span>|<span data-ttu-id="14563-234">指示是否阻止备份服务。</span><span class="sxs-lookup"><span data-stu-id="14563-234">Indicates whether or not to block backup service.</span></span>|
|<span data-ttu-id="14563-235">wifiBlockEditConfigurations</span><span class="sxs-lookup"><span data-stu-id="14563-235">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="14563-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="14563-236">Boolean</span></span>|<span data-ttu-id="14563-237">指示是否阻止用户编辑 wifi 连接设置。</span><span class="sxs-lookup"><span data-stu-id="14563-237">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|



## <a name="response"></a><span data-ttu-id="14563-238">响应</span><span class="sxs-lookup"><span data-stu-id="14563-238">Response</span></span>
<span data-ttu-id="14563-239">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [aospDeviceOwnerDeviceConfiguration](../resources/intune-deviceconfig-aospdeviceownerdeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="14563-239">If successful, this method returns a `200 OK` response code and an updated [aospDeviceOwnerDeviceConfiguration](../resources/intune-deviceconfig-aospdeviceownerdeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14563-240">示例</span><span class="sxs-lookup"><span data-stu-id="14563-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="14563-241">请求</span><span class="sxs-lookup"><span data-stu-id="14563-241">Request</span></span>
<span data-ttu-id="14563-242">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="14563-242">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="14563-243">响应</span><span class="sxs-lookup"><span data-stu-id="14563-243">Response</span></span>
<span data-ttu-id="14563-p117">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="14563-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




