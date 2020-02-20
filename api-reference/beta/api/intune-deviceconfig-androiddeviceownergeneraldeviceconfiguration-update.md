---
title: 更新 androidDeviceOwnerGeneralDeviceConfiguration
description: 更新 androidDeviceOwnerGeneralDeviceConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dbd3350a23f805caddb7b9ce22f0b812a4efd9e2
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/20/2020
ms.locfileid: "42160261"
---
# <a name="update-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="8fe13-103">更新 androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="8fe13-103">Update androidDeviceOwnerGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="8fe13-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8fe13-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8fe13-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8fe13-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8fe13-106">更新[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8fe13-106">Update the properties of a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8fe13-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="8fe13-107">Prerequisites</span></span>
<span data-ttu-id="8fe13-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8fe13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8fe13-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8fe13-110">Permission type</span></span>|<span data-ttu-id="8fe13-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8fe13-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8fe13-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8fe13-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8fe13-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8fe13-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8fe13-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8fe13-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8fe13-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8fe13-115">Not supported.</span></span>|
|<span data-ttu-id="8fe13-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8fe13-116">Application</span></span>|<span data-ttu-id="8fe13-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8fe13-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8fe13-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8fe13-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="8fe13-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8fe13-119">Request headers</span></span>
|<span data-ttu-id="8fe13-120">标头</span><span class="sxs-lookup"><span data-stu-id="8fe13-120">Header</span></span>|<span data-ttu-id="8fe13-121">值</span><span class="sxs-lookup"><span data-stu-id="8fe13-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8fe13-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8fe13-122">Authorization</span></span>|<span data-ttu-id="8fe13-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8fe13-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8fe13-124">接受</span><span class="sxs-lookup"><span data-stu-id="8fe13-124">Accept</span></span>|<span data-ttu-id="8fe13-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8fe13-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8fe13-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8fe13-126">Request body</span></span>
<span data-ttu-id="8fe13-127">在请求正文中，提供[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8fe13-127">In the request body, supply a JSON representation for the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="8fe13-128">下表显示创建[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8fe13-128">The following table shows the properties that are required when you create the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="8fe13-129">属性</span><span class="sxs-lookup"><span data-stu-id="8fe13-129">Property</span></span>|<span data-ttu-id="8fe13-130">类型</span><span class="sxs-lookup"><span data-stu-id="8fe13-130">Type</span></span>|<span data-ttu-id="8fe13-131">说明</span><span class="sxs-lookup"><span data-stu-id="8fe13-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8fe13-132">id</span><span class="sxs-lookup"><span data-stu-id="8fe13-132">id</span></span>|<span data-ttu-id="8fe13-133">字符串</span><span class="sxs-lookup"><span data-stu-id="8fe13-133">String</span></span>|<span data-ttu-id="8fe13-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="8fe13-134">Key of the entity.</span></span> <span data-ttu-id="8fe13-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8fe13-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8fe13-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8fe13-136">lastModifiedDateTime</span></span>|<span data-ttu-id="8fe13-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8fe13-137">DateTimeOffset</span></span>|<span data-ttu-id="8fe13-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="8fe13-138">DateTime the object was last modified.</span></span> <span data-ttu-id="8fe13-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8fe13-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8fe13-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8fe13-140">roleScopeTagIds</span></span>|<span data-ttu-id="8fe13-141">String collection</span><span class="sxs-lookup"><span data-stu-id="8fe13-141">String collection</span></span>|<span data-ttu-id="8fe13-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="8fe13-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8fe13-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8fe13-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8fe13-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="8fe13-144">supportsScopeTags</span></span>|<span data-ttu-id="8fe13-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fe13-145">Boolean</span></span>|<span data-ttu-id="8fe13-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="8fe13-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8fe13-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="8fe13-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8fe13-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="8fe13-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8fe13-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8fe13-149">This property is read-only.</span></span> <span data-ttu-id="8fe13-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8fe13-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8fe13-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8fe13-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="8fe13-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8fe13-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="8fe13-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="8fe13-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="8fe13-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8fe13-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8fe13-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8fe13-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="8fe13-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8fe13-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="8fe13-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="8fe13-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="8fe13-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8fe13-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8fe13-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="8fe13-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="8fe13-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="8fe13-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="8fe13-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="8fe13-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="8fe13-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8fe13-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8fe13-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8fe13-163">createdDateTime</span></span>|<span data-ttu-id="8fe13-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8fe13-164">DateTimeOffset</span></span>|<span data-ttu-id="8fe13-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="8fe13-165">DateTime the object was created.</span></span> <span data-ttu-id="8fe13-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8fe13-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8fe13-167">说明</span><span class="sxs-lookup"><span data-stu-id="8fe13-167">description</span></span>|<span data-ttu-id="8fe13-168">String</span><span class="sxs-lookup"><span data-stu-id="8fe13-168">String</span></span>|<span data-ttu-id="8fe13-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="8fe13-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8fe13-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8fe13-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8fe13-171">displayName</span><span class="sxs-lookup"><span data-stu-id="8fe13-171">displayName</span></span>|<span data-ttu-id="8fe13-172">String</span><span class="sxs-lookup"><span data-stu-id="8fe13-172">String</span></span>|<span data-ttu-id="8fe13-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="8fe13-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8fe13-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8fe13-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8fe13-175">version</span><span class="sxs-lookup"><span data-stu-id="8fe13-175">version</span></span>|<span data-ttu-id="8fe13-176">Int32</span><span class="sxs-lookup"><span data-stu-id="8fe13-176">Int32</span></span>|<span data-ttu-id="8fe13-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="8fe13-177">Version of the device configuration.</span></span> <span data-ttu-id="8fe13-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8fe13-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8fe13-179">accountsBlockModification</span><span class="sxs-lookup"><span data-stu-id="8fe13-179">accountsBlockModification</span></span>|<span data-ttu-id="8fe13-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fe13-180">Boolean</span></span>|<span data-ttu-id="8fe13-181">指示是否禁用添加或删除帐户。</span><span class="sxs-lookup"><span data-stu-id="8fe13-181">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="8fe13-182">appsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="8fe13-182">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="8fe13-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fe13-183">Boolean</span></span>|<span data-ttu-id="8fe13-184">指示是否允许用户启用 "未知源" 设置。</span><span class="sxs-lookup"><span data-stu-id="8fe13-184">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="8fe13-185">appsAutoUpdatePolicy</span><span class="sxs-lookup"><span data-stu-id="8fe13-185">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="8fe13-186">androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="8fe13-186">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="8fe13-187">指示应用程序自动更新策略的值。</span><span class="sxs-lookup"><span data-stu-id="8fe13-187">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="8fe13-188">可取值为：`notConfigured`、`userChoice`、`never`、`wiFiOnly`、`always`。</span><span class="sxs-lookup"><span data-stu-id="8fe13-188">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="8fe13-189">appsDefaultPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="8fe13-189">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="8fe13-190">androidDeviceOwnerDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="8fe13-190">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="8fe13-191">指示对运行时权限请求的权限策略（如果专门没有为应用程序定义）。</span><span class="sxs-lookup"><span data-stu-id="8fe13-191">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="8fe13-192">可取值为：`deviceDefault`、`prompt`、`autoGrant`、`autoDeny`。</span><span class="sxs-lookup"><span data-stu-id="8fe13-192">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="8fe13-193">appsRecommendSkippingFirstUseHints</span><span class="sxs-lookup"><span data-stu-id="8fe13-193">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="8fe13-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fe13-194">Boolean</span></span>|<span data-ttu-id="8fe13-195">是否建议所有应用都将跳过他们可能已添加的任何首次使用提示。</span><span class="sxs-lookup"><span data-stu-id="8fe13-195">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="8fe13-196">bluetoothBlockConfiguration</span><span class="sxs-lookup"><span data-stu-id="8fe13-196">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="8fe13-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fe13-197">Boolean</span></span>|<span data-ttu-id="8fe13-198">指示是否阻止用户配置蓝牙。</span><span class="sxs-lookup"><span data-stu-id="8fe13-198">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="8fe13-199">bluetoothBlockContactSharing</span><span class="sxs-lookup"><span data-stu-id="8fe13-199">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="8fe13-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fe13-200">Boolean</span></span>|<span data-ttu-id="8fe13-201">指示是否阻止用户通过蓝牙共享联系人。</span><span class="sxs-lookup"><span data-stu-id="8fe13-201">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="8fe13-202">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="8fe13-202">cameraBlocked</span></span>|<span data-ttu-id="8fe13-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fe13-203">Boolean</span></span>|<span data-ttu-id="8fe13-204">指示是否禁用相机的使用。</span><span class="sxs-lookup"><span data-stu-id="8fe13-204">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="8fe13-205">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="8fe13-205">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="8fe13-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fe13-206">Boolean</span></span>|<span data-ttu-id="8fe13-207">指示是否阻止 Wi-Fi 网络共享。</span><span class="sxs-lookup"><span data-stu-id="8fe13-207">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="8fe13-208">certificateCredentialConfigurationDisabled</span><span class="sxs-lookup"><span data-stu-id="8fe13-208">certificateCredentialConfigurationDisabled</span></span>|<span data-ttu-id="8fe13-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fe13-209">Boolean</span></span>|<span data-ttu-id="8fe13-210">指示是否阻止来自任何证书凭据配置的用户。</span><span class="sxs-lookup"><span data-stu-id="8fe13-210">Indicates whether or not to block users from any certificate credential configuration.</span></span>|
|<span data-ttu-id="8fe13-211">dataRoamingBlocked</span><span class="sxs-lookup"><span data-stu-id="8fe13-211">dataRoamingBlocked</span></span>|<span data-ttu-id="8fe13-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fe13-212">Boolean</span></span>|<span data-ttu-id="8fe13-213">指示是否阻止用户使用数据漫游。</span><span class="sxs-lookup"><span data-stu-id="8fe13-213">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="8fe13-214">dateTimeConfigurationBlocked</span><span class="sxs-lookup"><span data-stu-id="8fe13-214">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="8fe13-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fe13-215">Boolean</span></span>|<span data-ttu-id="8fe13-216">指示是否阻止用户手动更改设备上的日期或时间</span><span class="sxs-lookup"><span data-stu-id="8fe13-216">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="8fe13-217">factoryResetDeviceAdministratorEmails</span><span class="sxs-lookup"><span data-stu-id="8fe13-217">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="8fe13-218">String collection</span><span class="sxs-lookup"><span data-stu-id="8fe13-218">String collection</span></span>|<span data-ttu-id="8fe13-219">在设备出厂重置之前，将需要进行身份验证的 Google 帐户电子邮件的列表，然后才能对其进行设置。</span><span class="sxs-lookup"><span data-stu-id="8fe13-219">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="8fe13-220">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="8fe13-220">factoryResetBlocked</span></span>|<span data-ttu-id="8fe13-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fe13-221">Boolean</span></span>|<span data-ttu-id="8fe13-222">指示是否禁用了 "设置" 中的 "恢复出厂设置" 选项。</span><span class="sxs-lookup"><span data-stu-id="8fe13-222">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="8fe13-223">globalProxy</span><span class="sxs-lookup"><span data-stu-id="8fe13-223">globalProxy</span></span>|[<span data-ttu-id="8fe13-224">androidDeviceOwnerGlobalProxy</span><span class="sxs-lookup"><span data-stu-id="8fe13-224">androidDeviceOwnerGlobalProxy</span></span>](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)|<span data-ttu-id="8fe13-225">代理是与主机、端口和已排除的主机直接建立的。</span><span class="sxs-lookup"><span data-stu-id="8fe13-225">Proxy is set up directly with host, port and excluded hosts.</span></span>|
|<span data-ttu-id="8fe13-226">googleAccountsBlocked</span><span class="sxs-lookup"><span data-stu-id="8fe13-226">googleAccountsBlocked</span></span>|<span data-ttu-id="8fe13-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fe13-227">Boolean</span></span>|<span data-ttu-id="8fe13-228">指示是否将阻止 google 帐户。</span><span class="sxs-lookup"><span data-stu-id="8fe13-228">Indicates whether or not google accounts will be blocked.</span></span>|
|<span data-ttu-id="8fe13-229">kioskModeScreenSaverConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="8fe13-229">kioskModeScreenSaverConfigurationEnabled</span></span>|<span data-ttu-id="8fe13-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fe13-230">Boolean</span></span>|<span data-ttu-id="8fe13-231">是否启用屏幕保护程序模式或不启用展台模式。</span><span class="sxs-lookup"><span data-stu-id="8fe13-231">Whether or not to enable screen saver mode or not in Kiosk Mode.</span></span>|
|<span data-ttu-id="8fe13-232">kioskModeScreenSaverImageUrl</span><span class="sxs-lookup"><span data-stu-id="8fe13-232">kioskModeScreenSaverImageUrl</span></span>|<span data-ttu-id="8fe13-233">String</span><span class="sxs-lookup"><span data-stu-id="8fe13-233">String</span></span>|<span data-ttu-id="8fe13-234">将作为展台模式下设备的屏幕保护程序的图像的 URL。</span><span class="sxs-lookup"><span data-stu-id="8fe13-234">URL for an image that will be the device's screen saver in Kiosk Mode.</span></span>|
|<span data-ttu-id="8fe13-235">kioskModeScreenSaverDisplayTimeInSeconds</span><span class="sxs-lookup"><span data-stu-id="8fe13-235">kioskModeScreenSaverDisplayTimeInSeconds</span></span>|<span data-ttu-id="8fe13-236">Int32</span><span class="sxs-lookup"><span data-stu-id="8fe13-236">Int32</span></span>|<span data-ttu-id="8fe13-237">设备将在展台模式下显示屏幕保护程序的秒数。</span><span class="sxs-lookup"><span data-stu-id="8fe13-237">The number of seconds that the device will display the screen saver for in Kiosk Mode.</span></span> <span data-ttu-id="8fe13-238">有效值为0至9999999</span><span class="sxs-lookup"><span data-stu-id="8fe13-238">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="8fe13-239">kioskModeScreenSaverStartDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="8fe13-239">kioskModeScreenSaverStartDelayInSeconds</span></span>|<span data-ttu-id="8fe13-240">Int32</span><span class="sxs-lookup"><span data-stu-id="8fe13-240">Int32</span></span>|<span data-ttu-id="8fe13-241">在 Kiosk 模式下显示屏幕保护程序之前设备需要保持非活动状态的秒数。</span><span class="sxs-lookup"><span data-stu-id="8fe13-241">The number of seconds the device needs to be inactive for before the screen saver is shown in Kiosk Mode.</span></span> <span data-ttu-id="8fe13-242">有效值为1至9999999</span><span class="sxs-lookup"><span data-stu-id="8fe13-242">Valid values 1 to 9999999</span></span>|
|<span data-ttu-id="8fe13-243">kioskModeScreenSaverDetectMediaDisabled</span><span class="sxs-lookup"><span data-stu-id="8fe13-243">kioskModeScreenSaverDetectMediaDisabled</span></span>|<span data-ttu-id="8fe13-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fe13-244">Boolean</span></span>|<span data-ttu-id="8fe13-245">如果音频/视频在展台模式下播放，则设备屏幕是否应显示屏幕保护程序。</span><span class="sxs-lookup"><span data-stu-id="8fe13-245">Whether or not the device screen should show the screen saver if audio/video is playing in Kiosk Mode.</span></span>|
|<span data-ttu-id="8fe13-246">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="8fe13-246">kioskModeApps</span></span>|<span data-ttu-id="8fe13-247">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8fe13-247">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="8fe13-248">设备处于展台模式时将显示的托管应用列表。</span><span class="sxs-lookup"><span data-stu-id="8fe13-248">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="8fe13-249">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="8fe13-249">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="8fe13-250">kioskModeWallpaperUrl</span><span class="sxs-lookup"><span data-stu-id="8fe13-250">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="8fe13-251">String</span><span class="sxs-lookup"><span data-stu-id="8fe13-251">String</span></span>|<span data-ttu-id="8fe13-252">在设备处于展台模式时用于墙纸的可公开访问图像的 URL。</span><span class="sxs-lookup"><span data-stu-id="8fe13-252">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="8fe13-253">kioskModeExitCode</span><span class="sxs-lookup"><span data-stu-id="8fe13-253">kioskModeExitCode</span></span>|<span data-ttu-id="8fe13-254">String</span><span class="sxs-lookup"><span data-stu-id="8fe13-254">String</span></span>|<span data-ttu-id="8fe13-255">退出代码，以允许用户在设备处于展台模式时从展台模式中进行转义。</span><span class="sxs-lookup"><span data-stu-id="8fe13-255">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="8fe13-256">kioskModeVirtualHomeButtonEnabled</span><span class="sxs-lookup"><span data-stu-id="8fe13-256">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="8fe13-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fe13-257">Boolean</span></span>|<span data-ttu-id="8fe13-258">设备处于展台模式时是否显示虚拟 "主页" 按钮。</span><span class="sxs-lookup"><span data-stu-id="8fe13-258">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="8fe13-259">kioskModeVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="8fe13-259">kioskModeVirtualHomeButtonType</span></span>|[<span data-ttu-id="8fe13-260">androidDeviceOwnerVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="8fe13-260">androidDeviceOwnerVirtualHomeButtonType</span></span>](../resources/intune-deviceconfig-androiddeviceownervirtualhomebuttontype.md)|<span data-ttu-id="8fe13-261">指示虚拟 home 按钮是否为向上轻扫主页按钮或浮动主页按钮。</span><span class="sxs-lookup"><span data-stu-id="8fe13-261">Indicates whether the virtual home button is a swipe up home button or a floating home button.</span></span> <span data-ttu-id="8fe13-262">可取值为：`notConfigured`、`swipeUp`、`floating`。</span><span class="sxs-lookup"><span data-stu-id="8fe13-262">Possible values are: `notConfigured`, `swipeUp`, `floating`.</span></span>|
|<span data-ttu-id="8fe13-263">kioskModeBluetoothConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="8fe13-263">kioskModeBluetoothConfigurationEnabled</span></span>|<span data-ttu-id="8fe13-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fe13-264">Boolean</span></span>|<span data-ttu-id="8fe13-265">是否允许用户在展台模式下配置蓝牙设置。</span><span class="sxs-lookup"><span data-stu-id="8fe13-265">Whether or not to allow a user to configure Bluetooth settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="8fe13-266">kioskModeWiFiConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="8fe13-266">kioskModeWiFiConfigurationEnabled</span></span>|<span data-ttu-id="8fe13-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fe13-267">Boolean</span></span>|<span data-ttu-id="8fe13-268">是否允许用户在展台模式下配置 Wi-fi 设置。</span><span class="sxs-lookup"><span data-stu-id="8fe13-268">Whether or not to allow a user to configure Wi-Fi settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="8fe13-269">kioskModeFlashlightConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="8fe13-269">kioskModeFlashlightConfigurationEnabled</span></span>|<span data-ttu-id="8fe13-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fe13-270">Boolean</span></span>|<span data-ttu-id="8fe13-271">是否允许用户在展台模式下使用该模式。</span><span class="sxs-lookup"><span data-stu-id="8fe13-271">Whether or not to allow a user to use the flashlight in Kiosk Mode.</span></span>|
|<span data-ttu-id="8fe13-272">kioskModeMediaVolumeConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="8fe13-272">kioskModeMediaVolumeConfigurationEnabled</span></span>|<span data-ttu-id="8fe13-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fe13-273">Boolean</span></span>|<span data-ttu-id="8fe13-274">是否允许用户在展台模式下更改媒体音量。</span><span class="sxs-lookup"><span data-stu-id="8fe13-274">Whether or not to allow a user to change the media volume in Kiosk Mode.</span></span>|
|<span data-ttu-id="8fe13-275">microphoneForceMute</span><span class="sxs-lookup"><span data-stu-id="8fe13-275">microphoneForceMute</span></span>|<span data-ttu-id="8fe13-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fe13-276">Boolean</span></span>|<span data-ttu-id="8fe13-277">指示是否阻止观众在设备上的麦克风。</span><span class="sxs-lookup"><span data-stu-id="8fe13-277">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="8fe13-278">networkEscapeHatchAllowed</span><span class="sxs-lookup"><span data-stu-id="8fe13-278">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="8fe13-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fe13-279">Boolean</span></span>|<span data-ttu-id="8fe13-280">指示在引导时设备是否允许连接到临时网络连接。</span><span class="sxs-lookup"><span data-stu-id="8fe13-280">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="8fe13-281">nfcBlockOutgoingBeam</span><span class="sxs-lookup"><span data-stu-id="8fe13-281">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="8fe13-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fe13-282">Boolean</span></span>|<span data-ttu-id="8fe13-283">指示是否阻止 NFC 传出横梁。</span><span class="sxs-lookup"><span data-stu-id="8fe13-283">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="8fe13-284">passwordBlockKeyguard</span><span class="sxs-lookup"><span data-stu-id="8fe13-284">passwordBlockKeyguard</span></span>|<span data-ttu-id="8fe13-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fe13-285">Boolean</span></span>|<span data-ttu-id="8fe13-286">指示是否禁用 keyguard。</span><span class="sxs-lookup"><span data-stu-id="8fe13-286">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="8fe13-287">passwordBlockKeyguardFeatures</span><span class="sxs-lookup"><span data-stu-id="8fe13-287">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="8fe13-288">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md)集合</span><span class="sxs-lookup"><span data-stu-id="8fe13-288">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="8fe13-289">要阻止的设备 keyguard 功能的列表。</span><span class="sxs-lookup"><span data-stu-id="8fe13-289">List of device keyguard features to block.</span></span> <span data-ttu-id="8fe13-290">该集合最多可包含 7 个元素。</span><span class="sxs-lookup"><span data-stu-id="8fe13-290">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="8fe13-291">可取值为：`notConfigured`、`camera`、`notifications`、`unredactedNotifications`、`trustAgents`、`fingerprint`、`remoteInput`、`allFeatures`。</span><span class="sxs-lookup"><span data-stu-id="8fe13-291">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="8fe13-292">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="8fe13-292">passwordExpirationDays</span></span>|<span data-ttu-id="8fe13-293">Int32</span><span class="sxs-lookup"><span data-stu-id="8fe13-293">Int32</span></span>|<span data-ttu-id="8fe13-294">指示在密码过期之前可以设置密码的时间量（以秒为单位）以及需要新密码的时间（以秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="8fe13-294">Indicates the amount of time in seconds that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="8fe13-295">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="8fe13-295">Valid values 1 to 365</span></span>|
|<span data-ttu-id="8fe13-296">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="8fe13-296">passwordMinimumLength</span></span>|<span data-ttu-id="8fe13-297">Int32</span><span class="sxs-lookup"><span data-stu-id="8fe13-297">Int32</span></span>|<span data-ttu-id="8fe13-298">指示设备上所需密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="8fe13-298">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="8fe13-299">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="8fe13-299">Valid values 4 to 16</span></span>|
|<span data-ttu-id="8fe13-300">passwordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="8fe13-300">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="8fe13-301">Int32</span><span class="sxs-lookup"><span data-stu-id="8fe13-301">Int32</span></span>|<span data-ttu-id="8fe13-302">指示设备密码所需的字母字符的最小数量。</span><span class="sxs-lookup"><span data-stu-id="8fe13-302">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="8fe13-303">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="8fe13-303">Valid values 1 to 16</span></span>|
|<span data-ttu-id="8fe13-304">passwordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="8fe13-304">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="8fe13-305">Int32</span><span class="sxs-lookup"><span data-stu-id="8fe13-305">Int32</span></span>|<span data-ttu-id="8fe13-306">指示设备密码所需的最小小写字符数。</span><span class="sxs-lookup"><span data-stu-id="8fe13-306">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="8fe13-307">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="8fe13-307">Valid values 1 to 16</span></span>|
|<span data-ttu-id="8fe13-308">passwordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="8fe13-308">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="8fe13-309">Int32</span><span class="sxs-lookup"><span data-stu-id="8fe13-309">Int32</span></span>|<span data-ttu-id="8fe13-310">指示设备密码所需的最小非字母字符数。</span><span class="sxs-lookup"><span data-stu-id="8fe13-310">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="8fe13-311">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="8fe13-311">Valid values 1 to 16</span></span>|
|<span data-ttu-id="8fe13-312">passwordMinimumNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="8fe13-312">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="8fe13-313">Int32</span><span class="sxs-lookup"><span data-stu-id="8fe13-313">Int32</span></span>|<span data-ttu-id="8fe13-314">指示设备密码所需的最小数字字符数。</span><span class="sxs-lookup"><span data-stu-id="8fe13-314">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="8fe13-315">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="8fe13-315">Valid values 1 to 16</span></span>|
|<span data-ttu-id="8fe13-316">passwordMinimumSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="8fe13-316">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="8fe13-317">Int32</span><span class="sxs-lookup"><span data-stu-id="8fe13-317">Int32</span></span>|<span data-ttu-id="8fe13-318">指示设备密码所需的最小符号字符数。</span><span class="sxs-lookup"><span data-stu-id="8fe13-318">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="8fe13-319">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="8fe13-319">Valid values 1 to 16</span></span>|
|<span data-ttu-id="8fe13-320">passwordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="8fe13-320">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="8fe13-321">Int32</span><span class="sxs-lookup"><span data-stu-id="8fe13-321">Int32</span></span>|<span data-ttu-id="8fe13-322">指示设备密码所需的最小上限 caseletter 字符数。</span><span class="sxs-lookup"><span data-stu-id="8fe13-322">Indicates the minimum number of upper caseletter characters required for device password.</span></span> <span data-ttu-id="8fe13-323">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="8fe13-323">Valid values 1 to 16</span></span>|
|<span data-ttu-id="8fe13-324">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="8fe13-324">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="8fe13-325">Int32</span><span class="sxs-lookup"><span data-stu-id="8fe13-325">Int32</span></span>|<span data-ttu-id="8fe13-326">屏幕超时之前的不活动时间（毫秒）。</span><span class="sxs-lookup"><span data-stu-id="8fe13-326">Milliseconds of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="8fe13-327">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="8fe13-327">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="8fe13-328">Int32</span><span class="sxs-lookup"><span data-stu-id="8fe13-328">Int32</span></span>|<span data-ttu-id="8fe13-329">指示密码历史记录的长度，其中用户将不能输入与历史记录中的任何密码相同的新密码。</span><span class="sxs-lookup"><span data-stu-id="8fe13-329">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="8fe13-330">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="8fe13-330">Valid values 0 to 24</span></span>|
|<span data-ttu-id="8fe13-331">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="8fe13-331">passwordRequiredType</span></span>|[<span data-ttu-id="8fe13-332">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="8fe13-332">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="8fe13-333">指示设备上所需的最小密码质量。</span><span class="sxs-lookup"><span data-stu-id="8fe13-333">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="8fe13-334">可取值为：`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`customPassword`。</span><span class="sxs-lookup"><span data-stu-id="8fe13-334">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|
|<span data-ttu-id="8fe13-335">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="8fe13-335">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="8fe13-336">Int32</span><span class="sxs-lookup"><span data-stu-id="8fe13-336">Int32</span></span>|<span data-ttu-id="8fe13-337">指示用户在擦除设备之前可以输入不正确密码的次数。</span><span class="sxs-lookup"><span data-stu-id="8fe13-337">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="8fe13-338">有效值为 4 至 11</span><span class="sxs-lookup"><span data-stu-id="8fe13-338">Valid values 4 to 11</span></span>|
|<span data-ttu-id="8fe13-339">playStoreMode</span><span class="sxs-lookup"><span data-stu-id="8fe13-339">playStoreMode</span></span>|[<span data-ttu-id="8fe13-340">androidDeviceOwnerPlayStoreMode</span><span class="sxs-lookup"><span data-stu-id="8fe13-340">androidDeviceOwnerPlayStoreMode</span></span>](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|<span data-ttu-id="8fe13-341">指示设备的播放存储模式。</span><span class="sxs-lookup"><span data-stu-id="8fe13-341">Indicates the Play Store mode of the device.</span></span> <span data-ttu-id="8fe13-342">可取值为：`notConfigured`、`allowList`、`blockList`。</span><span class="sxs-lookup"><span data-stu-id="8fe13-342">Possible values are: `notConfigured`, `allowList`, `blockList`.</span></span>|
|<span data-ttu-id="8fe13-343">safeBootBlocked</span><span class="sxs-lookup"><span data-stu-id="8fe13-343">safeBootBlocked</span></span>|<span data-ttu-id="8fe13-344">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fe13-344">Boolean</span></span>|<span data-ttu-id="8fe13-345">指示是否禁用重新启动设备到安全启动。</span><span class="sxs-lookup"><span data-stu-id="8fe13-345">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="8fe13-346">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="8fe13-346">screenCaptureBlocked</span></span>|<span data-ttu-id="8fe13-347">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fe13-347">Boolean</span></span>|<span data-ttu-id="8fe13-348">指示是否禁用获取屏幕截图的功能。</span><span class="sxs-lookup"><span data-stu-id="8fe13-348">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="8fe13-349">securityAllowDebuggingFeatures</span><span class="sxs-lookup"><span data-stu-id="8fe13-349">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="8fe13-350">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fe13-350">Boolean</span></span>|<span data-ttu-id="8fe13-351">指示是否阻止用户启用设备上的调试功能。</span><span class="sxs-lookup"><span data-stu-id="8fe13-351">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="8fe13-352">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="8fe13-352">securityRequireVerifyApps</span></span>|<span data-ttu-id="8fe13-353">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fe13-353">Boolean</span></span>|<span data-ttu-id="8fe13-354">指示是否需要验证应用。</span><span class="sxs-lookup"><span data-stu-id="8fe13-354">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="8fe13-355">statusBarBlocked</span><span class="sxs-lookup"><span data-stu-id="8fe13-355">statusBarBlocked</span></span>|<span data-ttu-id="8fe13-356">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fe13-356">Boolean</span></span>|<span data-ttu-id="8fe13-357">指示是否禁用状态栏，包括通知、快速设置和其他屏幕重叠。</span><span class="sxs-lookup"><span data-stu-id="8fe13-357">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="8fe13-358">stayOnModes</span><span class="sxs-lookup"><span data-stu-id="8fe13-358">stayOnModes</span></span>|<span data-ttu-id="8fe13-359">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)集合</span><span class="sxs-lookup"><span data-stu-id="8fe13-359">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="8fe13-360">设备的显示将保持开机状态的模式列表。</span><span class="sxs-lookup"><span data-stu-id="8fe13-360">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="8fe13-361">此集合最多可包含4个元素。</span><span class="sxs-lookup"><span data-stu-id="8fe13-361">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="8fe13-362">可取值为：`notConfigured`、`ac`、`usb`、`wireless`。</span><span class="sxs-lookup"><span data-stu-id="8fe13-362">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="8fe13-363">storageAllowUsb</span><span class="sxs-lookup"><span data-stu-id="8fe13-363">storageAllowUsb</span></span>|<span data-ttu-id="8fe13-364">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fe13-364">Boolean</span></span>|<span data-ttu-id="8fe13-365">指示是否允许 USB 大容量存储。</span><span class="sxs-lookup"><span data-stu-id="8fe13-365">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="8fe13-366">storageBlockExternalMedia</span><span class="sxs-lookup"><span data-stu-id="8fe13-366">storageBlockExternalMedia</span></span>|<span data-ttu-id="8fe13-367">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fe13-367">Boolean</span></span>|<span data-ttu-id="8fe13-368">指示是否阻止外部媒体。</span><span class="sxs-lookup"><span data-stu-id="8fe13-368">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="8fe13-369">storageBlockUsbFileTransfer</span><span class="sxs-lookup"><span data-stu-id="8fe13-369">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="8fe13-370">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fe13-370">Boolean</span></span>|<span data-ttu-id="8fe13-371">指示是否阻止 USB 文件传输。</span><span class="sxs-lookup"><span data-stu-id="8fe13-371">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="8fe13-372">systemUpdateWindowStartMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="8fe13-372">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="8fe13-373">Int32</span><span class="sxs-lookup"><span data-stu-id="8fe13-373">Int32</span></span>|<span data-ttu-id="8fe13-374">指示系统更新窗口午夜后启动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="8fe13-374">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="8fe13-375">有效值为0至1440</span><span class="sxs-lookup"><span data-stu-id="8fe13-375">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="8fe13-376">systemUpdateWindowEndMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="8fe13-376">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="8fe13-377">Int32</span><span class="sxs-lookup"><span data-stu-id="8fe13-377">Int32</span></span>|<span data-ttu-id="8fe13-378">指示系统更新窗口结束后的分钟数。</span><span class="sxs-lookup"><span data-stu-id="8fe13-378">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="8fe13-379">有效值为0至1440</span><span class="sxs-lookup"><span data-stu-id="8fe13-379">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="8fe13-380">systemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="8fe13-380">systemUpdateInstallType</span></span>|[<span data-ttu-id="8fe13-381">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="8fe13-381">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="8fe13-382">系统更新配置的类型。</span><span class="sxs-lookup"><span data-stu-id="8fe13-382">The type of system update configuration.</span></span> <span data-ttu-id="8fe13-383">可取值为：`deviceDefault`、`postpone`、`windowed`、`automatic`。</span><span class="sxs-lookup"><span data-stu-id="8fe13-383">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="8fe13-384">systemWindowsBlocked</span><span class="sxs-lookup"><span data-stu-id="8fe13-384">systemWindowsBlocked</span></span>|<span data-ttu-id="8fe13-385">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fe13-385">Boolean</span></span>|<span data-ttu-id="8fe13-386">是否阻止 Android 系统提示符窗口，如 toast、电话活动和系统通知。</span><span class="sxs-lookup"><span data-stu-id="8fe13-386">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="8fe13-387">usersBlockAdd</span><span class="sxs-lookup"><span data-stu-id="8fe13-387">usersBlockAdd</span></span>|<span data-ttu-id="8fe13-388">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fe13-388">Boolean</span></span>|<span data-ttu-id="8fe13-389">指示是否禁用添加用户和配置文件。</span><span class="sxs-lookup"><span data-stu-id="8fe13-389">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="8fe13-390">usersBlockRemove</span><span class="sxs-lookup"><span data-stu-id="8fe13-390">usersBlockRemove</span></span>|<span data-ttu-id="8fe13-391">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fe13-391">Boolean</span></span>|<span data-ttu-id="8fe13-392">指示是否禁用从设备中删除其他用户。</span><span class="sxs-lookup"><span data-stu-id="8fe13-392">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="8fe13-393">volumeBlockAdjustment</span><span class="sxs-lookup"><span data-stu-id="8fe13-393">volumeBlockAdjustment</span></span>|<span data-ttu-id="8fe13-394">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fe13-394">Boolean</span></span>|<span data-ttu-id="8fe13-395">指示是否禁用了调整主音量。</span><span class="sxs-lookup"><span data-stu-id="8fe13-395">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="8fe13-396">vpnAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="8fe13-396">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="8fe13-397">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fe13-397">Boolean</span></span>|<span data-ttu-id="8fe13-398">如果指定了 always on VPN 包名称，则在断开 VPN 连接时是否锁定网络流量。</span><span class="sxs-lookup"><span data-stu-id="8fe13-398">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="8fe13-399">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="8fe13-399">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="8fe13-400">String</span><span class="sxs-lookup"><span data-stu-id="8fe13-400">String</span></span>|<span data-ttu-id="8fe13-401">将处理永不启用 VPN 连接的应用程序的 Android 应用程序包名称。</span><span class="sxs-lookup"><span data-stu-id="8fe13-401">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="8fe13-402">wifiBlockEditConfigurations</span><span class="sxs-lookup"><span data-stu-id="8fe13-402">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="8fe13-403">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fe13-403">Boolean</span></span>|<span data-ttu-id="8fe13-404">指示是否阻止用户编辑 wifi 连接设置。</span><span class="sxs-lookup"><span data-stu-id="8fe13-404">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="8fe13-405">wifiBlockEditPolicyDefinedConfigurations</span><span class="sxs-lookup"><span data-stu-id="8fe13-405">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="8fe13-406">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fe13-406">Boolean</span></span>|<span data-ttu-id="8fe13-407">指示是否阻止用户仅编辑策略定义的网络。</span><span class="sxs-lookup"><span data-stu-id="8fe13-407">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|



## <a name="response"></a><span data-ttu-id="8fe13-408">响应</span><span class="sxs-lookup"><span data-stu-id="8fe13-408">Response</span></span>
<span data-ttu-id="8fe13-409">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8fe13-409">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8fe13-410">示例</span><span class="sxs-lookup"><span data-stu-id="8fe13-410">Example</span></span>

### <a name="request"></a><span data-ttu-id="8fe13-411">请求</span><span class="sxs-lookup"><span data-stu-id="8fe13-411">Request</span></span>
<span data-ttu-id="8fe13-412">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8fe13-412">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 4374

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

### <a name="response"></a><span data-ttu-id="8fe13-413">响应</span><span class="sxs-lookup"><span data-stu-id="8fe13-413">Response</span></span>
<span data-ttu-id="8fe13-p136">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8fe13-p136">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4546

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





