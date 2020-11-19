---
title: 更新 androidDeviceOwnerGeneralDeviceConfiguration
description: 更新 androidDeviceOwnerGeneralDeviceConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8a0180d973c1474e1ea9fe9778b98c9bfb03eb52
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49240906"
---
# <a name="update-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="58155-103">更新 androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="58155-103">Update androidDeviceOwnerGeneralDeviceConfiguration</span></span>

<span data-ttu-id="58155-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58155-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="58155-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="58155-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58155-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="58155-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58155-107">更新 [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="58155-107">Update the properties of a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="58155-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="58155-108">Prerequisites</span></span>
<span data-ttu-id="58155-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="58155-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58155-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="58155-111">Permission type</span></span>|<span data-ttu-id="58155-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="58155-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58155-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="58155-113">Delegated (work or school account)</span></span>|<span data-ttu-id="58155-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58155-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="58155-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="58155-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58155-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="58155-116">Not supported.</span></span>|
|<span data-ttu-id="58155-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="58155-117">Application</span></span>|<span data-ttu-id="58155-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58155-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="58155-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="58155-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="58155-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="58155-120">Request headers</span></span>
|<span data-ttu-id="58155-121">标头</span><span class="sxs-lookup"><span data-stu-id="58155-121">Header</span></span>|<span data-ttu-id="58155-122">值</span><span class="sxs-lookup"><span data-stu-id="58155-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58155-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="58155-123">Authorization</span></span>|<span data-ttu-id="58155-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="58155-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58155-125">接受</span><span class="sxs-lookup"><span data-stu-id="58155-125">Accept</span></span>|<span data-ttu-id="58155-126">application/json</span><span class="sxs-lookup"><span data-stu-id="58155-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58155-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="58155-127">Request body</span></span>
<span data-ttu-id="58155-128">在请求正文中，提供 [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="58155-128">In the request body, supply a JSON representation for the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="58155-129">下表显示创建 [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="58155-129">The following table shows the properties that are required when you create the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="58155-130">属性</span><span class="sxs-lookup"><span data-stu-id="58155-130">Property</span></span>|<span data-ttu-id="58155-131">类型</span><span class="sxs-lookup"><span data-stu-id="58155-131">Type</span></span>|<span data-ttu-id="58155-132">说明</span><span class="sxs-lookup"><span data-stu-id="58155-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58155-133">id</span><span class="sxs-lookup"><span data-stu-id="58155-133">id</span></span>|<span data-ttu-id="58155-134">String</span><span class="sxs-lookup"><span data-stu-id="58155-134">String</span></span>|<span data-ttu-id="58155-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="58155-135">Key of the entity.</span></span> <span data-ttu-id="58155-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58155-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58155-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="58155-137">lastModifiedDateTime</span></span>|<span data-ttu-id="58155-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58155-138">DateTimeOffset</span></span>|<span data-ttu-id="58155-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="58155-139">DateTime the object was last modified.</span></span> <span data-ttu-id="58155-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58155-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58155-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="58155-141">roleScopeTagIds</span></span>|<span data-ttu-id="58155-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="58155-142">String collection</span></span>|<span data-ttu-id="58155-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="58155-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="58155-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58155-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58155-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="58155-145">supportsScopeTags</span></span>|<span data-ttu-id="58155-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-146">Boolean</span></span>|<span data-ttu-id="58155-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="58155-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="58155-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="58155-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="58155-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="58155-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="58155-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="58155-150">This property is read-only.</span></span> <span data-ttu-id="58155-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58155-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58155-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="58155-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="58155-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="58155-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="58155-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="58155-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="58155-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58155-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58155-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="58155-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="58155-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="58155-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="58155-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="58155-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="58155-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58155-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58155-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="58155-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="58155-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="58155-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="58155-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="58155-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="58155-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58155-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58155-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="58155-164">createdDateTime</span></span>|<span data-ttu-id="58155-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58155-165">DateTimeOffset</span></span>|<span data-ttu-id="58155-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="58155-166">DateTime the object was created.</span></span> <span data-ttu-id="58155-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58155-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58155-168">description</span><span class="sxs-lookup"><span data-stu-id="58155-168">description</span></span>|<span data-ttu-id="58155-169">String</span><span class="sxs-lookup"><span data-stu-id="58155-169">String</span></span>|<span data-ttu-id="58155-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="58155-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="58155-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58155-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58155-172">displayName</span><span class="sxs-lookup"><span data-stu-id="58155-172">displayName</span></span>|<span data-ttu-id="58155-173">String</span><span class="sxs-lookup"><span data-stu-id="58155-173">String</span></span>|<span data-ttu-id="58155-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="58155-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="58155-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58155-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58155-176">version</span><span class="sxs-lookup"><span data-stu-id="58155-176">version</span></span>|<span data-ttu-id="58155-177">Int32</span><span class="sxs-lookup"><span data-stu-id="58155-177">Int32</span></span>|<span data-ttu-id="58155-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="58155-178">Version of the device configuration.</span></span> <span data-ttu-id="58155-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58155-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58155-180">accountsBlockModification</span><span class="sxs-lookup"><span data-stu-id="58155-180">accountsBlockModification</span></span>|<span data-ttu-id="58155-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-181">Boolean</span></span>|<span data-ttu-id="58155-182">指示是否禁用添加或删除帐户。</span><span class="sxs-lookup"><span data-stu-id="58155-182">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="58155-183">appsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="58155-183">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="58155-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-184">Boolean</span></span>|<span data-ttu-id="58155-185">指示是否允许用户启用 "未知源" 设置。</span><span class="sxs-lookup"><span data-stu-id="58155-185">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="58155-186">appsAutoUpdatePolicy</span><span class="sxs-lookup"><span data-stu-id="58155-186">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="58155-187">androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="58155-187">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="58155-188">指示应用程序自动更新策略的值。</span><span class="sxs-lookup"><span data-stu-id="58155-188">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="58155-189">可取值为：`notConfigured`、`userChoice`、`never`、`wiFiOnly`、`always`。</span><span class="sxs-lookup"><span data-stu-id="58155-189">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="58155-190">appsDefaultPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="58155-190">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="58155-191">androidDeviceOwnerDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="58155-191">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="58155-192">指示对运行时权限请求的权限策略（如果专门没有为应用程序定义）。</span><span class="sxs-lookup"><span data-stu-id="58155-192">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="58155-193">可取值为：`deviceDefault`、`prompt`、`autoGrant`、`autoDeny`。</span><span class="sxs-lookup"><span data-stu-id="58155-193">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="58155-194">appsRecommendSkippingFirstUseHints</span><span class="sxs-lookup"><span data-stu-id="58155-194">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="58155-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-195">Boolean</span></span>|<span data-ttu-id="58155-196">是否建议所有应用都将跳过他们可能已添加的任何首次使用提示。</span><span class="sxs-lookup"><span data-stu-id="58155-196">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="58155-197">bluetoothBlockConfiguration</span><span class="sxs-lookup"><span data-stu-id="58155-197">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="58155-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-198">Boolean</span></span>|<span data-ttu-id="58155-199">指示是否阻止用户配置蓝牙。</span><span class="sxs-lookup"><span data-stu-id="58155-199">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="58155-200">bluetoothBlockContactSharing</span><span class="sxs-lookup"><span data-stu-id="58155-200">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="58155-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-201">Boolean</span></span>|<span data-ttu-id="58155-202">指示是否阻止用户通过蓝牙共享联系人。</span><span class="sxs-lookup"><span data-stu-id="58155-202">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="58155-203">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="58155-203">cameraBlocked</span></span>|<span data-ttu-id="58155-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-204">Boolean</span></span>|<span data-ttu-id="58155-205">指示是否禁用相机的使用。</span><span class="sxs-lookup"><span data-stu-id="58155-205">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="58155-206">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="58155-206">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="58155-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-207">Boolean</span></span>|<span data-ttu-id="58155-208">指示是否阻止 Wi-Fi 网络共享。</span><span class="sxs-lookup"><span data-stu-id="58155-208">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="58155-209">certificateCredentialConfigurationDisabled</span><span class="sxs-lookup"><span data-stu-id="58155-209">certificateCredentialConfigurationDisabled</span></span>|<span data-ttu-id="58155-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-210">Boolean</span></span>|<span data-ttu-id="58155-211">指示是否阻止来自任何证书凭据配置的用户。</span><span class="sxs-lookup"><span data-stu-id="58155-211">Indicates whether or not to block users from any certificate credential configuration.</span></span>|
|<span data-ttu-id="58155-212">microsoftLauncherConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="58155-212">microsoftLauncherConfigurationEnabled</span></span>|<span data-ttu-id="58155-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-213">Boolean</span></span>|<span data-ttu-id="58155-214">指示是否要配置 Microsoft 启动器。</span><span class="sxs-lookup"><span data-stu-id="58155-214">Indicates whether or not to you want configure Microsoft Launcher.</span></span>|
|<span data-ttu-id="58155-215">microsoftLauncherCustomWallpaperEnabled</span><span class="sxs-lookup"><span data-stu-id="58155-215">microsoftLauncherCustomWallpaperEnabled</span></span>|<span data-ttu-id="58155-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-216">Boolean</span></span>|<span data-ttu-id="58155-217">指示是否在目标设备上配置墙纸。</span><span class="sxs-lookup"><span data-stu-id="58155-217">Indicates whether or not to configure the wallpaper on the targeted devices.</span></span>|
|<span data-ttu-id="58155-218">microsoftLauncherCustomWallpaperImageUrl</span><span class="sxs-lookup"><span data-stu-id="58155-218">microsoftLauncherCustomWallpaperImageUrl</span></span>|<span data-ttu-id="58155-219">String</span><span class="sxs-lookup"><span data-stu-id="58155-219">String</span></span>|<span data-ttu-id="58155-220">指示用作目标设备墙纸的图像文件的 URL。</span><span class="sxs-lookup"><span data-stu-id="58155-220">Indicates the URL for the image file to use as the wallpaper on the targeted devices.</span></span>|
|<span data-ttu-id="58155-221">microsoftLauncherCustomWallpaperAllowUserModification</span><span class="sxs-lookup"><span data-stu-id="58155-221">microsoftLauncherCustomWallpaperAllowUserModification</span></span>|<span data-ttu-id="58155-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-222">Boolean</span></span>|<span data-ttu-id="58155-223">指示用户是否可以修改墙纸以个性化设置其设备。</span><span class="sxs-lookup"><span data-stu-id="58155-223">Indicates whether or not the user can modify the wallpaper to personalize their device.</span></span>|
|<span data-ttu-id="58155-224">microsoftLauncherFeedEnabled</span><span class="sxs-lookup"><span data-stu-id="58155-224">microsoftLauncherFeedEnabled</span></span>|<span data-ttu-id="58155-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-225">Boolean</span></span>|<span data-ttu-id="58155-226">指示是否要在设备上启用启动器源。</span><span class="sxs-lookup"><span data-stu-id="58155-226">Indicates whether or not you want to enable the launcher feed on the device.</span></span>|
|<span data-ttu-id="58155-227">microsoftLauncherFeedAllowUserModification</span><span class="sxs-lookup"><span data-stu-id="58155-227">microsoftLauncherFeedAllowUserModification</span></span>|<span data-ttu-id="58155-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-228">Boolean</span></span>|<span data-ttu-id="58155-229">指示用户是否可以修改设备上的启动器源。</span><span class="sxs-lookup"><span data-stu-id="58155-229">Indicates whether or not the user can modify the launcher feed on the device.</span></span>|
|<span data-ttu-id="58155-230">microsoftLauncherDockPresenceConfiguration</span><span class="sxs-lookup"><span data-stu-id="58155-230">microsoftLauncherDockPresenceConfiguration</span></span>|[<span data-ttu-id="58155-231">microsoftLauncherDockPresence</span><span class="sxs-lookup"><span data-stu-id="58155-231">microsoftLauncherDockPresence</span></span>](../resources/intune-deviceconfig-microsoftlauncherdockpresence.md)|<span data-ttu-id="58155-232">指示是否要配置设备停靠。</span><span class="sxs-lookup"><span data-stu-id="58155-232">Indicates whether or not you want to configure the device dock.</span></span> <span data-ttu-id="58155-233">可取值为：`notConfigured`、`show`、`hide`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="58155-233">Possible values are: `notConfigured`, `show`, `hide`, `disabled`.</span></span>|
|<span data-ttu-id="58155-234">microsoftLauncherDockPresenceAllowUserModification</span><span class="sxs-lookup"><span data-stu-id="58155-234">microsoftLauncherDockPresenceAllowUserModification</span></span>|<span data-ttu-id="58155-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-235">Boolean</span></span>|<span data-ttu-id="58155-236">指示用户是否可以修改设备上的设备停靠配置。</span><span class="sxs-lookup"><span data-stu-id="58155-236">Indicates whether or not the user can modify the device dock configuration on the device.</span></span>|
|<span data-ttu-id="58155-237">microsoftLauncherSearchBarPlacementConfiguration</span><span class="sxs-lookup"><span data-stu-id="58155-237">microsoftLauncherSearchBarPlacementConfiguration</span></span>|[<span data-ttu-id="58155-238">microsoftLauncherSearchBarPlacement</span><span class="sxs-lookup"><span data-stu-id="58155-238">microsoftLauncherSearchBarPlacement</span></span>](../resources/intune-deviceconfig-microsoftlaunchersearchbarplacement.md)|<span data-ttu-id="58155-239">指示设备上的搜索栏的布局配置。</span><span class="sxs-lookup"><span data-stu-id="58155-239">Indicates the search bar placement configuration on the device.</span></span> <span data-ttu-id="58155-240">可取值为：`notConfigured`、`top`、`bottom`、`hide`。</span><span class="sxs-lookup"><span data-stu-id="58155-240">Possible values are: `notConfigured`, `top`, `bottom`, `hide`.</span></span>|
|<span data-ttu-id="58155-241">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="58155-241">enrollmentProfile</span></span>|[<span data-ttu-id="58155-242">androidDeviceOwnerEnrollmentProfileType</span><span class="sxs-lookup"><span data-stu-id="58155-242">androidDeviceOwnerEnrollmentProfileType</span></span>](../resources/intune-deviceconfig-androiddeviceownerenrollmentprofiletype.md)|<span data-ttu-id="58155-243">指示要配置的注册配置文件。</span><span class="sxs-lookup"><span data-stu-id="58155-243">Indicates which enrollment profile you want to configure.</span></span> <span data-ttu-id="58155-244">可取值为：`notConfigured`、`dedicatedDevice`、`fullyManaged`。</span><span class="sxs-lookup"><span data-stu-id="58155-244">Possible values are: `notConfigured`, `dedicatedDevice`, `fullyManaged`.</span></span>|
|<span data-ttu-id="58155-245">dataRoamingBlocked</span><span class="sxs-lookup"><span data-stu-id="58155-245">dataRoamingBlocked</span></span>|<span data-ttu-id="58155-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-246">Boolean</span></span>|<span data-ttu-id="58155-247">指示是否阻止用户使用数据漫游。</span><span class="sxs-lookup"><span data-stu-id="58155-247">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="58155-248">dateTimeConfigurationBlocked</span><span class="sxs-lookup"><span data-stu-id="58155-248">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="58155-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-249">Boolean</span></span>|<span data-ttu-id="58155-250">指示是否阻止用户手动更改设备上的日期或时间</span><span class="sxs-lookup"><span data-stu-id="58155-250">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="58155-251">factoryResetDeviceAdministratorEmails</span><span class="sxs-lookup"><span data-stu-id="58155-251">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="58155-252">String 集合</span><span class="sxs-lookup"><span data-stu-id="58155-252">String collection</span></span>|<span data-ttu-id="58155-253">在设备出厂重置之前，将需要进行身份验证的 Google 帐户电子邮件的列表，然后才能对其进行设置。</span><span class="sxs-lookup"><span data-stu-id="58155-253">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="58155-254">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="58155-254">factoryResetBlocked</span></span>|<span data-ttu-id="58155-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-255">Boolean</span></span>|<span data-ttu-id="58155-256">指示是否禁用了 "设置" 中的 "恢复出厂设置" 选项。</span><span class="sxs-lookup"><span data-stu-id="58155-256">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="58155-257">globalProxy</span><span class="sxs-lookup"><span data-stu-id="58155-257">globalProxy</span></span>|[<span data-ttu-id="58155-258">androidDeviceOwnerGlobalProxy</span><span class="sxs-lookup"><span data-stu-id="58155-258">androidDeviceOwnerGlobalProxy</span></span>](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)|<span data-ttu-id="58155-259">代理是与主机、端口和已排除的主机直接建立的。</span><span class="sxs-lookup"><span data-stu-id="58155-259">Proxy is set up directly with host, port and excluded hosts.</span></span>|
|<span data-ttu-id="58155-260">googleAccountsBlocked</span><span class="sxs-lookup"><span data-stu-id="58155-260">googleAccountsBlocked</span></span>|<span data-ttu-id="58155-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-261">Boolean</span></span>|<span data-ttu-id="58155-262">指示是否将阻止 google 帐户。</span><span class="sxs-lookup"><span data-stu-id="58155-262">Indicates whether or not google accounts will be blocked.</span></span>|
|<span data-ttu-id="58155-263">kioskCustomizationDeviceSettingsBlocked</span><span class="sxs-lookup"><span data-stu-id="58155-263">kioskCustomizationDeviceSettingsBlocked</span></span>|<span data-ttu-id="58155-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-264">Boolean</span></span>|<span data-ttu-id="58155-265">指示用户是否可以在展台模式下访问设备的 "设置" 应用程序。</span><span class="sxs-lookup"><span data-stu-id="58155-265">Indicates whether a user can access the device's Settings app while in Kiosk Mode.</span></span>|
|<span data-ttu-id="58155-266">kioskCustomizationPowerButtonActionsBlocked</span><span class="sxs-lookup"><span data-stu-id="58155-266">kioskCustomizationPowerButtonActionsBlocked</span></span>|<span data-ttu-id="58155-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-267">Boolean</span></span>|<span data-ttu-id="58155-268">用户长按展台模式下设备的电源按钮时是否显示电源菜单。</span><span class="sxs-lookup"><span data-stu-id="58155-268">Whether the power menu is shown when a user long presses the Power button of a device in Kiosk Mode.</span></span>|
|<span data-ttu-id="58155-269">kioskCustomizationStatusBar</span><span class="sxs-lookup"><span data-stu-id="58155-269">kioskCustomizationStatusBar</span></span>|[<span data-ttu-id="58155-270">androidDeviceOwnerKioskCustomizationStatusBar</span><span class="sxs-lookup"><span data-stu-id="58155-270">androidDeviceOwnerKioskCustomizationStatusBar</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskcustomizationstatusbar.md)|<span data-ttu-id="58155-271">指示是否在展台模式下禁用系统信息和通知。</span><span class="sxs-lookup"><span data-stu-id="58155-271">Indicates whether system info and notifications are disabled in Kiosk Mode.</span></span> <span data-ttu-id="58155-272">可取值为：`notConfigured`、`notificationsAndSystemInfoEnabled`、`systemInfoOnly`。</span><span class="sxs-lookup"><span data-stu-id="58155-272">Possible values are: `notConfigured`, `notificationsAndSystemInfoEnabled`, `systemInfoOnly`.</span></span>|
|<span data-ttu-id="58155-273">kioskCustomizationSystemErrorWarnings</span><span class="sxs-lookup"><span data-stu-id="58155-273">kioskCustomizationSystemErrorWarnings</span></span>|<span data-ttu-id="58155-274">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-274">Boolean</span></span>|<span data-ttu-id="58155-275">指示在展台模式下是否显示崩溃的或未响应的应用程序的系统错误对话框。</span><span class="sxs-lookup"><span data-stu-id="58155-275">Indicates whether system error dialogs for crashed or unresponsive apps are shown in Kiosk Mode.</span></span>|
|<span data-ttu-id="58155-276">kioskCustomizationSystemNavigation</span><span class="sxs-lookup"><span data-stu-id="58155-276">kioskCustomizationSystemNavigation</span></span>|[<span data-ttu-id="58155-277">androidDeviceOwnerKioskCustomizationSystemNavigation</span><span class="sxs-lookup"><span data-stu-id="58155-277">androidDeviceOwnerKioskCustomizationSystemNavigation</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskcustomizationsystemnavigation.md)|<span data-ttu-id="58155-278">指示在展台模式下启用的导航功能。</span><span class="sxs-lookup"><span data-stu-id="58155-278">Indicates which navigation features are enabled in Kiosk Mode.</span></span> <span data-ttu-id="58155-279">可取值为：`notConfigured`、`navigationEnabled`、`homeButtonOnly`。</span><span class="sxs-lookup"><span data-stu-id="58155-279">Possible values are: `notConfigured`, `navigationEnabled`, `homeButtonOnly`.</span></span>|
|<span data-ttu-id="58155-280">kioskModeScreenSaverConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="58155-280">kioskModeScreenSaverConfigurationEnabled</span></span>|<span data-ttu-id="58155-281">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-281">Boolean</span></span>|<span data-ttu-id="58155-282">是否启用屏幕保护程序模式或不启用展台模式。</span><span class="sxs-lookup"><span data-stu-id="58155-282">Whether or not to enable screen saver mode or not in Kiosk Mode.</span></span>|
|<span data-ttu-id="58155-283">kioskModeScreenSaverImageUrl</span><span class="sxs-lookup"><span data-stu-id="58155-283">kioskModeScreenSaverImageUrl</span></span>|<span data-ttu-id="58155-284">String</span><span class="sxs-lookup"><span data-stu-id="58155-284">String</span></span>|<span data-ttu-id="58155-285">将作为展台模式下设备的屏幕保护程序的图像的 URL。</span><span class="sxs-lookup"><span data-stu-id="58155-285">URL for an image that will be the device's screen saver in Kiosk Mode.</span></span>|
|<span data-ttu-id="58155-286">kioskModeScreenSaverDisplayTimeInSeconds</span><span class="sxs-lookup"><span data-stu-id="58155-286">kioskModeScreenSaverDisplayTimeInSeconds</span></span>|<span data-ttu-id="58155-287">Int32</span><span class="sxs-lookup"><span data-stu-id="58155-287">Int32</span></span>|<span data-ttu-id="58155-288">设备将在展台模式下显示屏幕保护程序的秒数。</span><span class="sxs-lookup"><span data-stu-id="58155-288">The number of seconds that the device will display the screen saver for in Kiosk Mode.</span></span> <span data-ttu-id="58155-289">有效值为0至9999999</span><span class="sxs-lookup"><span data-stu-id="58155-289">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="58155-290">kioskModeScreenSaverStartDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="58155-290">kioskModeScreenSaverStartDelayInSeconds</span></span>|<span data-ttu-id="58155-291">Int32</span><span class="sxs-lookup"><span data-stu-id="58155-291">Int32</span></span>|<span data-ttu-id="58155-292">在 Kiosk 模式下显示屏幕保护程序之前设备需要保持非活动状态的秒数。</span><span class="sxs-lookup"><span data-stu-id="58155-292">The number of seconds the device needs to be inactive for before the screen saver is shown in Kiosk Mode.</span></span> <span data-ttu-id="58155-293">有效值为1至9999999</span><span class="sxs-lookup"><span data-stu-id="58155-293">Valid values 1 to 9999999</span></span>|
|<span data-ttu-id="58155-294">kioskModeScreenSaverDetectMediaDisabled</span><span class="sxs-lookup"><span data-stu-id="58155-294">kioskModeScreenSaverDetectMediaDisabled</span></span>|<span data-ttu-id="58155-295">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-295">Boolean</span></span>|<span data-ttu-id="58155-296">如果音频/视频在展台模式下播放，则设备屏幕是否应显示屏幕保护程序。</span><span class="sxs-lookup"><span data-stu-id="58155-296">Whether or not the device screen should show the screen saver if audio/video is playing in Kiosk Mode.</span></span>|
|<span data-ttu-id="58155-297">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="58155-297">kioskModeApps</span></span>|<span data-ttu-id="58155-298">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="58155-298">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="58155-299">设备处于展台模式时将显示的托管应用列表。</span><span class="sxs-lookup"><span data-stu-id="58155-299">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="58155-300">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="58155-300">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="58155-301">kioskModeWallpaperUrl</span><span class="sxs-lookup"><span data-stu-id="58155-301">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="58155-302">String</span><span class="sxs-lookup"><span data-stu-id="58155-302">String</span></span>|<span data-ttu-id="58155-303">在设备处于展台模式时用于墙纸的可公开访问图像的 URL。</span><span class="sxs-lookup"><span data-stu-id="58155-303">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="58155-304">kioskModeExitCode</span><span class="sxs-lookup"><span data-stu-id="58155-304">kioskModeExitCode</span></span>|<span data-ttu-id="58155-305">String</span><span class="sxs-lookup"><span data-stu-id="58155-305">String</span></span>|<span data-ttu-id="58155-306">退出代码，以允许用户在设备处于展台模式时从展台模式中进行转义。</span><span class="sxs-lookup"><span data-stu-id="58155-306">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="58155-307">kioskModeVirtualHomeButtonEnabled</span><span class="sxs-lookup"><span data-stu-id="58155-307">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="58155-308">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-308">Boolean</span></span>|<span data-ttu-id="58155-309">设备处于展台模式时是否显示虚拟 "主页" 按钮。</span><span class="sxs-lookup"><span data-stu-id="58155-309">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="58155-310">kioskModeVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="58155-310">kioskModeVirtualHomeButtonType</span></span>|[<span data-ttu-id="58155-311">androidDeviceOwnerVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="58155-311">androidDeviceOwnerVirtualHomeButtonType</span></span>](../resources/intune-deviceconfig-androiddeviceownervirtualhomebuttontype.md)|<span data-ttu-id="58155-312">指示虚拟 home 按钮是否为向上轻扫主页按钮或浮动主页按钮。</span><span class="sxs-lookup"><span data-stu-id="58155-312">Indicates whether the virtual home button is a swipe up home button or a floating home button.</span></span> <span data-ttu-id="58155-313">可取值为：`notConfigured`、`swipeUp`、`floating`。</span><span class="sxs-lookup"><span data-stu-id="58155-313">Possible values are: `notConfigured`, `swipeUp`, `floating`.</span></span>|
|<span data-ttu-id="58155-314">kioskModeBluetoothConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="58155-314">kioskModeBluetoothConfigurationEnabled</span></span>|<span data-ttu-id="58155-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-315">Boolean</span></span>|<span data-ttu-id="58155-316">是否允许用户在展台模式下配置蓝牙设置。</span><span class="sxs-lookup"><span data-stu-id="58155-316">Whether or not to allow a user to configure Bluetooth settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="58155-317">kioskModeWiFiConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="58155-317">kioskModeWiFiConfigurationEnabled</span></span>|<span data-ttu-id="58155-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-318">Boolean</span></span>|<span data-ttu-id="58155-319">是否允许用户在展台模式下配置 Wi-Fi 设置。</span><span class="sxs-lookup"><span data-stu-id="58155-319">Whether or not to allow a user to configure Wi-Fi settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="58155-320">kioskModeFlashlightConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="58155-320">kioskModeFlashlightConfigurationEnabled</span></span>|<span data-ttu-id="58155-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-321">Boolean</span></span>|<span data-ttu-id="58155-322">是否允许用户在展台模式下使用该模式。</span><span class="sxs-lookup"><span data-stu-id="58155-322">Whether or not to allow a user to use the flashlight in Kiosk Mode.</span></span>|
|<span data-ttu-id="58155-323">kioskModeMediaVolumeConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="58155-323">kioskModeMediaVolumeConfigurationEnabled</span></span>|<span data-ttu-id="58155-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-324">Boolean</span></span>|<span data-ttu-id="58155-325">是否允许用户在展台模式下更改媒体音量。</span><span class="sxs-lookup"><span data-stu-id="58155-325">Whether or not to allow a user to change the media volume in Kiosk Mode.</span></span>|
|<span data-ttu-id="58155-326">kioskModeShowDeviceInfo</span><span class="sxs-lookup"><span data-stu-id="58155-326">kioskModeShowDeviceInfo</span></span>|<span data-ttu-id="58155-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-327">Boolean</span></span>|<span data-ttu-id="58155-328">是否允许用户访问基本设备信息。</span><span class="sxs-lookup"><span data-stu-id="58155-328">Whether or not to allow a user to access basic device information.</span></span>|
|<span data-ttu-id="58155-329">kioskModeManagedSettingsEntryDisabled</span><span class="sxs-lookup"><span data-stu-id="58155-329">kioskModeManagedSettingsEntryDisabled</span></span>|<span data-ttu-id="58155-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-330">Boolean</span></span>|<span data-ttu-id="58155-331">是否在展台模式下在托管的主屏幕上显示托管设置入口点。</span><span class="sxs-lookup"><span data-stu-id="58155-331">Whether or not to display the Managed Settings entry point on the managed home screen in Kiosk Mode.</span></span>|
|<span data-ttu-id="58155-332">kioskModeDebugMenuEasyAccessEnabled</span><span class="sxs-lookup"><span data-stu-id="58155-332">kioskModeDebugMenuEasyAccessEnabled</span></span>|<span data-ttu-id="58155-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-333">Boolean</span></span>|<span data-ttu-id="58155-334">是否允许用户在展台模式下轻松访问 "调试" 菜单。</span><span class="sxs-lookup"><span data-stu-id="58155-334">Whether or not to allow a user to easy access to the debug menu in Kiosk Mode.</span></span>|
|<span data-ttu-id="58155-335">kioskModeShowAppNotificationBadge</span><span class="sxs-lookup"><span data-stu-id="58155-335">kioskModeShowAppNotificationBadge</span></span>|<span data-ttu-id="58155-336">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-336">Boolean</span></span>|<span data-ttu-id="58155-337">是否在展台模式下显示应用程序通知徽章。</span><span class="sxs-lookup"><span data-stu-id="58155-337">Whether or not to display application notification badges in Kiosk Mode.</span></span>|
|<span data-ttu-id="58155-338">kioskModeScreenOrientation</span><span class="sxs-lookup"><span data-stu-id="58155-338">kioskModeScreenOrientation</span></span>|[<span data-ttu-id="58155-339">androidDeviceOwnerKioskModeScreenOrientation</span><span class="sxs-lookup"><span data-stu-id="58155-339">androidDeviceOwnerKioskModeScreenOrientation</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskmodescreenorientation.md)|<span data-ttu-id="58155-340">在展台模式下管理的主屏幕的屏幕方向配置。</span><span class="sxs-lookup"><span data-stu-id="58155-340">Screen orientation configuration for managed home screen in Kiosk Mode.</span></span> <span data-ttu-id="58155-341">可取值为：`notConfigured`、`portrait`、`landscape`、`autoRotate`。</span><span class="sxs-lookup"><span data-stu-id="58155-341">Possible values are: `notConfigured`, `portrait`, `landscape`, `autoRotate`.</span></span>|
|<span data-ttu-id="58155-342">kioskModeIconSize</span><span class="sxs-lookup"><span data-stu-id="58155-342">kioskModeIconSize</span></span>|[<span data-ttu-id="58155-343">androidDeviceOwnerKioskModeIconSize</span><span class="sxs-lookup"><span data-stu-id="58155-343">androidDeviceOwnerKioskModeIconSize</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskmodeiconsize.md)|<span data-ttu-id="58155-344">在展台模式下，管理的主屏幕的图标大小配置。</span><span class="sxs-lookup"><span data-stu-id="58155-344">Icon size configuration for managed home screen in Kiosk Mode.</span></span> <span data-ttu-id="58155-345">可取值为：`notConfigured`、`smallest`、`small`、`regular`、`large`、`largest`。</span><span class="sxs-lookup"><span data-stu-id="58155-345">Possible values are: `notConfigured`, `smallest`, `small`, `regular`, `large`, `largest`.</span></span>|
|<span data-ttu-id="58155-346">kioskModeFolderIcon</span><span class="sxs-lookup"><span data-stu-id="58155-346">kioskModeFolderIcon</span></span>|[<span data-ttu-id="58155-347">androidDeviceOwnerKioskModeFolderIcon</span><span class="sxs-lookup"><span data-stu-id="58155-347">androidDeviceOwnerKioskModeFolderIcon</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskmodefoldericon.md)|<span data-ttu-id="58155-348">展台模式下的托管主屏幕的文件夹图标配置。</span><span class="sxs-lookup"><span data-stu-id="58155-348">Folder icon configuration for managed home screen in Kiosk Mode.</span></span> <span data-ttu-id="58155-349">可取值为：`notConfigured`、`darkSquare`、`darkCircle`、`lightSquare`、`lightCircle`。</span><span class="sxs-lookup"><span data-stu-id="58155-349">Possible values are: `notConfigured`, `darkSquare`, `darkCircle`, `lightSquare`, `lightCircle`.</span></span>|
|<span data-ttu-id="58155-350">kioskModeWifiAllowedSsids</span><span class="sxs-lookup"><span data-stu-id="58155-350">kioskModeWifiAllowedSsids</span></span>|<span data-ttu-id="58155-351">String 集合</span><span class="sxs-lookup"><span data-stu-id="58155-351">String collection</span></span>|<span data-ttu-id="58155-352">可供用户在展台模式下进行配置的受限制的 WIFI Ssid 集。</span><span class="sxs-lookup"><span data-stu-id="58155-352">The restricted set of WIFI SSIDs available for the user to configure in Kiosk Mode.</span></span> <span data-ttu-id="58155-353">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="58155-353">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="58155-354">microphoneForceMute</span><span class="sxs-lookup"><span data-stu-id="58155-354">microphoneForceMute</span></span>|<span data-ttu-id="58155-355">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-355">Boolean</span></span>|<span data-ttu-id="58155-356">指示是否阻止观众在设备上的麦克风。</span><span class="sxs-lookup"><span data-stu-id="58155-356">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="58155-357">networkEscapeHatchAllowed</span><span class="sxs-lookup"><span data-stu-id="58155-357">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="58155-358">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-358">Boolean</span></span>|<span data-ttu-id="58155-359">指示在引导时设备是否允许连接到临时网络连接。</span><span class="sxs-lookup"><span data-stu-id="58155-359">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="58155-360">nfcBlockOutgoingBeam</span><span class="sxs-lookup"><span data-stu-id="58155-360">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="58155-361">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-361">Boolean</span></span>|<span data-ttu-id="58155-362">指示是否阻止 NFC 传出横梁。</span><span class="sxs-lookup"><span data-stu-id="58155-362">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="58155-363">passwordBlockKeyguard</span><span class="sxs-lookup"><span data-stu-id="58155-363">passwordBlockKeyguard</span></span>|<span data-ttu-id="58155-364">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-364">Boolean</span></span>|<span data-ttu-id="58155-365">指示是否禁用 keyguard。</span><span class="sxs-lookup"><span data-stu-id="58155-365">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="58155-366">passwordBlockKeyguardFeatures</span><span class="sxs-lookup"><span data-stu-id="58155-366">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="58155-367">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) 集合</span><span class="sxs-lookup"><span data-stu-id="58155-367">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="58155-368">要阻止的设备 keyguard 功能的列表。</span><span class="sxs-lookup"><span data-stu-id="58155-368">List of device keyguard features to block.</span></span> <span data-ttu-id="58155-369">该集合最多可包含 7 个元素。</span><span class="sxs-lookup"><span data-stu-id="58155-369">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="58155-370">可取值为：`notConfigured`、`camera`、`notifications`、`unredactedNotifications`、`trustAgents`、`fingerprint`、`remoteInput`、`allFeatures`。</span><span class="sxs-lookup"><span data-stu-id="58155-370">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="58155-371">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="58155-371">passwordExpirationDays</span></span>|<span data-ttu-id="58155-372">Int32</span><span class="sxs-lookup"><span data-stu-id="58155-372">Int32</span></span>|<span data-ttu-id="58155-373">指示密码在过期之前可以设置的时间量，并需要新密码。</span><span class="sxs-lookup"><span data-stu-id="58155-373">Indicates the amount of time that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="58155-374">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="58155-374">Valid values 1 to 365</span></span>|
|<span data-ttu-id="58155-375">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="58155-375">passwordMinimumLength</span></span>|<span data-ttu-id="58155-376">Int32</span><span class="sxs-lookup"><span data-stu-id="58155-376">Int32</span></span>|<span data-ttu-id="58155-377">指示设备上所需密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="58155-377">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="58155-378">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="58155-378">Valid values 4 to 16</span></span>|
|<span data-ttu-id="58155-379">passwordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="58155-379">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="58155-380">Int32</span><span class="sxs-lookup"><span data-stu-id="58155-380">Int32</span></span>|<span data-ttu-id="58155-381">指示设备密码所需的字母字符的最小数量。</span><span class="sxs-lookup"><span data-stu-id="58155-381">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="58155-382">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="58155-382">Valid values 1 to 16</span></span>|
|<span data-ttu-id="58155-383">passwordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="58155-383">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="58155-384">Int32</span><span class="sxs-lookup"><span data-stu-id="58155-384">Int32</span></span>|<span data-ttu-id="58155-385">指示设备密码所需的最小小写字符数。</span><span class="sxs-lookup"><span data-stu-id="58155-385">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="58155-386">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="58155-386">Valid values 1 to 16</span></span>|
|<span data-ttu-id="58155-387">passwordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="58155-387">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="58155-388">Int32</span><span class="sxs-lookup"><span data-stu-id="58155-388">Int32</span></span>|<span data-ttu-id="58155-389">指示设备密码所需的最小非字母字符数。</span><span class="sxs-lookup"><span data-stu-id="58155-389">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="58155-390">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="58155-390">Valid values 1 to 16</span></span>|
|<span data-ttu-id="58155-391">passwordMinimumNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="58155-391">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="58155-392">Int32</span><span class="sxs-lookup"><span data-stu-id="58155-392">Int32</span></span>|<span data-ttu-id="58155-393">指示设备密码所需的最小数字字符数。</span><span class="sxs-lookup"><span data-stu-id="58155-393">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="58155-394">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="58155-394">Valid values 1 to 16</span></span>|
|<span data-ttu-id="58155-395">passwordMinimumSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="58155-395">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="58155-396">Int32</span><span class="sxs-lookup"><span data-stu-id="58155-396">Int32</span></span>|<span data-ttu-id="58155-397">指示设备密码所需的最小符号字符数。</span><span class="sxs-lookup"><span data-stu-id="58155-397">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="58155-398">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="58155-398">Valid values 1 to 16</span></span>|
|<span data-ttu-id="58155-399">passwordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="58155-399">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="58155-400">Int32</span><span class="sxs-lookup"><span data-stu-id="58155-400">Int32</span></span>|<span data-ttu-id="58155-401">指示设备密码所需的大写字母字符的最小数量。</span><span class="sxs-lookup"><span data-stu-id="58155-401">Indicates the minimum number of upper case letter characters required for device password.</span></span> <span data-ttu-id="58155-402">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="58155-402">Valid values 1 to 16</span></span>|
|<span data-ttu-id="58155-403">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="58155-403">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="58155-404">Int32</span><span class="sxs-lookup"><span data-stu-id="58155-404">Int32</span></span>|<span data-ttu-id="58155-405">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="58155-405">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="58155-406">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="58155-406">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="58155-407">Int32</span><span class="sxs-lookup"><span data-stu-id="58155-407">Int32</span></span>|<span data-ttu-id="58155-408">指示密码历史记录的长度，其中用户将不能输入与历史记录中的任何密码相同的新密码。</span><span class="sxs-lookup"><span data-stu-id="58155-408">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="58155-409">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="58155-409">Valid values 0 to 24</span></span>|
|<span data-ttu-id="58155-410">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="58155-410">passwordRequiredType</span></span>|[<span data-ttu-id="58155-411">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="58155-411">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="58155-412">指示设备上所需的最小密码质量。</span><span class="sxs-lookup"><span data-stu-id="58155-412">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="58155-413">可取值为：`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`customPassword`。</span><span class="sxs-lookup"><span data-stu-id="58155-413">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|
|<span data-ttu-id="58155-414">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="58155-414">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="58155-415">Int32</span><span class="sxs-lookup"><span data-stu-id="58155-415">Int32</span></span>|<span data-ttu-id="58155-416">指示用户在擦除设备之前可以输入不正确密码的次数。</span><span class="sxs-lookup"><span data-stu-id="58155-416">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="58155-417">有效值为 4 至 11</span><span class="sxs-lookup"><span data-stu-id="58155-417">Valid values 4 to 11</span></span>|
|<span data-ttu-id="58155-418">playStoreMode</span><span class="sxs-lookup"><span data-stu-id="58155-418">playStoreMode</span></span>|[<span data-ttu-id="58155-419">androidDeviceOwnerPlayStoreMode</span><span class="sxs-lookup"><span data-stu-id="58155-419">androidDeviceOwnerPlayStoreMode</span></span>](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|<span data-ttu-id="58155-420">指示设备的播放存储模式。</span><span class="sxs-lookup"><span data-stu-id="58155-420">Indicates the Play Store mode of the device.</span></span> <span data-ttu-id="58155-421">可取值为：`notConfigured`、`allowList`、`blockList`。</span><span class="sxs-lookup"><span data-stu-id="58155-421">Possible values are: `notConfigured`, `allowList`, `blockList`.</span></span>|
|<span data-ttu-id="58155-422">safeBootBlocked</span><span class="sxs-lookup"><span data-stu-id="58155-422">safeBootBlocked</span></span>|<span data-ttu-id="58155-423">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-423">Boolean</span></span>|<span data-ttu-id="58155-424">指示是否禁用重新启动设备到安全启动。</span><span class="sxs-lookup"><span data-stu-id="58155-424">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="58155-425">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="58155-425">screenCaptureBlocked</span></span>|<span data-ttu-id="58155-426">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-426">Boolean</span></span>|<span data-ttu-id="58155-427">指示是否禁用获取屏幕截图的功能。</span><span class="sxs-lookup"><span data-stu-id="58155-427">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="58155-428">securityAllowDebuggingFeatures</span><span class="sxs-lookup"><span data-stu-id="58155-428">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="58155-429">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-429">Boolean</span></span>|<span data-ttu-id="58155-430">指示是否阻止用户启用设备上的调试功能。</span><span class="sxs-lookup"><span data-stu-id="58155-430">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="58155-431">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="58155-431">securityRequireVerifyApps</span></span>|<span data-ttu-id="58155-432">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-432">Boolean</span></span>|<span data-ttu-id="58155-433">指示是否需要验证应用。</span><span class="sxs-lookup"><span data-stu-id="58155-433">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="58155-434">statusBarBlocked</span><span class="sxs-lookup"><span data-stu-id="58155-434">statusBarBlocked</span></span>|<span data-ttu-id="58155-435">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-435">Boolean</span></span>|<span data-ttu-id="58155-436">指示是否禁用状态栏，包括通知、快速设置和其他屏幕重叠。</span><span class="sxs-lookup"><span data-stu-id="58155-436">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="58155-437">stayOnModes</span><span class="sxs-lookup"><span data-stu-id="58155-437">stayOnModes</span></span>|<span data-ttu-id="58155-438">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) 集合</span><span class="sxs-lookup"><span data-stu-id="58155-438">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="58155-439">设备的显示将保持开机状态的模式列表。</span><span class="sxs-lookup"><span data-stu-id="58155-439">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="58155-440">此集合最多可包含4个元素。</span><span class="sxs-lookup"><span data-stu-id="58155-440">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="58155-441">可取值为：`notConfigured`、`ac`、`usb`、`wireless`。</span><span class="sxs-lookup"><span data-stu-id="58155-441">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="58155-442">storageAllowUsb</span><span class="sxs-lookup"><span data-stu-id="58155-442">storageAllowUsb</span></span>|<span data-ttu-id="58155-443">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-443">Boolean</span></span>|<span data-ttu-id="58155-444">指示是否允许 USB 大容量存储。</span><span class="sxs-lookup"><span data-stu-id="58155-444">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="58155-445">storageBlockExternalMedia</span><span class="sxs-lookup"><span data-stu-id="58155-445">storageBlockExternalMedia</span></span>|<span data-ttu-id="58155-446">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-446">Boolean</span></span>|<span data-ttu-id="58155-447">指示是否阻止外部媒体。</span><span class="sxs-lookup"><span data-stu-id="58155-447">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="58155-448">storageBlockUsbFileTransfer</span><span class="sxs-lookup"><span data-stu-id="58155-448">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="58155-449">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-449">Boolean</span></span>|<span data-ttu-id="58155-450">指示是否阻止 USB 文件传输。</span><span class="sxs-lookup"><span data-stu-id="58155-450">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="58155-451">systemUpdateWindowStartMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="58155-451">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="58155-452">Int32</span><span class="sxs-lookup"><span data-stu-id="58155-452">Int32</span></span>|<span data-ttu-id="58155-453">指示系统更新窗口午夜后启动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="58155-453">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="58155-454">有效值为0至1440</span><span class="sxs-lookup"><span data-stu-id="58155-454">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="58155-455">systemUpdateWindowEndMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="58155-455">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="58155-456">Int32</span><span class="sxs-lookup"><span data-stu-id="58155-456">Int32</span></span>|<span data-ttu-id="58155-457">指示系统更新窗口结束后的分钟数。</span><span class="sxs-lookup"><span data-stu-id="58155-457">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="58155-458">有效值为0至1440</span><span class="sxs-lookup"><span data-stu-id="58155-458">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="58155-459">systemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="58155-459">systemUpdateInstallType</span></span>|[<span data-ttu-id="58155-460">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="58155-460">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="58155-461">系统更新配置的类型。</span><span class="sxs-lookup"><span data-stu-id="58155-461">The type of system update configuration.</span></span> <span data-ttu-id="58155-462">可取值为：`deviceDefault`、`postpone`、`windowed`、`automatic`。</span><span class="sxs-lookup"><span data-stu-id="58155-462">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="58155-463">systemWindowsBlocked</span><span class="sxs-lookup"><span data-stu-id="58155-463">systemWindowsBlocked</span></span>|<span data-ttu-id="58155-464">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-464">Boolean</span></span>|<span data-ttu-id="58155-465">是否阻止 Android 系统提示符窗口，如 toast、电话活动和系统通知。</span><span class="sxs-lookup"><span data-stu-id="58155-465">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="58155-466">usersBlockAdd</span><span class="sxs-lookup"><span data-stu-id="58155-466">usersBlockAdd</span></span>|<span data-ttu-id="58155-467">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-467">Boolean</span></span>|<span data-ttu-id="58155-468">指示是否禁用添加用户和配置文件。</span><span class="sxs-lookup"><span data-stu-id="58155-468">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="58155-469">usersBlockRemove</span><span class="sxs-lookup"><span data-stu-id="58155-469">usersBlockRemove</span></span>|<span data-ttu-id="58155-470">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-470">Boolean</span></span>|<span data-ttu-id="58155-471">指示是否禁用从设备中删除其他用户。</span><span class="sxs-lookup"><span data-stu-id="58155-471">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="58155-472">volumeBlockAdjustment</span><span class="sxs-lookup"><span data-stu-id="58155-472">volumeBlockAdjustment</span></span>|<span data-ttu-id="58155-473">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-473">Boolean</span></span>|<span data-ttu-id="58155-474">指示是否禁用了调整主音量。</span><span class="sxs-lookup"><span data-stu-id="58155-474">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="58155-475">vpnAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="58155-475">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="58155-476">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-476">Boolean</span></span>|<span data-ttu-id="58155-477">如果指定了 always on VPN 包名称，则在断开 VPN 连接时是否锁定网络流量。</span><span class="sxs-lookup"><span data-stu-id="58155-477">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="58155-478">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="58155-478">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="58155-479">String</span><span class="sxs-lookup"><span data-stu-id="58155-479">String</span></span>|<span data-ttu-id="58155-480">将处理永不启用 VPN 连接的应用程序的 Android 应用程序包名称。</span><span class="sxs-lookup"><span data-stu-id="58155-480">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="58155-481">wifiBlockEditConfigurations</span><span class="sxs-lookup"><span data-stu-id="58155-481">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="58155-482">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-482">Boolean</span></span>|<span data-ttu-id="58155-483">指示是否阻止用户编辑 wifi 连接设置。</span><span class="sxs-lookup"><span data-stu-id="58155-483">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="58155-484">wifiBlockEditPolicyDefinedConfigurations</span><span class="sxs-lookup"><span data-stu-id="58155-484">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="58155-485">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-485">Boolean</span></span>|<span data-ttu-id="58155-486">指示是否阻止用户仅编辑策略定义的网络。</span><span class="sxs-lookup"><span data-stu-id="58155-486">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|
|<span data-ttu-id="58155-487">personalProfileAppsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="58155-487">personalProfileAppsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="58155-488">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-488">Boolean</span></span>|<span data-ttu-id="58155-489">指示用户是否可以在个人配置文件上安装来自未知源的应用程序。</span><span class="sxs-lookup"><span data-stu-id="58155-489">Indicates whether the user can install apps from unknown sources on the personal profile.</span></span>|
|<span data-ttu-id="58155-490">personalProfileCameraBlocked</span><span class="sxs-lookup"><span data-stu-id="58155-490">personalProfileCameraBlocked</span></span>|<span data-ttu-id="58155-491">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-491">Boolean</span></span>|<span data-ttu-id="58155-492">指示是否禁用个人配置文件上的摄像头的使用。</span><span class="sxs-lookup"><span data-stu-id="58155-492">Indicates whether to disable the use of the camera on the personal profile.</span></span>|
|<span data-ttu-id="58155-493">personalProfileScreenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="58155-493">personalProfileScreenCaptureBlocked</span></span>|<span data-ttu-id="58155-494">Boolean</span><span class="sxs-lookup"><span data-stu-id="58155-494">Boolean</span></span>|<span data-ttu-id="58155-495">指示是否禁用在个人配置文件上采用屏幕截图的功能。</span><span class="sxs-lookup"><span data-stu-id="58155-495">Indicates whether to disable the capability to take screenshots on the personal profile.</span></span>|
|<span data-ttu-id="58155-496">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="58155-496">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="58155-497">Int32</span><span class="sxs-lookup"><span data-stu-id="58155-497">Int32</span></span>|<span data-ttu-id="58155-498">指示工作配置文件密码在过期之前可以设置的天数，并将需要新密码。</span><span class="sxs-lookup"><span data-stu-id="58155-498">Indicates the number of days that a work profile password can be set before it expires and a new password will be required.</span></span> <span data-ttu-id="58155-499">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="58155-499">Valid values 1 to 365</span></span>|
|<span data-ttu-id="58155-500">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="58155-500">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="58155-501">Int32</span><span class="sxs-lookup"><span data-stu-id="58155-501">Int32</span></span>|<span data-ttu-id="58155-502">指示工作配置文件密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="58155-502">Indicates the minimum length of the work profile password.</span></span> <span data-ttu-id="58155-503">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="58155-503">Valid values 4 to 16</span></span>|
|<span data-ttu-id="58155-504">workProfilePasswordMinimumNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="58155-504">workProfilePasswordMinimumNumericCharacters</span></span>|<span data-ttu-id="58155-505">Int32</span><span class="sxs-lookup"><span data-stu-id="58155-505">Int32</span></span>|<span data-ttu-id="58155-506">指示工作配置文件密码所需的最小数字字符数。</span><span class="sxs-lookup"><span data-stu-id="58155-506">Indicates the minimum number of numeric characters required for the work profile password.</span></span> <span data-ttu-id="58155-507">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="58155-507">Valid values 1 to 16</span></span>|
|<span data-ttu-id="58155-508">workProfilePasswordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="58155-508">workProfilePasswordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="58155-509">Int32</span><span class="sxs-lookup"><span data-stu-id="58155-509">Int32</span></span>|<span data-ttu-id="58155-510">指示工作配置文件密码所需的最小非字母字符数。</span><span class="sxs-lookup"><span data-stu-id="58155-510">Indicates the minimum number of non-letter characters required for the work profile password.</span></span> <span data-ttu-id="58155-511">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="58155-511">Valid values 1 to 16</span></span>|
|<span data-ttu-id="58155-512">workProfilePasswordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="58155-512">workProfilePasswordMinimumLetterCharacters</span></span>|<span data-ttu-id="58155-513">Int32</span><span class="sxs-lookup"><span data-stu-id="58155-513">Int32</span></span>|<span data-ttu-id="58155-514">指示工作配置文件密码所需的字母字符的最小数量。</span><span class="sxs-lookup"><span data-stu-id="58155-514">Indicates the minimum number of letter characters required for the work profile password.</span></span> <span data-ttu-id="58155-515">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="58155-515">Valid values 1 to 16</span></span>|
|<span data-ttu-id="58155-516">workProfilePasswordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="58155-516">workProfilePasswordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="58155-517">Int32</span><span class="sxs-lookup"><span data-stu-id="58155-517">Int32</span></span>|<span data-ttu-id="58155-518">指示工作配置文件密码所需的最小小写字符数。</span><span class="sxs-lookup"><span data-stu-id="58155-518">Indicates the minimum number of lower-case characters required for the work profile password.</span></span> <span data-ttu-id="58155-519">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="58155-519">Valid values 1 to 16</span></span>|
|<span data-ttu-id="58155-520">workProfilePasswordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="58155-520">workProfilePasswordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="58155-521">Int32</span><span class="sxs-lookup"><span data-stu-id="58155-521">Int32</span></span>|<span data-ttu-id="58155-522">指示工作配置文件密码所需的大写字母字符的最小数量。</span><span class="sxs-lookup"><span data-stu-id="58155-522">Indicates the minimum number of upper-case letter characters required for the work profile password.</span></span> <span data-ttu-id="58155-523">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="58155-523">Valid values 1 to 16</span></span>|
|<span data-ttu-id="58155-524">workProfilePasswordMinimumSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="58155-524">workProfilePasswordMinimumSymbolCharacters</span></span>|<span data-ttu-id="58155-525">Int32</span><span class="sxs-lookup"><span data-stu-id="58155-525">Int32</span></span>|<span data-ttu-id="58155-526">指示工作配置文件密码所需的最小符号字符数。</span><span class="sxs-lookup"><span data-stu-id="58155-526">Indicates the minimum number of symbol characters required for the work profile password.</span></span> <span data-ttu-id="58155-527">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="58155-527">Valid values 1 to 16</span></span>|
|<span data-ttu-id="58155-528">workProfilePasswordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="58155-528">workProfilePasswordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="58155-529">Int32</span><span class="sxs-lookup"><span data-stu-id="58155-529">Int32</span></span>|<span data-ttu-id="58155-530">指示工作配置文件密码历史记录的长度，其中用户将不能输入与历史记录中的任何密码相同的新密码。</span><span class="sxs-lookup"><span data-stu-id="58155-530">Indicates the length of the work profile password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="58155-531">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="58155-531">Valid values 0 to 24</span></span>|
|<span data-ttu-id="58155-532">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="58155-532">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="58155-533">Int32</span><span class="sxs-lookup"><span data-stu-id="58155-533">Int32</span></span>|<span data-ttu-id="58155-534">指示用户在擦除设备之前可以输入不正确的工作配置文件密码的次数。</span><span class="sxs-lookup"><span data-stu-id="58155-534">Indicates the number of times a user can enter an incorrect work profile password before the device is wiped.</span></span> <span data-ttu-id="58155-535">有效值为 4 至 11</span><span class="sxs-lookup"><span data-stu-id="58155-535">Valid values 4 to 11</span></span>|
|<span data-ttu-id="58155-536">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="58155-536">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="58155-537">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="58155-537">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="58155-538">指示工作配置文件密码所需的最小密码质量。</span><span class="sxs-lookup"><span data-stu-id="58155-538">Indicates the minimum password quality required on the work profile password.</span></span> <span data-ttu-id="58155-539">可取值为：`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`customPassword`。</span><span class="sxs-lookup"><span data-stu-id="58155-539">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|



## <a name="response"></a><span data-ttu-id="58155-540">响应</span><span class="sxs-lookup"><span data-stu-id="58155-540">Response</span></span>
<span data-ttu-id="58155-541">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="58155-541">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58155-542">示例</span><span class="sxs-lookup"><span data-stu-id="58155-542">Example</span></span>

### <a name="request"></a><span data-ttu-id="58155-543">请求</span><span class="sxs-lookup"><span data-stu-id="58155-543">Request</span></span>
<span data-ttu-id="58155-544">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="58155-544">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 6387

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

### <a name="response"></a><span data-ttu-id="58155-545">响应</span><span class="sxs-lookup"><span data-stu-id="58155-545">Response</span></span>
<span data-ttu-id="58155-p156">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="58155-p156">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 6559

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




