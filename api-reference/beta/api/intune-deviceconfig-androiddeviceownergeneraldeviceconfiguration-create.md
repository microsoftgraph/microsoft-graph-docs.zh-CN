---
title: 创建 androidDeviceOwnerGeneralDeviceConfiguration
description: 创建新的 androidDeviceOwnerGeneralDeviceConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1d3037edf6d8c093472a7f3d8292859368482e19
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123377"
---
# <a name="create-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="e1ac9-103">创建 androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="e1ac9-103">Create androidDeviceOwnerGeneralDeviceConfiguration</span></span>

<span data-ttu-id="e1ac9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1ac9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e1ac9-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1ac9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1ac9-107">创建新的[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-107">Create a new [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e1ac9-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e1ac9-108">Prerequisites</span></span>
<span data-ttu-id="e1ac9-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="e1ac9-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="e1ac9-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1ac9-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1ac9-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e1ac9-111">Permission type</span></span>|<span data-ttu-id="e1ac9-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e1ac9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1ac9-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e1ac9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e1ac9-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1ac9-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e1ac9-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e1ac9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1ac9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-116">Not supported.</span></span>|
|<span data-ttu-id="e1ac9-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e1ac9-117">Application</span></span>|<span data-ttu-id="e1ac9-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1ac9-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1ac9-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e1ac9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e1ac9-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e1ac9-120">Request headers</span></span>
|<span data-ttu-id="e1ac9-121">标头</span><span class="sxs-lookup"><span data-stu-id="e1ac9-121">Header</span></span>|<span data-ttu-id="e1ac9-122">值</span><span class="sxs-lookup"><span data-stu-id="e1ac9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1ac9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1ac9-123">Authorization</span></span>|<span data-ttu-id="e1ac9-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1ac9-125">接受</span><span class="sxs-lookup"><span data-stu-id="e1ac9-125">Accept</span></span>|<span data-ttu-id="e1ac9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e1ac9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1ac9-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e1ac9-127">Request body</span></span>
<span data-ttu-id="e1ac9-128">在请求正文中，提供 androidDeviceOwnerGeneralDeviceConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-128">In the request body, supply a JSON representation for the androidDeviceOwnerGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="e1ac9-129">下表显示创建 androidDeviceOwnerGeneralDeviceConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-129">The following table shows the properties that are required when you create the androidDeviceOwnerGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="e1ac9-130">属性</span><span class="sxs-lookup"><span data-stu-id="e1ac9-130">Property</span></span>|<span data-ttu-id="e1ac9-131">类型</span><span class="sxs-lookup"><span data-stu-id="e1ac9-131">Type</span></span>|<span data-ttu-id="e1ac9-132">说明</span><span class="sxs-lookup"><span data-stu-id="e1ac9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1ac9-133">id</span><span class="sxs-lookup"><span data-stu-id="e1ac9-133">id</span></span>|<span data-ttu-id="e1ac9-134">字符串</span><span class="sxs-lookup"><span data-stu-id="e1ac9-134">String</span></span>|<span data-ttu-id="e1ac9-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-135">Key of the entity.</span></span> <span data-ttu-id="e1ac9-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e1ac9-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e1ac9-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e1ac9-137">lastModifiedDateTime</span></span>|<span data-ttu-id="e1ac9-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1ac9-138">DateTimeOffset</span></span>|<span data-ttu-id="e1ac9-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-139">DateTime the object was last modified.</span></span> <span data-ttu-id="e1ac9-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e1ac9-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e1ac9-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e1ac9-141">roleScopeTagIds</span></span>|<span data-ttu-id="e1ac9-142">String collection</span><span class="sxs-lookup"><span data-stu-id="e1ac9-142">String collection</span></span>|<span data-ttu-id="e1ac9-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e1ac9-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e1ac9-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e1ac9-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="e1ac9-145">supportsScopeTags</span></span>|<span data-ttu-id="e1ac9-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ac9-146">Boolean</span></span>|<span data-ttu-id="e1ac9-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e1ac9-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e1ac9-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e1ac9-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-150">This property is read-only.</span></span> <span data-ttu-id="e1ac9-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e1ac9-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e1ac9-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e1ac9-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="e1ac9-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e1ac9-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="e1ac9-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="e1ac9-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e1ac9-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e1ac9-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e1ac9-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="e1ac9-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e1ac9-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="e1ac9-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="e1ac9-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e1ac9-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e1ac9-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e1ac9-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="e1ac9-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e1ac9-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="e1ac9-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="e1ac9-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e1ac9-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e1ac9-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e1ac9-164">createdDateTime</span></span>|<span data-ttu-id="e1ac9-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1ac9-165">DateTimeOffset</span></span>|<span data-ttu-id="e1ac9-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-166">DateTime the object was created.</span></span> <span data-ttu-id="e1ac9-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e1ac9-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e1ac9-168">说明</span><span class="sxs-lookup"><span data-stu-id="e1ac9-168">description</span></span>|<span data-ttu-id="e1ac9-169">String</span><span class="sxs-lookup"><span data-stu-id="e1ac9-169">String</span></span>|<span data-ttu-id="e1ac9-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e1ac9-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e1ac9-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e1ac9-172">displayName</span><span class="sxs-lookup"><span data-stu-id="e1ac9-172">displayName</span></span>|<span data-ttu-id="e1ac9-173">String</span><span class="sxs-lookup"><span data-stu-id="e1ac9-173">String</span></span>|<span data-ttu-id="e1ac9-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e1ac9-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e1ac9-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e1ac9-176">version</span><span class="sxs-lookup"><span data-stu-id="e1ac9-176">version</span></span>|<span data-ttu-id="e1ac9-177">Int32</span><span class="sxs-lookup"><span data-stu-id="e1ac9-177">Int32</span></span>|<span data-ttu-id="e1ac9-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-178">Version of the device configuration.</span></span> <span data-ttu-id="e1ac9-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e1ac9-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e1ac9-180">accountsBlockModification</span><span class="sxs-lookup"><span data-stu-id="e1ac9-180">accountsBlockModification</span></span>|<span data-ttu-id="e1ac9-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ac9-181">Boolean</span></span>|<span data-ttu-id="e1ac9-182">指示是否禁用添加或删除帐户。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-182">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="e1ac9-183">appsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="e1ac9-183">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="e1ac9-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ac9-184">Boolean</span></span>|<span data-ttu-id="e1ac9-185">指示是否允许用户启用 "未知源" 设置。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-185">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="e1ac9-186">appsAutoUpdatePolicy</span><span class="sxs-lookup"><span data-stu-id="e1ac9-186">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="e1ac9-187">androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="e1ac9-187">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="e1ac9-188">指示应用程序自动更新策略的值。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-188">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="e1ac9-189">可取值为：`notConfigured`、`userChoice`、`never`、`wiFiOnly`、`always`。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-189">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="e1ac9-190">appsDefaultPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="e1ac9-190">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="e1ac9-191">androidDeviceOwnerDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="e1ac9-191">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="e1ac9-192">指示对运行时权限请求的权限策略（如果专门没有为应用程序定义）。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-192">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="e1ac9-193">可取值为：`deviceDefault`、`prompt`、`autoGrant`、`autoDeny`。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-193">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="e1ac9-194">appsRecommendSkippingFirstUseHints</span><span class="sxs-lookup"><span data-stu-id="e1ac9-194">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="e1ac9-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ac9-195">Boolean</span></span>|<span data-ttu-id="e1ac9-196">是否建议所有应用都将跳过他们可能已添加的任何首次使用提示。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-196">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="e1ac9-197">bluetoothBlockConfiguration</span><span class="sxs-lookup"><span data-stu-id="e1ac9-197">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="e1ac9-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ac9-198">Boolean</span></span>|<span data-ttu-id="e1ac9-199">指示是否阻止用户配置蓝牙。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-199">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="e1ac9-200">bluetoothBlockContactSharing</span><span class="sxs-lookup"><span data-stu-id="e1ac9-200">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="e1ac9-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ac9-201">Boolean</span></span>|<span data-ttu-id="e1ac9-202">指示是否阻止用户通过蓝牙共享联系人。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-202">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="e1ac9-203">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="e1ac9-203">cameraBlocked</span></span>|<span data-ttu-id="e1ac9-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ac9-204">Boolean</span></span>|<span data-ttu-id="e1ac9-205">指示是否禁用相机的使用。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-205">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="e1ac9-206">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="e1ac9-206">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="e1ac9-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ac9-207">Boolean</span></span>|<span data-ttu-id="e1ac9-208">指示是否阻止 Wi-Fi 网络共享。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-208">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="e1ac9-209">certificateCredentialConfigurationDisabled</span><span class="sxs-lookup"><span data-stu-id="e1ac9-209">certificateCredentialConfigurationDisabled</span></span>|<span data-ttu-id="e1ac9-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ac9-210">Boolean</span></span>|<span data-ttu-id="e1ac9-211">指示是否阻止来自任何证书凭据配置的用户。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-211">Indicates whether or not to block users from any certificate credential configuration.</span></span>|
|<span data-ttu-id="e1ac9-212">microsoftLauncherConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="e1ac9-212">microsoftLauncherConfigurationEnabled</span></span>|<span data-ttu-id="e1ac9-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ac9-213">Boolean</span></span>|<span data-ttu-id="e1ac9-214">指示是否要配置 Microsoft 启动器。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-214">Indicates whether or not to you want configure Microsoft Launcher.</span></span>|
|<span data-ttu-id="e1ac9-215">microsoftLauncherCustomWallpaperEnabled</span><span class="sxs-lookup"><span data-stu-id="e1ac9-215">microsoftLauncherCustomWallpaperEnabled</span></span>|<span data-ttu-id="e1ac9-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ac9-216">Boolean</span></span>|<span data-ttu-id="e1ac9-217">指示是否在目标设备上配置墙纸。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-217">Indicates whether or not to configure the wallpaper on the targeted devices.</span></span>|
|<span data-ttu-id="e1ac9-218">microsoftLauncherCustomWallpaperImageUrl</span><span class="sxs-lookup"><span data-stu-id="e1ac9-218">microsoftLauncherCustomWallpaperImageUrl</span></span>|<span data-ttu-id="e1ac9-219">String</span><span class="sxs-lookup"><span data-stu-id="e1ac9-219">String</span></span>|<span data-ttu-id="e1ac9-220">指示用作目标设备墙纸的图像文件的 URL。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-220">Indicates the URL for the image file to use as the wallpaper on the targeted devices.</span></span>|
|<span data-ttu-id="e1ac9-221">microsoftLauncherCustomWallpaperAllowUserModification</span><span class="sxs-lookup"><span data-stu-id="e1ac9-221">microsoftLauncherCustomWallpaperAllowUserModification</span></span>|<span data-ttu-id="e1ac9-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ac9-222">Boolean</span></span>|<span data-ttu-id="e1ac9-223">指示用户是否可以修改墙纸以个性化设置其设备。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-223">Indicates whether or not the user can modify the wallpaper to personalize their device.</span></span>|
|<span data-ttu-id="e1ac9-224">microsoftLauncherFeedEnabled</span><span class="sxs-lookup"><span data-stu-id="e1ac9-224">microsoftLauncherFeedEnabled</span></span>|<span data-ttu-id="e1ac9-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ac9-225">Boolean</span></span>|<span data-ttu-id="e1ac9-226">指示是否要在设备上启用启动器源。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-226">Indicates whether or not you want to enable the launcher feed on the device.</span></span>|
|<span data-ttu-id="e1ac9-227">microsoftLauncherFeedAllowUserModification</span><span class="sxs-lookup"><span data-stu-id="e1ac9-227">microsoftLauncherFeedAllowUserModification</span></span>|<span data-ttu-id="e1ac9-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ac9-228">Boolean</span></span>|<span data-ttu-id="e1ac9-229">指示用户是否可以修改设备上的启动器源。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-229">Indicates whether or not the user can modify the launcher feed on the device.</span></span>|
|<span data-ttu-id="e1ac9-230">microsoftLauncherDockPresenceConfiguration</span><span class="sxs-lookup"><span data-stu-id="e1ac9-230">microsoftLauncherDockPresenceConfiguration</span></span>|[<span data-ttu-id="e1ac9-231">microsoftLauncherDockPresence</span><span class="sxs-lookup"><span data-stu-id="e1ac9-231">microsoftLauncherDockPresence</span></span>](../resources/intune-deviceconfig-microsoftlauncherdockpresence.md)|<span data-ttu-id="e1ac9-232">指示是否要配置设备停靠。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-232">Indicates whether or not you want to configure the device dock.</span></span> <span data-ttu-id="e1ac9-233">可取值为：`notConfigured`、`show`、`hide`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-233">Possible values are: `notConfigured`, `show`, `hide`, `disabled`.</span></span>|
|<span data-ttu-id="e1ac9-234">microsoftLauncherDockPresenceAllowUserModification</span><span class="sxs-lookup"><span data-stu-id="e1ac9-234">microsoftLauncherDockPresenceAllowUserModification</span></span>|<span data-ttu-id="e1ac9-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ac9-235">Boolean</span></span>|<span data-ttu-id="e1ac9-236">指示用户是否可以修改设备上的设备停靠配置。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-236">Indicates whether or not the user can modify the device dock configuration on the device.</span></span>|
|<span data-ttu-id="e1ac9-237">microsoftLauncherSearchBarPlacementConfiguration</span><span class="sxs-lookup"><span data-stu-id="e1ac9-237">microsoftLauncherSearchBarPlacementConfiguration</span></span>|[<span data-ttu-id="e1ac9-238">microsoftLauncherSearchBarPlacement</span><span class="sxs-lookup"><span data-stu-id="e1ac9-238">microsoftLauncherSearchBarPlacement</span></span>](../resources/intune-deviceconfig-microsoftlaunchersearchbarplacement.md)|<span data-ttu-id="e1ac9-239">指示设备上的搜索栏的布局配置。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-239">Indicates the search bar placement configuration on the device.</span></span> <span data-ttu-id="e1ac9-240">可取值为：`notConfigured`、`top`、`bottom`、`hide`。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-240">Possible values are: `notConfigured`, `top`, `bottom`, `hide`.</span></span>|
|<span data-ttu-id="e1ac9-241">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="e1ac9-241">enrollmentProfile</span></span>|[<span data-ttu-id="e1ac9-242">androidDeviceOwnerEnrollmentProfileType</span><span class="sxs-lookup"><span data-stu-id="e1ac9-242">androidDeviceOwnerEnrollmentProfileType</span></span>](../resources/intune-deviceconfig-androiddeviceownerenrollmentprofiletype.md)|<span data-ttu-id="e1ac9-243">指示要配置的注册配置文件。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-243">Indicates which enrollment profile you want to configure.</span></span> <span data-ttu-id="e1ac9-244">可取值为：`notConfigured`、`dedicatedDevice`、`fullyManaged`。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-244">Possible values are: `notConfigured`, `dedicatedDevice`, `fullyManaged`.</span></span>|
|<span data-ttu-id="e1ac9-245">dataRoamingBlocked</span><span class="sxs-lookup"><span data-stu-id="e1ac9-245">dataRoamingBlocked</span></span>|<span data-ttu-id="e1ac9-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ac9-246">Boolean</span></span>|<span data-ttu-id="e1ac9-247">指示是否阻止用户使用数据漫游。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-247">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="e1ac9-248">dateTimeConfigurationBlocked</span><span class="sxs-lookup"><span data-stu-id="e1ac9-248">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="e1ac9-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ac9-249">Boolean</span></span>|<span data-ttu-id="e1ac9-250">指示是否阻止用户手动更改设备上的日期或时间</span><span class="sxs-lookup"><span data-stu-id="e1ac9-250">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="e1ac9-251">factoryResetDeviceAdministratorEmails</span><span class="sxs-lookup"><span data-stu-id="e1ac9-251">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="e1ac9-252">String collection</span><span class="sxs-lookup"><span data-stu-id="e1ac9-252">String collection</span></span>|<span data-ttu-id="e1ac9-253">在设备出厂重置之前，将需要进行身份验证的 Google 帐户电子邮件的列表，然后才能对其进行设置。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-253">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="e1ac9-254">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="e1ac9-254">factoryResetBlocked</span></span>|<span data-ttu-id="e1ac9-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ac9-255">Boolean</span></span>|<span data-ttu-id="e1ac9-256">指示是否禁用了 "设置" 中的 "恢复出厂设置" 选项。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-256">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="e1ac9-257">globalProxy</span><span class="sxs-lookup"><span data-stu-id="e1ac9-257">globalProxy</span></span>|[<span data-ttu-id="e1ac9-258">androidDeviceOwnerGlobalProxy</span><span class="sxs-lookup"><span data-stu-id="e1ac9-258">androidDeviceOwnerGlobalProxy</span></span>](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)|<span data-ttu-id="e1ac9-259">代理是与主机、端口和已排除的主机直接建立的。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-259">Proxy is set up directly with host, port and excluded hosts.</span></span>|
|<span data-ttu-id="e1ac9-260">googleAccountsBlocked</span><span class="sxs-lookup"><span data-stu-id="e1ac9-260">googleAccountsBlocked</span></span>|<span data-ttu-id="e1ac9-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ac9-261">Boolean</span></span>|<span data-ttu-id="e1ac9-262">指示是否将阻止 google 帐户。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-262">Indicates whether or not google accounts will be blocked.</span></span>|
|<span data-ttu-id="e1ac9-263">kioskModeScreenSaverConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="e1ac9-263">kioskModeScreenSaverConfigurationEnabled</span></span>|<span data-ttu-id="e1ac9-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ac9-264">Boolean</span></span>|<span data-ttu-id="e1ac9-265">是否启用屏幕保护程序模式或不启用展台模式。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-265">Whether or not to enable screen saver mode or not in Kiosk Mode.</span></span>|
|<span data-ttu-id="e1ac9-266">kioskModeScreenSaverImageUrl</span><span class="sxs-lookup"><span data-stu-id="e1ac9-266">kioskModeScreenSaverImageUrl</span></span>|<span data-ttu-id="e1ac9-267">String</span><span class="sxs-lookup"><span data-stu-id="e1ac9-267">String</span></span>|<span data-ttu-id="e1ac9-268">将作为展台模式下设备的屏幕保护程序的图像的 URL。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-268">URL for an image that will be the device's screen saver in Kiosk Mode.</span></span>|
|<span data-ttu-id="e1ac9-269">kioskModeScreenSaverDisplayTimeInSeconds</span><span class="sxs-lookup"><span data-stu-id="e1ac9-269">kioskModeScreenSaverDisplayTimeInSeconds</span></span>|<span data-ttu-id="e1ac9-270">Int32</span><span class="sxs-lookup"><span data-stu-id="e1ac9-270">Int32</span></span>|<span data-ttu-id="e1ac9-271">设备将在展台模式下显示屏幕保护程序的秒数。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-271">The number of seconds that the device will display the screen saver for in Kiosk Mode.</span></span> <span data-ttu-id="e1ac9-272">有效值为0至9999999</span><span class="sxs-lookup"><span data-stu-id="e1ac9-272">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="e1ac9-273">kioskModeScreenSaverStartDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="e1ac9-273">kioskModeScreenSaverStartDelayInSeconds</span></span>|<span data-ttu-id="e1ac9-274">Int32</span><span class="sxs-lookup"><span data-stu-id="e1ac9-274">Int32</span></span>|<span data-ttu-id="e1ac9-275">在 Kiosk 模式下显示屏幕保护程序之前设备需要保持非活动状态的秒数。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-275">The number of seconds the device needs to be inactive for before the screen saver is shown in Kiosk Mode.</span></span> <span data-ttu-id="e1ac9-276">有效值为1至9999999</span><span class="sxs-lookup"><span data-stu-id="e1ac9-276">Valid values 1 to 9999999</span></span>|
|<span data-ttu-id="e1ac9-277">kioskModeScreenSaverDetectMediaDisabled</span><span class="sxs-lookup"><span data-stu-id="e1ac9-277">kioskModeScreenSaverDetectMediaDisabled</span></span>|<span data-ttu-id="e1ac9-278">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ac9-278">Boolean</span></span>|<span data-ttu-id="e1ac9-279">如果音频/视频在展台模式下播放，则设备屏幕是否应显示屏幕保护程序。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-279">Whether or not the device screen should show the screen saver if audio/video is playing in Kiosk Mode.</span></span>|
|<span data-ttu-id="e1ac9-280">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="e1ac9-280">kioskModeApps</span></span>|<span data-ttu-id="e1ac9-281">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e1ac9-281">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="e1ac9-282">设备处于展台模式时将显示的托管应用列表。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-282">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="e1ac9-283">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-283">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="e1ac9-284">kioskModeWallpaperUrl</span><span class="sxs-lookup"><span data-stu-id="e1ac9-284">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="e1ac9-285">String</span><span class="sxs-lookup"><span data-stu-id="e1ac9-285">String</span></span>|<span data-ttu-id="e1ac9-286">在设备处于展台模式时用于墙纸的可公开访问图像的 URL。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-286">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="e1ac9-287">kioskModeExitCode</span><span class="sxs-lookup"><span data-stu-id="e1ac9-287">kioskModeExitCode</span></span>|<span data-ttu-id="e1ac9-288">String</span><span class="sxs-lookup"><span data-stu-id="e1ac9-288">String</span></span>|<span data-ttu-id="e1ac9-289">退出代码，以允许用户在设备处于展台模式时从展台模式中进行转义。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-289">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="e1ac9-290">kioskModeVirtualHomeButtonEnabled</span><span class="sxs-lookup"><span data-stu-id="e1ac9-290">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="e1ac9-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ac9-291">Boolean</span></span>|<span data-ttu-id="e1ac9-292">设备处于展台模式时是否显示虚拟 "主页" 按钮。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-292">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="e1ac9-293">kioskModeVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="e1ac9-293">kioskModeVirtualHomeButtonType</span></span>|[<span data-ttu-id="e1ac9-294">androidDeviceOwnerVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="e1ac9-294">androidDeviceOwnerVirtualHomeButtonType</span></span>](../resources/intune-deviceconfig-androiddeviceownervirtualhomebuttontype.md)|<span data-ttu-id="e1ac9-295">指示虚拟 home 按钮是否为向上轻扫主页按钮或浮动主页按钮。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-295">Indicates whether the virtual home button is a swipe up home button or a floating home button.</span></span> <span data-ttu-id="e1ac9-296">可取值为：`notConfigured`、`swipeUp`、`floating`。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-296">Possible values are: `notConfigured`, `swipeUp`, `floating`.</span></span>|
|<span data-ttu-id="e1ac9-297">kioskModeBluetoothConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="e1ac9-297">kioskModeBluetoothConfigurationEnabled</span></span>|<span data-ttu-id="e1ac9-298">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ac9-298">Boolean</span></span>|<span data-ttu-id="e1ac9-299">是否允许用户在展台模式下配置蓝牙设置。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-299">Whether or not to allow a user to configure Bluetooth settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="e1ac9-300">kioskModeWiFiConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="e1ac9-300">kioskModeWiFiConfigurationEnabled</span></span>|<span data-ttu-id="e1ac9-301">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ac9-301">Boolean</span></span>|<span data-ttu-id="e1ac9-302">是否允许用户在展台模式下配置 Wi-fi 设置。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-302">Whether or not to allow a user to configure Wi-Fi settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="e1ac9-303">kioskModeFlashlightConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="e1ac9-303">kioskModeFlashlightConfigurationEnabled</span></span>|<span data-ttu-id="e1ac9-304">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ac9-304">Boolean</span></span>|<span data-ttu-id="e1ac9-305">是否允许用户在展台模式下使用该模式。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-305">Whether or not to allow a user to use the flashlight in Kiosk Mode.</span></span>|
|<span data-ttu-id="e1ac9-306">kioskModeMediaVolumeConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="e1ac9-306">kioskModeMediaVolumeConfigurationEnabled</span></span>|<span data-ttu-id="e1ac9-307">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ac9-307">Boolean</span></span>|<span data-ttu-id="e1ac9-308">是否允许用户在展台模式下更改媒体音量。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-308">Whether or not to allow a user to change the media volume in Kiosk Mode.</span></span>|
|<span data-ttu-id="e1ac9-309">kioskModeShowDeviceInfo</span><span class="sxs-lookup"><span data-stu-id="e1ac9-309">kioskModeShowDeviceInfo</span></span>|<span data-ttu-id="e1ac9-310">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ac9-310">Boolean</span></span>|<span data-ttu-id="e1ac9-311">是否允许用户访问基本设备信息。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-311">Whether or not to allow a user to access basic device information.</span></span>|
|<span data-ttu-id="e1ac9-312">kioskModeManagedSettingsEntryDisabled</span><span class="sxs-lookup"><span data-stu-id="e1ac9-312">kioskModeManagedSettingsEntryDisabled</span></span>|<span data-ttu-id="e1ac9-313">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ac9-313">Boolean</span></span>|<span data-ttu-id="e1ac9-314">是否在展台模式下在托管的主屏幕上显示托管设置入口点。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-314">Whether or not to display the Managed Settings entry point on the managed home screen in Kiosk Mode.</span></span>|
|<span data-ttu-id="e1ac9-315">kioskModeDebugMenuEasyAccessEnabled</span><span class="sxs-lookup"><span data-stu-id="e1ac9-315">kioskModeDebugMenuEasyAccessEnabled</span></span>|<span data-ttu-id="e1ac9-316">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ac9-316">Boolean</span></span>|<span data-ttu-id="e1ac9-317">是否允许用户在展台模式下轻松访问 "调试" 菜单。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-317">Whether or not to allow a user to easy access to the debug menu in Kiosk Mode.</span></span>|
|<span data-ttu-id="e1ac9-318">kioskModeShowAppNotificationBadge</span><span class="sxs-lookup"><span data-stu-id="e1ac9-318">kioskModeShowAppNotificationBadge</span></span>|<span data-ttu-id="e1ac9-319">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ac9-319">Boolean</span></span>|<span data-ttu-id="e1ac9-320">是否在展台模式下显示应用程序通知徽章。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-320">Whether or not to display application notification badges in Kiosk Mode.</span></span>|
|<span data-ttu-id="e1ac9-321">kioskModeScreenOrientation</span><span class="sxs-lookup"><span data-stu-id="e1ac9-321">kioskModeScreenOrientation</span></span>|[<span data-ttu-id="e1ac9-322">androidDeviceOwnerKioskModeScreenOrientation</span><span class="sxs-lookup"><span data-stu-id="e1ac9-322">androidDeviceOwnerKioskModeScreenOrientation</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskmodescreenorientation.md)|<span data-ttu-id="e1ac9-323">在展台模式下管理的主屏幕的屏幕方向配置。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-323">Screen orientation configuration for managed home screen in Kiosk Mode.</span></span> <span data-ttu-id="e1ac9-324">可取值为：`notConfigured`、`portrait`、`landscape`、`autoRotate`。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-324">Possible values are: `notConfigured`, `portrait`, `landscape`, `autoRotate`.</span></span>|
|<span data-ttu-id="e1ac9-325">kioskModeIconSize</span><span class="sxs-lookup"><span data-stu-id="e1ac9-325">kioskModeIconSize</span></span>|[<span data-ttu-id="e1ac9-326">androidDeviceOwnerKioskModeIconSize</span><span class="sxs-lookup"><span data-stu-id="e1ac9-326">androidDeviceOwnerKioskModeIconSize</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskmodeiconsize.md)|<span data-ttu-id="e1ac9-327">在展台模式下，管理的主屏幕的图标大小配置。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-327">Icon size configuration for managed home screen in Kiosk Mode.</span></span> <span data-ttu-id="e1ac9-328">可取值为：`notConfigured`、`smallest`、`small`、`regular`、`large`、`largest`。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-328">Possible values are: `notConfigured`, `smallest`, `small`, `regular`, `large`, `largest`.</span></span>|
|<span data-ttu-id="e1ac9-329">kioskModeFolderIcon</span><span class="sxs-lookup"><span data-stu-id="e1ac9-329">kioskModeFolderIcon</span></span>|[<span data-ttu-id="e1ac9-330">androidDeviceOwnerKioskModeFolderIcon</span><span class="sxs-lookup"><span data-stu-id="e1ac9-330">androidDeviceOwnerKioskModeFolderIcon</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskmodefoldericon.md)|<span data-ttu-id="e1ac9-331">展台模式下的托管主屏幕的文件夹图标配置。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-331">Folder icon configuration for managed home screen in Kiosk Mode.</span></span> <span data-ttu-id="e1ac9-332">可取值为：`notConfigured`、`darkSquare`、`darkCircle`、`lightSquare`、`lightCircle`。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-332">Possible values are: `notConfigured`, `darkSquare`, `darkCircle`, `lightSquare`, `lightCircle`.</span></span>|
|<span data-ttu-id="e1ac9-333">kioskModeWifiAllowedSsids</span><span class="sxs-lookup"><span data-stu-id="e1ac9-333">kioskModeWifiAllowedSsids</span></span>|<span data-ttu-id="e1ac9-334">String collection</span><span class="sxs-lookup"><span data-stu-id="e1ac9-334">String collection</span></span>|<span data-ttu-id="e1ac9-335">可供用户在展台模式下进行配置的受限制的 WIFI Ssid 集。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-335">The restricted set of WIFI SSIDs available for the user to configure in Kiosk Mode.</span></span> <span data-ttu-id="e1ac9-336">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-336">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="e1ac9-337">microphoneForceMute</span><span class="sxs-lookup"><span data-stu-id="e1ac9-337">microphoneForceMute</span></span>|<span data-ttu-id="e1ac9-338">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ac9-338">Boolean</span></span>|<span data-ttu-id="e1ac9-339">指示是否阻止观众在设备上的麦克风。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-339">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="e1ac9-340">networkEscapeHatchAllowed</span><span class="sxs-lookup"><span data-stu-id="e1ac9-340">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="e1ac9-341">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ac9-341">Boolean</span></span>|<span data-ttu-id="e1ac9-342">指示在引导时设备是否允许连接到临时网络连接。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-342">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="e1ac9-343">nfcBlockOutgoingBeam</span><span class="sxs-lookup"><span data-stu-id="e1ac9-343">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="e1ac9-344">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ac9-344">Boolean</span></span>|<span data-ttu-id="e1ac9-345">指示是否阻止 NFC 传出横梁。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-345">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="e1ac9-346">passwordBlockKeyguard</span><span class="sxs-lookup"><span data-stu-id="e1ac9-346">passwordBlockKeyguard</span></span>|<span data-ttu-id="e1ac9-347">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ac9-347">Boolean</span></span>|<span data-ttu-id="e1ac9-348">指示是否禁用 keyguard。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-348">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="e1ac9-349">passwordBlockKeyguardFeatures</span><span class="sxs-lookup"><span data-stu-id="e1ac9-349">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="e1ac9-350">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md)集合</span><span class="sxs-lookup"><span data-stu-id="e1ac9-350">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="e1ac9-351">要阻止的设备 keyguard 功能的列表。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-351">List of device keyguard features to block.</span></span> <span data-ttu-id="e1ac9-352">该集合最多可包含 7 个元素。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-352">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="e1ac9-353">可取值为：`notConfigured`、`camera`、`notifications`、`unredactedNotifications`、`trustAgents`、`fingerprint`、`remoteInput`、`allFeatures`。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-353">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="e1ac9-354">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="e1ac9-354">passwordExpirationDays</span></span>|<span data-ttu-id="e1ac9-355">Int32</span><span class="sxs-lookup"><span data-stu-id="e1ac9-355">Int32</span></span>|<span data-ttu-id="e1ac9-356">指示在密码过期之前可以设置密码的时间量（以秒为单位）以及需要新密码的时间（以秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-356">Indicates the amount of time in seconds that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="e1ac9-357">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-357">Valid values 1 to 365</span></span>|
|<span data-ttu-id="e1ac9-358">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="e1ac9-358">passwordMinimumLength</span></span>|<span data-ttu-id="e1ac9-359">Int32</span><span class="sxs-lookup"><span data-stu-id="e1ac9-359">Int32</span></span>|<span data-ttu-id="e1ac9-360">指示设备上所需密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-360">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="e1ac9-361">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="e1ac9-361">Valid values 4 to 16</span></span>|
|<span data-ttu-id="e1ac9-362">passwordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="e1ac9-362">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="e1ac9-363">Int32</span><span class="sxs-lookup"><span data-stu-id="e1ac9-363">Int32</span></span>|<span data-ttu-id="e1ac9-364">指示设备密码所需的字母字符的最小数量。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-364">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="e1ac9-365">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="e1ac9-365">Valid values 1 to 16</span></span>|
|<span data-ttu-id="e1ac9-366">passwordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="e1ac9-366">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="e1ac9-367">Int32</span><span class="sxs-lookup"><span data-stu-id="e1ac9-367">Int32</span></span>|<span data-ttu-id="e1ac9-368">指示设备密码所需的最小小写字符数。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-368">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="e1ac9-369">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="e1ac9-369">Valid values 1 to 16</span></span>|
|<span data-ttu-id="e1ac9-370">passwordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="e1ac9-370">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="e1ac9-371">Int32</span><span class="sxs-lookup"><span data-stu-id="e1ac9-371">Int32</span></span>|<span data-ttu-id="e1ac9-372">指示设备密码所需的最小非字母字符数。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-372">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="e1ac9-373">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="e1ac9-373">Valid values 1 to 16</span></span>|
|<span data-ttu-id="e1ac9-374">passwordMinimumNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="e1ac9-374">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="e1ac9-375">Int32</span><span class="sxs-lookup"><span data-stu-id="e1ac9-375">Int32</span></span>|<span data-ttu-id="e1ac9-376">指示设备密码所需的最小数字字符数。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-376">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="e1ac9-377">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="e1ac9-377">Valid values 1 to 16</span></span>|
|<span data-ttu-id="e1ac9-378">passwordMinimumSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="e1ac9-378">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="e1ac9-379">Int32</span><span class="sxs-lookup"><span data-stu-id="e1ac9-379">Int32</span></span>|<span data-ttu-id="e1ac9-380">指示设备密码所需的最小符号字符数。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-380">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="e1ac9-381">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="e1ac9-381">Valid values 1 to 16</span></span>|
|<span data-ttu-id="e1ac9-382">passwordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="e1ac9-382">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="e1ac9-383">Int32</span><span class="sxs-lookup"><span data-stu-id="e1ac9-383">Int32</span></span>|<span data-ttu-id="e1ac9-384">指示设备密码所需的最小上限 caseletter 字符数。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-384">Indicates the minimum number of upper caseletter characters required for device password.</span></span> <span data-ttu-id="e1ac9-385">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="e1ac9-385">Valid values 1 to 16</span></span>|
|<span data-ttu-id="e1ac9-386">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="e1ac9-386">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="e1ac9-387">Int32</span><span class="sxs-lookup"><span data-stu-id="e1ac9-387">Int32</span></span>|<span data-ttu-id="e1ac9-388">屏幕超时之前的不活动时间（毫秒）。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-388">Milliseconds of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="e1ac9-389">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="e1ac9-389">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="e1ac9-390">Int32</span><span class="sxs-lookup"><span data-stu-id="e1ac9-390">Int32</span></span>|<span data-ttu-id="e1ac9-391">指示密码历史记录的长度，其中用户将不能输入与历史记录中的任何密码相同的新密码。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-391">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="e1ac9-392">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="e1ac9-392">Valid values 0 to 24</span></span>|
|<span data-ttu-id="e1ac9-393">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="e1ac9-393">passwordRequiredType</span></span>|[<span data-ttu-id="e1ac9-394">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="e1ac9-394">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="e1ac9-395">指示设备上所需的最小密码质量。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-395">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="e1ac9-396">可取值为：`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`customPassword`。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-396">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|
|<span data-ttu-id="e1ac9-397">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="e1ac9-397">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="e1ac9-398">Int32</span><span class="sxs-lookup"><span data-stu-id="e1ac9-398">Int32</span></span>|<span data-ttu-id="e1ac9-399">指示用户在擦除设备之前可以输入不正确密码的次数。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-399">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="e1ac9-400">有效值为 4 至 11</span><span class="sxs-lookup"><span data-stu-id="e1ac9-400">Valid values 4 to 11</span></span>|
|<span data-ttu-id="e1ac9-401">playStoreMode</span><span class="sxs-lookup"><span data-stu-id="e1ac9-401">playStoreMode</span></span>|[<span data-ttu-id="e1ac9-402">androidDeviceOwnerPlayStoreMode</span><span class="sxs-lookup"><span data-stu-id="e1ac9-402">androidDeviceOwnerPlayStoreMode</span></span>](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|<span data-ttu-id="e1ac9-403">指示设备的播放存储模式。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-403">Indicates the Play Store mode of the device.</span></span> <span data-ttu-id="e1ac9-404">可取值为：`notConfigured`、`allowList`、`blockList`。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-404">Possible values are: `notConfigured`, `allowList`, `blockList`.</span></span>|
|<span data-ttu-id="e1ac9-405">safeBootBlocked</span><span class="sxs-lookup"><span data-stu-id="e1ac9-405">safeBootBlocked</span></span>|<span data-ttu-id="e1ac9-406">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ac9-406">Boolean</span></span>|<span data-ttu-id="e1ac9-407">指示是否禁用重新启动设备到安全启动。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-407">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="e1ac9-408">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="e1ac9-408">screenCaptureBlocked</span></span>|<span data-ttu-id="e1ac9-409">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ac9-409">Boolean</span></span>|<span data-ttu-id="e1ac9-410">指示是否禁用获取屏幕截图的功能。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-410">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="e1ac9-411">securityAllowDebuggingFeatures</span><span class="sxs-lookup"><span data-stu-id="e1ac9-411">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="e1ac9-412">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ac9-412">Boolean</span></span>|<span data-ttu-id="e1ac9-413">指示是否阻止用户启用设备上的调试功能。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-413">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="e1ac9-414">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="e1ac9-414">securityRequireVerifyApps</span></span>|<span data-ttu-id="e1ac9-415">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ac9-415">Boolean</span></span>|<span data-ttu-id="e1ac9-416">指示是否需要验证应用。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-416">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="e1ac9-417">statusBarBlocked</span><span class="sxs-lookup"><span data-stu-id="e1ac9-417">statusBarBlocked</span></span>|<span data-ttu-id="e1ac9-418">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ac9-418">Boolean</span></span>|<span data-ttu-id="e1ac9-419">指示是否禁用状态栏，包括通知、快速设置和其他屏幕重叠。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-419">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="e1ac9-420">stayOnModes</span><span class="sxs-lookup"><span data-stu-id="e1ac9-420">stayOnModes</span></span>|<span data-ttu-id="e1ac9-421">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)集合</span><span class="sxs-lookup"><span data-stu-id="e1ac9-421">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="e1ac9-422">设备的显示将保持开机状态的模式列表。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-422">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="e1ac9-423">此集合最多可包含4个元素。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-423">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="e1ac9-424">可取值为：`notConfigured`、`ac`、`usb`、`wireless`。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-424">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="e1ac9-425">storageAllowUsb</span><span class="sxs-lookup"><span data-stu-id="e1ac9-425">storageAllowUsb</span></span>|<span data-ttu-id="e1ac9-426">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ac9-426">Boolean</span></span>|<span data-ttu-id="e1ac9-427">指示是否允许 USB 大容量存储。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-427">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="e1ac9-428">storageBlockExternalMedia</span><span class="sxs-lookup"><span data-stu-id="e1ac9-428">storageBlockExternalMedia</span></span>|<span data-ttu-id="e1ac9-429">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ac9-429">Boolean</span></span>|<span data-ttu-id="e1ac9-430">指示是否阻止外部媒体。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-430">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="e1ac9-431">storageBlockUsbFileTransfer</span><span class="sxs-lookup"><span data-stu-id="e1ac9-431">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="e1ac9-432">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ac9-432">Boolean</span></span>|<span data-ttu-id="e1ac9-433">指示是否阻止 USB 文件传输。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-433">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="e1ac9-434">systemUpdateWindowStartMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="e1ac9-434">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="e1ac9-435">Int32</span><span class="sxs-lookup"><span data-stu-id="e1ac9-435">Int32</span></span>|<span data-ttu-id="e1ac9-436">指示系统更新窗口午夜后启动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-436">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="e1ac9-437">有效值为0至1440</span><span class="sxs-lookup"><span data-stu-id="e1ac9-437">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="e1ac9-438">systemUpdateWindowEndMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="e1ac9-438">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="e1ac9-439">Int32</span><span class="sxs-lookup"><span data-stu-id="e1ac9-439">Int32</span></span>|<span data-ttu-id="e1ac9-440">指示系统更新窗口结束后的分钟数。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-440">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="e1ac9-441">有效值为0至1440</span><span class="sxs-lookup"><span data-stu-id="e1ac9-441">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="e1ac9-442">systemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="e1ac9-442">systemUpdateInstallType</span></span>|[<span data-ttu-id="e1ac9-443">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="e1ac9-443">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="e1ac9-444">系统更新配置的类型。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-444">The type of system update configuration.</span></span> <span data-ttu-id="e1ac9-445">可取值为：`deviceDefault`、`postpone`、`windowed`、`automatic`。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-445">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="e1ac9-446">systemWindowsBlocked</span><span class="sxs-lookup"><span data-stu-id="e1ac9-446">systemWindowsBlocked</span></span>|<span data-ttu-id="e1ac9-447">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ac9-447">Boolean</span></span>|<span data-ttu-id="e1ac9-448">是否阻止 Android 系统提示符窗口，如 toast、电话活动和系统通知。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-448">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="e1ac9-449">usersBlockAdd</span><span class="sxs-lookup"><span data-stu-id="e1ac9-449">usersBlockAdd</span></span>|<span data-ttu-id="e1ac9-450">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ac9-450">Boolean</span></span>|<span data-ttu-id="e1ac9-451">指示是否禁用添加用户和配置文件。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-451">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="e1ac9-452">usersBlockRemove</span><span class="sxs-lookup"><span data-stu-id="e1ac9-452">usersBlockRemove</span></span>|<span data-ttu-id="e1ac9-453">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ac9-453">Boolean</span></span>|<span data-ttu-id="e1ac9-454">指示是否禁用从设备中删除其他用户。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-454">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="e1ac9-455">volumeBlockAdjustment</span><span class="sxs-lookup"><span data-stu-id="e1ac9-455">volumeBlockAdjustment</span></span>|<span data-ttu-id="e1ac9-456">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ac9-456">Boolean</span></span>|<span data-ttu-id="e1ac9-457">指示是否禁用了调整主音量。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-457">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="e1ac9-458">vpnAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="e1ac9-458">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="e1ac9-459">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ac9-459">Boolean</span></span>|<span data-ttu-id="e1ac9-460">如果指定了 always on VPN 包名称，则在断开 VPN 连接时是否锁定网络流量。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-460">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="e1ac9-461">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="e1ac9-461">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="e1ac9-462">String</span><span class="sxs-lookup"><span data-stu-id="e1ac9-462">String</span></span>|<span data-ttu-id="e1ac9-463">将处理永不启用 VPN 连接的应用程序的 Android 应用程序包名称。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-463">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="e1ac9-464">wifiBlockEditConfigurations</span><span class="sxs-lookup"><span data-stu-id="e1ac9-464">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="e1ac9-465">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ac9-465">Boolean</span></span>|<span data-ttu-id="e1ac9-466">指示是否阻止用户编辑 wifi 连接设置。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-466">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="e1ac9-467">wifiBlockEditPolicyDefinedConfigurations</span><span class="sxs-lookup"><span data-stu-id="e1ac9-467">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="e1ac9-468">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ac9-468">Boolean</span></span>|<span data-ttu-id="e1ac9-469">指示是否阻止用户仅编辑策略定义的网络。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-469">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|



## <a name="response"></a><span data-ttu-id="e1ac9-470">响应</span><span class="sxs-lookup"><span data-stu-id="e1ac9-470">Response</span></span>
<span data-ttu-id="e1ac9-471">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-471">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1ac9-472">示例</span><span class="sxs-lookup"><span data-stu-id="e1ac9-472">Example</span></span>

### <a name="request"></a><span data-ttu-id="e1ac9-473">请求</span><span class="sxs-lookup"><span data-stu-id="e1ac9-473">Request</span></span>
<span data-ttu-id="e1ac9-474">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e1ac9-474">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 5359

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
  "wifiBlockEditPolicyDefinedConfigurations": true
}
```

### <a name="response"></a><span data-ttu-id="e1ac9-475">响应</span><span class="sxs-lookup"><span data-stu-id="e1ac9-475">Response</span></span>
<span data-ttu-id="e1ac9-476">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="e1ac9-476">Here is an example of the response.</span></span> <span data-ttu-id="e1ac9-477">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="e1ac9-477">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="e1ac9-478">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="e1ac9-478">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 5531

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
  "wifiBlockEditPolicyDefinedConfigurations": true
}
```



