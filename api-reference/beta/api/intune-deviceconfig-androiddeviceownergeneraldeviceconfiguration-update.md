---
title: 更新 androidDeviceOwnerGeneralDeviceConfiguration
description: 更新 androidDeviceOwnerGeneralDeviceConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c9efd699bcbf1eaf9e968e38d0a7a6f72d5ef4a1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42450053"
---
# <a name="update-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="da3b3-103">更新 androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="da3b3-103">Update androidDeviceOwnerGeneralDeviceConfiguration</span></span>

<span data-ttu-id="da3b3-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="da3b3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="da3b3-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="da3b3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="da3b3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="da3b3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da3b3-107">更新[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="da3b3-107">Update the properties of a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="da3b3-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="da3b3-108">Prerequisites</span></span>
<span data-ttu-id="da3b3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="da3b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da3b3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="da3b3-111">Permission type</span></span>|<span data-ttu-id="da3b3-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="da3b3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da3b3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="da3b3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="da3b3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da3b3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="da3b3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="da3b3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da3b3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="da3b3-116">Not supported.</span></span>|
|<span data-ttu-id="da3b3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="da3b3-117">Application</span></span>|<span data-ttu-id="da3b3-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da3b3-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="da3b3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="da3b3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="da3b3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="da3b3-120">Request headers</span></span>
|<span data-ttu-id="da3b3-121">标头</span><span class="sxs-lookup"><span data-stu-id="da3b3-121">Header</span></span>|<span data-ttu-id="da3b3-122">值</span><span class="sxs-lookup"><span data-stu-id="da3b3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da3b3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="da3b3-123">Authorization</span></span>|<span data-ttu-id="da3b3-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="da3b3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da3b3-125">接受</span><span class="sxs-lookup"><span data-stu-id="da3b3-125">Accept</span></span>|<span data-ttu-id="da3b3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="da3b3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da3b3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="da3b3-127">Request body</span></span>
<span data-ttu-id="da3b3-128">在请求正文中，提供[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="da3b3-128">In the request body, supply a JSON representation for the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="da3b3-129">下表显示创建[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="da3b3-129">The following table shows the properties that are required when you create the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="da3b3-130">属性</span><span class="sxs-lookup"><span data-stu-id="da3b3-130">Property</span></span>|<span data-ttu-id="da3b3-131">类型</span><span class="sxs-lookup"><span data-stu-id="da3b3-131">Type</span></span>|<span data-ttu-id="da3b3-132">说明</span><span class="sxs-lookup"><span data-stu-id="da3b3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da3b3-133">id</span><span class="sxs-lookup"><span data-stu-id="da3b3-133">id</span></span>|<span data-ttu-id="da3b3-134">字符串</span><span class="sxs-lookup"><span data-stu-id="da3b3-134">String</span></span>|<span data-ttu-id="da3b3-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="da3b3-135">Key of the entity.</span></span> <span data-ttu-id="da3b3-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da3b3-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da3b3-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="da3b3-137">lastModifiedDateTime</span></span>|<span data-ttu-id="da3b3-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da3b3-138">DateTimeOffset</span></span>|<span data-ttu-id="da3b3-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="da3b3-139">DateTime the object was last modified.</span></span> <span data-ttu-id="da3b3-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da3b3-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da3b3-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="da3b3-141">roleScopeTagIds</span></span>|<span data-ttu-id="da3b3-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="da3b3-142">String collection</span></span>|<span data-ttu-id="da3b3-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="da3b3-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="da3b3-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da3b3-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da3b3-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="da3b3-145">supportsScopeTags</span></span>|<span data-ttu-id="da3b3-146">布尔</span><span class="sxs-lookup"><span data-stu-id="da3b3-146">Boolean</span></span>|<span data-ttu-id="da3b3-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="da3b3-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="da3b3-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="da3b3-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="da3b3-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="da3b3-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="da3b3-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="da3b3-150">This property is read-only.</span></span> <span data-ttu-id="da3b3-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da3b3-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da3b3-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="da3b3-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="da3b3-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="da3b3-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="da3b3-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="da3b3-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="da3b3-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da3b3-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da3b3-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="da3b3-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="da3b3-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="da3b3-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="da3b3-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="da3b3-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="da3b3-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da3b3-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da3b3-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="da3b3-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="da3b3-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="da3b3-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="da3b3-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="da3b3-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="da3b3-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da3b3-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da3b3-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="da3b3-164">createdDateTime</span></span>|<span data-ttu-id="da3b3-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da3b3-165">DateTimeOffset</span></span>|<span data-ttu-id="da3b3-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="da3b3-166">DateTime the object was created.</span></span> <span data-ttu-id="da3b3-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da3b3-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da3b3-168">说明</span><span class="sxs-lookup"><span data-stu-id="da3b3-168">description</span></span>|<span data-ttu-id="da3b3-169">String</span><span class="sxs-lookup"><span data-stu-id="da3b3-169">String</span></span>|<span data-ttu-id="da3b3-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="da3b3-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="da3b3-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da3b3-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da3b3-172">displayName</span><span class="sxs-lookup"><span data-stu-id="da3b3-172">displayName</span></span>|<span data-ttu-id="da3b3-173">String</span><span class="sxs-lookup"><span data-stu-id="da3b3-173">String</span></span>|<span data-ttu-id="da3b3-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="da3b3-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="da3b3-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da3b3-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da3b3-176">version</span><span class="sxs-lookup"><span data-stu-id="da3b3-176">version</span></span>|<span data-ttu-id="da3b3-177">Int32</span><span class="sxs-lookup"><span data-stu-id="da3b3-177">Int32</span></span>|<span data-ttu-id="da3b3-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="da3b3-178">Version of the device configuration.</span></span> <span data-ttu-id="da3b3-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da3b3-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da3b3-180">accountsBlockModification</span><span class="sxs-lookup"><span data-stu-id="da3b3-180">accountsBlockModification</span></span>|<span data-ttu-id="da3b3-181">布尔</span><span class="sxs-lookup"><span data-stu-id="da3b3-181">Boolean</span></span>|<span data-ttu-id="da3b3-182">指示是否禁用添加或删除帐户。</span><span class="sxs-lookup"><span data-stu-id="da3b3-182">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="da3b3-183">appsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="da3b3-183">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="da3b3-184">布尔</span><span class="sxs-lookup"><span data-stu-id="da3b3-184">Boolean</span></span>|<span data-ttu-id="da3b3-185">指示是否允许用户启用 "未知源" 设置。</span><span class="sxs-lookup"><span data-stu-id="da3b3-185">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="da3b3-186">appsAutoUpdatePolicy</span><span class="sxs-lookup"><span data-stu-id="da3b3-186">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="da3b3-187">androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="da3b3-187">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="da3b3-188">指示应用程序自动更新策略的值。</span><span class="sxs-lookup"><span data-stu-id="da3b3-188">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="da3b3-189">可取值为：`notConfigured`、`userChoice`、`never`、`wiFiOnly`、`always`。</span><span class="sxs-lookup"><span data-stu-id="da3b3-189">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="da3b3-190">appsDefaultPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="da3b3-190">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="da3b3-191">androidDeviceOwnerDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="da3b3-191">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="da3b3-192">指示对运行时权限请求的权限策略（如果专门没有为应用程序定义）。</span><span class="sxs-lookup"><span data-stu-id="da3b3-192">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="da3b3-193">可取值为：`deviceDefault`、`prompt`、`autoGrant`、`autoDeny`。</span><span class="sxs-lookup"><span data-stu-id="da3b3-193">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="da3b3-194">appsRecommendSkippingFirstUseHints</span><span class="sxs-lookup"><span data-stu-id="da3b3-194">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="da3b3-195">布尔</span><span class="sxs-lookup"><span data-stu-id="da3b3-195">Boolean</span></span>|<span data-ttu-id="da3b3-196">是否建议所有应用都将跳过他们可能已添加的任何首次使用提示。</span><span class="sxs-lookup"><span data-stu-id="da3b3-196">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="da3b3-197">bluetoothBlockConfiguration</span><span class="sxs-lookup"><span data-stu-id="da3b3-197">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="da3b3-198">布尔</span><span class="sxs-lookup"><span data-stu-id="da3b3-198">Boolean</span></span>|<span data-ttu-id="da3b3-199">指示是否阻止用户配置蓝牙。</span><span class="sxs-lookup"><span data-stu-id="da3b3-199">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="da3b3-200">bluetoothBlockContactSharing</span><span class="sxs-lookup"><span data-stu-id="da3b3-200">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="da3b3-201">布尔</span><span class="sxs-lookup"><span data-stu-id="da3b3-201">Boolean</span></span>|<span data-ttu-id="da3b3-202">指示是否阻止用户通过蓝牙共享联系人。</span><span class="sxs-lookup"><span data-stu-id="da3b3-202">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="da3b3-203">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="da3b3-203">cameraBlocked</span></span>|<span data-ttu-id="da3b3-204">布尔</span><span class="sxs-lookup"><span data-stu-id="da3b3-204">Boolean</span></span>|<span data-ttu-id="da3b3-205">指示是否禁用相机的使用。</span><span class="sxs-lookup"><span data-stu-id="da3b3-205">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="da3b3-206">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="da3b3-206">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="da3b3-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="da3b3-207">Boolean</span></span>|<span data-ttu-id="da3b3-208">指示是否阻止 Wi-Fi 网络共享。</span><span class="sxs-lookup"><span data-stu-id="da3b3-208">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="da3b3-209">certificateCredentialConfigurationDisabled</span><span class="sxs-lookup"><span data-stu-id="da3b3-209">certificateCredentialConfigurationDisabled</span></span>|<span data-ttu-id="da3b3-210">布尔</span><span class="sxs-lookup"><span data-stu-id="da3b3-210">Boolean</span></span>|<span data-ttu-id="da3b3-211">指示是否阻止来自任何证书凭据配置的用户。</span><span class="sxs-lookup"><span data-stu-id="da3b3-211">Indicates whether or not to block users from any certificate credential configuration.</span></span>|
|<span data-ttu-id="da3b3-212">dataRoamingBlocked</span><span class="sxs-lookup"><span data-stu-id="da3b3-212">dataRoamingBlocked</span></span>|<span data-ttu-id="da3b3-213">布尔</span><span class="sxs-lookup"><span data-stu-id="da3b3-213">Boolean</span></span>|<span data-ttu-id="da3b3-214">指示是否阻止用户使用数据漫游。</span><span class="sxs-lookup"><span data-stu-id="da3b3-214">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="da3b3-215">dateTimeConfigurationBlocked</span><span class="sxs-lookup"><span data-stu-id="da3b3-215">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="da3b3-216">布尔</span><span class="sxs-lookup"><span data-stu-id="da3b3-216">Boolean</span></span>|<span data-ttu-id="da3b3-217">指示是否阻止用户手动更改设备上的日期或时间</span><span class="sxs-lookup"><span data-stu-id="da3b3-217">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="da3b3-218">factoryResetDeviceAdministratorEmails</span><span class="sxs-lookup"><span data-stu-id="da3b3-218">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="da3b3-219">String 集合</span><span class="sxs-lookup"><span data-stu-id="da3b3-219">String collection</span></span>|<span data-ttu-id="da3b3-220">在设备出厂重置之前，将需要进行身份验证的 Google 帐户电子邮件的列表，然后才能对其进行设置。</span><span class="sxs-lookup"><span data-stu-id="da3b3-220">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="da3b3-221">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="da3b3-221">factoryResetBlocked</span></span>|<span data-ttu-id="da3b3-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="da3b3-222">Boolean</span></span>|<span data-ttu-id="da3b3-223">指示是否禁用了 "设置" 中的 "恢复出厂设置" 选项。</span><span class="sxs-lookup"><span data-stu-id="da3b3-223">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="da3b3-224">globalProxy</span><span class="sxs-lookup"><span data-stu-id="da3b3-224">globalProxy</span></span>|[<span data-ttu-id="da3b3-225">androidDeviceOwnerGlobalProxy</span><span class="sxs-lookup"><span data-stu-id="da3b3-225">androidDeviceOwnerGlobalProxy</span></span>](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)|<span data-ttu-id="da3b3-226">代理是与主机、端口和已排除的主机直接建立的。</span><span class="sxs-lookup"><span data-stu-id="da3b3-226">Proxy is set up directly with host, port and excluded hosts.</span></span>|
|<span data-ttu-id="da3b3-227">googleAccountsBlocked</span><span class="sxs-lookup"><span data-stu-id="da3b3-227">googleAccountsBlocked</span></span>|<span data-ttu-id="da3b3-228">布尔</span><span class="sxs-lookup"><span data-stu-id="da3b3-228">Boolean</span></span>|<span data-ttu-id="da3b3-229">指示是否将阻止 google 帐户。</span><span class="sxs-lookup"><span data-stu-id="da3b3-229">Indicates whether or not google accounts will be blocked.</span></span>|
|<span data-ttu-id="da3b3-230">kioskModeScreenSaverConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="da3b3-230">kioskModeScreenSaverConfigurationEnabled</span></span>|<span data-ttu-id="da3b3-231">布尔</span><span class="sxs-lookup"><span data-stu-id="da3b3-231">Boolean</span></span>|<span data-ttu-id="da3b3-232">是否启用屏幕保护程序模式或不启用展台模式。</span><span class="sxs-lookup"><span data-stu-id="da3b3-232">Whether or not to enable screen saver mode or not in Kiosk Mode.</span></span>|
|<span data-ttu-id="da3b3-233">kioskModeScreenSaverImageUrl</span><span class="sxs-lookup"><span data-stu-id="da3b3-233">kioskModeScreenSaverImageUrl</span></span>|<span data-ttu-id="da3b3-234">String</span><span class="sxs-lookup"><span data-stu-id="da3b3-234">String</span></span>|<span data-ttu-id="da3b3-235">将作为展台模式下设备的屏幕保护程序的图像的 URL。</span><span class="sxs-lookup"><span data-stu-id="da3b3-235">URL for an image that will be the device's screen saver in Kiosk Mode.</span></span>|
|<span data-ttu-id="da3b3-236">kioskModeScreenSaverDisplayTimeInSeconds</span><span class="sxs-lookup"><span data-stu-id="da3b3-236">kioskModeScreenSaverDisplayTimeInSeconds</span></span>|<span data-ttu-id="da3b3-237">Int32</span><span class="sxs-lookup"><span data-stu-id="da3b3-237">Int32</span></span>|<span data-ttu-id="da3b3-238">设备将在展台模式下显示屏幕保护程序的秒数。</span><span class="sxs-lookup"><span data-stu-id="da3b3-238">The number of seconds that the device will display the screen saver for in Kiosk Mode.</span></span> <span data-ttu-id="da3b3-239">有效值为0至9999999</span><span class="sxs-lookup"><span data-stu-id="da3b3-239">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="da3b3-240">kioskModeScreenSaverStartDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="da3b3-240">kioskModeScreenSaverStartDelayInSeconds</span></span>|<span data-ttu-id="da3b3-241">Int32</span><span class="sxs-lookup"><span data-stu-id="da3b3-241">Int32</span></span>|<span data-ttu-id="da3b3-242">在 Kiosk 模式下显示屏幕保护程序之前设备需要保持非活动状态的秒数。</span><span class="sxs-lookup"><span data-stu-id="da3b3-242">The number of seconds the device needs to be inactive for before the screen saver is shown in Kiosk Mode.</span></span> <span data-ttu-id="da3b3-243">有效值为1至9999999</span><span class="sxs-lookup"><span data-stu-id="da3b3-243">Valid values 1 to 9999999</span></span>|
|<span data-ttu-id="da3b3-244">kioskModeScreenSaverDetectMediaDisabled</span><span class="sxs-lookup"><span data-stu-id="da3b3-244">kioskModeScreenSaverDetectMediaDisabled</span></span>|<span data-ttu-id="da3b3-245">布尔</span><span class="sxs-lookup"><span data-stu-id="da3b3-245">Boolean</span></span>|<span data-ttu-id="da3b3-246">如果音频/视频在展台模式下播放，则设备屏幕是否应显示屏幕保护程序。</span><span class="sxs-lookup"><span data-stu-id="da3b3-246">Whether or not the device screen should show the screen saver if audio/video is playing in Kiosk Mode.</span></span>|
|<span data-ttu-id="da3b3-247">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="da3b3-247">kioskModeApps</span></span>|<span data-ttu-id="da3b3-248">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="da3b3-248">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="da3b3-249">设备处于展台模式时将显示的托管应用列表。</span><span class="sxs-lookup"><span data-stu-id="da3b3-249">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="da3b3-250">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="da3b3-250">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="da3b3-251">kioskModeWallpaperUrl</span><span class="sxs-lookup"><span data-stu-id="da3b3-251">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="da3b3-252">String</span><span class="sxs-lookup"><span data-stu-id="da3b3-252">String</span></span>|<span data-ttu-id="da3b3-253">在设备处于展台模式时用于墙纸的可公开访问图像的 URL。</span><span class="sxs-lookup"><span data-stu-id="da3b3-253">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="da3b3-254">kioskModeExitCode</span><span class="sxs-lookup"><span data-stu-id="da3b3-254">kioskModeExitCode</span></span>|<span data-ttu-id="da3b3-255">String</span><span class="sxs-lookup"><span data-stu-id="da3b3-255">String</span></span>|<span data-ttu-id="da3b3-256">退出代码，以允许用户在设备处于展台模式时从展台模式中进行转义。</span><span class="sxs-lookup"><span data-stu-id="da3b3-256">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="da3b3-257">kioskModeVirtualHomeButtonEnabled</span><span class="sxs-lookup"><span data-stu-id="da3b3-257">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="da3b3-258">布尔</span><span class="sxs-lookup"><span data-stu-id="da3b3-258">Boolean</span></span>|<span data-ttu-id="da3b3-259">设备处于展台模式时是否显示虚拟 "主页" 按钮。</span><span class="sxs-lookup"><span data-stu-id="da3b3-259">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="da3b3-260">kioskModeVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="da3b3-260">kioskModeVirtualHomeButtonType</span></span>|[<span data-ttu-id="da3b3-261">androidDeviceOwnerVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="da3b3-261">androidDeviceOwnerVirtualHomeButtonType</span></span>](../resources/intune-deviceconfig-androiddeviceownervirtualhomebuttontype.md)|<span data-ttu-id="da3b3-262">指示虚拟 home 按钮是否为向上轻扫主页按钮或浮动主页按钮。</span><span class="sxs-lookup"><span data-stu-id="da3b3-262">Indicates whether the virtual home button is a swipe up home button or a floating home button.</span></span> <span data-ttu-id="da3b3-263">可取值为：`notConfigured`、`swipeUp`、`floating`。</span><span class="sxs-lookup"><span data-stu-id="da3b3-263">Possible values are: `notConfigured`, `swipeUp`, `floating`.</span></span>|
|<span data-ttu-id="da3b3-264">kioskModeBluetoothConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="da3b3-264">kioskModeBluetoothConfigurationEnabled</span></span>|<span data-ttu-id="da3b3-265">布尔</span><span class="sxs-lookup"><span data-stu-id="da3b3-265">Boolean</span></span>|<span data-ttu-id="da3b3-266">是否允许用户在展台模式下配置蓝牙设置。</span><span class="sxs-lookup"><span data-stu-id="da3b3-266">Whether or not to allow a user to configure Bluetooth settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="da3b3-267">kioskModeWiFiConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="da3b3-267">kioskModeWiFiConfigurationEnabled</span></span>|<span data-ttu-id="da3b3-268">布尔</span><span class="sxs-lookup"><span data-stu-id="da3b3-268">Boolean</span></span>|<span data-ttu-id="da3b3-269">是否允许用户在展台模式下配置 Wi-fi 设置。</span><span class="sxs-lookup"><span data-stu-id="da3b3-269">Whether or not to allow a user to configure Wi-Fi settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="da3b3-270">kioskModeFlashlightConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="da3b3-270">kioskModeFlashlightConfigurationEnabled</span></span>|<span data-ttu-id="da3b3-271">布尔</span><span class="sxs-lookup"><span data-stu-id="da3b3-271">Boolean</span></span>|<span data-ttu-id="da3b3-272">是否允许用户在展台模式下使用该模式。</span><span class="sxs-lookup"><span data-stu-id="da3b3-272">Whether or not to allow a user to use the flashlight in Kiosk Mode.</span></span>|
|<span data-ttu-id="da3b3-273">kioskModeMediaVolumeConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="da3b3-273">kioskModeMediaVolumeConfigurationEnabled</span></span>|<span data-ttu-id="da3b3-274">布尔</span><span class="sxs-lookup"><span data-stu-id="da3b3-274">Boolean</span></span>|<span data-ttu-id="da3b3-275">是否允许用户在展台模式下更改媒体音量。</span><span class="sxs-lookup"><span data-stu-id="da3b3-275">Whether or not to allow a user to change the media volume in Kiosk Mode.</span></span>|
|<span data-ttu-id="da3b3-276">microphoneForceMute</span><span class="sxs-lookup"><span data-stu-id="da3b3-276">microphoneForceMute</span></span>|<span data-ttu-id="da3b3-277">布尔</span><span class="sxs-lookup"><span data-stu-id="da3b3-277">Boolean</span></span>|<span data-ttu-id="da3b3-278">指示是否阻止观众在设备上的麦克风。</span><span class="sxs-lookup"><span data-stu-id="da3b3-278">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="da3b3-279">networkEscapeHatchAllowed</span><span class="sxs-lookup"><span data-stu-id="da3b3-279">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="da3b3-280">布尔</span><span class="sxs-lookup"><span data-stu-id="da3b3-280">Boolean</span></span>|<span data-ttu-id="da3b3-281">指示在引导时设备是否允许连接到临时网络连接。</span><span class="sxs-lookup"><span data-stu-id="da3b3-281">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="da3b3-282">nfcBlockOutgoingBeam</span><span class="sxs-lookup"><span data-stu-id="da3b3-282">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="da3b3-283">布尔</span><span class="sxs-lookup"><span data-stu-id="da3b3-283">Boolean</span></span>|<span data-ttu-id="da3b3-284">指示是否阻止 NFC 传出横梁。</span><span class="sxs-lookup"><span data-stu-id="da3b3-284">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="da3b3-285">passwordBlockKeyguard</span><span class="sxs-lookup"><span data-stu-id="da3b3-285">passwordBlockKeyguard</span></span>|<span data-ttu-id="da3b3-286">布尔</span><span class="sxs-lookup"><span data-stu-id="da3b3-286">Boolean</span></span>|<span data-ttu-id="da3b3-287">指示是否禁用 keyguard。</span><span class="sxs-lookup"><span data-stu-id="da3b3-287">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="da3b3-288">passwordBlockKeyguardFeatures</span><span class="sxs-lookup"><span data-stu-id="da3b3-288">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="da3b3-289">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md)集合</span><span class="sxs-lookup"><span data-stu-id="da3b3-289">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="da3b3-290">要阻止的设备 keyguard 功能的列表。</span><span class="sxs-lookup"><span data-stu-id="da3b3-290">List of device keyguard features to block.</span></span> <span data-ttu-id="da3b3-291">该集合最多可包含 7 个元素。</span><span class="sxs-lookup"><span data-stu-id="da3b3-291">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="da3b3-292">可取值为：`notConfigured`、`camera`、`notifications`、`unredactedNotifications`、`trustAgents`、`fingerprint`、`remoteInput`、`allFeatures`。</span><span class="sxs-lookup"><span data-stu-id="da3b3-292">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="da3b3-293">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="da3b3-293">passwordExpirationDays</span></span>|<span data-ttu-id="da3b3-294">Int32</span><span class="sxs-lookup"><span data-stu-id="da3b3-294">Int32</span></span>|<span data-ttu-id="da3b3-295">指示在密码过期之前可以设置密码的时间量（以秒为单位）以及需要新密码的时间（以秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="da3b3-295">Indicates the amount of time in seconds that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="da3b3-296">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="da3b3-296">Valid values 1 to 365</span></span>|
|<span data-ttu-id="da3b3-297">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="da3b3-297">passwordMinimumLength</span></span>|<span data-ttu-id="da3b3-298">Int32</span><span class="sxs-lookup"><span data-stu-id="da3b3-298">Int32</span></span>|<span data-ttu-id="da3b3-299">指示设备上所需密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="da3b3-299">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="da3b3-300">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="da3b3-300">Valid values 4 to 16</span></span>|
|<span data-ttu-id="da3b3-301">passwordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="da3b3-301">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="da3b3-302">Int32</span><span class="sxs-lookup"><span data-stu-id="da3b3-302">Int32</span></span>|<span data-ttu-id="da3b3-303">指示设备密码所需的字母字符的最小数量。</span><span class="sxs-lookup"><span data-stu-id="da3b3-303">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="da3b3-304">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="da3b3-304">Valid values 1 to 16</span></span>|
|<span data-ttu-id="da3b3-305">passwordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="da3b3-305">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="da3b3-306">Int32</span><span class="sxs-lookup"><span data-stu-id="da3b3-306">Int32</span></span>|<span data-ttu-id="da3b3-307">指示设备密码所需的最小小写字符数。</span><span class="sxs-lookup"><span data-stu-id="da3b3-307">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="da3b3-308">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="da3b3-308">Valid values 1 to 16</span></span>|
|<span data-ttu-id="da3b3-309">passwordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="da3b3-309">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="da3b3-310">Int32</span><span class="sxs-lookup"><span data-stu-id="da3b3-310">Int32</span></span>|<span data-ttu-id="da3b3-311">指示设备密码所需的最小非字母字符数。</span><span class="sxs-lookup"><span data-stu-id="da3b3-311">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="da3b3-312">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="da3b3-312">Valid values 1 to 16</span></span>|
|<span data-ttu-id="da3b3-313">passwordMinimumNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="da3b3-313">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="da3b3-314">Int32</span><span class="sxs-lookup"><span data-stu-id="da3b3-314">Int32</span></span>|<span data-ttu-id="da3b3-315">指示设备密码所需的最小数字字符数。</span><span class="sxs-lookup"><span data-stu-id="da3b3-315">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="da3b3-316">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="da3b3-316">Valid values 1 to 16</span></span>|
|<span data-ttu-id="da3b3-317">passwordMinimumSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="da3b3-317">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="da3b3-318">Int32</span><span class="sxs-lookup"><span data-stu-id="da3b3-318">Int32</span></span>|<span data-ttu-id="da3b3-319">指示设备密码所需的最小符号字符数。</span><span class="sxs-lookup"><span data-stu-id="da3b3-319">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="da3b3-320">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="da3b3-320">Valid values 1 to 16</span></span>|
|<span data-ttu-id="da3b3-321">passwordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="da3b3-321">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="da3b3-322">Int32</span><span class="sxs-lookup"><span data-stu-id="da3b3-322">Int32</span></span>|<span data-ttu-id="da3b3-323">指示设备密码所需的最小上限 caseletter 字符数。</span><span class="sxs-lookup"><span data-stu-id="da3b3-323">Indicates the minimum number of upper caseletter characters required for device password.</span></span> <span data-ttu-id="da3b3-324">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="da3b3-324">Valid values 1 to 16</span></span>|
|<span data-ttu-id="da3b3-325">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="da3b3-325">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="da3b3-326">Int32</span><span class="sxs-lookup"><span data-stu-id="da3b3-326">Int32</span></span>|<span data-ttu-id="da3b3-327">屏幕超时之前的不活动时间（毫秒）。</span><span class="sxs-lookup"><span data-stu-id="da3b3-327">Milliseconds of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="da3b3-328">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="da3b3-328">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="da3b3-329">Int32</span><span class="sxs-lookup"><span data-stu-id="da3b3-329">Int32</span></span>|<span data-ttu-id="da3b3-330">指示密码历史记录的长度，其中用户将不能输入与历史记录中的任何密码相同的新密码。</span><span class="sxs-lookup"><span data-stu-id="da3b3-330">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="da3b3-331">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="da3b3-331">Valid values 0 to 24</span></span>|
|<span data-ttu-id="da3b3-332">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="da3b3-332">passwordRequiredType</span></span>|[<span data-ttu-id="da3b3-333">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="da3b3-333">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="da3b3-334">指示设备上所需的最小密码质量。</span><span class="sxs-lookup"><span data-stu-id="da3b3-334">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="da3b3-335">可取值为：`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`customPassword`。</span><span class="sxs-lookup"><span data-stu-id="da3b3-335">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|
|<span data-ttu-id="da3b3-336">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="da3b3-336">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="da3b3-337">Int32</span><span class="sxs-lookup"><span data-stu-id="da3b3-337">Int32</span></span>|<span data-ttu-id="da3b3-338">指示用户在擦除设备之前可以输入不正确密码的次数。</span><span class="sxs-lookup"><span data-stu-id="da3b3-338">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="da3b3-339">有效值为 4 至 11</span><span class="sxs-lookup"><span data-stu-id="da3b3-339">Valid values 4 to 11</span></span>|
|<span data-ttu-id="da3b3-340">playStoreMode</span><span class="sxs-lookup"><span data-stu-id="da3b3-340">playStoreMode</span></span>|[<span data-ttu-id="da3b3-341">androidDeviceOwnerPlayStoreMode</span><span class="sxs-lookup"><span data-stu-id="da3b3-341">androidDeviceOwnerPlayStoreMode</span></span>](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|<span data-ttu-id="da3b3-342">指示设备的播放存储模式。</span><span class="sxs-lookup"><span data-stu-id="da3b3-342">Indicates the Play Store mode of the device.</span></span> <span data-ttu-id="da3b3-343">可取值为：`notConfigured`、`allowList`、`blockList`。</span><span class="sxs-lookup"><span data-stu-id="da3b3-343">Possible values are: `notConfigured`, `allowList`, `blockList`.</span></span>|
|<span data-ttu-id="da3b3-344">safeBootBlocked</span><span class="sxs-lookup"><span data-stu-id="da3b3-344">safeBootBlocked</span></span>|<span data-ttu-id="da3b3-345">布尔</span><span class="sxs-lookup"><span data-stu-id="da3b3-345">Boolean</span></span>|<span data-ttu-id="da3b3-346">指示是否禁用重新启动设备到安全启动。</span><span class="sxs-lookup"><span data-stu-id="da3b3-346">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="da3b3-347">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="da3b3-347">screenCaptureBlocked</span></span>|<span data-ttu-id="da3b3-348">Boolean</span><span class="sxs-lookup"><span data-stu-id="da3b3-348">Boolean</span></span>|<span data-ttu-id="da3b3-349">指示是否禁用获取屏幕截图的功能。</span><span class="sxs-lookup"><span data-stu-id="da3b3-349">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="da3b3-350">securityAllowDebuggingFeatures</span><span class="sxs-lookup"><span data-stu-id="da3b3-350">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="da3b3-351">布尔</span><span class="sxs-lookup"><span data-stu-id="da3b3-351">Boolean</span></span>|<span data-ttu-id="da3b3-352">指示是否阻止用户启用设备上的调试功能。</span><span class="sxs-lookup"><span data-stu-id="da3b3-352">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="da3b3-353">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="da3b3-353">securityRequireVerifyApps</span></span>|<span data-ttu-id="da3b3-354">布尔</span><span class="sxs-lookup"><span data-stu-id="da3b3-354">Boolean</span></span>|<span data-ttu-id="da3b3-355">指示是否需要验证应用。</span><span class="sxs-lookup"><span data-stu-id="da3b3-355">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="da3b3-356">statusBarBlocked</span><span class="sxs-lookup"><span data-stu-id="da3b3-356">statusBarBlocked</span></span>|<span data-ttu-id="da3b3-357">布尔</span><span class="sxs-lookup"><span data-stu-id="da3b3-357">Boolean</span></span>|<span data-ttu-id="da3b3-358">指示是否禁用状态栏，包括通知、快速设置和其他屏幕重叠。</span><span class="sxs-lookup"><span data-stu-id="da3b3-358">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="da3b3-359">stayOnModes</span><span class="sxs-lookup"><span data-stu-id="da3b3-359">stayOnModes</span></span>|<span data-ttu-id="da3b3-360">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)集合</span><span class="sxs-lookup"><span data-stu-id="da3b3-360">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="da3b3-361">设备的显示将保持开机状态的模式列表。</span><span class="sxs-lookup"><span data-stu-id="da3b3-361">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="da3b3-362">此集合最多可包含4个元素。</span><span class="sxs-lookup"><span data-stu-id="da3b3-362">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="da3b3-363">可取值为：`notConfigured`、`ac`、`usb`、`wireless`。</span><span class="sxs-lookup"><span data-stu-id="da3b3-363">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="da3b3-364">storageAllowUsb</span><span class="sxs-lookup"><span data-stu-id="da3b3-364">storageAllowUsb</span></span>|<span data-ttu-id="da3b3-365">布尔</span><span class="sxs-lookup"><span data-stu-id="da3b3-365">Boolean</span></span>|<span data-ttu-id="da3b3-366">指示是否允许 USB 大容量存储。</span><span class="sxs-lookup"><span data-stu-id="da3b3-366">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="da3b3-367">storageBlockExternalMedia</span><span class="sxs-lookup"><span data-stu-id="da3b3-367">storageBlockExternalMedia</span></span>|<span data-ttu-id="da3b3-368">布尔</span><span class="sxs-lookup"><span data-stu-id="da3b3-368">Boolean</span></span>|<span data-ttu-id="da3b3-369">指示是否阻止外部媒体。</span><span class="sxs-lookup"><span data-stu-id="da3b3-369">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="da3b3-370">storageBlockUsbFileTransfer</span><span class="sxs-lookup"><span data-stu-id="da3b3-370">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="da3b3-371">布尔</span><span class="sxs-lookup"><span data-stu-id="da3b3-371">Boolean</span></span>|<span data-ttu-id="da3b3-372">指示是否阻止 USB 文件传输。</span><span class="sxs-lookup"><span data-stu-id="da3b3-372">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="da3b3-373">systemUpdateWindowStartMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="da3b3-373">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="da3b3-374">Int32</span><span class="sxs-lookup"><span data-stu-id="da3b3-374">Int32</span></span>|<span data-ttu-id="da3b3-375">指示系统更新窗口午夜后启动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="da3b3-375">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="da3b3-376">有效值为0至1440</span><span class="sxs-lookup"><span data-stu-id="da3b3-376">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="da3b3-377">systemUpdateWindowEndMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="da3b3-377">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="da3b3-378">Int32</span><span class="sxs-lookup"><span data-stu-id="da3b3-378">Int32</span></span>|<span data-ttu-id="da3b3-379">指示系统更新窗口结束后的分钟数。</span><span class="sxs-lookup"><span data-stu-id="da3b3-379">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="da3b3-380">有效值为0至1440</span><span class="sxs-lookup"><span data-stu-id="da3b3-380">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="da3b3-381">systemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="da3b3-381">systemUpdateInstallType</span></span>|[<span data-ttu-id="da3b3-382">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="da3b3-382">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="da3b3-383">系统更新配置的类型。</span><span class="sxs-lookup"><span data-stu-id="da3b3-383">The type of system update configuration.</span></span> <span data-ttu-id="da3b3-384">可取值为：`deviceDefault`、`postpone`、`windowed`、`automatic`。</span><span class="sxs-lookup"><span data-stu-id="da3b3-384">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="da3b3-385">systemWindowsBlocked</span><span class="sxs-lookup"><span data-stu-id="da3b3-385">systemWindowsBlocked</span></span>|<span data-ttu-id="da3b3-386">布尔</span><span class="sxs-lookup"><span data-stu-id="da3b3-386">Boolean</span></span>|<span data-ttu-id="da3b3-387">是否阻止 Android 系统提示符窗口，如 toast、电话活动和系统通知。</span><span class="sxs-lookup"><span data-stu-id="da3b3-387">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="da3b3-388">usersBlockAdd</span><span class="sxs-lookup"><span data-stu-id="da3b3-388">usersBlockAdd</span></span>|<span data-ttu-id="da3b3-389">布尔</span><span class="sxs-lookup"><span data-stu-id="da3b3-389">Boolean</span></span>|<span data-ttu-id="da3b3-390">指示是否禁用添加用户和配置文件。</span><span class="sxs-lookup"><span data-stu-id="da3b3-390">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="da3b3-391">usersBlockRemove</span><span class="sxs-lookup"><span data-stu-id="da3b3-391">usersBlockRemove</span></span>|<span data-ttu-id="da3b3-392">布尔</span><span class="sxs-lookup"><span data-stu-id="da3b3-392">Boolean</span></span>|<span data-ttu-id="da3b3-393">指示是否禁用从设备中删除其他用户。</span><span class="sxs-lookup"><span data-stu-id="da3b3-393">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="da3b3-394">volumeBlockAdjustment</span><span class="sxs-lookup"><span data-stu-id="da3b3-394">volumeBlockAdjustment</span></span>|<span data-ttu-id="da3b3-395">布尔</span><span class="sxs-lookup"><span data-stu-id="da3b3-395">Boolean</span></span>|<span data-ttu-id="da3b3-396">指示是否禁用了调整主音量。</span><span class="sxs-lookup"><span data-stu-id="da3b3-396">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="da3b3-397">vpnAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="da3b3-397">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="da3b3-398">布尔</span><span class="sxs-lookup"><span data-stu-id="da3b3-398">Boolean</span></span>|<span data-ttu-id="da3b3-399">如果指定了 always on VPN 包名称，则在断开 VPN 连接时是否锁定网络流量。</span><span class="sxs-lookup"><span data-stu-id="da3b3-399">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="da3b3-400">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="da3b3-400">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="da3b3-401">String</span><span class="sxs-lookup"><span data-stu-id="da3b3-401">String</span></span>|<span data-ttu-id="da3b3-402">将处理永不启用 VPN 连接的应用程序的 Android 应用程序包名称。</span><span class="sxs-lookup"><span data-stu-id="da3b3-402">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="da3b3-403">wifiBlockEditConfigurations</span><span class="sxs-lookup"><span data-stu-id="da3b3-403">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="da3b3-404">布尔</span><span class="sxs-lookup"><span data-stu-id="da3b3-404">Boolean</span></span>|<span data-ttu-id="da3b3-405">指示是否阻止用户编辑 wifi 连接设置。</span><span class="sxs-lookup"><span data-stu-id="da3b3-405">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="da3b3-406">wifiBlockEditPolicyDefinedConfigurations</span><span class="sxs-lookup"><span data-stu-id="da3b3-406">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="da3b3-407">布尔</span><span class="sxs-lookup"><span data-stu-id="da3b3-407">Boolean</span></span>|<span data-ttu-id="da3b3-408">指示是否阻止用户仅编辑策略定义的网络。</span><span class="sxs-lookup"><span data-stu-id="da3b3-408">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|



## <a name="response"></a><span data-ttu-id="da3b3-409">响应</span><span class="sxs-lookup"><span data-stu-id="da3b3-409">Response</span></span>
<span data-ttu-id="da3b3-410">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="da3b3-410">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da3b3-411">示例</span><span class="sxs-lookup"><span data-stu-id="da3b3-411">Example</span></span>

### <a name="request"></a><span data-ttu-id="da3b3-412">请求</span><span class="sxs-lookup"><span data-stu-id="da3b3-412">Request</span></span>
<span data-ttu-id="da3b3-413">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="da3b3-413">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="da3b3-414">响应</span><span class="sxs-lookup"><span data-stu-id="da3b3-414">Response</span></span>
<span data-ttu-id="da3b3-p136">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="da3b3-p136">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





