---
title: 更新 androidDeviceOwnerGeneralDeviceConfiguration
description: 更新 androidDeviceOwnerGeneralDeviceConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cc6746dca524394be358d1a4c31fc5cfe53c001b
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793113"
---
# <a name="update-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="271c2-103">更新 androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="271c2-103">Update androidDeviceOwnerGeneralDeviceConfiguration</span></span>

<span data-ttu-id="271c2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="271c2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="271c2-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="271c2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="271c2-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="271c2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="271c2-107">更新[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="271c2-107">Update the properties of a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="271c2-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="271c2-108">Prerequisites</span></span>
<span data-ttu-id="271c2-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="271c2-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="271c2-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="271c2-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="271c2-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="271c2-111">Permission type</span></span>|<span data-ttu-id="271c2-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="271c2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="271c2-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="271c2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="271c2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="271c2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="271c2-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="271c2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="271c2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="271c2-116">Not supported.</span></span>|
|<span data-ttu-id="271c2-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="271c2-117">Application</span></span>|<span data-ttu-id="271c2-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="271c2-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="271c2-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="271c2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="271c2-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="271c2-120">Request headers</span></span>
|<span data-ttu-id="271c2-121">标头</span><span class="sxs-lookup"><span data-stu-id="271c2-121">Header</span></span>|<span data-ttu-id="271c2-122">值</span><span class="sxs-lookup"><span data-stu-id="271c2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="271c2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="271c2-123">Authorization</span></span>|<span data-ttu-id="271c2-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="271c2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="271c2-125">接受</span><span class="sxs-lookup"><span data-stu-id="271c2-125">Accept</span></span>|<span data-ttu-id="271c2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="271c2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="271c2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="271c2-127">Request body</span></span>
<span data-ttu-id="271c2-128">在请求正文中，提供[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="271c2-128">In the request body, supply a JSON representation for the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="271c2-129">下表显示创建[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="271c2-129">The following table shows the properties that are required when you create the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="271c2-130">属性</span><span class="sxs-lookup"><span data-stu-id="271c2-130">Property</span></span>|<span data-ttu-id="271c2-131">类型</span><span class="sxs-lookup"><span data-stu-id="271c2-131">Type</span></span>|<span data-ttu-id="271c2-132">说明</span><span class="sxs-lookup"><span data-stu-id="271c2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="271c2-133">id</span><span class="sxs-lookup"><span data-stu-id="271c2-133">id</span></span>|<span data-ttu-id="271c2-134">字符串</span><span class="sxs-lookup"><span data-stu-id="271c2-134">String</span></span>|<span data-ttu-id="271c2-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="271c2-135">Key of the entity.</span></span> <span data-ttu-id="271c2-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="271c2-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="271c2-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="271c2-137">lastModifiedDateTime</span></span>|<span data-ttu-id="271c2-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="271c2-138">DateTimeOffset</span></span>|<span data-ttu-id="271c2-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="271c2-139">DateTime the object was last modified.</span></span> <span data-ttu-id="271c2-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="271c2-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="271c2-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="271c2-141">roleScopeTagIds</span></span>|<span data-ttu-id="271c2-142">String collection</span><span class="sxs-lookup"><span data-stu-id="271c2-142">String collection</span></span>|<span data-ttu-id="271c2-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="271c2-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="271c2-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="271c2-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="271c2-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="271c2-145">supportsScopeTags</span></span>|<span data-ttu-id="271c2-146">布尔值</span><span class="sxs-lookup"><span data-stu-id="271c2-146">Boolean</span></span>|<span data-ttu-id="271c2-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="271c2-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="271c2-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="271c2-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="271c2-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="271c2-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="271c2-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="271c2-150">This property is read-only.</span></span> <span data-ttu-id="271c2-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="271c2-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="271c2-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="271c2-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="271c2-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="271c2-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="271c2-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="271c2-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="271c2-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="271c2-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="271c2-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="271c2-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="271c2-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="271c2-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="271c2-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="271c2-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="271c2-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="271c2-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="271c2-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="271c2-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="271c2-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="271c2-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="271c2-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="271c2-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="271c2-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="271c2-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="271c2-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="271c2-164">createdDateTime</span></span>|<span data-ttu-id="271c2-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="271c2-165">DateTimeOffset</span></span>|<span data-ttu-id="271c2-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="271c2-166">DateTime the object was created.</span></span> <span data-ttu-id="271c2-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="271c2-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="271c2-168">说明</span><span class="sxs-lookup"><span data-stu-id="271c2-168">description</span></span>|<span data-ttu-id="271c2-169">String</span><span class="sxs-lookup"><span data-stu-id="271c2-169">String</span></span>|<span data-ttu-id="271c2-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="271c2-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="271c2-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="271c2-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="271c2-172">displayName</span><span class="sxs-lookup"><span data-stu-id="271c2-172">displayName</span></span>|<span data-ttu-id="271c2-173">String</span><span class="sxs-lookup"><span data-stu-id="271c2-173">String</span></span>|<span data-ttu-id="271c2-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="271c2-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="271c2-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="271c2-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="271c2-176">version</span><span class="sxs-lookup"><span data-stu-id="271c2-176">version</span></span>|<span data-ttu-id="271c2-177">Int32</span><span class="sxs-lookup"><span data-stu-id="271c2-177">Int32</span></span>|<span data-ttu-id="271c2-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="271c2-178">Version of the device configuration.</span></span> <span data-ttu-id="271c2-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="271c2-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="271c2-180">accountsBlockModification</span><span class="sxs-lookup"><span data-stu-id="271c2-180">accountsBlockModification</span></span>|<span data-ttu-id="271c2-181">布尔值</span><span class="sxs-lookup"><span data-stu-id="271c2-181">Boolean</span></span>|<span data-ttu-id="271c2-182">指示是否禁用添加或删除帐户。</span><span class="sxs-lookup"><span data-stu-id="271c2-182">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="271c2-183">appsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="271c2-183">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="271c2-184">布尔值</span><span class="sxs-lookup"><span data-stu-id="271c2-184">Boolean</span></span>|<span data-ttu-id="271c2-185">指示是否允许用户启用 "未知源" 设置。</span><span class="sxs-lookup"><span data-stu-id="271c2-185">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="271c2-186">appsAutoUpdatePolicy</span><span class="sxs-lookup"><span data-stu-id="271c2-186">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="271c2-187">androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="271c2-187">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="271c2-188">指示应用程序自动更新策略的值。</span><span class="sxs-lookup"><span data-stu-id="271c2-188">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="271c2-189">可取值为：`notConfigured`、`userChoice`、`never`、`wiFiOnly`、`always`。</span><span class="sxs-lookup"><span data-stu-id="271c2-189">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="271c2-190">appsDefaultPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="271c2-190">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="271c2-191">androidDeviceOwnerDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="271c2-191">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="271c2-192">指示对运行时权限请求的权限策略（如果专门没有为应用程序定义）。</span><span class="sxs-lookup"><span data-stu-id="271c2-192">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="271c2-193">可取值为：`deviceDefault`、`prompt`、`autoGrant`、`autoDeny`。</span><span class="sxs-lookup"><span data-stu-id="271c2-193">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="271c2-194">appsRecommendSkippingFirstUseHints</span><span class="sxs-lookup"><span data-stu-id="271c2-194">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="271c2-195">布尔值</span><span class="sxs-lookup"><span data-stu-id="271c2-195">Boolean</span></span>|<span data-ttu-id="271c2-196">是否建议所有应用都将跳过他们可能已添加的任何首次使用提示。</span><span class="sxs-lookup"><span data-stu-id="271c2-196">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="271c2-197">bluetoothBlockConfiguration</span><span class="sxs-lookup"><span data-stu-id="271c2-197">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="271c2-198">布尔值</span><span class="sxs-lookup"><span data-stu-id="271c2-198">Boolean</span></span>|<span data-ttu-id="271c2-199">指示是否阻止用户配置蓝牙。</span><span class="sxs-lookup"><span data-stu-id="271c2-199">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="271c2-200">bluetoothBlockContactSharing</span><span class="sxs-lookup"><span data-stu-id="271c2-200">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="271c2-201">布尔值</span><span class="sxs-lookup"><span data-stu-id="271c2-201">Boolean</span></span>|<span data-ttu-id="271c2-202">指示是否阻止用户通过蓝牙共享联系人。</span><span class="sxs-lookup"><span data-stu-id="271c2-202">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="271c2-203">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="271c2-203">cameraBlocked</span></span>|<span data-ttu-id="271c2-204">布尔值</span><span class="sxs-lookup"><span data-stu-id="271c2-204">Boolean</span></span>|<span data-ttu-id="271c2-205">指示是否禁用相机的使用。</span><span class="sxs-lookup"><span data-stu-id="271c2-205">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="271c2-206">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="271c2-206">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="271c2-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="271c2-207">Boolean</span></span>|<span data-ttu-id="271c2-208">指示是否阻止 Wi-Fi 网络共享。</span><span class="sxs-lookup"><span data-stu-id="271c2-208">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="271c2-209">certificateCredentialConfigurationDisabled</span><span class="sxs-lookup"><span data-stu-id="271c2-209">certificateCredentialConfigurationDisabled</span></span>|<span data-ttu-id="271c2-210">布尔值</span><span class="sxs-lookup"><span data-stu-id="271c2-210">Boolean</span></span>|<span data-ttu-id="271c2-211">指示是否阻止来自任何证书凭据配置的用户。</span><span class="sxs-lookup"><span data-stu-id="271c2-211">Indicates whether or not to block users from any certificate credential configuration.</span></span>|
|<span data-ttu-id="271c2-212">microsoftLauncherConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="271c2-212">microsoftLauncherConfigurationEnabled</span></span>|<span data-ttu-id="271c2-213">布尔值</span><span class="sxs-lookup"><span data-stu-id="271c2-213">Boolean</span></span>|<span data-ttu-id="271c2-214">指示是否要配置 Microsoft 启动器。</span><span class="sxs-lookup"><span data-stu-id="271c2-214">Indicates whether or not to you want configure Microsoft Launcher.</span></span>|
|<span data-ttu-id="271c2-215">microsoftLauncherCustomWallpaperEnabled</span><span class="sxs-lookup"><span data-stu-id="271c2-215">microsoftLauncherCustomWallpaperEnabled</span></span>|<span data-ttu-id="271c2-216">布尔值</span><span class="sxs-lookup"><span data-stu-id="271c2-216">Boolean</span></span>|<span data-ttu-id="271c2-217">指示是否在目标设备上配置墙纸。</span><span class="sxs-lookup"><span data-stu-id="271c2-217">Indicates whether or not to configure the wallpaper on the targeted devices.</span></span>|
|<span data-ttu-id="271c2-218">microsoftLauncherCustomWallpaperImageUrl</span><span class="sxs-lookup"><span data-stu-id="271c2-218">microsoftLauncherCustomWallpaperImageUrl</span></span>|<span data-ttu-id="271c2-219">String</span><span class="sxs-lookup"><span data-stu-id="271c2-219">String</span></span>|<span data-ttu-id="271c2-220">指示用作目标设备墙纸的图像文件的 URL。</span><span class="sxs-lookup"><span data-stu-id="271c2-220">Indicates the URL for the image file to use as the wallpaper on the targeted devices.</span></span>|
|<span data-ttu-id="271c2-221">microsoftLauncherCustomWallpaperAllowUserModification</span><span class="sxs-lookup"><span data-stu-id="271c2-221">microsoftLauncherCustomWallpaperAllowUserModification</span></span>|<span data-ttu-id="271c2-222">布尔值</span><span class="sxs-lookup"><span data-stu-id="271c2-222">Boolean</span></span>|<span data-ttu-id="271c2-223">指示用户是否可以修改墙纸以个性化设置其设备。</span><span class="sxs-lookup"><span data-stu-id="271c2-223">Indicates whether or not the user can modify the wallpaper to personalize their device.</span></span>|
|<span data-ttu-id="271c2-224">microsoftLauncherFeedEnabled</span><span class="sxs-lookup"><span data-stu-id="271c2-224">microsoftLauncherFeedEnabled</span></span>|<span data-ttu-id="271c2-225">布尔值</span><span class="sxs-lookup"><span data-stu-id="271c2-225">Boolean</span></span>|<span data-ttu-id="271c2-226">指示是否要在设备上启用启动器源。</span><span class="sxs-lookup"><span data-stu-id="271c2-226">Indicates whether or not you want to enable the launcher feed on the device.</span></span>|
|<span data-ttu-id="271c2-227">microsoftLauncherFeedAllowUserModification</span><span class="sxs-lookup"><span data-stu-id="271c2-227">microsoftLauncherFeedAllowUserModification</span></span>|<span data-ttu-id="271c2-228">布尔值</span><span class="sxs-lookup"><span data-stu-id="271c2-228">Boolean</span></span>|<span data-ttu-id="271c2-229">指示用户是否可以修改设备上的启动器源。</span><span class="sxs-lookup"><span data-stu-id="271c2-229">Indicates whether or not the user can modify the launcher feed on the device.</span></span>|
|<span data-ttu-id="271c2-230">microsoftLauncherDockPresenceConfiguration</span><span class="sxs-lookup"><span data-stu-id="271c2-230">microsoftLauncherDockPresenceConfiguration</span></span>|[<span data-ttu-id="271c2-231">microsoftLauncherDockPresence</span><span class="sxs-lookup"><span data-stu-id="271c2-231">microsoftLauncherDockPresence</span></span>](../resources/intune-deviceconfig-microsoftlauncherdockpresence.md)|<span data-ttu-id="271c2-232">指示是否要配置设备停靠。</span><span class="sxs-lookup"><span data-stu-id="271c2-232">Indicates whether or not you want to configure the device dock.</span></span> <span data-ttu-id="271c2-233">可取值为：`notConfigured`、`show`、`hide`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="271c2-233">Possible values are: `notConfigured`, `show`, `hide`, `disabled`.</span></span>|
|<span data-ttu-id="271c2-234">microsoftLauncherDockPresenceAllowUserModification</span><span class="sxs-lookup"><span data-stu-id="271c2-234">microsoftLauncherDockPresenceAllowUserModification</span></span>|<span data-ttu-id="271c2-235">布尔值</span><span class="sxs-lookup"><span data-stu-id="271c2-235">Boolean</span></span>|<span data-ttu-id="271c2-236">指示用户是否可以修改设备上的设备停靠配置。</span><span class="sxs-lookup"><span data-stu-id="271c2-236">Indicates whether or not the user can modify the device dock configuration on the device.</span></span>|
|<span data-ttu-id="271c2-237">microsoftLauncherSearchBarPlacementConfiguration</span><span class="sxs-lookup"><span data-stu-id="271c2-237">microsoftLauncherSearchBarPlacementConfiguration</span></span>|[<span data-ttu-id="271c2-238">microsoftLauncherSearchBarPlacement</span><span class="sxs-lookup"><span data-stu-id="271c2-238">microsoftLauncherSearchBarPlacement</span></span>](../resources/intune-deviceconfig-microsoftlaunchersearchbarplacement.md)|<span data-ttu-id="271c2-239">指示设备上的搜索栏的布局配置。</span><span class="sxs-lookup"><span data-stu-id="271c2-239">Indicates the search bar placement configuration on the device.</span></span> <span data-ttu-id="271c2-240">可取值为：`notConfigured`、`top`、`bottom`、`hide`。</span><span class="sxs-lookup"><span data-stu-id="271c2-240">Possible values are: `notConfigured`, `top`, `bottom`, `hide`.</span></span>|
|<span data-ttu-id="271c2-241">microsoftLauncherSearchBarPlacementAllowUserModification</span><span class="sxs-lookup"><span data-stu-id="271c2-241">microsoftLauncherSearchBarPlacementAllowUserModification</span></span>|<span data-ttu-id="271c2-242">布尔值</span><span class="sxs-lookup"><span data-stu-id="271c2-242">Boolean</span></span>|<span data-ttu-id="271c2-243">指示用户是否可以修改设备上的搜索栏的位置。</span><span class="sxs-lookup"><span data-stu-id="271c2-243">Indicates whether the user can modify the search bar placement on the device.</span></span>|
|<span data-ttu-id="271c2-244">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="271c2-244">enrollmentProfile</span></span>|[<span data-ttu-id="271c2-245">androidDeviceOwnerEnrollmentProfileType</span><span class="sxs-lookup"><span data-stu-id="271c2-245">androidDeviceOwnerEnrollmentProfileType</span></span>](../resources/intune-deviceconfig-androiddeviceownerenrollmentprofiletype.md)|<span data-ttu-id="271c2-246">指示要配置的注册配置文件。</span><span class="sxs-lookup"><span data-stu-id="271c2-246">Indicates which enrollment profile you want to configure.</span></span> <span data-ttu-id="271c2-247">可取值为：`notConfigured`、`dedicatedDevice`、`fullyManaged`。</span><span class="sxs-lookup"><span data-stu-id="271c2-247">Possible values are: `notConfigured`, `dedicatedDevice`, `fullyManaged`.</span></span>|
|<span data-ttu-id="271c2-248">dataRoamingBlocked</span><span class="sxs-lookup"><span data-stu-id="271c2-248">dataRoamingBlocked</span></span>|<span data-ttu-id="271c2-249">布尔值</span><span class="sxs-lookup"><span data-stu-id="271c2-249">Boolean</span></span>|<span data-ttu-id="271c2-250">指示是否阻止用户使用数据漫游。</span><span class="sxs-lookup"><span data-stu-id="271c2-250">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="271c2-251">dateTimeConfigurationBlocked</span><span class="sxs-lookup"><span data-stu-id="271c2-251">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="271c2-252">布尔值</span><span class="sxs-lookup"><span data-stu-id="271c2-252">Boolean</span></span>|<span data-ttu-id="271c2-253">指示是否阻止用户手动更改设备上的日期或时间</span><span class="sxs-lookup"><span data-stu-id="271c2-253">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="271c2-254">factoryResetDeviceAdministratorEmails</span><span class="sxs-lookup"><span data-stu-id="271c2-254">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="271c2-255">String collection</span><span class="sxs-lookup"><span data-stu-id="271c2-255">String collection</span></span>|<span data-ttu-id="271c2-256">在设备出厂重置之前，将需要进行身份验证的 Google 帐户电子邮件的列表，然后才能对其进行设置。</span><span class="sxs-lookup"><span data-stu-id="271c2-256">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="271c2-257">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="271c2-257">factoryResetBlocked</span></span>|<span data-ttu-id="271c2-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="271c2-258">Boolean</span></span>|<span data-ttu-id="271c2-259">指示是否禁用了 "设置" 中的 "恢复出厂设置" 选项。</span><span class="sxs-lookup"><span data-stu-id="271c2-259">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="271c2-260">globalProxy</span><span class="sxs-lookup"><span data-stu-id="271c2-260">globalProxy</span></span>|[<span data-ttu-id="271c2-261">androidDeviceOwnerGlobalProxy</span><span class="sxs-lookup"><span data-stu-id="271c2-261">androidDeviceOwnerGlobalProxy</span></span>](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)|<span data-ttu-id="271c2-262">代理是与主机、端口和已排除的主机直接建立的。</span><span class="sxs-lookup"><span data-stu-id="271c2-262">Proxy is set up directly with host, port and excluded hosts.</span></span>|
|<span data-ttu-id="271c2-263">googleAccountsBlocked</span><span class="sxs-lookup"><span data-stu-id="271c2-263">googleAccountsBlocked</span></span>|<span data-ttu-id="271c2-264">布尔值</span><span class="sxs-lookup"><span data-stu-id="271c2-264">Boolean</span></span>|<span data-ttu-id="271c2-265">指示是否将阻止 google 帐户。</span><span class="sxs-lookup"><span data-stu-id="271c2-265">Indicates whether or not google accounts will be blocked.</span></span>|
|<span data-ttu-id="271c2-266">kioskModeScreenSaverConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="271c2-266">kioskModeScreenSaverConfigurationEnabled</span></span>|<span data-ttu-id="271c2-267">布尔值</span><span class="sxs-lookup"><span data-stu-id="271c2-267">Boolean</span></span>|<span data-ttu-id="271c2-268">是否启用屏幕保护程序模式或不启用展台模式。</span><span class="sxs-lookup"><span data-stu-id="271c2-268">Whether or not to enable screen saver mode or not in Kiosk Mode.</span></span>|
|<span data-ttu-id="271c2-269">kioskModeScreenSaverImageUrl</span><span class="sxs-lookup"><span data-stu-id="271c2-269">kioskModeScreenSaverImageUrl</span></span>|<span data-ttu-id="271c2-270">String</span><span class="sxs-lookup"><span data-stu-id="271c2-270">String</span></span>|<span data-ttu-id="271c2-271">将作为展台模式下设备的屏幕保护程序的图像的 URL。</span><span class="sxs-lookup"><span data-stu-id="271c2-271">URL for an image that will be the device's screen saver in Kiosk Mode.</span></span>|
|<span data-ttu-id="271c2-272">kioskModeScreenSaverDisplayTimeInSeconds</span><span class="sxs-lookup"><span data-stu-id="271c2-272">kioskModeScreenSaverDisplayTimeInSeconds</span></span>|<span data-ttu-id="271c2-273">Int32</span><span class="sxs-lookup"><span data-stu-id="271c2-273">Int32</span></span>|<span data-ttu-id="271c2-274">设备将在展台模式下显示屏幕保护程序的秒数。</span><span class="sxs-lookup"><span data-stu-id="271c2-274">The number of seconds that the device will display the screen saver for in Kiosk Mode.</span></span> <span data-ttu-id="271c2-275">有效值为0至9999999</span><span class="sxs-lookup"><span data-stu-id="271c2-275">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="271c2-276">kioskModeScreenSaverStartDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="271c2-276">kioskModeScreenSaverStartDelayInSeconds</span></span>|<span data-ttu-id="271c2-277">Int32</span><span class="sxs-lookup"><span data-stu-id="271c2-277">Int32</span></span>|<span data-ttu-id="271c2-278">在 Kiosk 模式下显示屏幕保护程序之前设备需要保持非活动状态的秒数。</span><span class="sxs-lookup"><span data-stu-id="271c2-278">The number of seconds the device needs to be inactive for before the screen saver is shown in Kiosk Mode.</span></span> <span data-ttu-id="271c2-279">有效值为1至9999999</span><span class="sxs-lookup"><span data-stu-id="271c2-279">Valid values 1 to 9999999</span></span>|
|<span data-ttu-id="271c2-280">kioskModeScreenSaverDetectMediaDisabled</span><span class="sxs-lookup"><span data-stu-id="271c2-280">kioskModeScreenSaverDetectMediaDisabled</span></span>|<span data-ttu-id="271c2-281">布尔值</span><span class="sxs-lookup"><span data-stu-id="271c2-281">Boolean</span></span>|<span data-ttu-id="271c2-282">如果音频/视频在展台模式下播放，则设备屏幕是否应显示屏幕保护程序。</span><span class="sxs-lookup"><span data-stu-id="271c2-282">Whether or not the device screen should show the screen saver if audio/video is playing in Kiosk Mode.</span></span>|
|<span data-ttu-id="271c2-283">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="271c2-283">kioskModeApps</span></span>|<span data-ttu-id="271c2-284">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="271c2-284">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="271c2-285">设备处于展台模式时将显示的托管应用列表。</span><span class="sxs-lookup"><span data-stu-id="271c2-285">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="271c2-286">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="271c2-286">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="271c2-287">kioskModeWallpaperUrl</span><span class="sxs-lookup"><span data-stu-id="271c2-287">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="271c2-288">String</span><span class="sxs-lookup"><span data-stu-id="271c2-288">String</span></span>|<span data-ttu-id="271c2-289">在设备处于展台模式时用于墙纸的可公开访问图像的 URL。</span><span class="sxs-lookup"><span data-stu-id="271c2-289">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="271c2-290">kioskModeExitCode</span><span class="sxs-lookup"><span data-stu-id="271c2-290">kioskModeExitCode</span></span>|<span data-ttu-id="271c2-291">String</span><span class="sxs-lookup"><span data-stu-id="271c2-291">String</span></span>|<span data-ttu-id="271c2-292">退出代码，以允许用户在设备处于展台模式时从展台模式中进行转义。</span><span class="sxs-lookup"><span data-stu-id="271c2-292">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="271c2-293">kioskModeVirtualHomeButtonEnabled</span><span class="sxs-lookup"><span data-stu-id="271c2-293">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="271c2-294">布尔值</span><span class="sxs-lookup"><span data-stu-id="271c2-294">Boolean</span></span>|<span data-ttu-id="271c2-295">设备处于展台模式时是否显示虚拟 "主页" 按钮。</span><span class="sxs-lookup"><span data-stu-id="271c2-295">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="271c2-296">kioskModeVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="271c2-296">kioskModeVirtualHomeButtonType</span></span>|[<span data-ttu-id="271c2-297">androidDeviceOwnerVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="271c2-297">androidDeviceOwnerVirtualHomeButtonType</span></span>](../resources/intune-deviceconfig-androiddeviceownervirtualhomebuttontype.md)|<span data-ttu-id="271c2-298">指示虚拟 home 按钮是否为向上轻扫主页按钮或浮动主页按钮。</span><span class="sxs-lookup"><span data-stu-id="271c2-298">Indicates whether the virtual home button is a swipe up home button or a floating home button.</span></span> <span data-ttu-id="271c2-299">可取值为：`notConfigured`、`swipeUp`、`floating`。</span><span class="sxs-lookup"><span data-stu-id="271c2-299">Possible values are: `notConfigured`, `swipeUp`, `floating`.</span></span>|
|<span data-ttu-id="271c2-300">kioskModeBluetoothConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="271c2-300">kioskModeBluetoothConfigurationEnabled</span></span>|<span data-ttu-id="271c2-301">布尔值</span><span class="sxs-lookup"><span data-stu-id="271c2-301">Boolean</span></span>|<span data-ttu-id="271c2-302">是否允许用户在展台模式下配置蓝牙设置。</span><span class="sxs-lookup"><span data-stu-id="271c2-302">Whether or not to allow a user to configure Bluetooth settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="271c2-303">kioskModeWiFiConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="271c2-303">kioskModeWiFiConfigurationEnabled</span></span>|<span data-ttu-id="271c2-304">布尔值</span><span class="sxs-lookup"><span data-stu-id="271c2-304">Boolean</span></span>|<span data-ttu-id="271c2-305">是否允许用户在展台模式下配置 Wi-fi 设置。</span><span class="sxs-lookup"><span data-stu-id="271c2-305">Whether or not to allow a user to configure Wi-Fi settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="271c2-306">kioskModeFlashlightConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="271c2-306">kioskModeFlashlightConfigurationEnabled</span></span>|<span data-ttu-id="271c2-307">布尔值</span><span class="sxs-lookup"><span data-stu-id="271c2-307">Boolean</span></span>|<span data-ttu-id="271c2-308">是否允许用户在展台模式下使用该模式。</span><span class="sxs-lookup"><span data-stu-id="271c2-308">Whether or not to allow a user to use the flashlight in Kiosk Mode.</span></span>|
|<span data-ttu-id="271c2-309">kioskModeMediaVolumeConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="271c2-309">kioskModeMediaVolumeConfigurationEnabled</span></span>|<span data-ttu-id="271c2-310">布尔值</span><span class="sxs-lookup"><span data-stu-id="271c2-310">Boolean</span></span>|<span data-ttu-id="271c2-311">是否允许用户在展台模式下更改媒体音量。</span><span class="sxs-lookup"><span data-stu-id="271c2-311">Whether or not to allow a user to change the media volume in Kiosk Mode.</span></span>|
|<span data-ttu-id="271c2-312">microphoneForceMute</span><span class="sxs-lookup"><span data-stu-id="271c2-312">microphoneForceMute</span></span>|<span data-ttu-id="271c2-313">布尔值</span><span class="sxs-lookup"><span data-stu-id="271c2-313">Boolean</span></span>|<span data-ttu-id="271c2-314">指示是否阻止观众在设备上的麦克风。</span><span class="sxs-lookup"><span data-stu-id="271c2-314">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="271c2-315">networkEscapeHatchAllowed</span><span class="sxs-lookup"><span data-stu-id="271c2-315">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="271c2-316">布尔值</span><span class="sxs-lookup"><span data-stu-id="271c2-316">Boolean</span></span>|<span data-ttu-id="271c2-317">指示在引导时设备是否允许连接到临时网络连接。</span><span class="sxs-lookup"><span data-stu-id="271c2-317">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="271c2-318">nfcBlockOutgoingBeam</span><span class="sxs-lookup"><span data-stu-id="271c2-318">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="271c2-319">布尔值</span><span class="sxs-lookup"><span data-stu-id="271c2-319">Boolean</span></span>|<span data-ttu-id="271c2-320">指示是否阻止 NFC 传出横梁。</span><span class="sxs-lookup"><span data-stu-id="271c2-320">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="271c2-321">passwordBlockKeyguard</span><span class="sxs-lookup"><span data-stu-id="271c2-321">passwordBlockKeyguard</span></span>|<span data-ttu-id="271c2-322">布尔值</span><span class="sxs-lookup"><span data-stu-id="271c2-322">Boolean</span></span>|<span data-ttu-id="271c2-323">指示是否禁用 keyguard。</span><span class="sxs-lookup"><span data-stu-id="271c2-323">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="271c2-324">passwordBlockKeyguardFeatures</span><span class="sxs-lookup"><span data-stu-id="271c2-324">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="271c2-325">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md)集合</span><span class="sxs-lookup"><span data-stu-id="271c2-325">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="271c2-326">要阻止的设备 keyguard 功能的列表。</span><span class="sxs-lookup"><span data-stu-id="271c2-326">List of device keyguard features to block.</span></span> <span data-ttu-id="271c2-327">该集合最多可包含 7 个元素。</span><span class="sxs-lookup"><span data-stu-id="271c2-327">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="271c2-328">可取值为：`notConfigured`、`camera`、`notifications`、`unredactedNotifications`、`trustAgents`、`fingerprint`、`remoteInput`、`allFeatures`。</span><span class="sxs-lookup"><span data-stu-id="271c2-328">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="271c2-329">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="271c2-329">passwordExpirationDays</span></span>|<span data-ttu-id="271c2-330">Int32</span><span class="sxs-lookup"><span data-stu-id="271c2-330">Int32</span></span>|<span data-ttu-id="271c2-331">指示在密码过期之前可以设置密码的时间量（以秒为单位）以及需要新密码的时间（以秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="271c2-331">Indicates the amount of time in seconds that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="271c2-332">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="271c2-332">Valid values 1 to 365</span></span>|
|<span data-ttu-id="271c2-333">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="271c2-333">passwordMinimumLength</span></span>|<span data-ttu-id="271c2-334">Int32</span><span class="sxs-lookup"><span data-stu-id="271c2-334">Int32</span></span>|<span data-ttu-id="271c2-335">指示设备上所需密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="271c2-335">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="271c2-336">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="271c2-336">Valid values 4 to 16</span></span>|
|<span data-ttu-id="271c2-337">passwordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="271c2-337">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="271c2-338">Int32</span><span class="sxs-lookup"><span data-stu-id="271c2-338">Int32</span></span>|<span data-ttu-id="271c2-339">指示设备密码所需的字母字符的最小数量。</span><span class="sxs-lookup"><span data-stu-id="271c2-339">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="271c2-340">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="271c2-340">Valid values 1 to 16</span></span>|
|<span data-ttu-id="271c2-341">passwordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="271c2-341">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="271c2-342">Int32</span><span class="sxs-lookup"><span data-stu-id="271c2-342">Int32</span></span>|<span data-ttu-id="271c2-343">指示设备密码所需的最小小写字符数。</span><span class="sxs-lookup"><span data-stu-id="271c2-343">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="271c2-344">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="271c2-344">Valid values 1 to 16</span></span>|
|<span data-ttu-id="271c2-345">passwordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="271c2-345">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="271c2-346">Int32</span><span class="sxs-lookup"><span data-stu-id="271c2-346">Int32</span></span>|<span data-ttu-id="271c2-347">指示设备密码所需的最小非字母字符数。</span><span class="sxs-lookup"><span data-stu-id="271c2-347">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="271c2-348">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="271c2-348">Valid values 1 to 16</span></span>|
|<span data-ttu-id="271c2-349">passwordMinimumNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="271c2-349">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="271c2-350">Int32</span><span class="sxs-lookup"><span data-stu-id="271c2-350">Int32</span></span>|<span data-ttu-id="271c2-351">指示设备密码所需的最小数字字符数。</span><span class="sxs-lookup"><span data-stu-id="271c2-351">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="271c2-352">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="271c2-352">Valid values 1 to 16</span></span>|
|<span data-ttu-id="271c2-353">passwordMinimumSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="271c2-353">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="271c2-354">Int32</span><span class="sxs-lookup"><span data-stu-id="271c2-354">Int32</span></span>|<span data-ttu-id="271c2-355">指示设备密码所需的最小符号字符数。</span><span class="sxs-lookup"><span data-stu-id="271c2-355">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="271c2-356">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="271c2-356">Valid values 1 to 16</span></span>|
|<span data-ttu-id="271c2-357">passwordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="271c2-357">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="271c2-358">Int32</span><span class="sxs-lookup"><span data-stu-id="271c2-358">Int32</span></span>|<span data-ttu-id="271c2-359">指示设备密码所需的最小上限 caseletter 字符数。</span><span class="sxs-lookup"><span data-stu-id="271c2-359">Indicates the minimum number of upper caseletter characters required for device password.</span></span> <span data-ttu-id="271c2-360">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="271c2-360">Valid values 1 to 16</span></span>|
|<span data-ttu-id="271c2-361">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="271c2-361">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="271c2-362">Int32</span><span class="sxs-lookup"><span data-stu-id="271c2-362">Int32</span></span>|<span data-ttu-id="271c2-363">屏幕超时之前的不活动时间（毫秒）。</span><span class="sxs-lookup"><span data-stu-id="271c2-363">Milliseconds of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="271c2-364">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="271c2-364">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="271c2-365">Int32</span><span class="sxs-lookup"><span data-stu-id="271c2-365">Int32</span></span>|<span data-ttu-id="271c2-366">指示密码历史记录的长度，其中用户将不能输入与历史记录中的任何密码相同的新密码。</span><span class="sxs-lookup"><span data-stu-id="271c2-366">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="271c2-367">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="271c2-367">Valid values 0 to 24</span></span>|
|<span data-ttu-id="271c2-368">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="271c2-368">passwordRequiredType</span></span>|[<span data-ttu-id="271c2-369">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="271c2-369">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="271c2-370">指示设备上所需的最小密码质量。</span><span class="sxs-lookup"><span data-stu-id="271c2-370">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="271c2-371">可取值为：`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`customPassword`。</span><span class="sxs-lookup"><span data-stu-id="271c2-371">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|
|<span data-ttu-id="271c2-372">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="271c2-372">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="271c2-373">Int32</span><span class="sxs-lookup"><span data-stu-id="271c2-373">Int32</span></span>|<span data-ttu-id="271c2-374">指示用户在擦除设备之前可以输入不正确密码的次数。</span><span class="sxs-lookup"><span data-stu-id="271c2-374">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="271c2-375">有效值为 4 至 11</span><span class="sxs-lookup"><span data-stu-id="271c2-375">Valid values 4 to 11</span></span>|
|<span data-ttu-id="271c2-376">playStoreMode</span><span class="sxs-lookup"><span data-stu-id="271c2-376">playStoreMode</span></span>|[<span data-ttu-id="271c2-377">androidDeviceOwnerPlayStoreMode</span><span class="sxs-lookup"><span data-stu-id="271c2-377">androidDeviceOwnerPlayStoreMode</span></span>](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|<span data-ttu-id="271c2-378">指示设备的播放存储模式。</span><span class="sxs-lookup"><span data-stu-id="271c2-378">Indicates the Play Store mode of the device.</span></span> <span data-ttu-id="271c2-379">可取值为：`notConfigured`、`allowList`、`blockList`。</span><span class="sxs-lookup"><span data-stu-id="271c2-379">Possible values are: `notConfigured`, `allowList`, `blockList`.</span></span>|
|<span data-ttu-id="271c2-380">safeBootBlocked</span><span class="sxs-lookup"><span data-stu-id="271c2-380">safeBootBlocked</span></span>|<span data-ttu-id="271c2-381">布尔值</span><span class="sxs-lookup"><span data-stu-id="271c2-381">Boolean</span></span>|<span data-ttu-id="271c2-382">指示是否禁用重新启动设备到安全启动。</span><span class="sxs-lookup"><span data-stu-id="271c2-382">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="271c2-383">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="271c2-383">screenCaptureBlocked</span></span>|<span data-ttu-id="271c2-384">Boolean</span><span class="sxs-lookup"><span data-stu-id="271c2-384">Boolean</span></span>|<span data-ttu-id="271c2-385">指示是否禁用获取屏幕截图的功能。</span><span class="sxs-lookup"><span data-stu-id="271c2-385">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="271c2-386">securityAllowDebuggingFeatures</span><span class="sxs-lookup"><span data-stu-id="271c2-386">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="271c2-387">布尔值</span><span class="sxs-lookup"><span data-stu-id="271c2-387">Boolean</span></span>|<span data-ttu-id="271c2-388">指示是否阻止用户启用设备上的调试功能。</span><span class="sxs-lookup"><span data-stu-id="271c2-388">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="271c2-389">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="271c2-389">securityRequireVerifyApps</span></span>|<span data-ttu-id="271c2-390">布尔值</span><span class="sxs-lookup"><span data-stu-id="271c2-390">Boolean</span></span>|<span data-ttu-id="271c2-391">指示是否需要验证应用。</span><span class="sxs-lookup"><span data-stu-id="271c2-391">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="271c2-392">statusBarBlocked</span><span class="sxs-lookup"><span data-stu-id="271c2-392">statusBarBlocked</span></span>|<span data-ttu-id="271c2-393">布尔值</span><span class="sxs-lookup"><span data-stu-id="271c2-393">Boolean</span></span>|<span data-ttu-id="271c2-394">指示是否禁用状态栏，包括通知、快速设置和其他屏幕重叠。</span><span class="sxs-lookup"><span data-stu-id="271c2-394">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="271c2-395">stayOnModes</span><span class="sxs-lookup"><span data-stu-id="271c2-395">stayOnModes</span></span>|<span data-ttu-id="271c2-396">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)集合</span><span class="sxs-lookup"><span data-stu-id="271c2-396">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="271c2-397">设备的显示将保持开机状态的模式列表。</span><span class="sxs-lookup"><span data-stu-id="271c2-397">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="271c2-398">此集合最多可包含4个元素。</span><span class="sxs-lookup"><span data-stu-id="271c2-398">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="271c2-399">可取值为：`notConfigured`、`ac`、`usb`、`wireless`。</span><span class="sxs-lookup"><span data-stu-id="271c2-399">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="271c2-400">storageAllowUsb</span><span class="sxs-lookup"><span data-stu-id="271c2-400">storageAllowUsb</span></span>|<span data-ttu-id="271c2-401">布尔值</span><span class="sxs-lookup"><span data-stu-id="271c2-401">Boolean</span></span>|<span data-ttu-id="271c2-402">指示是否允许 USB 大容量存储。</span><span class="sxs-lookup"><span data-stu-id="271c2-402">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="271c2-403">storageBlockExternalMedia</span><span class="sxs-lookup"><span data-stu-id="271c2-403">storageBlockExternalMedia</span></span>|<span data-ttu-id="271c2-404">布尔值</span><span class="sxs-lookup"><span data-stu-id="271c2-404">Boolean</span></span>|<span data-ttu-id="271c2-405">指示是否阻止外部媒体。</span><span class="sxs-lookup"><span data-stu-id="271c2-405">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="271c2-406">storageBlockUsbFileTransfer</span><span class="sxs-lookup"><span data-stu-id="271c2-406">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="271c2-407">布尔值</span><span class="sxs-lookup"><span data-stu-id="271c2-407">Boolean</span></span>|<span data-ttu-id="271c2-408">指示是否阻止 USB 文件传输。</span><span class="sxs-lookup"><span data-stu-id="271c2-408">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="271c2-409">systemUpdateWindowStartMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="271c2-409">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="271c2-410">Int32</span><span class="sxs-lookup"><span data-stu-id="271c2-410">Int32</span></span>|<span data-ttu-id="271c2-411">指示系统更新窗口午夜后启动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="271c2-411">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="271c2-412">有效值为0至1440</span><span class="sxs-lookup"><span data-stu-id="271c2-412">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="271c2-413">systemUpdateWindowEndMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="271c2-413">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="271c2-414">Int32</span><span class="sxs-lookup"><span data-stu-id="271c2-414">Int32</span></span>|<span data-ttu-id="271c2-415">指示系统更新窗口结束后的分钟数。</span><span class="sxs-lookup"><span data-stu-id="271c2-415">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="271c2-416">有效值为0至1440</span><span class="sxs-lookup"><span data-stu-id="271c2-416">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="271c2-417">systemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="271c2-417">systemUpdateInstallType</span></span>|[<span data-ttu-id="271c2-418">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="271c2-418">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="271c2-419">系统更新配置的类型。</span><span class="sxs-lookup"><span data-stu-id="271c2-419">The type of system update configuration.</span></span> <span data-ttu-id="271c2-420">可取值为：`deviceDefault`、`postpone`、`windowed`、`automatic`。</span><span class="sxs-lookup"><span data-stu-id="271c2-420">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="271c2-421">systemWindowsBlocked</span><span class="sxs-lookup"><span data-stu-id="271c2-421">systemWindowsBlocked</span></span>|<span data-ttu-id="271c2-422">布尔值</span><span class="sxs-lookup"><span data-stu-id="271c2-422">Boolean</span></span>|<span data-ttu-id="271c2-423">是否阻止 Android 系统提示符窗口，如 toast、电话活动和系统通知。</span><span class="sxs-lookup"><span data-stu-id="271c2-423">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="271c2-424">usersBlockAdd</span><span class="sxs-lookup"><span data-stu-id="271c2-424">usersBlockAdd</span></span>|<span data-ttu-id="271c2-425">布尔值</span><span class="sxs-lookup"><span data-stu-id="271c2-425">Boolean</span></span>|<span data-ttu-id="271c2-426">指示是否禁用添加用户和配置文件。</span><span class="sxs-lookup"><span data-stu-id="271c2-426">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="271c2-427">usersBlockRemove</span><span class="sxs-lookup"><span data-stu-id="271c2-427">usersBlockRemove</span></span>|<span data-ttu-id="271c2-428">布尔值</span><span class="sxs-lookup"><span data-stu-id="271c2-428">Boolean</span></span>|<span data-ttu-id="271c2-429">指示是否禁用从设备中删除其他用户。</span><span class="sxs-lookup"><span data-stu-id="271c2-429">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="271c2-430">volumeBlockAdjustment</span><span class="sxs-lookup"><span data-stu-id="271c2-430">volumeBlockAdjustment</span></span>|<span data-ttu-id="271c2-431">布尔值</span><span class="sxs-lookup"><span data-stu-id="271c2-431">Boolean</span></span>|<span data-ttu-id="271c2-432">指示是否禁用了调整主音量。</span><span class="sxs-lookup"><span data-stu-id="271c2-432">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="271c2-433">vpnAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="271c2-433">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="271c2-434">布尔值</span><span class="sxs-lookup"><span data-stu-id="271c2-434">Boolean</span></span>|<span data-ttu-id="271c2-435">如果指定了 always on VPN 包名称，则在断开 VPN 连接时是否锁定网络流量。</span><span class="sxs-lookup"><span data-stu-id="271c2-435">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="271c2-436">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="271c2-436">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="271c2-437">String</span><span class="sxs-lookup"><span data-stu-id="271c2-437">String</span></span>|<span data-ttu-id="271c2-438">将处理永不启用 VPN 连接的应用程序的 Android 应用程序包名称。</span><span class="sxs-lookup"><span data-stu-id="271c2-438">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="271c2-439">wifiBlockEditConfigurations</span><span class="sxs-lookup"><span data-stu-id="271c2-439">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="271c2-440">布尔值</span><span class="sxs-lookup"><span data-stu-id="271c2-440">Boolean</span></span>|<span data-ttu-id="271c2-441">指示是否阻止用户编辑 wifi 连接设置。</span><span class="sxs-lookup"><span data-stu-id="271c2-441">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="271c2-442">wifiBlockEditPolicyDefinedConfigurations</span><span class="sxs-lookup"><span data-stu-id="271c2-442">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="271c2-443">布尔值</span><span class="sxs-lookup"><span data-stu-id="271c2-443">Boolean</span></span>|<span data-ttu-id="271c2-444">指示是否阻止用户仅编辑策略定义的网络。</span><span class="sxs-lookup"><span data-stu-id="271c2-444">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|



## <a name="response"></a><span data-ttu-id="271c2-445">响应</span><span class="sxs-lookup"><span data-stu-id="271c2-445">Response</span></span>
<span data-ttu-id="271c2-446">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="271c2-446">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="271c2-447">示例</span><span class="sxs-lookup"><span data-stu-id="271c2-447">Example</span></span>

### <a name="request"></a><span data-ttu-id="271c2-448">请求</span><span class="sxs-lookup"><span data-stu-id="271c2-448">Request</span></span>
<span data-ttu-id="271c2-449">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="271c2-449">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 5044

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
  "microsoftLauncherSearchBarPlacementAllowUserModification": true,
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
  "wifiBlockEditPolicyDefinedConfigurations": true
}
```

### <a name="response"></a><span data-ttu-id="271c2-450">响应</span><span class="sxs-lookup"><span data-stu-id="271c2-450">Response</span></span>
<span data-ttu-id="271c2-451">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="271c2-451">Here is an example of the response.</span></span> <span data-ttu-id="271c2-452">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="271c2-452">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="271c2-453">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="271c2-453">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 5216

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
  "microsoftLauncherSearchBarPlacementAllowUserModification": true,
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
  "wifiBlockEditPolicyDefinedConfigurations": true
}
```



