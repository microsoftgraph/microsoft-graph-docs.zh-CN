---
title: 更新 androidDeviceOwnerGeneralDeviceConfiguration
description: 更新 androidDeviceOwnerGeneralDeviceConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ec76020364ee73e173804a47acd29c5225af17cf
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178722"
---
# <a name="update-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="5af2f-103">更新 androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="5af2f-103">Update androidDeviceOwnerGeneralDeviceConfiguration</span></span>

<span data-ttu-id="5af2f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5af2f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5af2f-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5af2f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5af2f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5af2f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5af2f-107">更新[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5af2f-107">Update the properties of a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5af2f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="5af2f-108">Prerequisites</span></span>
<span data-ttu-id="5af2f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5af2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5af2f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5af2f-111">Permission type</span></span>|<span data-ttu-id="5af2f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5af2f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5af2f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5af2f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5af2f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5af2f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5af2f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5af2f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5af2f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5af2f-116">Not supported.</span></span>|
|<span data-ttu-id="5af2f-117">Application</span><span class="sxs-lookup"><span data-stu-id="5af2f-117">Application</span></span>|<span data-ttu-id="5af2f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5af2f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5af2f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5af2f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="5af2f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5af2f-120">Request headers</span></span>
|<span data-ttu-id="5af2f-121">标头</span><span class="sxs-lookup"><span data-stu-id="5af2f-121">Header</span></span>|<span data-ttu-id="5af2f-122">值</span><span class="sxs-lookup"><span data-stu-id="5af2f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5af2f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5af2f-123">Authorization</span></span>|<span data-ttu-id="5af2f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5af2f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5af2f-125">接受</span><span class="sxs-lookup"><span data-stu-id="5af2f-125">Accept</span></span>|<span data-ttu-id="5af2f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5af2f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5af2f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5af2f-127">Request body</span></span>
<span data-ttu-id="5af2f-128">在请求正文中，提供[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5af2f-128">In the request body, supply a JSON representation for the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="5af2f-129">下表显示创建[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5af2f-129">The following table shows the properties that are required when you create the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="5af2f-130">属性</span><span class="sxs-lookup"><span data-stu-id="5af2f-130">Property</span></span>|<span data-ttu-id="5af2f-131">类型</span><span class="sxs-lookup"><span data-stu-id="5af2f-131">Type</span></span>|<span data-ttu-id="5af2f-132">说明</span><span class="sxs-lookup"><span data-stu-id="5af2f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5af2f-133">id</span><span class="sxs-lookup"><span data-stu-id="5af2f-133">id</span></span>|<span data-ttu-id="5af2f-134">字符串</span><span class="sxs-lookup"><span data-stu-id="5af2f-134">String</span></span>|<span data-ttu-id="5af2f-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5af2f-135">Key of the entity.</span></span> <span data-ttu-id="5af2f-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5af2f-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5af2f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5af2f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="5af2f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5af2f-138">DateTimeOffset</span></span>|<span data-ttu-id="5af2f-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="5af2f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="5af2f-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5af2f-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5af2f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5af2f-141">roleScopeTagIds</span></span>|<span data-ttu-id="5af2f-142">字符串集合</span><span class="sxs-lookup"><span data-stu-id="5af2f-142">String collection</span></span>|<span data-ttu-id="5af2f-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="5af2f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5af2f-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5af2f-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5af2f-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="5af2f-145">supportsScopeTags</span></span>|<span data-ttu-id="5af2f-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="5af2f-146">Boolean</span></span>|<span data-ttu-id="5af2f-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="5af2f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5af2f-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="5af2f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5af2f-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="5af2f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5af2f-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5af2f-150">This property is read-only.</span></span> <span data-ttu-id="5af2f-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5af2f-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5af2f-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5af2f-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="5af2f-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5af2f-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="5af2f-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="5af2f-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="5af2f-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5af2f-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5af2f-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5af2f-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="5af2f-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5af2f-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="5af2f-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="5af2f-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="5af2f-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5af2f-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5af2f-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="5af2f-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="5af2f-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="5af2f-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="5af2f-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="5af2f-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="5af2f-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5af2f-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5af2f-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5af2f-164">createdDateTime</span></span>|<span data-ttu-id="5af2f-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5af2f-165">DateTimeOffset</span></span>|<span data-ttu-id="5af2f-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="5af2f-166">DateTime the object was created.</span></span> <span data-ttu-id="5af2f-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5af2f-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5af2f-168">说明</span><span class="sxs-lookup"><span data-stu-id="5af2f-168">description</span></span>|<span data-ttu-id="5af2f-169">String</span><span class="sxs-lookup"><span data-stu-id="5af2f-169">String</span></span>|<span data-ttu-id="5af2f-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="5af2f-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5af2f-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5af2f-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5af2f-172">displayName</span><span class="sxs-lookup"><span data-stu-id="5af2f-172">displayName</span></span>|<span data-ttu-id="5af2f-173">String</span><span class="sxs-lookup"><span data-stu-id="5af2f-173">String</span></span>|<span data-ttu-id="5af2f-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="5af2f-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5af2f-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5af2f-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5af2f-176">version</span><span class="sxs-lookup"><span data-stu-id="5af2f-176">version</span></span>|<span data-ttu-id="5af2f-177">Int32</span><span class="sxs-lookup"><span data-stu-id="5af2f-177">Int32</span></span>|<span data-ttu-id="5af2f-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="5af2f-178">Version of the device configuration.</span></span> <span data-ttu-id="5af2f-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5af2f-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5af2f-180">accountsBlockModification</span><span class="sxs-lookup"><span data-stu-id="5af2f-180">accountsBlockModification</span></span>|<span data-ttu-id="5af2f-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="5af2f-181">Boolean</span></span>|<span data-ttu-id="5af2f-182">指示是否禁用添加或删除帐户。</span><span class="sxs-lookup"><span data-stu-id="5af2f-182">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="5af2f-183">appsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="5af2f-183">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="5af2f-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="5af2f-184">Boolean</span></span>|<span data-ttu-id="5af2f-185">指示是否允许用户启用 "未知源" 设置。</span><span class="sxs-lookup"><span data-stu-id="5af2f-185">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="5af2f-186">appsAutoUpdatePolicy</span><span class="sxs-lookup"><span data-stu-id="5af2f-186">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="5af2f-187">androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="5af2f-187">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="5af2f-188">指示应用程序自动更新策略的值。</span><span class="sxs-lookup"><span data-stu-id="5af2f-188">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="5af2f-189">可取值为：`notConfigured`、`userChoice`、`never`、`wiFiOnly`、`always`。</span><span class="sxs-lookup"><span data-stu-id="5af2f-189">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="5af2f-190">appsDefaultPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="5af2f-190">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="5af2f-191">androidDeviceOwnerDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="5af2f-191">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="5af2f-192">指示对运行时权限请求的权限策略（如果专门没有为应用程序定义）。</span><span class="sxs-lookup"><span data-stu-id="5af2f-192">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="5af2f-193">可取值为：`deviceDefault`、`prompt`、`autoGrant`、`autoDeny`。</span><span class="sxs-lookup"><span data-stu-id="5af2f-193">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="5af2f-194">appsRecommendSkippingFirstUseHints</span><span class="sxs-lookup"><span data-stu-id="5af2f-194">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="5af2f-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="5af2f-195">Boolean</span></span>|<span data-ttu-id="5af2f-196">是否建议所有应用都将跳过他们可能已添加的任何首次使用提示。</span><span class="sxs-lookup"><span data-stu-id="5af2f-196">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="5af2f-197">bluetoothBlockConfiguration</span><span class="sxs-lookup"><span data-stu-id="5af2f-197">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="5af2f-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="5af2f-198">Boolean</span></span>|<span data-ttu-id="5af2f-199">指示是否阻止用户配置蓝牙。</span><span class="sxs-lookup"><span data-stu-id="5af2f-199">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="5af2f-200">bluetoothBlockContactSharing</span><span class="sxs-lookup"><span data-stu-id="5af2f-200">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="5af2f-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="5af2f-201">Boolean</span></span>|<span data-ttu-id="5af2f-202">指示是否阻止用户通过蓝牙共享联系人。</span><span class="sxs-lookup"><span data-stu-id="5af2f-202">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="5af2f-203">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="5af2f-203">cameraBlocked</span></span>|<span data-ttu-id="5af2f-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="5af2f-204">Boolean</span></span>|<span data-ttu-id="5af2f-205">指示是否禁用相机的使用。</span><span class="sxs-lookup"><span data-stu-id="5af2f-205">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="5af2f-206">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="5af2f-206">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="5af2f-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="5af2f-207">Boolean</span></span>|<span data-ttu-id="5af2f-208">指示是否阻止 Wi-Fi 网络共享。</span><span class="sxs-lookup"><span data-stu-id="5af2f-208">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="5af2f-209">certificateCredentialConfigurationDisabled</span><span class="sxs-lookup"><span data-stu-id="5af2f-209">certificateCredentialConfigurationDisabled</span></span>|<span data-ttu-id="5af2f-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="5af2f-210">Boolean</span></span>|<span data-ttu-id="5af2f-211">指示是否阻止来自任何证书凭据配置的用户。</span><span class="sxs-lookup"><span data-stu-id="5af2f-211">Indicates whether or not to block users from any certificate credential configuration.</span></span>|
|<span data-ttu-id="5af2f-212">microsoftLauncherConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="5af2f-212">microsoftLauncherConfigurationEnabled</span></span>|<span data-ttu-id="5af2f-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="5af2f-213">Boolean</span></span>|<span data-ttu-id="5af2f-214">指示是否要配置 Microsoft 启动器。</span><span class="sxs-lookup"><span data-stu-id="5af2f-214">Indicates whether or not to you want configure Microsoft Launcher.</span></span>|
|<span data-ttu-id="5af2f-215">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="5af2f-215">enrollmentProfile</span></span>|[<span data-ttu-id="5af2f-216">androidDeviceOwnerEnrollmentProfileType</span><span class="sxs-lookup"><span data-stu-id="5af2f-216">androidDeviceOwnerEnrollmentProfileType</span></span>](../resources/intune-deviceconfig-androiddeviceownerenrollmentprofiletype.md)|<span data-ttu-id="5af2f-217">指示要配置的注册配置文件。</span><span class="sxs-lookup"><span data-stu-id="5af2f-217">Indicates which enrollment profile you want to configure.</span></span> <span data-ttu-id="5af2f-218">可取值为：`notConfigured`、`dedicatedDevice`、`fullyManaged`。</span><span class="sxs-lookup"><span data-stu-id="5af2f-218">Possible values are: `notConfigured`, `dedicatedDevice`, `fullyManaged`.</span></span>|
|<span data-ttu-id="5af2f-219">dataRoamingBlocked</span><span class="sxs-lookup"><span data-stu-id="5af2f-219">dataRoamingBlocked</span></span>|<span data-ttu-id="5af2f-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="5af2f-220">Boolean</span></span>|<span data-ttu-id="5af2f-221">指示是否阻止用户使用数据漫游。</span><span class="sxs-lookup"><span data-stu-id="5af2f-221">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="5af2f-222">dateTimeConfigurationBlocked</span><span class="sxs-lookup"><span data-stu-id="5af2f-222">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="5af2f-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="5af2f-223">Boolean</span></span>|<span data-ttu-id="5af2f-224">指示是否阻止用户手动更改设备上的日期或时间</span><span class="sxs-lookup"><span data-stu-id="5af2f-224">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="5af2f-225">factoryResetDeviceAdministratorEmails</span><span class="sxs-lookup"><span data-stu-id="5af2f-225">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="5af2f-226">字符串集合</span><span class="sxs-lookup"><span data-stu-id="5af2f-226">String collection</span></span>|<span data-ttu-id="5af2f-227">在设备出厂重置之前，将需要进行身份验证的 Google 帐户电子邮件的列表，然后才能对其进行设置。</span><span class="sxs-lookup"><span data-stu-id="5af2f-227">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="5af2f-228">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="5af2f-228">factoryResetBlocked</span></span>|<span data-ttu-id="5af2f-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="5af2f-229">Boolean</span></span>|<span data-ttu-id="5af2f-230">指示是否禁用了 "设置" 中的 "恢复出厂设置" 选项。</span><span class="sxs-lookup"><span data-stu-id="5af2f-230">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="5af2f-231">globalProxy</span><span class="sxs-lookup"><span data-stu-id="5af2f-231">globalProxy</span></span>|[<span data-ttu-id="5af2f-232">androidDeviceOwnerGlobalProxy</span><span class="sxs-lookup"><span data-stu-id="5af2f-232">androidDeviceOwnerGlobalProxy</span></span>](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)|<span data-ttu-id="5af2f-233">代理是与主机、端口和已排除的主机直接建立的。</span><span class="sxs-lookup"><span data-stu-id="5af2f-233">Proxy is set up directly with host, port and excluded hosts.</span></span>|
|<span data-ttu-id="5af2f-234">googleAccountsBlocked</span><span class="sxs-lookup"><span data-stu-id="5af2f-234">googleAccountsBlocked</span></span>|<span data-ttu-id="5af2f-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="5af2f-235">Boolean</span></span>|<span data-ttu-id="5af2f-236">指示是否将阻止 google 帐户。</span><span class="sxs-lookup"><span data-stu-id="5af2f-236">Indicates whether or not google accounts will be blocked.</span></span>|
|<span data-ttu-id="5af2f-237">kioskModeScreenSaverConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="5af2f-237">kioskModeScreenSaverConfigurationEnabled</span></span>|<span data-ttu-id="5af2f-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="5af2f-238">Boolean</span></span>|<span data-ttu-id="5af2f-239">是否启用屏幕保护程序模式或不启用展台模式。</span><span class="sxs-lookup"><span data-stu-id="5af2f-239">Whether or not to enable screen saver mode or not in Kiosk Mode.</span></span>|
|<span data-ttu-id="5af2f-240">kioskModeScreenSaverImageUrl</span><span class="sxs-lookup"><span data-stu-id="5af2f-240">kioskModeScreenSaverImageUrl</span></span>|<span data-ttu-id="5af2f-241">字符串</span><span class="sxs-lookup"><span data-stu-id="5af2f-241">String</span></span>|<span data-ttu-id="5af2f-242">将作为展台模式下设备的屏幕保护程序的图像的 URL。</span><span class="sxs-lookup"><span data-stu-id="5af2f-242">URL for an image that will be the device's screen saver in Kiosk Mode.</span></span>|
|<span data-ttu-id="5af2f-243">kioskModeScreenSaverDisplayTimeInSeconds</span><span class="sxs-lookup"><span data-stu-id="5af2f-243">kioskModeScreenSaverDisplayTimeInSeconds</span></span>|<span data-ttu-id="5af2f-244">Int32</span><span class="sxs-lookup"><span data-stu-id="5af2f-244">Int32</span></span>|<span data-ttu-id="5af2f-245">设备将在展台模式下显示屏幕保护程序的秒数。</span><span class="sxs-lookup"><span data-stu-id="5af2f-245">The number of seconds that the device will display the screen saver for in Kiosk Mode.</span></span> <span data-ttu-id="5af2f-246">有效值为0至9999999</span><span class="sxs-lookup"><span data-stu-id="5af2f-246">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="5af2f-247">kioskModeScreenSaverStartDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="5af2f-247">kioskModeScreenSaverStartDelayInSeconds</span></span>|<span data-ttu-id="5af2f-248">Int32</span><span class="sxs-lookup"><span data-stu-id="5af2f-248">Int32</span></span>|<span data-ttu-id="5af2f-249">在 Kiosk 模式下显示屏幕保护程序之前设备需要保持非活动状态的秒数。</span><span class="sxs-lookup"><span data-stu-id="5af2f-249">The number of seconds the device needs to be inactive for before the screen saver is shown in Kiosk Mode.</span></span> <span data-ttu-id="5af2f-250">有效值为1至9999999</span><span class="sxs-lookup"><span data-stu-id="5af2f-250">Valid values 1 to 9999999</span></span>|
|<span data-ttu-id="5af2f-251">kioskModeScreenSaverDetectMediaDisabled</span><span class="sxs-lookup"><span data-stu-id="5af2f-251">kioskModeScreenSaverDetectMediaDisabled</span></span>|<span data-ttu-id="5af2f-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="5af2f-252">Boolean</span></span>|<span data-ttu-id="5af2f-253">如果音频/视频在展台模式下播放，则设备屏幕是否应显示屏幕保护程序。</span><span class="sxs-lookup"><span data-stu-id="5af2f-253">Whether or not the device screen should show the screen saver if audio/video is playing in Kiosk Mode.</span></span>|
|<span data-ttu-id="5af2f-254">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="5af2f-254">kioskModeApps</span></span>|<span data-ttu-id="5af2f-255">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5af2f-255">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="5af2f-256">设备处于展台模式时将显示的托管应用列表。</span><span class="sxs-lookup"><span data-stu-id="5af2f-256">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="5af2f-257">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="5af2f-257">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="5af2f-258">kioskModeWallpaperUrl</span><span class="sxs-lookup"><span data-stu-id="5af2f-258">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="5af2f-259">字符串</span><span class="sxs-lookup"><span data-stu-id="5af2f-259">String</span></span>|<span data-ttu-id="5af2f-260">在设备处于展台模式时用于墙纸的可公开访问图像的 URL。</span><span class="sxs-lookup"><span data-stu-id="5af2f-260">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="5af2f-261">kioskModeExitCode</span><span class="sxs-lookup"><span data-stu-id="5af2f-261">kioskModeExitCode</span></span>|<span data-ttu-id="5af2f-262">字符串</span><span class="sxs-lookup"><span data-stu-id="5af2f-262">String</span></span>|<span data-ttu-id="5af2f-263">退出代码，以允许用户在设备处于展台模式时从展台模式中进行转义。</span><span class="sxs-lookup"><span data-stu-id="5af2f-263">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="5af2f-264">kioskModeVirtualHomeButtonEnabled</span><span class="sxs-lookup"><span data-stu-id="5af2f-264">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="5af2f-265">Boolean</span><span class="sxs-lookup"><span data-stu-id="5af2f-265">Boolean</span></span>|<span data-ttu-id="5af2f-266">设备处于展台模式时是否显示虚拟 "主页" 按钮。</span><span class="sxs-lookup"><span data-stu-id="5af2f-266">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="5af2f-267">kioskModeVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="5af2f-267">kioskModeVirtualHomeButtonType</span></span>|[<span data-ttu-id="5af2f-268">androidDeviceOwnerVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="5af2f-268">androidDeviceOwnerVirtualHomeButtonType</span></span>](../resources/intune-deviceconfig-androiddeviceownervirtualhomebuttontype.md)|<span data-ttu-id="5af2f-269">指示虚拟 home 按钮是否为向上轻扫主页按钮或浮动主页按钮。</span><span class="sxs-lookup"><span data-stu-id="5af2f-269">Indicates whether the virtual home button is a swipe up home button or a floating home button.</span></span> <span data-ttu-id="5af2f-270">可取值为：`notConfigured`、`swipeUp`、`floating`。</span><span class="sxs-lookup"><span data-stu-id="5af2f-270">Possible values are: `notConfigured`, `swipeUp`, `floating`.</span></span>|
|<span data-ttu-id="5af2f-271">kioskModeBluetoothConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="5af2f-271">kioskModeBluetoothConfigurationEnabled</span></span>|<span data-ttu-id="5af2f-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="5af2f-272">Boolean</span></span>|<span data-ttu-id="5af2f-273">是否允许用户在展台模式下配置蓝牙设置。</span><span class="sxs-lookup"><span data-stu-id="5af2f-273">Whether or not to allow a user to configure Bluetooth settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="5af2f-274">kioskModeWiFiConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="5af2f-274">kioskModeWiFiConfigurationEnabled</span></span>|<span data-ttu-id="5af2f-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="5af2f-275">Boolean</span></span>|<span data-ttu-id="5af2f-276">是否允许用户在展台模式下配置 Wi-fi 设置。</span><span class="sxs-lookup"><span data-stu-id="5af2f-276">Whether or not to allow a user to configure Wi-Fi settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="5af2f-277">kioskModeFlashlightConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="5af2f-277">kioskModeFlashlightConfigurationEnabled</span></span>|<span data-ttu-id="5af2f-278">Boolean</span><span class="sxs-lookup"><span data-stu-id="5af2f-278">Boolean</span></span>|<span data-ttu-id="5af2f-279">是否允许用户在展台模式下使用该模式。</span><span class="sxs-lookup"><span data-stu-id="5af2f-279">Whether or not to allow a user to use the flashlight in Kiosk Mode.</span></span>|
|<span data-ttu-id="5af2f-280">kioskModeMediaVolumeConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="5af2f-280">kioskModeMediaVolumeConfigurationEnabled</span></span>|<span data-ttu-id="5af2f-281">Boolean</span><span class="sxs-lookup"><span data-stu-id="5af2f-281">Boolean</span></span>|<span data-ttu-id="5af2f-282">是否允许用户在展台模式下更改媒体音量。</span><span class="sxs-lookup"><span data-stu-id="5af2f-282">Whether or not to allow a user to change the media volume in Kiosk Mode.</span></span>|
|<span data-ttu-id="5af2f-283">microphoneForceMute</span><span class="sxs-lookup"><span data-stu-id="5af2f-283">microphoneForceMute</span></span>|<span data-ttu-id="5af2f-284">Boolean</span><span class="sxs-lookup"><span data-stu-id="5af2f-284">Boolean</span></span>|<span data-ttu-id="5af2f-285">指示是否阻止观众在设备上的麦克风。</span><span class="sxs-lookup"><span data-stu-id="5af2f-285">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="5af2f-286">networkEscapeHatchAllowed</span><span class="sxs-lookup"><span data-stu-id="5af2f-286">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="5af2f-287">Boolean</span><span class="sxs-lookup"><span data-stu-id="5af2f-287">Boolean</span></span>|<span data-ttu-id="5af2f-288">指示在引导时设备是否允许连接到临时网络连接。</span><span class="sxs-lookup"><span data-stu-id="5af2f-288">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="5af2f-289">nfcBlockOutgoingBeam</span><span class="sxs-lookup"><span data-stu-id="5af2f-289">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="5af2f-290">Boolean</span><span class="sxs-lookup"><span data-stu-id="5af2f-290">Boolean</span></span>|<span data-ttu-id="5af2f-291">指示是否阻止 NFC 传出横梁。</span><span class="sxs-lookup"><span data-stu-id="5af2f-291">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="5af2f-292">passwordBlockKeyguard</span><span class="sxs-lookup"><span data-stu-id="5af2f-292">passwordBlockKeyguard</span></span>|<span data-ttu-id="5af2f-293">Boolean</span><span class="sxs-lookup"><span data-stu-id="5af2f-293">Boolean</span></span>|<span data-ttu-id="5af2f-294">指示是否禁用 keyguard。</span><span class="sxs-lookup"><span data-stu-id="5af2f-294">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="5af2f-295">passwordBlockKeyguardFeatures</span><span class="sxs-lookup"><span data-stu-id="5af2f-295">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="5af2f-296">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md)集合</span><span class="sxs-lookup"><span data-stu-id="5af2f-296">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="5af2f-297">要阻止的设备 keyguard 功能的列表。</span><span class="sxs-lookup"><span data-stu-id="5af2f-297">List of device keyguard features to block.</span></span> <span data-ttu-id="5af2f-298">该集合最多可包含 7 个元素。</span><span class="sxs-lookup"><span data-stu-id="5af2f-298">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="5af2f-299">可取值为：`notConfigured`、`camera`、`notifications`、`unredactedNotifications`、`trustAgents`、`fingerprint`、`remoteInput`、`allFeatures`。</span><span class="sxs-lookup"><span data-stu-id="5af2f-299">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="5af2f-300">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="5af2f-300">passwordExpirationDays</span></span>|<span data-ttu-id="5af2f-301">Int32</span><span class="sxs-lookup"><span data-stu-id="5af2f-301">Int32</span></span>|<span data-ttu-id="5af2f-302">指示在密码过期之前可以设置密码的时间量（以秒为单位）以及需要新密码的时间（以秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="5af2f-302">Indicates the amount of time in seconds that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="5af2f-303">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="5af2f-303">Valid values 1 to 365</span></span>|
|<span data-ttu-id="5af2f-304">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="5af2f-304">passwordMinimumLength</span></span>|<span data-ttu-id="5af2f-305">Int32</span><span class="sxs-lookup"><span data-stu-id="5af2f-305">Int32</span></span>|<span data-ttu-id="5af2f-306">指示设备上所需密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="5af2f-306">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="5af2f-307">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="5af2f-307">Valid values 4 to 16</span></span>|
|<span data-ttu-id="5af2f-308">passwordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="5af2f-308">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="5af2f-309">Int32</span><span class="sxs-lookup"><span data-stu-id="5af2f-309">Int32</span></span>|<span data-ttu-id="5af2f-310">指示设备密码所需的字母字符的最小数量。</span><span class="sxs-lookup"><span data-stu-id="5af2f-310">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="5af2f-311">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="5af2f-311">Valid values 1 to 16</span></span>|
|<span data-ttu-id="5af2f-312">passwordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="5af2f-312">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="5af2f-313">Int32</span><span class="sxs-lookup"><span data-stu-id="5af2f-313">Int32</span></span>|<span data-ttu-id="5af2f-314">指示设备密码所需的最小小写字符数。</span><span class="sxs-lookup"><span data-stu-id="5af2f-314">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="5af2f-315">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="5af2f-315">Valid values 1 to 16</span></span>|
|<span data-ttu-id="5af2f-316">passwordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="5af2f-316">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="5af2f-317">Int32</span><span class="sxs-lookup"><span data-stu-id="5af2f-317">Int32</span></span>|<span data-ttu-id="5af2f-318">指示设备密码所需的最小非字母字符数。</span><span class="sxs-lookup"><span data-stu-id="5af2f-318">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="5af2f-319">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="5af2f-319">Valid values 1 to 16</span></span>|
|<span data-ttu-id="5af2f-320">passwordMinimumNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="5af2f-320">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="5af2f-321">Int32</span><span class="sxs-lookup"><span data-stu-id="5af2f-321">Int32</span></span>|<span data-ttu-id="5af2f-322">指示设备密码所需的最小数字字符数。</span><span class="sxs-lookup"><span data-stu-id="5af2f-322">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="5af2f-323">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="5af2f-323">Valid values 1 to 16</span></span>|
|<span data-ttu-id="5af2f-324">passwordMinimumSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="5af2f-324">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="5af2f-325">Int32</span><span class="sxs-lookup"><span data-stu-id="5af2f-325">Int32</span></span>|<span data-ttu-id="5af2f-326">指示设备密码所需的最小符号字符数。</span><span class="sxs-lookup"><span data-stu-id="5af2f-326">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="5af2f-327">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="5af2f-327">Valid values 1 to 16</span></span>|
|<span data-ttu-id="5af2f-328">passwordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="5af2f-328">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="5af2f-329">Int32</span><span class="sxs-lookup"><span data-stu-id="5af2f-329">Int32</span></span>|<span data-ttu-id="5af2f-330">指示设备密码所需的最小上限 caseletter 字符数。</span><span class="sxs-lookup"><span data-stu-id="5af2f-330">Indicates the minimum number of upper caseletter characters required for device password.</span></span> <span data-ttu-id="5af2f-331">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="5af2f-331">Valid values 1 to 16</span></span>|
|<span data-ttu-id="5af2f-332">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="5af2f-332">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="5af2f-333">Int32</span><span class="sxs-lookup"><span data-stu-id="5af2f-333">Int32</span></span>|<span data-ttu-id="5af2f-334">屏幕超时之前的不活动时间（毫秒）。</span><span class="sxs-lookup"><span data-stu-id="5af2f-334">Milliseconds of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="5af2f-335">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="5af2f-335">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="5af2f-336">Int32</span><span class="sxs-lookup"><span data-stu-id="5af2f-336">Int32</span></span>|<span data-ttu-id="5af2f-337">指示密码历史记录的长度，其中用户将不能输入与历史记录中的任何密码相同的新密码。</span><span class="sxs-lookup"><span data-stu-id="5af2f-337">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="5af2f-338">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="5af2f-338">Valid values 0 to 24</span></span>|
|<span data-ttu-id="5af2f-339">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="5af2f-339">passwordRequiredType</span></span>|[<span data-ttu-id="5af2f-340">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="5af2f-340">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="5af2f-341">指示设备上所需的最小密码质量。</span><span class="sxs-lookup"><span data-stu-id="5af2f-341">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="5af2f-342">可取值为：`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`customPassword`。</span><span class="sxs-lookup"><span data-stu-id="5af2f-342">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|
|<span data-ttu-id="5af2f-343">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="5af2f-343">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="5af2f-344">Int32</span><span class="sxs-lookup"><span data-stu-id="5af2f-344">Int32</span></span>|<span data-ttu-id="5af2f-345">指示用户在擦除设备之前可以输入不正确密码的次数。</span><span class="sxs-lookup"><span data-stu-id="5af2f-345">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="5af2f-346">有效值为 4 至 11</span><span class="sxs-lookup"><span data-stu-id="5af2f-346">Valid values 4 to 11</span></span>|
|<span data-ttu-id="5af2f-347">playStoreMode</span><span class="sxs-lookup"><span data-stu-id="5af2f-347">playStoreMode</span></span>|[<span data-ttu-id="5af2f-348">androidDeviceOwnerPlayStoreMode</span><span class="sxs-lookup"><span data-stu-id="5af2f-348">androidDeviceOwnerPlayStoreMode</span></span>](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|<span data-ttu-id="5af2f-349">指示设备的播放存储模式。</span><span class="sxs-lookup"><span data-stu-id="5af2f-349">Indicates the Play Store mode of the device.</span></span> <span data-ttu-id="5af2f-350">可取值为：`notConfigured`、`allowList`、`blockList`。</span><span class="sxs-lookup"><span data-stu-id="5af2f-350">Possible values are: `notConfigured`, `allowList`, `blockList`.</span></span>|
|<span data-ttu-id="5af2f-351">safeBootBlocked</span><span class="sxs-lookup"><span data-stu-id="5af2f-351">safeBootBlocked</span></span>|<span data-ttu-id="5af2f-352">Boolean</span><span class="sxs-lookup"><span data-stu-id="5af2f-352">Boolean</span></span>|<span data-ttu-id="5af2f-353">指示是否禁用重新启动设备到安全启动。</span><span class="sxs-lookup"><span data-stu-id="5af2f-353">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="5af2f-354">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="5af2f-354">screenCaptureBlocked</span></span>|<span data-ttu-id="5af2f-355">Boolean</span><span class="sxs-lookup"><span data-stu-id="5af2f-355">Boolean</span></span>|<span data-ttu-id="5af2f-356">指示是否禁用获取屏幕截图的功能。</span><span class="sxs-lookup"><span data-stu-id="5af2f-356">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="5af2f-357">securityAllowDebuggingFeatures</span><span class="sxs-lookup"><span data-stu-id="5af2f-357">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="5af2f-358">Boolean</span><span class="sxs-lookup"><span data-stu-id="5af2f-358">Boolean</span></span>|<span data-ttu-id="5af2f-359">指示是否阻止用户启用设备上的调试功能。</span><span class="sxs-lookup"><span data-stu-id="5af2f-359">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="5af2f-360">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="5af2f-360">securityRequireVerifyApps</span></span>|<span data-ttu-id="5af2f-361">Boolean</span><span class="sxs-lookup"><span data-stu-id="5af2f-361">Boolean</span></span>|<span data-ttu-id="5af2f-362">指示是否需要验证应用。</span><span class="sxs-lookup"><span data-stu-id="5af2f-362">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="5af2f-363">statusBarBlocked</span><span class="sxs-lookup"><span data-stu-id="5af2f-363">statusBarBlocked</span></span>|<span data-ttu-id="5af2f-364">Boolean</span><span class="sxs-lookup"><span data-stu-id="5af2f-364">Boolean</span></span>|<span data-ttu-id="5af2f-365">指示是否禁用状态栏，包括通知、快速设置和其他屏幕重叠。</span><span class="sxs-lookup"><span data-stu-id="5af2f-365">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="5af2f-366">stayOnModes</span><span class="sxs-lookup"><span data-stu-id="5af2f-366">stayOnModes</span></span>|<span data-ttu-id="5af2f-367">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)集合</span><span class="sxs-lookup"><span data-stu-id="5af2f-367">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="5af2f-368">设备的显示将保持开机状态的模式列表。</span><span class="sxs-lookup"><span data-stu-id="5af2f-368">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="5af2f-369">此集合最多可包含4个元素。</span><span class="sxs-lookup"><span data-stu-id="5af2f-369">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="5af2f-370">可取值为：`notConfigured`、`ac`、`usb`、`wireless`。</span><span class="sxs-lookup"><span data-stu-id="5af2f-370">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="5af2f-371">storageAllowUsb</span><span class="sxs-lookup"><span data-stu-id="5af2f-371">storageAllowUsb</span></span>|<span data-ttu-id="5af2f-372">Boolean</span><span class="sxs-lookup"><span data-stu-id="5af2f-372">Boolean</span></span>|<span data-ttu-id="5af2f-373">指示是否允许 USB 大容量存储。</span><span class="sxs-lookup"><span data-stu-id="5af2f-373">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="5af2f-374">storageBlockExternalMedia</span><span class="sxs-lookup"><span data-stu-id="5af2f-374">storageBlockExternalMedia</span></span>|<span data-ttu-id="5af2f-375">Boolean</span><span class="sxs-lookup"><span data-stu-id="5af2f-375">Boolean</span></span>|<span data-ttu-id="5af2f-376">指示是否阻止外部媒体。</span><span class="sxs-lookup"><span data-stu-id="5af2f-376">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="5af2f-377">storageBlockUsbFileTransfer</span><span class="sxs-lookup"><span data-stu-id="5af2f-377">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="5af2f-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="5af2f-378">Boolean</span></span>|<span data-ttu-id="5af2f-379">指示是否阻止 USB 文件传输。</span><span class="sxs-lookup"><span data-stu-id="5af2f-379">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="5af2f-380">systemUpdateWindowStartMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="5af2f-380">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="5af2f-381">Int32</span><span class="sxs-lookup"><span data-stu-id="5af2f-381">Int32</span></span>|<span data-ttu-id="5af2f-382">指示系统更新窗口午夜后启动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="5af2f-382">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="5af2f-383">有效值为0至1440</span><span class="sxs-lookup"><span data-stu-id="5af2f-383">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="5af2f-384">systemUpdateWindowEndMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="5af2f-384">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="5af2f-385">Int32</span><span class="sxs-lookup"><span data-stu-id="5af2f-385">Int32</span></span>|<span data-ttu-id="5af2f-386">指示系统更新窗口结束后的分钟数。</span><span class="sxs-lookup"><span data-stu-id="5af2f-386">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="5af2f-387">有效值为0至1440</span><span class="sxs-lookup"><span data-stu-id="5af2f-387">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="5af2f-388">systemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="5af2f-388">systemUpdateInstallType</span></span>|[<span data-ttu-id="5af2f-389">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="5af2f-389">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="5af2f-390">系统更新配置的类型。</span><span class="sxs-lookup"><span data-stu-id="5af2f-390">The type of system update configuration.</span></span> <span data-ttu-id="5af2f-391">可取值为：`deviceDefault`、`postpone`、`windowed`、`automatic`。</span><span class="sxs-lookup"><span data-stu-id="5af2f-391">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="5af2f-392">systemWindowsBlocked</span><span class="sxs-lookup"><span data-stu-id="5af2f-392">systemWindowsBlocked</span></span>|<span data-ttu-id="5af2f-393">Boolean</span><span class="sxs-lookup"><span data-stu-id="5af2f-393">Boolean</span></span>|<span data-ttu-id="5af2f-394">是否阻止 Android 系统提示符窗口，如 toast、电话活动和系统通知。</span><span class="sxs-lookup"><span data-stu-id="5af2f-394">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="5af2f-395">usersBlockAdd</span><span class="sxs-lookup"><span data-stu-id="5af2f-395">usersBlockAdd</span></span>|<span data-ttu-id="5af2f-396">Boolean</span><span class="sxs-lookup"><span data-stu-id="5af2f-396">Boolean</span></span>|<span data-ttu-id="5af2f-397">指示是否禁用添加用户和配置文件。</span><span class="sxs-lookup"><span data-stu-id="5af2f-397">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="5af2f-398">usersBlockRemove</span><span class="sxs-lookup"><span data-stu-id="5af2f-398">usersBlockRemove</span></span>|<span data-ttu-id="5af2f-399">Boolean</span><span class="sxs-lookup"><span data-stu-id="5af2f-399">Boolean</span></span>|<span data-ttu-id="5af2f-400">指示是否禁用从设备中删除其他用户。</span><span class="sxs-lookup"><span data-stu-id="5af2f-400">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="5af2f-401">volumeBlockAdjustment</span><span class="sxs-lookup"><span data-stu-id="5af2f-401">volumeBlockAdjustment</span></span>|<span data-ttu-id="5af2f-402">Boolean</span><span class="sxs-lookup"><span data-stu-id="5af2f-402">Boolean</span></span>|<span data-ttu-id="5af2f-403">指示是否禁用了调整主音量。</span><span class="sxs-lookup"><span data-stu-id="5af2f-403">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="5af2f-404">vpnAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="5af2f-404">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="5af2f-405">Boolean</span><span class="sxs-lookup"><span data-stu-id="5af2f-405">Boolean</span></span>|<span data-ttu-id="5af2f-406">如果指定了 always on VPN 包名称，则在断开 VPN 连接时是否锁定网络流量。</span><span class="sxs-lookup"><span data-stu-id="5af2f-406">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="5af2f-407">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="5af2f-407">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="5af2f-408">字符串</span><span class="sxs-lookup"><span data-stu-id="5af2f-408">String</span></span>|<span data-ttu-id="5af2f-409">将处理永不启用 VPN 连接的应用程序的 Android 应用程序包名称。</span><span class="sxs-lookup"><span data-stu-id="5af2f-409">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="5af2f-410">wifiBlockEditConfigurations</span><span class="sxs-lookup"><span data-stu-id="5af2f-410">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="5af2f-411">Boolean</span><span class="sxs-lookup"><span data-stu-id="5af2f-411">Boolean</span></span>|<span data-ttu-id="5af2f-412">指示是否阻止用户编辑 wifi 连接设置。</span><span class="sxs-lookup"><span data-stu-id="5af2f-412">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="5af2f-413">wifiBlockEditPolicyDefinedConfigurations</span><span class="sxs-lookup"><span data-stu-id="5af2f-413">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="5af2f-414">Boolean</span><span class="sxs-lookup"><span data-stu-id="5af2f-414">Boolean</span></span>|<span data-ttu-id="5af2f-415">指示是否阻止用户仅编辑策略定义的网络。</span><span class="sxs-lookup"><span data-stu-id="5af2f-415">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|



## <a name="response"></a><span data-ttu-id="5af2f-416">响应</span><span class="sxs-lookup"><span data-stu-id="5af2f-416">Response</span></span>
<span data-ttu-id="5af2f-417">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5af2f-417">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5af2f-418">示例</span><span class="sxs-lookup"><span data-stu-id="5af2f-418">Example</span></span>

### <a name="request"></a><span data-ttu-id="5af2f-419">请求</span><span class="sxs-lookup"><span data-stu-id="5af2f-419">Request</span></span>
<span data-ttu-id="5af2f-420">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5af2f-420">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 4467

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

### <a name="response"></a><span data-ttu-id="5af2f-421">响应</span><span class="sxs-lookup"><span data-stu-id="5af2f-421">Response</span></span>
<span data-ttu-id="5af2f-p137">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5af2f-p137">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4639

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



