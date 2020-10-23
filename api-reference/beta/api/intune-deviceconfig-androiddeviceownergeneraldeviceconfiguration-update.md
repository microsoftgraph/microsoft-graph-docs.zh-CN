---
title: 更新 androidDeviceOwnerGeneralDeviceConfiguration
description: 更新 androidDeviceOwnerGeneralDeviceConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 030808c780cf118408090941453515fcc3b8f953
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48690558"
---
# <a name="update-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="9df31-103">更新 androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="9df31-103">Update androidDeviceOwnerGeneralDeviceConfiguration</span></span>

<span data-ttu-id="9df31-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9df31-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9df31-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9df31-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9df31-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9df31-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9df31-107">更新 [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9df31-107">Update the properties of a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9df31-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9df31-108">Prerequisites</span></span>
<span data-ttu-id="9df31-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9df31-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9df31-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9df31-111">Permission type</span></span>|<span data-ttu-id="9df31-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9df31-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9df31-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9df31-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9df31-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9df31-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9df31-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9df31-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9df31-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9df31-116">Not supported.</span></span>|
|<span data-ttu-id="9df31-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9df31-117">Application</span></span>|<span data-ttu-id="9df31-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9df31-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9df31-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9df31-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="9df31-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9df31-120">Request headers</span></span>
|<span data-ttu-id="9df31-121">标头</span><span class="sxs-lookup"><span data-stu-id="9df31-121">Header</span></span>|<span data-ttu-id="9df31-122">值</span><span class="sxs-lookup"><span data-stu-id="9df31-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9df31-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9df31-123">Authorization</span></span>|<span data-ttu-id="9df31-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9df31-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9df31-125">接受</span><span class="sxs-lookup"><span data-stu-id="9df31-125">Accept</span></span>|<span data-ttu-id="9df31-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9df31-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9df31-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9df31-127">Request body</span></span>
<span data-ttu-id="9df31-128">在请求正文中，提供 [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9df31-128">In the request body, supply a JSON representation for the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="9df31-129">下表显示创建 [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9df31-129">The following table shows the properties that are required when you create the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="9df31-130">属性</span><span class="sxs-lookup"><span data-stu-id="9df31-130">Property</span></span>|<span data-ttu-id="9df31-131">类型</span><span class="sxs-lookup"><span data-stu-id="9df31-131">Type</span></span>|<span data-ttu-id="9df31-132">说明</span><span class="sxs-lookup"><span data-stu-id="9df31-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9df31-133">id</span><span class="sxs-lookup"><span data-stu-id="9df31-133">id</span></span>|<span data-ttu-id="9df31-134">String</span><span class="sxs-lookup"><span data-stu-id="9df31-134">String</span></span>|<span data-ttu-id="9df31-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9df31-135">Key of the entity.</span></span> <span data-ttu-id="9df31-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9df31-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9df31-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9df31-137">lastModifiedDateTime</span></span>|<span data-ttu-id="9df31-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9df31-138">DateTimeOffset</span></span>|<span data-ttu-id="9df31-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="9df31-139">DateTime the object was last modified.</span></span> <span data-ttu-id="9df31-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9df31-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9df31-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9df31-141">roleScopeTagIds</span></span>|<span data-ttu-id="9df31-142">String collection</span><span class="sxs-lookup"><span data-stu-id="9df31-142">String collection</span></span>|<span data-ttu-id="9df31-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="9df31-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9df31-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9df31-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9df31-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9df31-145">supportsScopeTags</span></span>|<span data-ttu-id="9df31-146">布尔</span><span class="sxs-lookup"><span data-stu-id="9df31-146">Boolean</span></span>|<span data-ttu-id="9df31-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="9df31-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9df31-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="9df31-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9df31-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="9df31-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9df31-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9df31-150">This property is read-only.</span></span> <span data-ttu-id="9df31-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9df31-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9df31-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9df31-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="9df31-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9df31-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="9df31-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="9df31-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="9df31-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9df31-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9df31-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9df31-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="9df31-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9df31-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="9df31-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="9df31-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="9df31-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9df31-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9df31-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9df31-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="9df31-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9df31-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="9df31-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="9df31-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="9df31-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9df31-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9df31-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9df31-164">createdDateTime</span></span>|<span data-ttu-id="9df31-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9df31-165">DateTimeOffset</span></span>|<span data-ttu-id="9df31-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="9df31-166">DateTime the object was created.</span></span> <span data-ttu-id="9df31-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9df31-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9df31-168">说明</span><span class="sxs-lookup"><span data-stu-id="9df31-168">description</span></span>|<span data-ttu-id="9df31-169">String</span><span class="sxs-lookup"><span data-stu-id="9df31-169">String</span></span>|<span data-ttu-id="9df31-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="9df31-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9df31-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9df31-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9df31-172">displayName</span><span class="sxs-lookup"><span data-stu-id="9df31-172">displayName</span></span>|<span data-ttu-id="9df31-173">String</span><span class="sxs-lookup"><span data-stu-id="9df31-173">String</span></span>|<span data-ttu-id="9df31-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="9df31-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9df31-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9df31-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9df31-176">version</span><span class="sxs-lookup"><span data-stu-id="9df31-176">version</span></span>|<span data-ttu-id="9df31-177">Int32</span><span class="sxs-lookup"><span data-stu-id="9df31-177">Int32</span></span>|<span data-ttu-id="9df31-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="9df31-178">Version of the device configuration.</span></span> <span data-ttu-id="9df31-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9df31-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9df31-180">accountsBlockModification</span><span class="sxs-lookup"><span data-stu-id="9df31-180">accountsBlockModification</span></span>|<span data-ttu-id="9df31-181">布尔</span><span class="sxs-lookup"><span data-stu-id="9df31-181">Boolean</span></span>|<span data-ttu-id="9df31-182">指示是否禁用添加或删除帐户。</span><span class="sxs-lookup"><span data-stu-id="9df31-182">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="9df31-183">appsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="9df31-183">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="9df31-184">布尔</span><span class="sxs-lookup"><span data-stu-id="9df31-184">Boolean</span></span>|<span data-ttu-id="9df31-185">指示是否允许用户启用 "未知源" 设置。</span><span class="sxs-lookup"><span data-stu-id="9df31-185">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="9df31-186">appsAutoUpdatePolicy</span><span class="sxs-lookup"><span data-stu-id="9df31-186">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="9df31-187">androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="9df31-187">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="9df31-188">指示应用程序自动更新策略的值。</span><span class="sxs-lookup"><span data-stu-id="9df31-188">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="9df31-189">可取值为：`notConfigured`、`userChoice`、`never`、`wiFiOnly`、`always`。</span><span class="sxs-lookup"><span data-stu-id="9df31-189">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="9df31-190">appsDefaultPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="9df31-190">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="9df31-191">androidDeviceOwnerDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="9df31-191">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="9df31-192">指示对运行时权限请求的权限策略（如果专门没有为应用程序定义）。</span><span class="sxs-lookup"><span data-stu-id="9df31-192">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="9df31-193">可取值为：`deviceDefault`、`prompt`、`autoGrant`、`autoDeny`。</span><span class="sxs-lookup"><span data-stu-id="9df31-193">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="9df31-194">appsRecommendSkippingFirstUseHints</span><span class="sxs-lookup"><span data-stu-id="9df31-194">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="9df31-195">布尔</span><span class="sxs-lookup"><span data-stu-id="9df31-195">Boolean</span></span>|<span data-ttu-id="9df31-196">是否建议所有应用都将跳过他们可能已添加的任何首次使用提示。</span><span class="sxs-lookup"><span data-stu-id="9df31-196">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="9df31-197">bluetoothBlockConfiguration</span><span class="sxs-lookup"><span data-stu-id="9df31-197">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="9df31-198">布尔</span><span class="sxs-lookup"><span data-stu-id="9df31-198">Boolean</span></span>|<span data-ttu-id="9df31-199">指示是否阻止用户配置蓝牙。</span><span class="sxs-lookup"><span data-stu-id="9df31-199">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="9df31-200">bluetoothBlockContactSharing</span><span class="sxs-lookup"><span data-stu-id="9df31-200">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="9df31-201">布尔</span><span class="sxs-lookup"><span data-stu-id="9df31-201">Boolean</span></span>|<span data-ttu-id="9df31-202">指示是否阻止用户通过蓝牙共享联系人。</span><span class="sxs-lookup"><span data-stu-id="9df31-202">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="9df31-203">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="9df31-203">cameraBlocked</span></span>|<span data-ttu-id="9df31-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="9df31-204">Boolean</span></span>|<span data-ttu-id="9df31-205">指示是否禁用相机的使用。</span><span class="sxs-lookup"><span data-stu-id="9df31-205">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="9df31-206">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="9df31-206">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="9df31-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="9df31-207">Boolean</span></span>|<span data-ttu-id="9df31-208">指示是否阻止 Wi-Fi 网络共享。</span><span class="sxs-lookup"><span data-stu-id="9df31-208">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="9df31-209">certificateCredentialConfigurationDisabled</span><span class="sxs-lookup"><span data-stu-id="9df31-209">certificateCredentialConfigurationDisabled</span></span>|<span data-ttu-id="9df31-210">布尔</span><span class="sxs-lookup"><span data-stu-id="9df31-210">Boolean</span></span>|<span data-ttu-id="9df31-211">指示是否阻止来自任何证书凭据配置的用户。</span><span class="sxs-lookup"><span data-stu-id="9df31-211">Indicates whether or not to block users from any certificate credential configuration.</span></span>|
|<span data-ttu-id="9df31-212">microsoftLauncherConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="9df31-212">microsoftLauncherConfigurationEnabled</span></span>|<span data-ttu-id="9df31-213">布尔</span><span class="sxs-lookup"><span data-stu-id="9df31-213">Boolean</span></span>|<span data-ttu-id="9df31-214">指示是否要配置 Microsoft 启动器。</span><span class="sxs-lookup"><span data-stu-id="9df31-214">Indicates whether or not to you want configure Microsoft Launcher.</span></span>|
|<span data-ttu-id="9df31-215">microsoftLauncherCustomWallpaperEnabled</span><span class="sxs-lookup"><span data-stu-id="9df31-215">microsoftLauncherCustomWallpaperEnabled</span></span>|<span data-ttu-id="9df31-216">布尔</span><span class="sxs-lookup"><span data-stu-id="9df31-216">Boolean</span></span>|<span data-ttu-id="9df31-217">指示是否在目标设备上配置墙纸。</span><span class="sxs-lookup"><span data-stu-id="9df31-217">Indicates whether or not to configure the wallpaper on the targeted devices.</span></span>|
|<span data-ttu-id="9df31-218">microsoftLauncherCustomWallpaperImageUrl</span><span class="sxs-lookup"><span data-stu-id="9df31-218">microsoftLauncherCustomWallpaperImageUrl</span></span>|<span data-ttu-id="9df31-219">String</span><span class="sxs-lookup"><span data-stu-id="9df31-219">String</span></span>|<span data-ttu-id="9df31-220">指示用作目标设备墙纸的图像文件的 URL。</span><span class="sxs-lookup"><span data-stu-id="9df31-220">Indicates the URL for the image file to use as the wallpaper on the targeted devices.</span></span>|
|<span data-ttu-id="9df31-221">microsoftLauncherCustomWallpaperAllowUserModification</span><span class="sxs-lookup"><span data-stu-id="9df31-221">microsoftLauncherCustomWallpaperAllowUserModification</span></span>|<span data-ttu-id="9df31-222">布尔</span><span class="sxs-lookup"><span data-stu-id="9df31-222">Boolean</span></span>|<span data-ttu-id="9df31-223">指示用户是否可以修改墙纸以个性化设置其设备。</span><span class="sxs-lookup"><span data-stu-id="9df31-223">Indicates whether or not the user can modify the wallpaper to personalize their device.</span></span>|
|<span data-ttu-id="9df31-224">microsoftLauncherFeedEnabled</span><span class="sxs-lookup"><span data-stu-id="9df31-224">microsoftLauncherFeedEnabled</span></span>|<span data-ttu-id="9df31-225">布尔</span><span class="sxs-lookup"><span data-stu-id="9df31-225">Boolean</span></span>|<span data-ttu-id="9df31-226">指示是否要在设备上启用启动器源。</span><span class="sxs-lookup"><span data-stu-id="9df31-226">Indicates whether or not you want to enable the launcher feed on the device.</span></span>|
|<span data-ttu-id="9df31-227">microsoftLauncherFeedAllowUserModification</span><span class="sxs-lookup"><span data-stu-id="9df31-227">microsoftLauncherFeedAllowUserModification</span></span>|<span data-ttu-id="9df31-228">布尔</span><span class="sxs-lookup"><span data-stu-id="9df31-228">Boolean</span></span>|<span data-ttu-id="9df31-229">指示用户是否可以修改设备上的启动器源。</span><span class="sxs-lookup"><span data-stu-id="9df31-229">Indicates whether or not the user can modify the launcher feed on the device.</span></span>|
|<span data-ttu-id="9df31-230">microsoftLauncherDockPresenceConfiguration</span><span class="sxs-lookup"><span data-stu-id="9df31-230">microsoftLauncherDockPresenceConfiguration</span></span>|[<span data-ttu-id="9df31-231">microsoftLauncherDockPresence</span><span class="sxs-lookup"><span data-stu-id="9df31-231">microsoftLauncherDockPresence</span></span>](../resources/intune-deviceconfig-microsoftlauncherdockpresence.md)|<span data-ttu-id="9df31-232">指示是否要配置设备停靠。</span><span class="sxs-lookup"><span data-stu-id="9df31-232">Indicates whether or not you want to configure the device dock.</span></span> <span data-ttu-id="9df31-233">可取值为：`notConfigured`、`show`、`hide`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="9df31-233">Possible values are: `notConfigured`, `show`, `hide`, `disabled`.</span></span>|
|<span data-ttu-id="9df31-234">microsoftLauncherDockPresenceAllowUserModification</span><span class="sxs-lookup"><span data-stu-id="9df31-234">microsoftLauncherDockPresenceAllowUserModification</span></span>|<span data-ttu-id="9df31-235">布尔</span><span class="sxs-lookup"><span data-stu-id="9df31-235">Boolean</span></span>|<span data-ttu-id="9df31-236">指示用户是否可以修改设备上的设备停靠配置。</span><span class="sxs-lookup"><span data-stu-id="9df31-236">Indicates whether or not the user can modify the device dock configuration on the device.</span></span>|
|<span data-ttu-id="9df31-237">microsoftLauncherSearchBarPlacementConfiguration</span><span class="sxs-lookup"><span data-stu-id="9df31-237">microsoftLauncherSearchBarPlacementConfiguration</span></span>|[<span data-ttu-id="9df31-238">microsoftLauncherSearchBarPlacement</span><span class="sxs-lookup"><span data-stu-id="9df31-238">microsoftLauncherSearchBarPlacement</span></span>](../resources/intune-deviceconfig-microsoftlaunchersearchbarplacement.md)|<span data-ttu-id="9df31-239">指示设备上的搜索栏的布局配置。</span><span class="sxs-lookup"><span data-stu-id="9df31-239">Indicates the search bar placement configuration on the device.</span></span> <span data-ttu-id="9df31-240">可取值为：`notConfigured`、`top`、`bottom`、`hide`。</span><span class="sxs-lookup"><span data-stu-id="9df31-240">Possible values are: `notConfigured`, `top`, `bottom`, `hide`.</span></span>|
|<span data-ttu-id="9df31-241">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="9df31-241">enrollmentProfile</span></span>|[<span data-ttu-id="9df31-242">androidDeviceOwnerEnrollmentProfileType</span><span class="sxs-lookup"><span data-stu-id="9df31-242">androidDeviceOwnerEnrollmentProfileType</span></span>](../resources/intune-deviceconfig-androiddeviceownerenrollmentprofiletype.md)|<span data-ttu-id="9df31-243">指示要配置的注册配置文件。</span><span class="sxs-lookup"><span data-stu-id="9df31-243">Indicates which enrollment profile you want to configure.</span></span> <span data-ttu-id="9df31-244">可取值为：`notConfigured`、`dedicatedDevice`、`fullyManaged`。</span><span class="sxs-lookup"><span data-stu-id="9df31-244">Possible values are: `notConfigured`, `dedicatedDevice`, `fullyManaged`.</span></span>|
|<span data-ttu-id="9df31-245">dataRoamingBlocked</span><span class="sxs-lookup"><span data-stu-id="9df31-245">dataRoamingBlocked</span></span>|<span data-ttu-id="9df31-246">布尔</span><span class="sxs-lookup"><span data-stu-id="9df31-246">Boolean</span></span>|<span data-ttu-id="9df31-247">指示是否阻止用户使用数据漫游。</span><span class="sxs-lookup"><span data-stu-id="9df31-247">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="9df31-248">dateTimeConfigurationBlocked</span><span class="sxs-lookup"><span data-stu-id="9df31-248">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="9df31-249">布尔</span><span class="sxs-lookup"><span data-stu-id="9df31-249">Boolean</span></span>|<span data-ttu-id="9df31-250">指示是否阻止用户手动更改设备上的日期或时间</span><span class="sxs-lookup"><span data-stu-id="9df31-250">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="9df31-251">factoryResetDeviceAdministratorEmails</span><span class="sxs-lookup"><span data-stu-id="9df31-251">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="9df31-252">String collection</span><span class="sxs-lookup"><span data-stu-id="9df31-252">String collection</span></span>|<span data-ttu-id="9df31-253">在设备出厂重置之前，将需要进行身份验证的 Google 帐户电子邮件的列表，然后才能对其进行设置。</span><span class="sxs-lookup"><span data-stu-id="9df31-253">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="9df31-254">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="9df31-254">factoryResetBlocked</span></span>|<span data-ttu-id="9df31-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="9df31-255">Boolean</span></span>|<span data-ttu-id="9df31-256">指示是否禁用了 "设置" 中的 "恢复出厂设置" 选项。</span><span class="sxs-lookup"><span data-stu-id="9df31-256">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="9df31-257">globalProxy</span><span class="sxs-lookup"><span data-stu-id="9df31-257">globalProxy</span></span>|[<span data-ttu-id="9df31-258">androidDeviceOwnerGlobalProxy</span><span class="sxs-lookup"><span data-stu-id="9df31-258">androidDeviceOwnerGlobalProxy</span></span>](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)|<span data-ttu-id="9df31-259">代理是与主机、端口和已排除的主机直接建立的。</span><span class="sxs-lookup"><span data-stu-id="9df31-259">Proxy is set up directly with host, port and excluded hosts.</span></span>|
|<span data-ttu-id="9df31-260">googleAccountsBlocked</span><span class="sxs-lookup"><span data-stu-id="9df31-260">googleAccountsBlocked</span></span>|<span data-ttu-id="9df31-261">布尔</span><span class="sxs-lookup"><span data-stu-id="9df31-261">Boolean</span></span>|<span data-ttu-id="9df31-262">指示是否将阻止 google 帐户。</span><span class="sxs-lookup"><span data-stu-id="9df31-262">Indicates whether or not google accounts will be blocked.</span></span>|
|<span data-ttu-id="9df31-263">kioskModeScreenSaverConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="9df31-263">kioskModeScreenSaverConfigurationEnabled</span></span>|<span data-ttu-id="9df31-264">布尔</span><span class="sxs-lookup"><span data-stu-id="9df31-264">Boolean</span></span>|<span data-ttu-id="9df31-265">是否启用屏幕保护程序模式或不启用展台模式。</span><span class="sxs-lookup"><span data-stu-id="9df31-265">Whether or not to enable screen saver mode or not in Kiosk Mode.</span></span>|
|<span data-ttu-id="9df31-266">kioskModeScreenSaverImageUrl</span><span class="sxs-lookup"><span data-stu-id="9df31-266">kioskModeScreenSaverImageUrl</span></span>|<span data-ttu-id="9df31-267">String</span><span class="sxs-lookup"><span data-stu-id="9df31-267">String</span></span>|<span data-ttu-id="9df31-268">将作为展台模式下设备的屏幕保护程序的图像的 URL。</span><span class="sxs-lookup"><span data-stu-id="9df31-268">URL for an image that will be the device's screen saver in Kiosk Mode.</span></span>|
|<span data-ttu-id="9df31-269">kioskModeScreenSaverDisplayTimeInSeconds</span><span class="sxs-lookup"><span data-stu-id="9df31-269">kioskModeScreenSaverDisplayTimeInSeconds</span></span>|<span data-ttu-id="9df31-270">Int32</span><span class="sxs-lookup"><span data-stu-id="9df31-270">Int32</span></span>|<span data-ttu-id="9df31-271">设备将在展台模式下显示屏幕保护程序的秒数。</span><span class="sxs-lookup"><span data-stu-id="9df31-271">The number of seconds that the device will display the screen saver for in Kiosk Mode.</span></span> <span data-ttu-id="9df31-272">有效值为0至9999999</span><span class="sxs-lookup"><span data-stu-id="9df31-272">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="9df31-273">kioskModeScreenSaverStartDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="9df31-273">kioskModeScreenSaverStartDelayInSeconds</span></span>|<span data-ttu-id="9df31-274">Int32</span><span class="sxs-lookup"><span data-stu-id="9df31-274">Int32</span></span>|<span data-ttu-id="9df31-275">在 Kiosk 模式下显示屏幕保护程序之前设备需要保持非活动状态的秒数。</span><span class="sxs-lookup"><span data-stu-id="9df31-275">The number of seconds the device needs to be inactive for before the screen saver is shown in Kiosk Mode.</span></span> <span data-ttu-id="9df31-276">有效值为1至9999999</span><span class="sxs-lookup"><span data-stu-id="9df31-276">Valid values 1 to 9999999</span></span>|
|<span data-ttu-id="9df31-277">kioskModeScreenSaverDetectMediaDisabled</span><span class="sxs-lookup"><span data-stu-id="9df31-277">kioskModeScreenSaverDetectMediaDisabled</span></span>|<span data-ttu-id="9df31-278">布尔</span><span class="sxs-lookup"><span data-stu-id="9df31-278">Boolean</span></span>|<span data-ttu-id="9df31-279">如果音频/视频在展台模式下播放，则设备屏幕是否应显示屏幕保护程序。</span><span class="sxs-lookup"><span data-stu-id="9df31-279">Whether or not the device screen should show the screen saver if audio/video is playing in Kiosk Mode.</span></span>|
|<span data-ttu-id="9df31-280">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="9df31-280">kioskModeApps</span></span>|<span data-ttu-id="9df31-281">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9df31-281">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="9df31-282">设备处于展台模式时将显示的托管应用列表。</span><span class="sxs-lookup"><span data-stu-id="9df31-282">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="9df31-283">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="9df31-283">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="9df31-284">kioskModeWallpaperUrl</span><span class="sxs-lookup"><span data-stu-id="9df31-284">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="9df31-285">String</span><span class="sxs-lookup"><span data-stu-id="9df31-285">String</span></span>|<span data-ttu-id="9df31-286">在设备处于展台模式时用于墙纸的可公开访问图像的 URL。</span><span class="sxs-lookup"><span data-stu-id="9df31-286">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="9df31-287">kioskModeExitCode</span><span class="sxs-lookup"><span data-stu-id="9df31-287">kioskModeExitCode</span></span>|<span data-ttu-id="9df31-288">String</span><span class="sxs-lookup"><span data-stu-id="9df31-288">String</span></span>|<span data-ttu-id="9df31-289">退出代码，以允许用户在设备处于展台模式时从展台模式中进行转义。</span><span class="sxs-lookup"><span data-stu-id="9df31-289">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="9df31-290">kioskModeVirtualHomeButtonEnabled</span><span class="sxs-lookup"><span data-stu-id="9df31-290">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="9df31-291">布尔</span><span class="sxs-lookup"><span data-stu-id="9df31-291">Boolean</span></span>|<span data-ttu-id="9df31-292">设备处于展台模式时是否显示虚拟 "主页" 按钮。</span><span class="sxs-lookup"><span data-stu-id="9df31-292">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="9df31-293">kioskModeVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="9df31-293">kioskModeVirtualHomeButtonType</span></span>|[<span data-ttu-id="9df31-294">androidDeviceOwnerVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="9df31-294">androidDeviceOwnerVirtualHomeButtonType</span></span>](../resources/intune-deviceconfig-androiddeviceownervirtualhomebuttontype.md)|<span data-ttu-id="9df31-295">指示虚拟 home 按钮是否为向上轻扫主页按钮或浮动主页按钮。</span><span class="sxs-lookup"><span data-stu-id="9df31-295">Indicates whether the virtual home button is a swipe up home button or a floating home button.</span></span> <span data-ttu-id="9df31-296">可取值为：`notConfigured`、`swipeUp`、`floating`。</span><span class="sxs-lookup"><span data-stu-id="9df31-296">Possible values are: `notConfigured`, `swipeUp`, `floating`.</span></span>|
|<span data-ttu-id="9df31-297">kioskModeBluetoothConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="9df31-297">kioskModeBluetoothConfigurationEnabled</span></span>|<span data-ttu-id="9df31-298">布尔</span><span class="sxs-lookup"><span data-stu-id="9df31-298">Boolean</span></span>|<span data-ttu-id="9df31-299">是否允许用户在展台模式下配置蓝牙设置。</span><span class="sxs-lookup"><span data-stu-id="9df31-299">Whether or not to allow a user to configure Bluetooth settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="9df31-300">kioskModeWiFiConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="9df31-300">kioskModeWiFiConfigurationEnabled</span></span>|<span data-ttu-id="9df31-301">布尔</span><span class="sxs-lookup"><span data-stu-id="9df31-301">Boolean</span></span>|<span data-ttu-id="9df31-302">是否允许用户在展台模式下配置 Wi-Fi 设置。</span><span class="sxs-lookup"><span data-stu-id="9df31-302">Whether or not to allow a user to configure Wi-Fi settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="9df31-303">kioskModeFlashlightConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="9df31-303">kioskModeFlashlightConfigurationEnabled</span></span>|<span data-ttu-id="9df31-304">布尔</span><span class="sxs-lookup"><span data-stu-id="9df31-304">Boolean</span></span>|<span data-ttu-id="9df31-305">是否允许用户在展台模式下使用该模式。</span><span class="sxs-lookup"><span data-stu-id="9df31-305">Whether or not to allow a user to use the flashlight in Kiosk Mode.</span></span>|
|<span data-ttu-id="9df31-306">kioskModeMediaVolumeConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="9df31-306">kioskModeMediaVolumeConfigurationEnabled</span></span>|<span data-ttu-id="9df31-307">布尔</span><span class="sxs-lookup"><span data-stu-id="9df31-307">Boolean</span></span>|<span data-ttu-id="9df31-308">是否允许用户在展台模式下更改媒体音量。</span><span class="sxs-lookup"><span data-stu-id="9df31-308">Whether or not to allow a user to change the media volume in Kiosk Mode.</span></span>|
|<span data-ttu-id="9df31-309">kioskModeShowDeviceInfo</span><span class="sxs-lookup"><span data-stu-id="9df31-309">kioskModeShowDeviceInfo</span></span>|<span data-ttu-id="9df31-310">布尔</span><span class="sxs-lookup"><span data-stu-id="9df31-310">Boolean</span></span>|<span data-ttu-id="9df31-311">是否允许用户访问基本设备信息。</span><span class="sxs-lookup"><span data-stu-id="9df31-311">Whether or not to allow a user to access basic device information.</span></span>|
|<span data-ttu-id="9df31-312">kioskModeManagedSettingsEntryDisabled</span><span class="sxs-lookup"><span data-stu-id="9df31-312">kioskModeManagedSettingsEntryDisabled</span></span>|<span data-ttu-id="9df31-313">布尔</span><span class="sxs-lookup"><span data-stu-id="9df31-313">Boolean</span></span>|<span data-ttu-id="9df31-314">是否在展台模式下在托管的主屏幕上显示托管设置入口点。</span><span class="sxs-lookup"><span data-stu-id="9df31-314">Whether or not to display the Managed Settings entry point on the managed home screen in Kiosk Mode.</span></span>|
|<span data-ttu-id="9df31-315">kioskModeDebugMenuEasyAccessEnabled</span><span class="sxs-lookup"><span data-stu-id="9df31-315">kioskModeDebugMenuEasyAccessEnabled</span></span>|<span data-ttu-id="9df31-316">布尔</span><span class="sxs-lookup"><span data-stu-id="9df31-316">Boolean</span></span>|<span data-ttu-id="9df31-317">是否允许用户在展台模式下轻松访问 "调试" 菜单。</span><span class="sxs-lookup"><span data-stu-id="9df31-317">Whether or not to allow a user to easy access to the debug menu in Kiosk Mode.</span></span>|
|<span data-ttu-id="9df31-318">kioskModeShowAppNotificationBadge</span><span class="sxs-lookup"><span data-stu-id="9df31-318">kioskModeShowAppNotificationBadge</span></span>|<span data-ttu-id="9df31-319">布尔</span><span class="sxs-lookup"><span data-stu-id="9df31-319">Boolean</span></span>|<span data-ttu-id="9df31-320">是否在展台模式下显示应用程序通知徽章。</span><span class="sxs-lookup"><span data-stu-id="9df31-320">Whether or not to display application notification badges in Kiosk Mode.</span></span>|
|<span data-ttu-id="9df31-321">kioskModeScreenOrientation</span><span class="sxs-lookup"><span data-stu-id="9df31-321">kioskModeScreenOrientation</span></span>|[<span data-ttu-id="9df31-322">androidDeviceOwnerKioskModeScreenOrientation</span><span class="sxs-lookup"><span data-stu-id="9df31-322">androidDeviceOwnerKioskModeScreenOrientation</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskmodescreenorientation.md)|<span data-ttu-id="9df31-323">在展台模式下管理的主屏幕的屏幕方向配置。</span><span class="sxs-lookup"><span data-stu-id="9df31-323">Screen orientation configuration for managed home screen in Kiosk Mode.</span></span> <span data-ttu-id="9df31-324">可取值为：`notConfigured`、`portrait`、`landscape`、`autoRotate`。</span><span class="sxs-lookup"><span data-stu-id="9df31-324">Possible values are: `notConfigured`, `portrait`, `landscape`, `autoRotate`.</span></span>|
|<span data-ttu-id="9df31-325">kioskModeIconSize</span><span class="sxs-lookup"><span data-stu-id="9df31-325">kioskModeIconSize</span></span>|[<span data-ttu-id="9df31-326">androidDeviceOwnerKioskModeIconSize</span><span class="sxs-lookup"><span data-stu-id="9df31-326">androidDeviceOwnerKioskModeIconSize</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskmodeiconsize.md)|<span data-ttu-id="9df31-327">在展台模式下，管理的主屏幕的图标大小配置。</span><span class="sxs-lookup"><span data-stu-id="9df31-327">Icon size configuration for managed home screen in Kiosk Mode.</span></span> <span data-ttu-id="9df31-328">可取值为：`notConfigured`、`smallest`、`small`、`regular`、`large`、`largest`。</span><span class="sxs-lookup"><span data-stu-id="9df31-328">Possible values are: `notConfigured`, `smallest`, `small`, `regular`, `large`, `largest`.</span></span>|
|<span data-ttu-id="9df31-329">kioskModeFolderIcon</span><span class="sxs-lookup"><span data-stu-id="9df31-329">kioskModeFolderIcon</span></span>|[<span data-ttu-id="9df31-330">androidDeviceOwnerKioskModeFolderIcon</span><span class="sxs-lookup"><span data-stu-id="9df31-330">androidDeviceOwnerKioskModeFolderIcon</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskmodefoldericon.md)|<span data-ttu-id="9df31-331">展台模式下的托管主屏幕的文件夹图标配置。</span><span class="sxs-lookup"><span data-stu-id="9df31-331">Folder icon configuration for managed home screen in Kiosk Mode.</span></span> <span data-ttu-id="9df31-332">可取值为：`notConfigured`、`darkSquare`、`darkCircle`、`lightSquare`、`lightCircle`。</span><span class="sxs-lookup"><span data-stu-id="9df31-332">Possible values are: `notConfigured`, `darkSquare`, `darkCircle`, `lightSquare`, `lightCircle`.</span></span>|
|<span data-ttu-id="9df31-333">kioskModeWifiAllowedSsids</span><span class="sxs-lookup"><span data-stu-id="9df31-333">kioskModeWifiAllowedSsids</span></span>|<span data-ttu-id="9df31-334">String collection</span><span class="sxs-lookup"><span data-stu-id="9df31-334">String collection</span></span>|<span data-ttu-id="9df31-335">可供用户在展台模式下进行配置的受限制的 WIFI Ssid 集。</span><span class="sxs-lookup"><span data-stu-id="9df31-335">The restricted set of WIFI SSIDs available for the user to configure in Kiosk Mode.</span></span> <span data-ttu-id="9df31-336">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="9df31-336">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="9df31-337">microphoneForceMute</span><span class="sxs-lookup"><span data-stu-id="9df31-337">microphoneForceMute</span></span>|<span data-ttu-id="9df31-338">布尔</span><span class="sxs-lookup"><span data-stu-id="9df31-338">Boolean</span></span>|<span data-ttu-id="9df31-339">指示是否阻止观众在设备上的麦克风。</span><span class="sxs-lookup"><span data-stu-id="9df31-339">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="9df31-340">networkEscapeHatchAllowed</span><span class="sxs-lookup"><span data-stu-id="9df31-340">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="9df31-341">布尔</span><span class="sxs-lookup"><span data-stu-id="9df31-341">Boolean</span></span>|<span data-ttu-id="9df31-342">指示在引导时设备是否允许连接到临时网络连接。</span><span class="sxs-lookup"><span data-stu-id="9df31-342">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="9df31-343">nfcBlockOutgoingBeam</span><span class="sxs-lookup"><span data-stu-id="9df31-343">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="9df31-344">布尔</span><span class="sxs-lookup"><span data-stu-id="9df31-344">Boolean</span></span>|<span data-ttu-id="9df31-345">指示是否阻止 NFC 传出横梁。</span><span class="sxs-lookup"><span data-stu-id="9df31-345">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="9df31-346">passwordBlockKeyguard</span><span class="sxs-lookup"><span data-stu-id="9df31-346">passwordBlockKeyguard</span></span>|<span data-ttu-id="9df31-347">布尔</span><span class="sxs-lookup"><span data-stu-id="9df31-347">Boolean</span></span>|<span data-ttu-id="9df31-348">指示是否禁用 keyguard。</span><span class="sxs-lookup"><span data-stu-id="9df31-348">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="9df31-349">passwordBlockKeyguardFeatures</span><span class="sxs-lookup"><span data-stu-id="9df31-349">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="9df31-350">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9df31-350">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="9df31-351">要阻止的设备 keyguard 功能的列表。</span><span class="sxs-lookup"><span data-stu-id="9df31-351">List of device keyguard features to block.</span></span> <span data-ttu-id="9df31-352">该集合最多可包含 7 个元素。</span><span class="sxs-lookup"><span data-stu-id="9df31-352">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="9df31-353">可取值为：`notConfigured`、`camera`、`notifications`、`unredactedNotifications`、`trustAgents`、`fingerprint`、`remoteInput`、`allFeatures`。</span><span class="sxs-lookup"><span data-stu-id="9df31-353">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="9df31-354">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="9df31-354">passwordExpirationDays</span></span>|<span data-ttu-id="9df31-355">Int32</span><span class="sxs-lookup"><span data-stu-id="9df31-355">Int32</span></span>|<span data-ttu-id="9df31-356">指示密码在过期之前可以设置的时间量，并需要新密码。</span><span class="sxs-lookup"><span data-stu-id="9df31-356">Indicates the amount of time that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="9df31-357">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="9df31-357">Valid values 1 to 365</span></span>|
|<span data-ttu-id="9df31-358">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="9df31-358">passwordMinimumLength</span></span>|<span data-ttu-id="9df31-359">Int32</span><span class="sxs-lookup"><span data-stu-id="9df31-359">Int32</span></span>|<span data-ttu-id="9df31-360">指示设备上所需密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="9df31-360">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="9df31-361">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="9df31-361">Valid values 4 to 16</span></span>|
|<span data-ttu-id="9df31-362">passwordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="9df31-362">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="9df31-363">Int32</span><span class="sxs-lookup"><span data-stu-id="9df31-363">Int32</span></span>|<span data-ttu-id="9df31-364">指示设备密码所需的字母字符的最小数量。</span><span class="sxs-lookup"><span data-stu-id="9df31-364">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="9df31-365">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="9df31-365">Valid values 1 to 16</span></span>|
|<span data-ttu-id="9df31-366">passwordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="9df31-366">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="9df31-367">Int32</span><span class="sxs-lookup"><span data-stu-id="9df31-367">Int32</span></span>|<span data-ttu-id="9df31-368">指示设备密码所需的最小小写字符数。</span><span class="sxs-lookup"><span data-stu-id="9df31-368">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="9df31-369">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="9df31-369">Valid values 1 to 16</span></span>|
|<span data-ttu-id="9df31-370">passwordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="9df31-370">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="9df31-371">Int32</span><span class="sxs-lookup"><span data-stu-id="9df31-371">Int32</span></span>|<span data-ttu-id="9df31-372">指示设备密码所需的最小非字母字符数。</span><span class="sxs-lookup"><span data-stu-id="9df31-372">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="9df31-373">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="9df31-373">Valid values 1 to 16</span></span>|
|<span data-ttu-id="9df31-374">passwordMinimumNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="9df31-374">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="9df31-375">Int32</span><span class="sxs-lookup"><span data-stu-id="9df31-375">Int32</span></span>|<span data-ttu-id="9df31-376">指示设备密码所需的最小数字字符数。</span><span class="sxs-lookup"><span data-stu-id="9df31-376">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="9df31-377">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="9df31-377">Valid values 1 to 16</span></span>|
|<span data-ttu-id="9df31-378">passwordMinimumSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="9df31-378">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="9df31-379">Int32</span><span class="sxs-lookup"><span data-stu-id="9df31-379">Int32</span></span>|<span data-ttu-id="9df31-380">指示设备密码所需的最小符号字符数。</span><span class="sxs-lookup"><span data-stu-id="9df31-380">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="9df31-381">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="9df31-381">Valid values 1 to 16</span></span>|
|<span data-ttu-id="9df31-382">passwordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="9df31-382">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="9df31-383">Int32</span><span class="sxs-lookup"><span data-stu-id="9df31-383">Int32</span></span>|<span data-ttu-id="9df31-384">指示设备密码所需的大写字母字符的最小数量。</span><span class="sxs-lookup"><span data-stu-id="9df31-384">Indicates the minimum number of upper case letter characters required for device password.</span></span> <span data-ttu-id="9df31-385">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="9df31-385">Valid values 1 to 16</span></span>|
|<span data-ttu-id="9df31-386">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="9df31-386">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="9df31-387">Int32</span><span class="sxs-lookup"><span data-stu-id="9df31-387">Int32</span></span>|<span data-ttu-id="9df31-388">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="9df31-388">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="9df31-389">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="9df31-389">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="9df31-390">Int32</span><span class="sxs-lookup"><span data-stu-id="9df31-390">Int32</span></span>|<span data-ttu-id="9df31-391">指示密码历史记录的长度，其中用户将不能输入与历史记录中的任何密码相同的新密码。</span><span class="sxs-lookup"><span data-stu-id="9df31-391">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="9df31-392">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="9df31-392">Valid values 0 to 24</span></span>|
|<span data-ttu-id="9df31-393">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="9df31-393">passwordRequiredType</span></span>|[<span data-ttu-id="9df31-394">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="9df31-394">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="9df31-395">指示设备上所需的最小密码质量。</span><span class="sxs-lookup"><span data-stu-id="9df31-395">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="9df31-396">可取值为：`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`customPassword`。</span><span class="sxs-lookup"><span data-stu-id="9df31-396">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|
|<span data-ttu-id="9df31-397">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="9df31-397">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="9df31-398">Int32</span><span class="sxs-lookup"><span data-stu-id="9df31-398">Int32</span></span>|<span data-ttu-id="9df31-399">指示用户在擦除设备之前可以输入不正确密码的次数。</span><span class="sxs-lookup"><span data-stu-id="9df31-399">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="9df31-400">有效值为 4 至 11</span><span class="sxs-lookup"><span data-stu-id="9df31-400">Valid values 4 to 11</span></span>|
|<span data-ttu-id="9df31-401">playStoreMode</span><span class="sxs-lookup"><span data-stu-id="9df31-401">playStoreMode</span></span>|[<span data-ttu-id="9df31-402">androidDeviceOwnerPlayStoreMode</span><span class="sxs-lookup"><span data-stu-id="9df31-402">androidDeviceOwnerPlayStoreMode</span></span>](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|<span data-ttu-id="9df31-403">指示设备的播放存储模式。</span><span class="sxs-lookup"><span data-stu-id="9df31-403">Indicates the Play Store mode of the device.</span></span> <span data-ttu-id="9df31-404">可取值为：`notConfigured`、`allowList`、`blockList`。</span><span class="sxs-lookup"><span data-stu-id="9df31-404">Possible values are: `notConfigured`, `allowList`, `blockList`.</span></span>|
|<span data-ttu-id="9df31-405">safeBootBlocked</span><span class="sxs-lookup"><span data-stu-id="9df31-405">safeBootBlocked</span></span>|<span data-ttu-id="9df31-406">布尔</span><span class="sxs-lookup"><span data-stu-id="9df31-406">Boolean</span></span>|<span data-ttu-id="9df31-407">指示是否禁用重新启动设备到安全启动。</span><span class="sxs-lookup"><span data-stu-id="9df31-407">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="9df31-408">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="9df31-408">screenCaptureBlocked</span></span>|<span data-ttu-id="9df31-409">Boolean</span><span class="sxs-lookup"><span data-stu-id="9df31-409">Boolean</span></span>|<span data-ttu-id="9df31-410">指示是否禁用获取屏幕截图的功能。</span><span class="sxs-lookup"><span data-stu-id="9df31-410">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="9df31-411">securityAllowDebuggingFeatures</span><span class="sxs-lookup"><span data-stu-id="9df31-411">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="9df31-412">布尔</span><span class="sxs-lookup"><span data-stu-id="9df31-412">Boolean</span></span>|<span data-ttu-id="9df31-413">指示是否阻止用户启用设备上的调试功能。</span><span class="sxs-lookup"><span data-stu-id="9df31-413">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="9df31-414">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="9df31-414">securityRequireVerifyApps</span></span>|<span data-ttu-id="9df31-415">Boolean</span><span class="sxs-lookup"><span data-stu-id="9df31-415">Boolean</span></span>|<span data-ttu-id="9df31-416">指示是否需要验证应用。</span><span class="sxs-lookup"><span data-stu-id="9df31-416">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="9df31-417">statusBarBlocked</span><span class="sxs-lookup"><span data-stu-id="9df31-417">statusBarBlocked</span></span>|<span data-ttu-id="9df31-418">布尔</span><span class="sxs-lookup"><span data-stu-id="9df31-418">Boolean</span></span>|<span data-ttu-id="9df31-419">指示是否禁用状态栏，包括通知、快速设置和其他屏幕重叠。</span><span class="sxs-lookup"><span data-stu-id="9df31-419">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="9df31-420">stayOnModes</span><span class="sxs-lookup"><span data-stu-id="9df31-420">stayOnModes</span></span>|<span data-ttu-id="9df31-421">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9df31-421">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="9df31-422">设备的显示将保持开机状态的模式列表。</span><span class="sxs-lookup"><span data-stu-id="9df31-422">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="9df31-423">此集合最多可包含4个元素。</span><span class="sxs-lookup"><span data-stu-id="9df31-423">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="9df31-424">可取值为：`notConfigured`、`ac`、`usb`、`wireless`。</span><span class="sxs-lookup"><span data-stu-id="9df31-424">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="9df31-425">storageAllowUsb</span><span class="sxs-lookup"><span data-stu-id="9df31-425">storageAllowUsb</span></span>|<span data-ttu-id="9df31-426">布尔</span><span class="sxs-lookup"><span data-stu-id="9df31-426">Boolean</span></span>|<span data-ttu-id="9df31-427">指示是否允许 USB 大容量存储。</span><span class="sxs-lookup"><span data-stu-id="9df31-427">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="9df31-428">storageBlockExternalMedia</span><span class="sxs-lookup"><span data-stu-id="9df31-428">storageBlockExternalMedia</span></span>|<span data-ttu-id="9df31-429">布尔</span><span class="sxs-lookup"><span data-stu-id="9df31-429">Boolean</span></span>|<span data-ttu-id="9df31-430">指示是否阻止外部媒体。</span><span class="sxs-lookup"><span data-stu-id="9df31-430">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="9df31-431">storageBlockUsbFileTransfer</span><span class="sxs-lookup"><span data-stu-id="9df31-431">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="9df31-432">布尔</span><span class="sxs-lookup"><span data-stu-id="9df31-432">Boolean</span></span>|<span data-ttu-id="9df31-433">指示是否阻止 USB 文件传输。</span><span class="sxs-lookup"><span data-stu-id="9df31-433">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="9df31-434">systemUpdateWindowStartMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="9df31-434">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="9df31-435">Int32</span><span class="sxs-lookup"><span data-stu-id="9df31-435">Int32</span></span>|<span data-ttu-id="9df31-436">指示系统更新窗口午夜后启动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="9df31-436">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="9df31-437">有效值为0至1440</span><span class="sxs-lookup"><span data-stu-id="9df31-437">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="9df31-438">systemUpdateWindowEndMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="9df31-438">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="9df31-439">Int32</span><span class="sxs-lookup"><span data-stu-id="9df31-439">Int32</span></span>|<span data-ttu-id="9df31-440">指示系统更新窗口结束后的分钟数。</span><span class="sxs-lookup"><span data-stu-id="9df31-440">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="9df31-441">有效值为0至1440</span><span class="sxs-lookup"><span data-stu-id="9df31-441">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="9df31-442">systemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="9df31-442">systemUpdateInstallType</span></span>|[<span data-ttu-id="9df31-443">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="9df31-443">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="9df31-444">系统更新配置的类型。</span><span class="sxs-lookup"><span data-stu-id="9df31-444">The type of system update configuration.</span></span> <span data-ttu-id="9df31-445">可取值为：`deviceDefault`、`postpone`、`windowed`、`automatic`。</span><span class="sxs-lookup"><span data-stu-id="9df31-445">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="9df31-446">systemWindowsBlocked</span><span class="sxs-lookup"><span data-stu-id="9df31-446">systemWindowsBlocked</span></span>|<span data-ttu-id="9df31-447">布尔</span><span class="sxs-lookup"><span data-stu-id="9df31-447">Boolean</span></span>|<span data-ttu-id="9df31-448">是否阻止 Android 系统提示符窗口，如 toast、电话活动和系统通知。</span><span class="sxs-lookup"><span data-stu-id="9df31-448">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="9df31-449">usersBlockAdd</span><span class="sxs-lookup"><span data-stu-id="9df31-449">usersBlockAdd</span></span>|<span data-ttu-id="9df31-450">布尔</span><span class="sxs-lookup"><span data-stu-id="9df31-450">Boolean</span></span>|<span data-ttu-id="9df31-451">指示是否禁用添加用户和配置文件。</span><span class="sxs-lookup"><span data-stu-id="9df31-451">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="9df31-452">usersBlockRemove</span><span class="sxs-lookup"><span data-stu-id="9df31-452">usersBlockRemove</span></span>|<span data-ttu-id="9df31-453">布尔</span><span class="sxs-lookup"><span data-stu-id="9df31-453">Boolean</span></span>|<span data-ttu-id="9df31-454">指示是否禁用从设备中删除其他用户。</span><span class="sxs-lookup"><span data-stu-id="9df31-454">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="9df31-455">volumeBlockAdjustment</span><span class="sxs-lookup"><span data-stu-id="9df31-455">volumeBlockAdjustment</span></span>|<span data-ttu-id="9df31-456">布尔</span><span class="sxs-lookup"><span data-stu-id="9df31-456">Boolean</span></span>|<span data-ttu-id="9df31-457">指示是否禁用了调整主音量。</span><span class="sxs-lookup"><span data-stu-id="9df31-457">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="9df31-458">vpnAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="9df31-458">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="9df31-459">布尔</span><span class="sxs-lookup"><span data-stu-id="9df31-459">Boolean</span></span>|<span data-ttu-id="9df31-460">如果指定了 always on VPN 包名称，则在断开 VPN 连接时是否锁定网络流量。</span><span class="sxs-lookup"><span data-stu-id="9df31-460">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="9df31-461">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="9df31-461">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="9df31-462">String</span><span class="sxs-lookup"><span data-stu-id="9df31-462">String</span></span>|<span data-ttu-id="9df31-463">将处理永不启用 VPN 连接的应用程序的 Android 应用程序包名称。</span><span class="sxs-lookup"><span data-stu-id="9df31-463">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="9df31-464">wifiBlockEditConfigurations</span><span class="sxs-lookup"><span data-stu-id="9df31-464">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="9df31-465">布尔</span><span class="sxs-lookup"><span data-stu-id="9df31-465">Boolean</span></span>|<span data-ttu-id="9df31-466">指示是否阻止用户编辑 wifi 连接设置。</span><span class="sxs-lookup"><span data-stu-id="9df31-466">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="9df31-467">wifiBlockEditPolicyDefinedConfigurations</span><span class="sxs-lookup"><span data-stu-id="9df31-467">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="9df31-468">布尔</span><span class="sxs-lookup"><span data-stu-id="9df31-468">Boolean</span></span>|<span data-ttu-id="9df31-469">指示是否阻止用户仅编辑策略定义的网络。</span><span class="sxs-lookup"><span data-stu-id="9df31-469">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|
|<span data-ttu-id="9df31-470">personalProfileAppsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="9df31-470">personalProfileAppsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="9df31-471">布尔</span><span class="sxs-lookup"><span data-stu-id="9df31-471">Boolean</span></span>|<span data-ttu-id="9df31-472">指示用户是否可以在个人配置文件上安装来自未知源的应用程序。</span><span class="sxs-lookup"><span data-stu-id="9df31-472">Indicates whether the user can install apps from unknown sources on the personal profile.</span></span>|
|<span data-ttu-id="9df31-473">personalProfileCameraBlocked</span><span class="sxs-lookup"><span data-stu-id="9df31-473">personalProfileCameraBlocked</span></span>|<span data-ttu-id="9df31-474">布尔</span><span class="sxs-lookup"><span data-stu-id="9df31-474">Boolean</span></span>|<span data-ttu-id="9df31-475">指示是否禁用个人配置文件上的摄像头的使用。</span><span class="sxs-lookup"><span data-stu-id="9df31-475">Indicates whether to disable the use of the camera on the personal profile.</span></span>|
|<span data-ttu-id="9df31-476">personalProfileScreenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="9df31-476">personalProfileScreenCaptureBlocked</span></span>|<span data-ttu-id="9df31-477">布尔</span><span class="sxs-lookup"><span data-stu-id="9df31-477">Boolean</span></span>|<span data-ttu-id="9df31-478">指示是否禁用在个人配置文件上采用屏幕截图的功能。</span><span class="sxs-lookup"><span data-stu-id="9df31-478">Indicates whether to disable the capability to take screenshots on the personal profile.</span></span>|
|<span data-ttu-id="9df31-479">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="9df31-479">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="9df31-480">Int32</span><span class="sxs-lookup"><span data-stu-id="9df31-480">Int32</span></span>|<span data-ttu-id="9df31-481">指示工作配置文件密码在过期之前可以设置的天数，并将需要新密码。</span><span class="sxs-lookup"><span data-stu-id="9df31-481">Indicates the number of days that a work profile password can be set before it expires and a new password will be required.</span></span> <span data-ttu-id="9df31-482">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="9df31-482">Valid values 1 to 365</span></span>|
|<span data-ttu-id="9df31-483">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="9df31-483">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="9df31-484">Int32</span><span class="sxs-lookup"><span data-stu-id="9df31-484">Int32</span></span>|<span data-ttu-id="9df31-485">指示工作配置文件密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="9df31-485">Indicates the minimum length of the work profile password.</span></span> <span data-ttu-id="9df31-486">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="9df31-486">Valid values 4 to 16</span></span>|
|<span data-ttu-id="9df31-487">workProfilePasswordMinimumNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="9df31-487">workProfilePasswordMinimumNumericCharacters</span></span>|<span data-ttu-id="9df31-488">Int32</span><span class="sxs-lookup"><span data-stu-id="9df31-488">Int32</span></span>|<span data-ttu-id="9df31-489">指示工作配置文件密码所需的最小数字字符数。</span><span class="sxs-lookup"><span data-stu-id="9df31-489">Indicates the minimum number of numeric characters required for the work profile password.</span></span> <span data-ttu-id="9df31-490">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="9df31-490">Valid values 1 to 16</span></span>|
|<span data-ttu-id="9df31-491">workProfilePasswordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="9df31-491">workProfilePasswordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="9df31-492">Int32</span><span class="sxs-lookup"><span data-stu-id="9df31-492">Int32</span></span>|<span data-ttu-id="9df31-493">指示工作配置文件密码所需的最小非字母字符数。</span><span class="sxs-lookup"><span data-stu-id="9df31-493">Indicates the minimum number of non-letter characters required for the work profile password.</span></span> <span data-ttu-id="9df31-494">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="9df31-494">Valid values 1 to 16</span></span>|
|<span data-ttu-id="9df31-495">workProfilePasswordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="9df31-495">workProfilePasswordMinimumLetterCharacters</span></span>|<span data-ttu-id="9df31-496">Int32</span><span class="sxs-lookup"><span data-stu-id="9df31-496">Int32</span></span>|<span data-ttu-id="9df31-497">指示工作配置文件密码所需的字母字符的最小数量。</span><span class="sxs-lookup"><span data-stu-id="9df31-497">Indicates the minimum number of letter characters required for the work profile password.</span></span> <span data-ttu-id="9df31-498">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="9df31-498">Valid values 1 to 16</span></span>|
|<span data-ttu-id="9df31-499">workProfilePasswordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="9df31-499">workProfilePasswordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="9df31-500">Int32</span><span class="sxs-lookup"><span data-stu-id="9df31-500">Int32</span></span>|<span data-ttu-id="9df31-501">指示工作配置文件密码所需的最小小写字符数。</span><span class="sxs-lookup"><span data-stu-id="9df31-501">Indicates the minimum number of lower-case characters required for the work profile password.</span></span> <span data-ttu-id="9df31-502">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="9df31-502">Valid values 1 to 16</span></span>|
|<span data-ttu-id="9df31-503">workProfilePasswordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="9df31-503">workProfilePasswordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="9df31-504">Int32</span><span class="sxs-lookup"><span data-stu-id="9df31-504">Int32</span></span>|<span data-ttu-id="9df31-505">指示工作配置文件密码所需的大写字母字符的最小数量。</span><span class="sxs-lookup"><span data-stu-id="9df31-505">Indicates the minimum number of upper-case letter characters required for the work profile password.</span></span> <span data-ttu-id="9df31-506">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="9df31-506">Valid values 1 to 16</span></span>|
|<span data-ttu-id="9df31-507">workProfilePasswordMinimumSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="9df31-507">workProfilePasswordMinimumSymbolCharacters</span></span>|<span data-ttu-id="9df31-508">Int32</span><span class="sxs-lookup"><span data-stu-id="9df31-508">Int32</span></span>|<span data-ttu-id="9df31-509">指示工作配置文件密码所需的最小符号字符数。</span><span class="sxs-lookup"><span data-stu-id="9df31-509">Indicates the minimum number of symbol characters required for the work profile password.</span></span> <span data-ttu-id="9df31-510">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="9df31-510">Valid values 1 to 16</span></span>|
|<span data-ttu-id="9df31-511">workProfilePasswordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="9df31-511">workProfilePasswordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="9df31-512">Int32</span><span class="sxs-lookup"><span data-stu-id="9df31-512">Int32</span></span>|<span data-ttu-id="9df31-513">指示工作配置文件密码历史记录的长度，其中用户将不能输入与历史记录中的任何密码相同的新密码。</span><span class="sxs-lookup"><span data-stu-id="9df31-513">Indicates the length of the work profile password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="9df31-514">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="9df31-514">Valid values 0 to 24</span></span>|
|<span data-ttu-id="9df31-515">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="9df31-515">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="9df31-516">Int32</span><span class="sxs-lookup"><span data-stu-id="9df31-516">Int32</span></span>|<span data-ttu-id="9df31-517">指示用户在擦除设备之前可以输入不正确的工作配置文件密码的次数。</span><span class="sxs-lookup"><span data-stu-id="9df31-517">Indicates the number of times a user can enter an incorrect work profile password before the device is wiped.</span></span> <span data-ttu-id="9df31-518">有效值为 4 至 11</span><span class="sxs-lookup"><span data-stu-id="9df31-518">Valid values 4 to 11</span></span>|
|<span data-ttu-id="9df31-519">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="9df31-519">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="9df31-520">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="9df31-520">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="9df31-521">指示工作配置文件密码所需的最小密码质量。</span><span class="sxs-lookup"><span data-stu-id="9df31-521">Indicates the minimum password quality required on the work profile password.</span></span> <span data-ttu-id="9df31-522">可取值为：`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`customPassword`。</span><span class="sxs-lookup"><span data-stu-id="9df31-522">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|



## <a name="response"></a><span data-ttu-id="9df31-523">响应</span><span class="sxs-lookup"><span data-stu-id="9df31-523">Response</span></span>
<span data-ttu-id="9df31-524">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9df31-524">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9df31-525">示例</span><span class="sxs-lookup"><span data-stu-id="9df31-525">Example</span></span>

### <a name="request"></a><span data-ttu-id="9df31-526">请求</span><span class="sxs-lookup"><span data-stu-id="9df31-526">Request</span></span>
<span data-ttu-id="9df31-527">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9df31-527">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 6096

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

### <a name="response"></a><span data-ttu-id="9df31-528">响应</span><span class="sxs-lookup"><span data-stu-id="9df31-528">Response</span></span>
<span data-ttu-id="9df31-p154">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9df31-p154">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 6268

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





