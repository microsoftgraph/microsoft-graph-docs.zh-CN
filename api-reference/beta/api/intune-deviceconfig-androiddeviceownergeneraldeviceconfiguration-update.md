---
title: 更新 androidDeviceOwnerGeneralDeviceConfiguration
description: 更新 androidDeviceOwnerGeneralDeviceConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0a64994ec79fe60e121d920027576302837bcbaa
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155242"
---
# <a name="update-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="cd558-103">更新 androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="cd558-103">Update androidDeviceOwnerGeneralDeviceConfiguration</span></span>

<span data-ttu-id="cd558-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd558-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cd558-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cd558-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cd558-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cd558-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd558-107">更新 [androidDeviceOwnerGeneralDeviceConfiguration 对象](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="cd558-107">Update the properties of a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cd558-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="cd558-108">Prerequisites</span></span>
<span data-ttu-id="cd558-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cd558-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd558-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="cd558-111">Permission type</span></span>|<span data-ttu-id="cd558-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cd558-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd558-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cd558-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cd558-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd558-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cd558-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cd558-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd558-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cd558-116">Not supported.</span></span>|
|<span data-ttu-id="cd558-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="cd558-117">Application</span></span>|<span data-ttu-id="cd558-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd558-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd558-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cd558-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="cd558-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="cd558-120">Request headers</span></span>
|<span data-ttu-id="cd558-121">标头</span><span class="sxs-lookup"><span data-stu-id="cd558-121">Header</span></span>|<span data-ttu-id="cd558-122">值</span><span class="sxs-lookup"><span data-stu-id="cd558-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cd558-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd558-123">Authorization</span></span>|<span data-ttu-id="cd558-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cd558-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cd558-125">接受</span><span class="sxs-lookup"><span data-stu-id="cd558-125">Accept</span></span>|<span data-ttu-id="cd558-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cd558-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd558-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="cd558-127">Request body</span></span>
<span data-ttu-id="cd558-128">在请求正文中，提供 [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cd558-128">In the request body, supply a JSON representation for the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="cd558-129">下表显示创建 [androidDeviceOwnerGeneralDeviceConfiguration 时所需的属性](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="cd558-129">The following table shows the properties that are required when you create the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="cd558-130">属性</span><span class="sxs-lookup"><span data-stu-id="cd558-130">Property</span></span>|<span data-ttu-id="cd558-131">类型</span><span class="sxs-lookup"><span data-stu-id="cd558-131">Type</span></span>|<span data-ttu-id="cd558-132">说明</span><span class="sxs-lookup"><span data-stu-id="cd558-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd558-133">id</span><span class="sxs-lookup"><span data-stu-id="cd558-133">id</span></span>|<span data-ttu-id="cd558-134">String</span><span class="sxs-lookup"><span data-stu-id="cd558-134">String</span></span>|<span data-ttu-id="cd558-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="cd558-135">Key of the entity.</span></span> <span data-ttu-id="cd558-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd558-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cd558-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cd558-137">lastModifiedDateTime</span></span>|<span data-ttu-id="cd558-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd558-138">DateTimeOffset</span></span>|<span data-ttu-id="cd558-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="cd558-139">DateTime the object was last modified.</span></span> <span data-ttu-id="cd558-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd558-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cd558-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cd558-141">roleScopeTagIds</span></span>|<span data-ttu-id="cd558-142">字符串集合</span><span class="sxs-lookup"><span data-stu-id="cd558-142">String collection</span></span>|<span data-ttu-id="cd558-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="cd558-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="cd558-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd558-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cd558-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="cd558-145">supportsScopeTags</span></span>|<span data-ttu-id="cd558-146">布尔</span><span class="sxs-lookup"><span data-stu-id="cd558-146">Boolean</span></span>|<span data-ttu-id="cd558-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="cd558-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="cd558-148">如果此值为 false 且实体对范围用户不可见，则不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="cd558-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="cd558-149">这适用于在 Silverlight 中创建的旧策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="cd558-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="cd558-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="cd558-150">This property is read-only.</span></span> <span data-ttu-id="cd558-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd558-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cd558-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="cd558-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="cd558-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="cd558-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="cd558-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="cd558-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="cd558-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd558-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cd558-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="cd558-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="cd558-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="cd558-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="cd558-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="cd558-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="cd558-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd558-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cd558-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="cd558-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="cd558-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="cd558-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="cd558-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="cd558-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="cd558-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd558-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cd558-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cd558-164">createdDateTime</span></span>|<span data-ttu-id="cd558-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd558-165">DateTimeOffset</span></span>|<span data-ttu-id="cd558-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="cd558-166">DateTime the object was created.</span></span> <span data-ttu-id="cd558-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd558-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cd558-168">说明</span><span class="sxs-lookup"><span data-stu-id="cd558-168">description</span></span>|<span data-ttu-id="cd558-169">String</span><span class="sxs-lookup"><span data-stu-id="cd558-169">String</span></span>|<span data-ttu-id="cd558-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="cd558-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="cd558-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd558-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cd558-172">displayName</span><span class="sxs-lookup"><span data-stu-id="cd558-172">displayName</span></span>|<span data-ttu-id="cd558-173">String</span><span class="sxs-lookup"><span data-stu-id="cd558-173">String</span></span>|<span data-ttu-id="cd558-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="cd558-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="cd558-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd558-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cd558-176">version</span><span class="sxs-lookup"><span data-stu-id="cd558-176">version</span></span>|<span data-ttu-id="cd558-177">Int32</span><span class="sxs-lookup"><span data-stu-id="cd558-177">Int32</span></span>|<span data-ttu-id="cd558-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="cd558-178">Version of the device configuration.</span></span> <span data-ttu-id="cd558-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd558-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cd558-180">accountsBlockModification</span><span class="sxs-lookup"><span data-stu-id="cd558-180">accountsBlockModification</span></span>|<span data-ttu-id="cd558-181">布尔</span><span class="sxs-lookup"><span data-stu-id="cd558-181">Boolean</span></span>|<span data-ttu-id="cd558-182">指示是否禁用添加或删除帐户。</span><span class="sxs-lookup"><span data-stu-id="cd558-182">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="cd558-183">appsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="cd558-183">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="cd558-184">布尔</span><span class="sxs-lookup"><span data-stu-id="cd558-184">Boolean</span></span>|<span data-ttu-id="cd558-185">指示是否允许用户启用未知源设置。</span><span class="sxs-lookup"><span data-stu-id="cd558-185">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="cd558-186">appsAutoUpdatePolicy</span><span class="sxs-lookup"><span data-stu-id="cd558-186">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="cd558-187">androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="cd558-187">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="cd558-188">指示应用自动更新策略的值。</span><span class="sxs-lookup"><span data-stu-id="cd558-188">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="cd558-189">可取值为：`notConfigured`、`userChoice`、`never`、`wiFiOnly`、`always`。</span><span class="sxs-lookup"><span data-stu-id="cd558-189">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="cd558-190">appsDefaultPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="cd558-190">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="cd558-191">androidDeviceOwnerDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="cd558-191">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="cd558-192">指示运行时权限请求的权限策略（如果未为应用专门定义）。</span><span class="sxs-lookup"><span data-stu-id="cd558-192">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="cd558-193">可取值为：`deviceDefault`、`prompt`、`autoGrant`、`autoDeny`。</span><span class="sxs-lookup"><span data-stu-id="cd558-193">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="cd558-194">appsRecommendSkippingFirstUseHints</span><span class="sxs-lookup"><span data-stu-id="cd558-194">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="cd558-195">布尔</span><span class="sxs-lookup"><span data-stu-id="cd558-195">Boolean</span></span>|<span data-ttu-id="cd558-196">是否推荐所有应用跳过他们可能添加的任何首次使用提示。</span><span class="sxs-lookup"><span data-stu-id="cd558-196">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="cd558-197">bluetoothBlockConfiguration</span><span class="sxs-lookup"><span data-stu-id="cd558-197">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="cd558-198">布尔</span><span class="sxs-lookup"><span data-stu-id="cd558-198">Boolean</span></span>|<span data-ttu-id="cd558-199">指示是否阻止用户配置蓝牙。</span><span class="sxs-lookup"><span data-stu-id="cd558-199">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="cd558-200">bluetoothBlockContactSharing</span><span class="sxs-lookup"><span data-stu-id="cd558-200">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="cd558-201">布尔</span><span class="sxs-lookup"><span data-stu-id="cd558-201">Boolean</span></span>|<span data-ttu-id="cd558-202">指示是否阻止用户通过蓝牙共享联系人。</span><span class="sxs-lookup"><span data-stu-id="cd558-202">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="cd558-203">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="cd558-203">cameraBlocked</span></span>|<span data-ttu-id="cd558-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd558-204">Boolean</span></span>|<span data-ttu-id="cd558-205">指示是否禁用相机的使用。</span><span class="sxs-lookup"><span data-stu-id="cd558-205">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="cd558-206">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="cd558-206">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="cd558-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd558-207">Boolean</span></span>|<span data-ttu-id="cd558-208">指示是否阻止 Wi-Fi 网络共享。</span><span class="sxs-lookup"><span data-stu-id="cd558-208">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="cd558-209">certificateCredentialConfigurationDisabled</span><span class="sxs-lookup"><span data-stu-id="cd558-209">certificateCredentialConfigurationDisabled</span></span>|<span data-ttu-id="cd558-210">布尔</span><span class="sxs-lookup"><span data-stu-id="cd558-210">Boolean</span></span>|<span data-ttu-id="cd558-211">指示是否阻止用户进行任何证书凭据配置。</span><span class="sxs-lookup"><span data-stu-id="cd558-211">Indicates whether or not to block users from any certificate credential configuration.</span></span>|
|<span data-ttu-id="cd558-212">microsoftLauncherConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="cd558-212">microsoftLauncherConfigurationEnabled</span></span>|<span data-ttu-id="cd558-213">布尔</span><span class="sxs-lookup"><span data-stu-id="cd558-213">Boolean</span></span>|<span data-ttu-id="cd558-214">指示是否要配置 Microsoft 启动器。</span><span class="sxs-lookup"><span data-stu-id="cd558-214">Indicates whether or not to you want configure Microsoft Launcher.</span></span>|
|<span data-ttu-id="cd558-215">microsoftLauncherCustomWallpaperEnabled</span><span class="sxs-lookup"><span data-stu-id="cd558-215">microsoftLauncherCustomWallpaperEnabled</span></span>|<span data-ttu-id="cd558-216">布尔</span><span class="sxs-lookup"><span data-stu-id="cd558-216">Boolean</span></span>|<span data-ttu-id="cd558-217">指示是否在目标设备上配置墙纸。</span><span class="sxs-lookup"><span data-stu-id="cd558-217">Indicates whether or not to configure the wallpaper on the targeted devices.</span></span>|
|<span data-ttu-id="cd558-218">microsoftLauncherCustomWallpaperImageUrl</span><span class="sxs-lookup"><span data-stu-id="cd558-218">microsoftLauncherCustomWallpaperImageUrl</span></span>|<span data-ttu-id="cd558-219">String</span><span class="sxs-lookup"><span data-stu-id="cd558-219">String</span></span>|<span data-ttu-id="cd558-220">指示要用作目标设备上墙纸的图像文件的 URL。</span><span class="sxs-lookup"><span data-stu-id="cd558-220">Indicates the URL for the image file to use as the wallpaper on the targeted devices.</span></span>|
|<span data-ttu-id="cd558-221">microsoftLauncherCustomWallpaperAllowUserModification</span><span class="sxs-lookup"><span data-stu-id="cd558-221">microsoftLauncherCustomWallpaperAllowUserModification</span></span>|<span data-ttu-id="cd558-222">布尔</span><span class="sxs-lookup"><span data-stu-id="cd558-222">Boolean</span></span>|<span data-ttu-id="cd558-223">指示用户是否可以修改墙纸以个性化设置其设备。</span><span class="sxs-lookup"><span data-stu-id="cd558-223">Indicates whether or not the user can modify the wallpaper to personalize their device.</span></span>|
|<span data-ttu-id="cd558-224">microsoftLauncherFeedEnabled</span><span class="sxs-lookup"><span data-stu-id="cd558-224">microsoftLauncherFeedEnabled</span></span>|<span data-ttu-id="cd558-225">布尔</span><span class="sxs-lookup"><span data-stu-id="cd558-225">Boolean</span></span>|<span data-ttu-id="cd558-226">指示是否要在设备上启用启动器源。</span><span class="sxs-lookup"><span data-stu-id="cd558-226">Indicates whether or not you want to enable the launcher feed on the device.</span></span>|
|<span data-ttu-id="cd558-227">microsoftLauncherFeedAllowUserModification</span><span class="sxs-lookup"><span data-stu-id="cd558-227">microsoftLauncherFeedAllowUserModification</span></span>|<span data-ttu-id="cd558-228">布尔</span><span class="sxs-lookup"><span data-stu-id="cd558-228">Boolean</span></span>|<span data-ttu-id="cd558-229">指示用户是否可以在设备上修改启动器源。</span><span class="sxs-lookup"><span data-stu-id="cd558-229">Indicates whether or not the user can modify the launcher feed on the device.</span></span>|
|<span data-ttu-id="cd558-230">microsoftLauncherDockPresenceConfiguration</span><span class="sxs-lookup"><span data-stu-id="cd558-230">microsoftLauncherDockPresenceConfiguration</span></span>|[<span data-ttu-id="cd558-231">microsoftLauncherDockPresence</span><span class="sxs-lookup"><span data-stu-id="cd558-231">microsoftLauncherDockPresence</span></span>](../resources/intune-deviceconfig-microsoftlauncherdockpresence.md)|<span data-ttu-id="cd558-232">指示是否要配置设备扩展坞。</span><span class="sxs-lookup"><span data-stu-id="cd558-232">Indicates whether or not you want to configure the device dock.</span></span> <span data-ttu-id="cd558-233">可取值为：`notConfigured`、`show`、`hide`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="cd558-233">Possible values are: `notConfigured`, `show`, `hide`, `disabled`.</span></span>|
|<span data-ttu-id="cd558-234">microsoftLauncherDockPresenceAllowUserModification</span><span class="sxs-lookup"><span data-stu-id="cd558-234">microsoftLauncherDockPresenceAllowUserModification</span></span>|<span data-ttu-id="cd558-235">布尔</span><span class="sxs-lookup"><span data-stu-id="cd558-235">Boolean</span></span>|<span data-ttu-id="cd558-236">指示用户是否可以修改设备上的设备扩展坞配置。</span><span class="sxs-lookup"><span data-stu-id="cd558-236">Indicates whether or not the user can modify the device dock configuration on the device.</span></span>|
|<span data-ttu-id="cd558-237">microsoftLauncherSearchBarPlacementConfiguration</span><span class="sxs-lookup"><span data-stu-id="cd558-237">microsoftLauncherSearchBarPlacementConfiguration</span></span>|[<span data-ttu-id="cd558-238">microsoftLauncherSearchBarPlacement</span><span class="sxs-lookup"><span data-stu-id="cd558-238">microsoftLauncherSearchBarPlacement</span></span>](../resources/intune-deviceconfig-microsoftlaunchersearchbarplacement.md)|<span data-ttu-id="cd558-239">指示设备上搜索栏放置配置。</span><span class="sxs-lookup"><span data-stu-id="cd558-239">Indicates the search bar placement configuration on the device.</span></span> <span data-ttu-id="cd558-240">可取值为：`notConfigured`、`top`、`bottom`、`hide`。</span><span class="sxs-lookup"><span data-stu-id="cd558-240">Possible values are: `notConfigured`, `top`, `bottom`, `hide`.</span></span>|
|<span data-ttu-id="cd558-241">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="cd558-241">enrollmentProfile</span></span>|[<span data-ttu-id="cd558-242">androidDeviceOwnerEnrollmentProfileType</span><span class="sxs-lookup"><span data-stu-id="cd558-242">androidDeviceOwnerEnrollmentProfileType</span></span>](../resources/intune-deviceconfig-androiddeviceownerenrollmentprofiletype.md)|<span data-ttu-id="cd558-243">指示要配置的注册配置文件。</span><span class="sxs-lookup"><span data-stu-id="cd558-243">Indicates which enrollment profile you want to configure.</span></span> <span data-ttu-id="cd558-244">可取值为：`notConfigured`、`dedicatedDevice`、`fullyManaged`。</span><span class="sxs-lookup"><span data-stu-id="cd558-244">Possible values are: `notConfigured`, `dedicatedDevice`, `fullyManaged`.</span></span>|
|<span data-ttu-id="cd558-245">dataRoamingBlocked</span><span class="sxs-lookup"><span data-stu-id="cd558-245">dataRoamingBlocked</span></span>|<span data-ttu-id="cd558-246">布尔</span><span class="sxs-lookup"><span data-stu-id="cd558-246">Boolean</span></span>|<span data-ttu-id="cd558-247">指示是否阻止用户进行数据漫游。</span><span class="sxs-lookup"><span data-stu-id="cd558-247">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="cd558-248">dateTimeConfigurationBlocked</span><span class="sxs-lookup"><span data-stu-id="cd558-248">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="cd558-249">布尔</span><span class="sxs-lookup"><span data-stu-id="cd558-249">Boolean</span></span>|<span data-ttu-id="cd558-250">指示是否阻止用户手动更改设备上的日期或时间</span><span class="sxs-lookup"><span data-stu-id="cd558-250">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="cd558-251">factoryResetDeviceAdministratorEmails</span><span class="sxs-lookup"><span data-stu-id="cd558-251">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="cd558-252">字符串集合</span><span class="sxs-lookup"><span data-stu-id="cd558-252">String collection</span></span>|<span data-ttu-id="cd558-253">在设备恢复出厂设置后需要进行身份验证的 Google 帐户电子邮件列表，才能进行设置。</span><span class="sxs-lookup"><span data-stu-id="cd558-253">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="cd558-254">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="cd558-254">factoryResetBlocked</span></span>|<span data-ttu-id="cd558-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd558-255">Boolean</span></span>|<span data-ttu-id="cd558-256">指示设置中的恢复出厂设置选项是否已禁用。</span><span class="sxs-lookup"><span data-stu-id="cd558-256">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="cd558-257">globalProxy</span><span class="sxs-lookup"><span data-stu-id="cd558-257">globalProxy</span></span>|[<span data-ttu-id="cd558-258">androidDeviceOwnerGlobalProxy</span><span class="sxs-lookup"><span data-stu-id="cd558-258">androidDeviceOwnerGlobalProxy</span></span>](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)|<span data-ttu-id="cd558-259">代理直接通过主机、端口和排除的主机进行设置。</span><span class="sxs-lookup"><span data-stu-id="cd558-259">Proxy is set up directly with host, port and excluded hosts.</span></span>|
|<span data-ttu-id="cd558-260">googleAccountsBlocked</span><span class="sxs-lookup"><span data-stu-id="cd558-260">googleAccountsBlocked</span></span>|<span data-ttu-id="cd558-261">布尔</span><span class="sxs-lookup"><span data-stu-id="cd558-261">Boolean</span></span>|<span data-ttu-id="cd558-262">指示 Google 帐户是否将被阻止。</span><span class="sxs-lookup"><span data-stu-id="cd558-262">Indicates whether or not google accounts will be blocked.</span></span>|
|<span data-ttu-id="cd558-263">kioskCustomizationDeviceSettingsBlocked</span><span class="sxs-lookup"><span data-stu-id="cd558-263">kioskCustomizationDeviceSettingsBlocked</span></span>|<span data-ttu-id="cd558-264">布尔</span><span class="sxs-lookup"><span data-stu-id="cd558-264">Boolean</span></span>|<span data-ttu-id="cd558-265">指示用户是否可以在展台模式下访问设备的"设置"应用。</span><span class="sxs-lookup"><span data-stu-id="cd558-265">Indicates whether a user can access the device's Settings app while in Kiosk Mode.</span></span>|
|<span data-ttu-id="cd558-266">kioskCustomizationPowerButtonActionsBlocked</span><span class="sxs-lookup"><span data-stu-id="cd558-266">kioskCustomizationPowerButtonActionsBlocked</span></span>|<span data-ttu-id="cd558-267">布尔</span><span class="sxs-lookup"><span data-stu-id="cd558-267">Boolean</span></span>|<span data-ttu-id="cd558-268">当用户长时间按展台模式下设备的电源按钮时是否显示电源菜单。</span><span class="sxs-lookup"><span data-stu-id="cd558-268">Whether the power menu is shown when a user long presses the Power button of a device in Kiosk Mode.</span></span>|
|<span data-ttu-id="cd558-269">kioskCustomizationStatusBar</span><span class="sxs-lookup"><span data-stu-id="cd558-269">kioskCustomizationStatusBar</span></span>|[<span data-ttu-id="cd558-270">androidDeviceOwnerKioskCustomizationStatusBar</span><span class="sxs-lookup"><span data-stu-id="cd558-270">androidDeviceOwnerKioskCustomizationStatusBar</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskcustomizationstatusbar.md)|<span data-ttu-id="cd558-271">指示是否在展台模式下禁用系统信息和通知。</span><span class="sxs-lookup"><span data-stu-id="cd558-271">Indicates whether system info and notifications are disabled in Kiosk Mode.</span></span> <span data-ttu-id="cd558-272">可取值为：`notConfigured`、`notificationsAndSystemInfoEnabled`、`systemInfoOnly`。</span><span class="sxs-lookup"><span data-stu-id="cd558-272">Possible values are: `notConfigured`, `notificationsAndSystemInfoEnabled`, `systemInfoOnly`.</span></span>|
|<span data-ttu-id="cd558-273">kioskCustomizationSystemErrorWarnings</span><span class="sxs-lookup"><span data-stu-id="cd558-273">kioskCustomizationSystemErrorWarnings</span></span>|<span data-ttu-id="cd558-274">布尔</span><span class="sxs-lookup"><span data-stu-id="cd558-274">Boolean</span></span>|<span data-ttu-id="cd558-275">指示崩溃或无响应应用的系统错误对话框是否在展台模式下显示。</span><span class="sxs-lookup"><span data-stu-id="cd558-275">Indicates whether system error dialogs for crashed or unresponsive apps are shown in Kiosk Mode.</span></span>|
|<span data-ttu-id="cd558-276">kioskCustomizationSystemNavigation</span><span class="sxs-lookup"><span data-stu-id="cd558-276">kioskCustomizationSystemNavigation</span></span>|[<span data-ttu-id="cd558-277">androidDeviceOwnerKioskCustomizationSystemNavigation</span><span class="sxs-lookup"><span data-stu-id="cd558-277">androidDeviceOwnerKioskCustomizationSystemNavigation</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskcustomizationsystemnavigation.md)|<span data-ttu-id="cd558-278">指示在展台模式下启用的导航功能。</span><span class="sxs-lookup"><span data-stu-id="cd558-278">Indicates which navigation features are enabled in Kiosk Mode.</span></span> <span data-ttu-id="cd558-279">可取值为：`notConfigured`、`navigationEnabled`、`homeButtonOnly`。</span><span class="sxs-lookup"><span data-stu-id="cd558-279">Possible values are: `notConfigured`, `navigationEnabled`, `homeButtonOnly`.</span></span>|
|<span data-ttu-id="cd558-280">kioskModeScreenSaverConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="cd558-280">kioskModeScreenSaverConfigurationEnabled</span></span>|<span data-ttu-id="cd558-281">布尔</span><span class="sxs-lookup"><span data-stu-id="cd558-281">Boolean</span></span>|<span data-ttu-id="cd558-282">是否在展台模式下启用屏幕保护程序模式。</span><span class="sxs-lookup"><span data-stu-id="cd558-282">Whether or not to enable screen saver mode or not in Kiosk Mode.</span></span>|
|<span data-ttu-id="cd558-283">kioskModeScreenSaverImageUrl</span><span class="sxs-lookup"><span data-stu-id="cd558-283">kioskModeScreenSaverImageUrl</span></span>|<span data-ttu-id="cd558-284">String</span><span class="sxs-lookup"><span data-stu-id="cd558-284">String</span></span>|<span data-ttu-id="cd558-285">将在展台模式下作为设备的屏幕保护程序的图像的 URL。</span><span class="sxs-lookup"><span data-stu-id="cd558-285">URL for an image that will be the device's screen saver in Kiosk Mode.</span></span>|
|<span data-ttu-id="cd558-286">kioskModeScreenSaverDisplayTimeInSeconds</span><span class="sxs-lookup"><span data-stu-id="cd558-286">kioskModeScreenSaverDisplayTimeInSeconds</span></span>|<span data-ttu-id="cd558-287">Int32</span><span class="sxs-lookup"><span data-stu-id="cd558-287">Int32</span></span>|<span data-ttu-id="cd558-288">设备将在展台模式下显示屏幕保护程序的秒数。</span><span class="sxs-lookup"><span data-stu-id="cd558-288">The number of seconds that the device will display the screen saver for in Kiosk Mode.</span></span> <span data-ttu-id="cd558-289">有效值为 0 到 9999999</span><span class="sxs-lookup"><span data-stu-id="cd558-289">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="cd558-290">kioskModeScreenSaverStartDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="cd558-290">kioskModeScreenSaverStartDelayInSeconds</span></span>|<span data-ttu-id="cd558-291">Int32</span><span class="sxs-lookup"><span data-stu-id="cd558-291">Int32</span></span>|<span data-ttu-id="cd558-292">在展台模式下显示屏幕保护程序之前，设备需要处于非活动状态的秒数。</span><span class="sxs-lookup"><span data-stu-id="cd558-292">The number of seconds the device needs to be inactive for before the screen saver is shown in Kiosk Mode.</span></span> <span data-ttu-id="cd558-293">有效值 1 到 9999999</span><span class="sxs-lookup"><span data-stu-id="cd558-293">Valid values 1 to 9999999</span></span>|
|<span data-ttu-id="cd558-294">kioskModeScreenSaverDetectMediaDisabled</span><span class="sxs-lookup"><span data-stu-id="cd558-294">kioskModeScreenSaverDetectMediaDisabled</span></span>|<span data-ttu-id="cd558-295">布尔</span><span class="sxs-lookup"><span data-stu-id="cd558-295">Boolean</span></span>|<span data-ttu-id="cd558-296">如果在展台模式下播放音频/视频，设备屏幕是否应该显示屏幕保护程序。</span><span class="sxs-lookup"><span data-stu-id="cd558-296">Whether or not the device screen should show the screen saver if audio/video is playing in Kiosk Mode.</span></span>|
|<span data-ttu-id="cd558-297">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="cd558-297">kioskModeApps</span></span>|<span data-ttu-id="cd558-298">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cd558-298">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="cd558-299">设备在展台模式下时将显示的托管应用列表。</span><span class="sxs-lookup"><span data-stu-id="cd558-299">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="cd558-300">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="cd558-300">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="cd558-301">kioskModeWallpaperUrl</span><span class="sxs-lookup"><span data-stu-id="cd558-301">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="cd558-302">String</span><span class="sxs-lookup"><span data-stu-id="cd558-302">String</span></span>|<span data-ttu-id="cd558-303">设备在展台模式下时用于墙纸的可公开访问图像的 URL。</span><span class="sxs-lookup"><span data-stu-id="cd558-303">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="cd558-304">kioskModeExitCode</span><span class="sxs-lookup"><span data-stu-id="cd558-304">kioskModeExitCode</span></span>|<span data-ttu-id="cd558-305">String</span><span class="sxs-lookup"><span data-stu-id="cd558-305">String</span></span>|<span data-ttu-id="cd558-306">退出代码以允许用户在设备进入展台模式时从展台模式进行转义。</span><span class="sxs-lookup"><span data-stu-id="cd558-306">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="cd558-307">kioskModeVirtualHomeButtonEnabled</span><span class="sxs-lookup"><span data-stu-id="cd558-307">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="cd558-308">布尔</span><span class="sxs-lookup"><span data-stu-id="cd558-308">Boolean</span></span>|<span data-ttu-id="cd558-309">设备在展台模式下时是否显示虚拟主页按钮。</span><span class="sxs-lookup"><span data-stu-id="cd558-309">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="cd558-310">kioskModeVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="cd558-310">kioskModeVirtualHomeButtonType</span></span>|[<span data-ttu-id="cd558-311">androidDeviceOwnerVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="cd558-311">androidDeviceOwnerVirtualHomeButtonType</span></span>](../resources/intune-deviceconfig-androiddeviceownervirtualhomebuttontype.md)|<span data-ttu-id="cd558-312">指示虚拟主页按钮是向上轻扫"开始"按钮还是浮动"主页"按钮。</span><span class="sxs-lookup"><span data-stu-id="cd558-312">Indicates whether the virtual home button is a swipe up home button or a floating home button.</span></span> <span data-ttu-id="cd558-313">可取值为：`notConfigured`、`swipeUp`、`floating`。</span><span class="sxs-lookup"><span data-stu-id="cd558-313">Possible values are: `notConfigured`, `swipeUp`, `floating`.</span></span>|
|<span data-ttu-id="cd558-314">kioskModeBluetoothConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="cd558-314">kioskModeBluetoothConfigurationEnabled</span></span>|<span data-ttu-id="cd558-315">布尔</span><span class="sxs-lookup"><span data-stu-id="cd558-315">Boolean</span></span>|<span data-ttu-id="cd558-316">是否允许用户在展台模式下Bluetooth设置。</span><span class="sxs-lookup"><span data-stu-id="cd558-316">Whether or not to allow a user to configure Bluetooth settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="cd558-317">kioskModeWiFiConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="cd558-317">kioskModeWiFiConfigurationEnabled</span></span>|<span data-ttu-id="cd558-318">布尔</span><span class="sxs-lookup"><span data-stu-id="cd558-318">Boolean</span></span>|<span data-ttu-id="cd558-319">是否允许用户在展台模式下配置Wi-Fi设置。</span><span class="sxs-lookup"><span data-stu-id="cd558-319">Whether or not to allow a user to configure Wi-Fi settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="cd558-320">kioskModeFlashlightConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="cd558-320">kioskModeFlashlightConfigurationEnabled</span></span>|<span data-ttu-id="cd558-321">布尔</span><span class="sxs-lookup"><span data-stu-id="cd558-321">Boolean</span></span>|<span data-ttu-id="cd558-322">是否允许用户在展台模式下使用闪光灯。</span><span class="sxs-lookup"><span data-stu-id="cd558-322">Whether or not to allow a user to use the flashlight in Kiosk Mode.</span></span>|
|<span data-ttu-id="cd558-323">kioskModeMediaVolumeConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="cd558-323">kioskModeMediaVolumeConfigurationEnabled</span></span>|<span data-ttu-id="cd558-324">布尔</span><span class="sxs-lookup"><span data-stu-id="cd558-324">Boolean</span></span>|<span data-ttu-id="cd558-325">是否允许用户在展台模式下更改媒体卷。</span><span class="sxs-lookup"><span data-stu-id="cd558-325">Whether or not to allow a user to change the media volume in Kiosk Mode.</span></span>|
|<span data-ttu-id="cd558-326">kioskModeShowDeviceInfo</span><span class="sxs-lookup"><span data-stu-id="cd558-326">kioskModeShowDeviceInfo</span></span>|<span data-ttu-id="cd558-327">布尔</span><span class="sxs-lookup"><span data-stu-id="cd558-327">Boolean</span></span>|<span data-ttu-id="cd558-328">是否允许用户访问基本设备信息。</span><span class="sxs-lookup"><span data-stu-id="cd558-328">Whether or not to allow a user to access basic device information.</span></span>|
|<span data-ttu-id="cd558-329">kioskModeManagedSettingsEntryDisabled</span><span class="sxs-lookup"><span data-stu-id="cd558-329">kioskModeManagedSettingsEntryDisabled</span></span>|<span data-ttu-id="cd558-330">布尔</span><span class="sxs-lookup"><span data-stu-id="cd558-330">Boolean</span></span>|<span data-ttu-id="cd558-331">是否在展台模式下在托管主屏幕上显示托管设置入口点。</span><span class="sxs-lookup"><span data-stu-id="cd558-331">Whether or not to display the Managed Settings entry point on the managed home screen in Kiosk Mode.</span></span>|
|<span data-ttu-id="cd558-332">kioskModeDebugMenuEasyAccessEnabled</span><span class="sxs-lookup"><span data-stu-id="cd558-332">kioskModeDebugMenuEasyAccessEnabled</span></span>|<span data-ttu-id="cd558-333">布尔</span><span class="sxs-lookup"><span data-stu-id="cd558-333">Boolean</span></span>|<span data-ttu-id="cd558-334">是否允许用户在展台模式下轻松访问调试菜单。</span><span class="sxs-lookup"><span data-stu-id="cd558-334">Whether or not to allow a user to easy access to the debug menu in Kiosk Mode.</span></span>|
|<span data-ttu-id="cd558-335">kioskModeShowAppNotificationBadge</span><span class="sxs-lookup"><span data-stu-id="cd558-335">kioskModeShowAppNotificationBadge</span></span>|<span data-ttu-id="cd558-336">布尔</span><span class="sxs-lookup"><span data-stu-id="cd558-336">Boolean</span></span>|<span data-ttu-id="cd558-337">是否在展台模式下显示应用程序通知锁屏提醒。</span><span class="sxs-lookup"><span data-stu-id="cd558-337">Whether or not to display application notification badges in Kiosk Mode.</span></span>|
|<span data-ttu-id="cd558-338">kioskModeScreenOrientation</span><span class="sxs-lookup"><span data-stu-id="cd558-338">kioskModeScreenOrientation</span></span>|[<span data-ttu-id="cd558-339">androidDeviceOwnerKioskModeScreenOrientation</span><span class="sxs-lookup"><span data-stu-id="cd558-339">androidDeviceOwnerKioskModeScreenOrientation</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskmodescreenorientation.md)|<span data-ttu-id="cd558-340">展台模式下托管主屏幕的屏幕方向配置。</span><span class="sxs-lookup"><span data-stu-id="cd558-340">Screen orientation configuration for managed home screen in Kiosk Mode.</span></span> <span data-ttu-id="cd558-341">可取值为：`notConfigured`、`portrait`、`landscape`、`autoRotate`。</span><span class="sxs-lookup"><span data-stu-id="cd558-341">Possible values are: `notConfigured`, `portrait`, `landscape`, `autoRotate`.</span></span>|
|<span data-ttu-id="cd558-342">kioskModeIconSize</span><span class="sxs-lookup"><span data-stu-id="cd558-342">kioskModeIconSize</span></span>|[<span data-ttu-id="cd558-343">androidDeviceOwnerKioskModeIconSize</span><span class="sxs-lookup"><span data-stu-id="cd558-343">androidDeviceOwnerKioskModeIconSize</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskmodeiconsize.md)|<span data-ttu-id="cd558-344">展台模式下托管主屏幕的图标大小配置。</span><span class="sxs-lookup"><span data-stu-id="cd558-344">Icon size configuration for managed home screen in Kiosk Mode.</span></span> <span data-ttu-id="cd558-345">可取值为：`notConfigured`、`smallest`、`small`、`regular`、`large`、`largest`。</span><span class="sxs-lookup"><span data-stu-id="cd558-345">Possible values are: `notConfigured`, `smallest`, `small`, `regular`, `large`, `largest`.</span></span>|
|<span data-ttu-id="cd558-346">kioskModeFolderIcon</span><span class="sxs-lookup"><span data-stu-id="cd558-346">kioskModeFolderIcon</span></span>|[<span data-ttu-id="cd558-347">androidDeviceOwnerKioskModeFolderIcon</span><span class="sxs-lookup"><span data-stu-id="cd558-347">androidDeviceOwnerKioskModeFolderIcon</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskmodefoldericon.md)|<span data-ttu-id="cd558-348">展台模式下托管主屏幕的文件夹图标配置。</span><span class="sxs-lookup"><span data-stu-id="cd558-348">Folder icon configuration for managed home screen in Kiosk Mode.</span></span> <span data-ttu-id="cd558-349">可取值为：`notConfigured`、`darkSquare`、`darkCircle`、`lightSquare`、`lightCircle`。</span><span class="sxs-lookup"><span data-stu-id="cd558-349">Possible values are: `notConfigured`, `darkSquare`, `darkCircle`, `lightSquare`, `lightCircle`.</span></span>|
|<span data-ttu-id="cd558-350">kioskModeWifiAllowedSsids</span><span class="sxs-lookup"><span data-stu-id="cd558-350">kioskModeWifiAllowedSsids</span></span>|<span data-ttu-id="cd558-351">字符串集合</span><span class="sxs-lookup"><span data-stu-id="cd558-351">String collection</span></span>|<span data-ttu-id="cd558-352">可供用户在展台模式下配置的受限 WIFI SSID 集。</span><span class="sxs-lookup"><span data-stu-id="cd558-352">The restricted set of WIFI SSIDs available for the user to configure in Kiosk Mode.</span></span> <span data-ttu-id="cd558-353">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="cd558-353">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="cd558-354">kioskModeAppOrderEnabled</span><span class="sxs-lookup"><span data-stu-id="cd558-354">kioskModeAppOrderEnabled</span></span>|<span data-ttu-id="cd558-355">布尔</span><span class="sxs-lookup"><span data-stu-id="cd558-355">Boolean</span></span>|<span data-ttu-id="cd558-356">是否在展台模式下启用应用排序。</span><span class="sxs-lookup"><span data-stu-id="cd558-356">Whether or not to enable app ordering in Kiosk Mode.</span></span>|
|<span data-ttu-id="cd558-357">kioskModeAppsInFolderOrderedByName</span><span class="sxs-lookup"><span data-stu-id="cd558-357">kioskModeAppsInFolderOrderedByName</span></span>|<span data-ttu-id="cd558-358">布尔</span><span class="sxs-lookup"><span data-stu-id="cd558-358">Boolean</span></span>|<span data-ttu-id="cd558-359">是否在展台模式下对文件夹中的应用程序进行字母顺序排序。</span><span class="sxs-lookup"><span data-stu-id="cd558-359">Whether or not to alphabetize applications within a folder in Kiosk Mode.</span></span>|
|<span data-ttu-id="cd558-360">kioskModeGridHeight</span><span class="sxs-lookup"><span data-stu-id="cd558-360">kioskModeGridHeight</span></span>|<span data-ttu-id="cd558-361">Int32</span><span class="sxs-lookup"><span data-stu-id="cd558-361">Int32</span></span>|<span data-ttu-id="cd558-362">在展台模式下启用应用排序的托管主屏幕网格的行数。</span><span class="sxs-lookup"><span data-stu-id="cd558-362">Number of rows for Managed Home Screen grid with app ordering enabled in Kiosk Mode.</span></span> <span data-ttu-id="cd558-363">有效值为 1 到 9999999</span><span class="sxs-lookup"><span data-stu-id="cd558-363">Valid values 1 to 9999999</span></span>|
|<span data-ttu-id="cd558-364">kioskModeGridWidth</span><span class="sxs-lookup"><span data-stu-id="cd558-364">kioskModeGridWidth</span></span>|<span data-ttu-id="cd558-365">Int32</span><span class="sxs-lookup"><span data-stu-id="cd558-365">Int32</span></span>|<span data-ttu-id="cd558-366">在展台模式下启用应用排序的托管主屏幕网格的列数。</span><span class="sxs-lookup"><span data-stu-id="cd558-366">Number of columns for Managed Home Screen grid with app ordering enabled in Kiosk Mode.</span></span> <span data-ttu-id="cd558-367">有效值为 1 到 9999999</span><span class="sxs-lookup"><span data-stu-id="cd558-367">Valid values 1 to 9999999</span></span>|
|<span data-ttu-id="cd558-368">kioskModeLockHomeScreen</span><span class="sxs-lookup"><span data-stu-id="cd558-368">kioskModeLockHomeScreen</span></span>|<span data-ttu-id="cd558-369">布尔</span><span class="sxs-lookup"><span data-stu-id="cd558-369">Boolean</span></span>|<span data-ttu-id="cd558-370">是否在展台模式下将主屏幕锁定给最终用户。</span><span class="sxs-lookup"><span data-stu-id="cd558-370">Whether or not to lock home screen to the end user in Kiosk Mode.</span></span>|
|<span data-ttu-id="cd558-371">kioskModeManagedFolders</span><span class="sxs-lookup"><span data-stu-id="cd558-371">kioskModeManagedFolders</span></span>|<span data-ttu-id="cd558-372">[androidDeviceOwnerKioskModeManagedFolder](../resources/intune-deviceconfig-androiddeviceownerkioskmodemanagedfolder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cd558-372">[androidDeviceOwnerKioskModeManagedFolder](../resources/intune-deviceconfig-androiddeviceownerkioskmodemanagedfolder.md) collection</span></span>|<span data-ttu-id="cd558-373">展台模式下设备的托管文件夹列表。</span><span class="sxs-lookup"><span data-stu-id="cd558-373">A list of managed folders for a device in Kiosk Mode.</span></span> <span data-ttu-id="cd558-374">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="cd558-374">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="cd558-375">kioskModeAppPositions</span><span class="sxs-lookup"><span data-stu-id="cd558-375">kioskModeAppPositions</span></span>|<span data-ttu-id="cd558-376">[androidDeviceOwnerKioskModeAppPositionItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodeapppositionitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cd558-376">[androidDeviceOwnerKioskModeAppPositionItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodeapppositionitem.md) collection</span></span>|<span data-ttu-id="cd558-377">展台模式托管主屏幕上项目的排序。</span><span class="sxs-lookup"><span data-stu-id="cd558-377">The ordering of items on Kiosk Mode Managed Home Screen.</span></span> <span data-ttu-id="cd558-378">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="cd558-378">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="cd558-379">microphoneForceMute</span><span class="sxs-lookup"><span data-stu-id="cd558-379">microphoneForceMute</span></span>|<span data-ttu-id="cd558-380">布尔</span><span class="sxs-lookup"><span data-stu-id="cd558-380">Boolean</span></span>|<span data-ttu-id="cd558-381">指示是否阻止取消设备上麦克风的静音。</span><span class="sxs-lookup"><span data-stu-id="cd558-381">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="cd558-382">networkEscapeHatchAllowed</span><span class="sxs-lookup"><span data-stu-id="cd558-382">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="cd558-383">布尔</span><span class="sxs-lookup"><span data-stu-id="cd558-383">Boolean</span></span>|<span data-ttu-id="cd558-384">指示设备是否允许在启动时连接到临时网络连接。</span><span class="sxs-lookup"><span data-stu-id="cd558-384">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="cd558-385">nfcBlockOutgoingBeam</span><span class="sxs-lookup"><span data-stu-id="cd558-385">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="cd558-386">布尔</span><span class="sxs-lookup"><span data-stu-id="cd558-386">Boolean</span></span>|<span data-ttu-id="cd558-387">指示是否阻止 NFC 传出灯。</span><span class="sxs-lookup"><span data-stu-id="cd558-387">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="cd558-388">passwordBlockKeyguard</span><span class="sxs-lookup"><span data-stu-id="cd558-388">passwordBlockKeyguard</span></span>|<span data-ttu-id="cd558-389">布尔</span><span class="sxs-lookup"><span data-stu-id="cd558-389">Boolean</span></span>|<span data-ttu-id="cd558-390">指示是否已禁用键保护。</span><span class="sxs-lookup"><span data-stu-id="cd558-390">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="cd558-391">passwordBlockKeyguardFeatures</span><span class="sxs-lookup"><span data-stu-id="cd558-391">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="cd558-392">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cd558-392">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="cd558-393">要阻止的设备键盘保护功能列表。</span><span class="sxs-lookup"><span data-stu-id="cd558-393">List of device keyguard features to block.</span></span> <span data-ttu-id="cd558-394">该集合最多可包含 7 个元素。</span><span class="sxs-lookup"><span data-stu-id="cd558-394">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="cd558-395">可取值为：`notConfigured`、`camera`、`notifications`、`unredactedNotifications`、`trustAgents`、`fingerprint`、`remoteInput`、`allFeatures`。</span><span class="sxs-lookup"><span data-stu-id="cd558-395">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="cd558-396">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="cd558-396">passwordExpirationDays</span></span>|<span data-ttu-id="cd558-397">Int32</span><span class="sxs-lookup"><span data-stu-id="cd558-397">Int32</span></span>|<span data-ttu-id="cd558-398">指示密码过期前可以设置密码的时间量，并且需要新密码。</span><span class="sxs-lookup"><span data-stu-id="cd558-398">Indicates the amount of time that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="cd558-399">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="cd558-399">Valid values 1 to 365</span></span>|
|<span data-ttu-id="cd558-400">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="cd558-400">passwordMinimumLength</span></span>|<span data-ttu-id="cd558-401">Int32</span><span class="sxs-lookup"><span data-stu-id="cd558-401">Int32</span></span>|<span data-ttu-id="cd558-402">指示设备上所需的密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="cd558-402">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="cd558-403">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="cd558-403">Valid values 4 to 16</span></span>|
|<span data-ttu-id="cd558-404">passwordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="cd558-404">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="cd558-405">Int32</span><span class="sxs-lookup"><span data-stu-id="cd558-405">Int32</span></span>|<span data-ttu-id="cd558-406">指示设备密码所需的最小字母字符数。</span><span class="sxs-lookup"><span data-stu-id="cd558-406">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="cd558-407">有效值 1 到 16</span><span class="sxs-lookup"><span data-stu-id="cd558-407">Valid values 1 to 16</span></span>|
|<span data-ttu-id="cd558-408">passwordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="cd558-408">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="cd558-409">Int32</span><span class="sxs-lookup"><span data-stu-id="cd558-409">Int32</span></span>|<span data-ttu-id="cd558-410">指示设备密码所需的最小小写字符数。</span><span class="sxs-lookup"><span data-stu-id="cd558-410">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="cd558-411">有效值 1 到 16</span><span class="sxs-lookup"><span data-stu-id="cd558-411">Valid values 1 to 16</span></span>|
|<span data-ttu-id="cd558-412">passwordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="cd558-412">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="cd558-413">Int32</span><span class="sxs-lookup"><span data-stu-id="cd558-413">Int32</span></span>|<span data-ttu-id="cd558-414">指示设备密码所需的最少非字母字符数。</span><span class="sxs-lookup"><span data-stu-id="cd558-414">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="cd558-415">有效值 1 到 16</span><span class="sxs-lookup"><span data-stu-id="cd558-415">Valid values 1 to 16</span></span>|
|<span data-ttu-id="cd558-416">passwordMinimumNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="cd558-416">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="cd558-417">Int32</span><span class="sxs-lookup"><span data-stu-id="cd558-417">Int32</span></span>|<span data-ttu-id="cd558-418">指示设备密码所需的最少数字字符数。</span><span class="sxs-lookup"><span data-stu-id="cd558-418">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="cd558-419">有效值 1 到 16</span><span class="sxs-lookup"><span data-stu-id="cd558-419">Valid values 1 to 16</span></span>|
|<span data-ttu-id="cd558-420">passwordMinimumSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="cd558-420">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="cd558-421">Int32</span><span class="sxs-lookup"><span data-stu-id="cd558-421">Int32</span></span>|<span data-ttu-id="cd558-422">指示设备密码所需的最小符号字符数。</span><span class="sxs-lookup"><span data-stu-id="cd558-422">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="cd558-423">有效值 1 到 16</span><span class="sxs-lookup"><span data-stu-id="cd558-423">Valid values 1 to 16</span></span>|
|<span data-ttu-id="cd558-424">passwordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="cd558-424">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="cd558-425">Int32</span><span class="sxs-lookup"><span data-stu-id="cd558-425">Int32</span></span>|<span data-ttu-id="cd558-426">指示设备密码所需的大写字母字符的最小数目。</span><span class="sxs-lookup"><span data-stu-id="cd558-426">Indicates the minimum number of upper case letter characters required for device password.</span></span> <span data-ttu-id="cd558-427">有效值 1 到 16</span><span class="sxs-lookup"><span data-stu-id="cd558-427">Valid values 1 to 16</span></span>|
|<span data-ttu-id="cd558-428">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="cd558-428">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="cd558-429">Int32</span><span class="sxs-lookup"><span data-stu-id="cd558-429">Int32</span></span>|<span data-ttu-id="cd558-430">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="cd558-430">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="cd558-431">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="cd558-431">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="cd558-432">Int32</span><span class="sxs-lookup"><span data-stu-id="cd558-432">Int32</span></span>|<span data-ttu-id="cd558-433">指示密码历史记录的长度，用户将无法输入与历史记录中任何密码相同的新密码。</span><span class="sxs-lookup"><span data-stu-id="cd558-433">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="cd558-434">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="cd558-434">Valid values 0 to 24</span></span>|
|<span data-ttu-id="cd558-435">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="cd558-435">passwordRequiredType</span></span>|[<span data-ttu-id="cd558-436">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="cd558-436">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="cd558-437">指示设备上所需的最低密码质量。</span><span class="sxs-lookup"><span data-stu-id="cd558-437">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="cd558-438">可取值为：`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`customPassword`。</span><span class="sxs-lookup"><span data-stu-id="cd558-438">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|
|<span data-ttu-id="cd558-439">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="cd558-439">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="cd558-440">Int32</span><span class="sxs-lookup"><span data-stu-id="cd558-440">Int32</span></span>|<span data-ttu-id="cd558-441">指示擦除设备之前，用户可以输入错误密码次数。</span><span class="sxs-lookup"><span data-stu-id="cd558-441">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="cd558-442">有效值为 4 至 11</span><span class="sxs-lookup"><span data-stu-id="cd558-442">Valid values 4 to 11</span></span>|
|<span data-ttu-id="cd558-443">playStoreMode</span><span class="sxs-lookup"><span data-stu-id="cd558-443">playStoreMode</span></span>|[<span data-ttu-id="cd558-444">androidDeviceOwnerPlayStoreMode</span><span class="sxs-lookup"><span data-stu-id="cd558-444">androidDeviceOwnerPlayStoreMode</span></span>](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|<span data-ttu-id="cd558-445">指示设备的 Play Store 模式。</span><span class="sxs-lookup"><span data-stu-id="cd558-445">Indicates the Play Store mode of the device.</span></span> <span data-ttu-id="cd558-446">可取值为：`notConfigured`、`allowList`、`blockList`。</span><span class="sxs-lookup"><span data-stu-id="cd558-446">Possible values are: `notConfigured`, `allowList`, `blockList`.</span></span>|
|<span data-ttu-id="cd558-447">safeBootBlocked</span><span class="sxs-lookup"><span data-stu-id="cd558-447">safeBootBlocked</span></span>|<span data-ttu-id="cd558-448">布尔</span><span class="sxs-lookup"><span data-stu-id="cd558-448">Boolean</span></span>|<span data-ttu-id="cd558-449">指示是否禁用将设备重启到安全启动。</span><span class="sxs-lookup"><span data-stu-id="cd558-449">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="cd558-450">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="cd558-450">screenCaptureBlocked</span></span>|<span data-ttu-id="cd558-451">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd558-451">Boolean</span></span>|<span data-ttu-id="cd558-452">指示是否禁用屏幕截图功能。</span><span class="sxs-lookup"><span data-stu-id="cd558-452">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="cd558-453">securityAllowDebuggingFeatures</span><span class="sxs-lookup"><span data-stu-id="cd558-453">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="cd558-454">布尔</span><span class="sxs-lookup"><span data-stu-id="cd558-454">Boolean</span></span>|<span data-ttu-id="cd558-455">指示是否阻止用户在设备上启用调试功能。</span><span class="sxs-lookup"><span data-stu-id="cd558-455">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="cd558-456">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="cd558-456">securityRequireVerifyApps</span></span>|<span data-ttu-id="cd558-457">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd558-457">Boolean</span></span>|<span data-ttu-id="cd558-458">指示是否需要验证应用。</span><span class="sxs-lookup"><span data-stu-id="cd558-458">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="cd558-459">statusBarBlocked</span><span class="sxs-lookup"><span data-stu-id="cd558-459">statusBarBlocked</span></span>|<span data-ttu-id="cd558-460">布尔</span><span class="sxs-lookup"><span data-stu-id="cd558-460">Boolean</span></span>|<span data-ttu-id="cd558-461">指示是否禁用状态栏，包括通知、快速设置和其他屏幕覆盖。</span><span class="sxs-lookup"><span data-stu-id="cd558-461">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="cd558-462">stayOnModes</span><span class="sxs-lookup"><span data-stu-id="cd558-462">stayOnModes</span></span>|<span data-ttu-id="cd558-463">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cd558-463">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="cd558-464">设备显示器将保持打开状态的模式列表。</span><span class="sxs-lookup"><span data-stu-id="cd558-464">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="cd558-465">此集合最多可包含 4 个元素。</span><span class="sxs-lookup"><span data-stu-id="cd558-465">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="cd558-466">可取值为：`notConfigured`、`ac`、`usb`、`wireless`。</span><span class="sxs-lookup"><span data-stu-id="cd558-466">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="cd558-467">storageAllowUsb</span><span class="sxs-lookup"><span data-stu-id="cd558-467">storageAllowUsb</span></span>|<span data-ttu-id="cd558-468">布尔</span><span class="sxs-lookup"><span data-stu-id="cd558-468">Boolean</span></span>|<span data-ttu-id="cd558-469">指示是否允许 USB 大容量存储。</span><span class="sxs-lookup"><span data-stu-id="cd558-469">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="cd558-470">storageBlockExternalMedia</span><span class="sxs-lookup"><span data-stu-id="cd558-470">storageBlockExternalMedia</span></span>|<span data-ttu-id="cd558-471">布尔</span><span class="sxs-lookup"><span data-stu-id="cd558-471">Boolean</span></span>|<span data-ttu-id="cd558-472">指示是否阻止外部媒体。</span><span class="sxs-lookup"><span data-stu-id="cd558-472">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="cd558-473">storageBlockUsbFileTransfer</span><span class="sxs-lookup"><span data-stu-id="cd558-473">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="cd558-474">布尔</span><span class="sxs-lookup"><span data-stu-id="cd558-474">Boolean</span></span>|<span data-ttu-id="cd558-475">指示是否阻止 USB 文件传输。</span><span class="sxs-lookup"><span data-stu-id="cd558-475">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="cd558-476">systemUpdateWindowStartMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="cd558-476">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="cd558-477">Int32</span><span class="sxs-lookup"><span data-stu-id="cd558-477">Int32</span></span>|<span data-ttu-id="cd558-478">指示系统更新窗口在午夜后启动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="cd558-478">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="cd558-479">有效值为 0 到 1440</span><span class="sxs-lookup"><span data-stu-id="cd558-479">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="cd558-480">systemUpdateWindowEndMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="cd558-480">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="cd558-481">Int32</span><span class="sxs-lookup"><span data-stu-id="cd558-481">Int32</span></span>|<span data-ttu-id="cd558-482">指示系统更新窗口午夜后结束的分钟数。</span><span class="sxs-lookup"><span data-stu-id="cd558-482">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="cd558-483">有效值为 0 到 1440</span><span class="sxs-lookup"><span data-stu-id="cd558-483">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="cd558-484">systemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="cd558-484">systemUpdateInstallType</span></span>|[<span data-ttu-id="cd558-485">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="cd558-485">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="cd558-486">系统更新配置的类型。</span><span class="sxs-lookup"><span data-stu-id="cd558-486">The type of system update configuration.</span></span> <span data-ttu-id="cd558-487">可取值为：`deviceDefault`、`postpone`、`windowed`、`automatic`。</span><span class="sxs-lookup"><span data-stu-id="cd558-487">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="cd558-488">systemWindowsBlocked</span><span class="sxs-lookup"><span data-stu-id="cd558-488">systemWindowsBlocked</span></span>|<span data-ttu-id="cd558-489">布尔</span><span class="sxs-lookup"><span data-stu-id="cd558-489">Boolean</span></span>|<span data-ttu-id="cd558-490">是否阻止 Android 系统提示窗口，如 Toast、手机活动和系统警报。</span><span class="sxs-lookup"><span data-stu-id="cd558-490">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="cd558-491">usersBlockAdd</span><span class="sxs-lookup"><span data-stu-id="cd558-491">usersBlockAdd</span></span>|<span data-ttu-id="cd558-492">布尔</span><span class="sxs-lookup"><span data-stu-id="cd558-492">Boolean</span></span>|<span data-ttu-id="cd558-493">指示是否禁用添加用户和配置文件。</span><span class="sxs-lookup"><span data-stu-id="cd558-493">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="cd558-494">usersBlockRemove</span><span class="sxs-lookup"><span data-stu-id="cd558-494">usersBlockRemove</span></span>|<span data-ttu-id="cd558-495">布尔</span><span class="sxs-lookup"><span data-stu-id="cd558-495">Boolean</span></span>|<span data-ttu-id="cd558-496">指示是否禁用从设备中删除其他用户。</span><span class="sxs-lookup"><span data-stu-id="cd558-496">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="cd558-497">volumeBlockAdjustment</span><span class="sxs-lookup"><span data-stu-id="cd558-497">volumeBlockAdjustment</span></span>|<span data-ttu-id="cd558-498">布尔</span><span class="sxs-lookup"><span data-stu-id="cd558-498">Boolean</span></span>|<span data-ttu-id="cd558-499">指示是否禁用调整主卷。</span><span class="sxs-lookup"><span data-stu-id="cd558-499">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="cd558-500">vpnAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="cd558-500">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="cd558-501">布尔</span><span class="sxs-lookup"><span data-stu-id="cd558-501">Boolean</span></span>|<span data-ttu-id="cd558-502">如果指定了始终启用 VPN 包的名称，是否在断开 VPN 时锁定网络流量。</span><span class="sxs-lookup"><span data-stu-id="cd558-502">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="cd558-503">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="cd558-503">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="cd558-504">String</span><span class="sxs-lookup"><span data-stu-id="cd558-504">String</span></span>|<span data-ttu-id="cd558-505">将处理始终打开 VPN 连接的应用的 Android 应用包名称。</span><span class="sxs-lookup"><span data-stu-id="cd558-505">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="cd558-506">wifiBlockEditConfigurations</span><span class="sxs-lookup"><span data-stu-id="cd558-506">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="cd558-507">布尔</span><span class="sxs-lookup"><span data-stu-id="cd558-507">Boolean</span></span>|<span data-ttu-id="cd558-508">指示是否阻止用户编辑 wifi 连接设置。</span><span class="sxs-lookup"><span data-stu-id="cd558-508">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="cd558-509">wifiBlockEditPolicyDefinedConfigurations</span><span class="sxs-lookup"><span data-stu-id="cd558-509">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="cd558-510">布尔</span><span class="sxs-lookup"><span data-stu-id="cd558-510">Boolean</span></span>|<span data-ttu-id="cd558-511">指示是否阻止用户仅编辑策略定义的网络。</span><span class="sxs-lookup"><span data-stu-id="cd558-511">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|
|<span data-ttu-id="cd558-512">personalProfileAppsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="cd558-512">personalProfileAppsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="cd558-513">布尔</span><span class="sxs-lookup"><span data-stu-id="cd558-513">Boolean</span></span>|<span data-ttu-id="cd558-514">指示用户是否可以在个人配置文件上安装来自未知源的应用。</span><span class="sxs-lookup"><span data-stu-id="cd558-514">Indicates whether the user can install apps from unknown sources on the personal profile.</span></span>|
|<span data-ttu-id="cd558-515">personalProfileCameraBlocked</span><span class="sxs-lookup"><span data-stu-id="cd558-515">personalProfileCameraBlocked</span></span>|<span data-ttu-id="cd558-516">布尔</span><span class="sxs-lookup"><span data-stu-id="cd558-516">Boolean</span></span>|<span data-ttu-id="cd558-517">指示是否禁用对个人配置文件使用相机。</span><span class="sxs-lookup"><span data-stu-id="cd558-517">Indicates whether to disable the use of the camera on the personal profile.</span></span>|
|<span data-ttu-id="cd558-518">personalProfileScreenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="cd558-518">personalProfileScreenCaptureBlocked</span></span>|<span data-ttu-id="cd558-519">布尔</span><span class="sxs-lookup"><span data-stu-id="cd558-519">Boolean</span></span>|<span data-ttu-id="cd558-520">指示是否禁用对个人配置文件进行屏幕截图的功能。</span><span class="sxs-lookup"><span data-stu-id="cd558-520">Indicates whether to disable the capability to take screenshots on the personal profile.</span></span>|
|<span data-ttu-id="cd558-521">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="cd558-521">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="cd558-522">Int32</span><span class="sxs-lookup"><span data-stu-id="cd558-522">Int32</span></span>|<span data-ttu-id="cd558-523">指示工作配置文件密码在过期前可以设置的天数，并且需要新密码。</span><span class="sxs-lookup"><span data-stu-id="cd558-523">Indicates the number of days that a work profile password can be set before it expires and a new password will be required.</span></span> <span data-ttu-id="cd558-524">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="cd558-524">Valid values 1 to 365</span></span>|
|<span data-ttu-id="cd558-525">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="cd558-525">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="cd558-526">Int32</span><span class="sxs-lookup"><span data-stu-id="cd558-526">Int32</span></span>|<span data-ttu-id="cd558-527">指示工作配置文件密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="cd558-527">Indicates the minimum length of the work profile password.</span></span> <span data-ttu-id="cd558-528">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="cd558-528">Valid values 4 to 16</span></span>|
|<span data-ttu-id="cd558-529">workProfilePasswordMinimumNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="cd558-529">workProfilePasswordMinimumNumericCharacters</span></span>|<span data-ttu-id="cd558-530">Int32</span><span class="sxs-lookup"><span data-stu-id="cd558-530">Int32</span></span>|<span data-ttu-id="cd558-531">指示工作配置文件密码所需的最少数字字符数。</span><span class="sxs-lookup"><span data-stu-id="cd558-531">Indicates the minimum number of numeric characters required for the work profile password.</span></span> <span data-ttu-id="cd558-532">有效值 1 到 16</span><span class="sxs-lookup"><span data-stu-id="cd558-532">Valid values 1 to 16</span></span>|
|<span data-ttu-id="cd558-533">workProfilePasswordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="cd558-533">workProfilePasswordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="cd558-534">Int32</span><span class="sxs-lookup"><span data-stu-id="cd558-534">Int32</span></span>|<span data-ttu-id="cd558-535">指示工作配置文件密码所需的最少非字母字符数。</span><span class="sxs-lookup"><span data-stu-id="cd558-535">Indicates the minimum number of non-letter characters required for the work profile password.</span></span> <span data-ttu-id="cd558-536">有效值 1 到 16</span><span class="sxs-lookup"><span data-stu-id="cd558-536">Valid values 1 to 16</span></span>|
|<span data-ttu-id="cd558-537">workProfilePasswordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="cd558-537">workProfilePasswordMinimumLetterCharacters</span></span>|<span data-ttu-id="cd558-538">Int32</span><span class="sxs-lookup"><span data-stu-id="cd558-538">Int32</span></span>|<span data-ttu-id="cd558-539">指示工作配置文件密码所需的最小字母字符数。</span><span class="sxs-lookup"><span data-stu-id="cd558-539">Indicates the minimum number of letter characters required for the work profile password.</span></span> <span data-ttu-id="cd558-540">有效值 1 到 16</span><span class="sxs-lookup"><span data-stu-id="cd558-540">Valid values 1 to 16</span></span>|
|<span data-ttu-id="cd558-541">workProfilePasswordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="cd558-541">workProfilePasswordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="cd558-542">Int32</span><span class="sxs-lookup"><span data-stu-id="cd558-542">Int32</span></span>|<span data-ttu-id="cd558-543">指示工作配置文件密码所需的最小小写字符数。</span><span class="sxs-lookup"><span data-stu-id="cd558-543">Indicates the minimum number of lower-case characters required for the work profile password.</span></span> <span data-ttu-id="cd558-544">有效值 1 到 16</span><span class="sxs-lookup"><span data-stu-id="cd558-544">Valid values 1 to 16</span></span>|
|<span data-ttu-id="cd558-545">workProfilePasswordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="cd558-545">workProfilePasswordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="cd558-546">Int32</span><span class="sxs-lookup"><span data-stu-id="cd558-546">Int32</span></span>|<span data-ttu-id="cd558-547">指示工作配置文件密码所需的最小大写字母字符数。</span><span class="sxs-lookup"><span data-stu-id="cd558-547">Indicates the minimum number of upper-case letter characters required for the work profile password.</span></span> <span data-ttu-id="cd558-548">有效值 1 到 16</span><span class="sxs-lookup"><span data-stu-id="cd558-548">Valid values 1 to 16</span></span>|
|<span data-ttu-id="cd558-549">workProfilePasswordMinimumSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="cd558-549">workProfilePasswordMinimumSymbolCharacters</span></span>|<span data-ttu-id="cd558-550">Int32</span><span class="sxs-lookup"><span data-stu-id="cd558-550">Int32</span></span>|<span data-ttu-id="cd558-551">指示工作配置文件密码所需的最小符号字符数。</span><span class="sxs-lookup"><span data-stu-id="cd558-551">Indicates the minimum number of symbol characters required for the work profile password.</span></span> <span data-ttu-id="cd558-552">有效值 1 到 16</span><span class="sxs-lookup"><span data-stu-id="cd558-552">Valid values 1 to 16</span></span>|
|<span data-ttu-id="cd558-553">workProfilePasswordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="cd558-553">workProfilePasswordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="cd558-554">Int32</span><span class="sxs-lookup"><span data-stu-id="cd558-554">Int32</span></span>|<span data-ttu-id="cd558-555">指示工作配置文件密码历史记录的长度，用户将无法输入与历史记录中任何密码相同的新密码。</span><span class="sxs-lookup"><span data-stu-id="cd558-555">Indicates the length of the work profile password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="cd558-556">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="cd558-556">Valid values 0 to 24</span></span>|
|<span data-ttu-id="cd558-557">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="cd558-557">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="cd558-558">Int32</span><span class="sxs-lookup"><span data-stu-id="cd558-558">Int32</span></span>|<span data-ttu-id="cd558-559">指示擦除设备之前，用户可以输入不正确的工作配置文件密码次数。</span><span class="sxs-lookup"><span data-stu-id="cd558-559">Indicates the number of times a user can enter an incorrect work profile password before the device is wiped.</span></span> <span data-ttu-id="cd558-560">有效值为 4 至 11</span><span class="sxs-lookup"><span data-stu-id="cd558-560">Valid values 4 to 11</span></span>|
|<span data-ttu-id="cd558-561">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="cd558-561">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="cd558-562">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="cd558-562">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="cd558-563">指示工作配置文件密码所需的最低密码质量。</span><span class="sxs-lookup"><span data-stu-id="cd558-563">Indicates the minimum password quality required on the work profile password.</span></span> <span data-ttu-id="cd558-564">可取值为：`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`customPassword`。</span><span class="sxs-lookup"><span data-stu-id="cd558-564">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|



## <a name="response"></a><span data-ttu-id="cd558-565">响应</span><span class="sxs-lookup"><span data-stu-id="cd558-565">Response</span></span>
<span data-ttu-id="cd558-566">如果成功，此方法在响应正文中返回响应代码和更新的 `200 OK` [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cd558-566">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd558-567">示例</span><span class="sxs-lookup"><span data-stu-id="cd558-567">Example</span></span>

### <a name="request"></a><span data-ttu-id="cd558-568">请求</span><span class="sxs-lookup"><span data-stu-id="cd558-568">Request</span></span>
<span data-ttu-id="cd558-569">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cd558-569">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 7313

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
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
  "accountsBlockModification": true,
  "appsAllowInstallFromUnknownSources": true,
  "appsAutoUpdatePolicy": "userChoice",
  "appsDefaultPermissionPolicy": "prompt",
  "appsRecommendSkippingFirstUseHints": true,
  "bluetoothBlockConfiguration": true,
  "bluetoothBlockContactSharing": true,
  "cameraBlocked": true,
  "cellularBlockWiFiTethering": true,
  "certificateCredentialConfigurationDisabled": true,
  "microsoftLauncherConfigurationEnabled": true,
  "microsoftLauncherCustomWallpaperEnabled": true,
  "microsoftLauncherCustomWallpaperImageUrl": "https://example.com/microsoftLauncherCustomWallpaperImageUrl/",
  "microsoftLauncherCustomWallpaperAllowUserModification": true,
  "microsoftLauncherFeedEnabled": true,
  "microsoftLauncherFeedAllowUserModification": true,
  "microsoftLauncherDockPresenceConfiguration": "show",
  "microsoftLauncherDockPresenceAllowUserModification": true,
  "microsoftLauncherSearchBarPlacementConfiguration": "top",
  "enrollmentProfile": "dedicatedDevice",
  "dataRoamingBlocked": true,
  "dateTimeConfigurationBlocked": true,
  "factoryResetDeviceAdministratorEmails": [
    "Factory Reset Device Administrator Emails value"
  ],
  "factoryResetBlocked": true,
  "globalProxy": {
    "@odata.type": "microsoft.graph.androidDeviceOwnerGlobalProxyAutoConfig",
    "proxyAutoConfigURL": "Proxy Auto Config URL value"
  },
  "googleAccountsBlocked": true,
  "kioskCustomizationDeviceSettingsBlocked": true,
  "kioskCustomizationPowerButtonActionsBlocked": true,
  "kioskCustomizationStatusBar": "notificationsAndSystemInfoEnabled",
  "kioskCustomizationSystemErrorWarnings": true,
  "kioskCustomizationSystemNavigation": "navigationEnabled",
  "kioskModeScreenSaverConfigurationEnabled": true,
  "kioskModeScreenSaverImageUrl": "https://example.com/kioskModeScreenSaverImageUrl/",
  "kioskModeScreenSaverDisplayTimeInSeconds": 8,
  "kioskModeScreenSaverStartDelayInSeconds": 7,
  "kioskModeScreenSaverDetectMediaDisabled": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "kioskModeWallpaperUrl": "https://example.com/kioskModeWallpaperUrl/",
  "kioskModeExitCode": "Kiosk Mode Exit Code value",
  "kioskModeVirtualHomeButtonEnabled": true,
  "kioskModeVirtualHomeButtonType": "swipeUp",
  "kioskModeBluetoothConfigurationEnabled": true,
  "kioskModeWiFiConfigurationEnabled": true,
  "kioskModeFlashlightConfigurationEnabled": true,
  "kioskModeMediaVolumeConfigurationEnabled": true,
  "kioskModeShowDeviceInfo": true,
  "kioskModeManagedSettingsEntryDisabled": true,
  "kioskModeDebugMenuEasyAccessEnabled": true,
  "kioskModeShowAppNotificationBadge": true,
  "kioskModeScreenOrientation": "portrait",
  "kioskModeIconSize": "smallest",
  "kioskModeFolderIcon": "darkSquare",
  "kioskModeWifiAllowedSsids": [
    "Kiosk Mode Wifi Allowed Ssids value"
  ],
  "kioskModeAppOrderEnabled": true,
  "kioskModeAppsInFolderOrderedByName": true,
  "kioskModeGridHeight": 3,
  "kioskModeGridWidth": 2,
  "kioskModeLockHomeScreen": true,
  "kioskModeManagedFolders": [
    {
      "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeManagedFolder",
      "folderName": "Folder Name value",
      "folderIdentifier": "Folder Identifier value",
      "items": [
        {
          "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeWeblink",
          "label": "Label value",
          "link": "Link value"
        }
      ]
    }
  ],
  "kioskModeAppPositions": [
    {
      "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeAppPositionItem",
      "position": 8,
      "item": {
        "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeWeblink",
        "label": "Label value",
        "link": "Link value"
      }
    }
  ],
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordBlockKeyguardFeatures": [
    "camera"
  ],
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumLetterCharacters": 15,
  "passwordMinimumLowerCaseCharacters": 2,
  "passwordMinimumNonLetterCharacters": 2,
  "passwordMinimumNumericCharacters": 0,
  "passwordMinimumSymbolCharacters": 15,
  "passwordMinimumUpperCaseCharacters": 2,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordCountToBlock": 4,
  "passwordRequiredType": "required",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "playStoreMode": "allowList",
  "safeBootBlocked": true,
  "screenCaptureBlocked": true,
  "securityAllowDebuggingFeatures": true,
  "securityRequireVerifyApps": true,
  "statusBarBlocked": true,
  "stayOnModes": [
    "ac"
  ],
  "storageAllowUsb": true,
  "storageBlockExternalMedia": true,
  "storageBlockUsbFileTransfer": true,
  "systemUpdateWindowStartMinutesAfterMidnight": 11,
  "systemUpdateWindowEndMinutesAfterMidnight": 9,
  "systemUpdateInstallType": "postpone",
  "systemWindowsBlocked": true,
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "vpnAlwaysOnLockdownMode": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true,
  "personalProfileAppsAllowInstallFromUnknownSources": true,
  "personalProfileCameraBlocked": true,
  "personalProfileScreenCaptureBlocked": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinimumNumericCharacters": 11,
  "workProfilePasswordMinimumNonLetterCharacters": 13,
  "workProfilePasswordMinimumLetterCharacters": 10,
  "workProfilePasswordMinimumLowerCaseCharacters": 13,
  "workProfilePasswordMinimumUpperCaseCharacters": 13,
  "workProfilePasswordMinimumSymbolCharacters": 10,
  "workProfilePasswordPreviousPasswordCountToBlock": 15,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "required"
}
```

### <a name="response"></a><span data-ttu-id="cd558-570">响应</span><span class="sxs-lookup"><span data-stu-id="cd558-570">Response</span></span>
<span data-ttu-id="cd558-p160">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cd558-p160">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 7485

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
  "id": "edad943d-943d-edad-3d94-aded3d94aded",
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
  "accountsBlockModification": true,
  "appsAllowInstallFromUnknownSources": true,
  "appsAutoUpdatePolicy": "userChoice",
  "appsDefaultPermissionPolicy": "prompt",
  "appsRecommendSkippingFirstUseHints": true,
  "bluetoothBlockConfiguration": true,
  "bluetoothBlockContactSharing": true,
  "cameraBlocked": true,
  "cellularBlockWiFiTethering": true,
  "certificateCredentialConfigurationDisabled": true,
  "microsoftLauncherConfigurationEnabled": true,
  "microsoftLauncherCustomWallpaperEnabled": true,
  "microsoftLauncherCustomWallpaperImageUrl": "https://example.com/microsoftLauncherCustomWallpaperImageUrl/",
  "microsoftLauncherCustomWallpaperAllowUserModification": true,
  "microsoftLauncherFeedEnabled": true,
  "microsoftLauncherFeedAllowUserModification": true,
  "microsoftLauncherDockPresenceConfiguration": "show",
  "microsoftLauncherDockPresenceAllowUserModification": true,
  "microsoftLauncherSearchBarPlacementConfiguration": "top",
  "enrollmentProfile": "dedicatedDevice",
  "dataRoamingBlocked": true,
  "dateTimeConfigurationBlocked": true,
  "factoryResetDeviceAdministratorEmails": [
    "Factory Reset Device Administrator Emails value"
  ],
  "factoryResetBlocked": true,
  "globalProxy": {
    "@odata.type": "microsoft.graph.androidDeviceOwnerGlobalProxyAutoConfig",
    "proxyAutoConfigURL": "Proxy Auto Config URL value"
  },
  "googleAccountsBlocked": true,
  "kioskCustomizationDeviceSettingsBlocked": true,
  "kioskCustomizationPowerButtonActionsBlocked": true,
  "kioskCustomizationStatusBar": "notificationsAndSystemInfoEnabled",
  "kioskCustomizationSystemErrorWarnings": true,
  "kioskCustomizationSystemNavigation": "navigationEnabled",
  "kioskModeScreenSaverConfigurationEnabled": true,
  "kioskModeScreenSaverImageUrl": "https://example.com/kioskModeScreenSaverImageUrl/",
  "kioskModeScreenSaverDisplayTimeInSeconds": 8,
  "kioskModeScreenSaverStartDelayInSeconds": 7,
  "kioskModeScreenSaverDetectMediaDisabled": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "kioskModeWallpaperUrl": "https://example.com/kioskModeWallpaperUrl/",
  "kioskModeExitCode": "Kiosk Mode Exit Code value",
  "kioskModeVirtualHomeButtonEnabled": true,
  "kioskModeVirtualHomeButtonType": "swipeUp",
  "kioskModeBluetoothConfigurationEnabled": true,
  "kioskModeWiFiConfigurationEnabled": true,
  "kioskModeFlashlightConfigurationEnabled": true,
  "kioskModeMediaVolumeConfigurationEnabled": true,
  "kioskModeShowDeviceInfo": true,
  "kioskModeManagedSettingsEntryDisabled": true,
  "kioskModeDebugMenuEasyAccessEnabled": true,
  "kioskModeShowAppNotificationBadge": true,
  "kioskModeScreenOrientation": "portrait",
  "kioskModeIconSize": "smallest",
  "kioskModeFolderIcon": "darkSquare",
  "kioskModeWifiAllowedSsids": [
    "Kiosk Mode Wifi Allowed Ssids value"
  ],
  "kioskModeAppOrderEnabled": true,
  "kioskModeAppsInFolderOrderedByName": true,
  "kioskModeGridHeight": 3,
  "kioskModeGridWidth": 2,
  "kioskModeLockHomeScreen": true,
  "kioskModeManagedFolders": [
    {
      "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeManagedFolder",
      "folderName": "Folder Name value",
      "folderIdentifier": "Folder Identifier value",
      "items": [
        {
          "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeWeblink",
          "label": "Label value",
          "link": "Link value"
        }
      ]
    }
  ],
  "kioskModeAppPositions": [
    {
      "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeAppPositionItem",
      "position": 8,
      "item": {
        "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeWeblink",
        "label": "Label value",
        "link": "Link value"
      }
    }
  ],
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordBlockKeyguardFeatures": [
    "camera"
  ],
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumLetterCharacters": 15,
  "passwordMinimumLowerCaseCharacters": 2,
  "passwordMinimumNonLetterCharacters": 2,
  "passwordMinimumNumericCharacters": 0,
  "passwordMinimumSymbolCharacters": 15,
  "passwordMinimumUpperCaseCharacters": 2,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordCountToBlock": 4,
  "passwordRequiredType": "required",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "playStoreMode": "allowList",
  "safeBootBlocked": true,
  "screenCaptureBlocked": true,
  "securityAllowDebuggingFeatures": true,
  "securityRequireVerifyApps": true,
  "statusBarBlocked": true,
  "stayOnModes": [
    "ac"
  ],
  "storageAllowUsb": true,
  "storageBlockExternalMedia": true,
  "storageBlockUsbFileTransfer": true,
  "systemUpdateWindowStartMinutesAfterMidnight": 11,
  "systemUpdateWindowEndMinutesAfterMidnight": 9,
  "systemUpdateInstallType": "postpone",
  "systemWindowsBlocked": true,
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "vpnAlwaysOnLockdownMode": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true,
  "personalProfileAppsAllowInstallFromUnknownSources": true,
  "personalProfileCameraBlocked": true,
  "personalProfileScreenCaptureBlocked": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinimumNumericCharacters": 11,
  "workProfilePasswordMinimumNonLetterCharacters": 13,
  "workProfilePasswordMinimumLetterCharacters": 10,
  "workProfilePasswordMinimumLowerCaseCharacters": 13,
  "workProfilePasswordMinimumUpperCaseCharacters": 13,
  "workProfilePasswordMinimumSymbolCharacters": 10,
  "workProfilePasswordPreviousPasswordCountToBlock": 15,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "required"
}
```




