---
title: 创建 androidDeviceOwnerGeneralDeviceConfiguration
description: 创建新的 androidDeviceOwnerGeneralDeviceConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6ab466aca2100d4151ceedee5f95931014cebd28
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43350758"
---
# <a name="create-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="85e97-103">创建 androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="85e97-103">Create androidDeviceOwnerGeneralDeviceConfiguration</span></span>

<span data-ttu-id="85e97-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85e97-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="85e97-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="85e97-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="85e97-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="85e97-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85e97-107">创建新的[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="85e97-107">Create a new [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="85e97-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="85e97-108">Prerequisites</span></span>
<span data-ttu-id="85e97-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="85e97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85e97-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="85e97-111">Permission type</span></span>|<span data-ttu-id="85e97-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="85e97-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85e97-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="85e97-113">Delegated (work or school account)</span></span>|<span data-ttu-id="85e97-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85e97-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="85e97-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="85e97-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85e97-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="85e97-116">Not supported.</span></span>|
|<span data-ttu-id="85e97-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="85e97-117">Application</span></span>|<span data-ttu-id="85e97-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85e97-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="85e97-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="85e97-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="85e97-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="85e97-120">Request headers</span></span>
|<span data-ttu-id="85e97-121">标头</span><span class="sxs-lookup"><span data-stu-id="85e97-121">Header</span></span>|<span data-ttu-id="85e97-122">值</span><span class="sxs-lookup"><span data-stu-id="85e97-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85e97-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="85e97-123">Authorization</span></span>|<span data-ttu-id="85e97-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="85e97-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85e97-125">接受</span><span class="sxs-lookup"><span data-stu-id="85e97-125">Accept</span></span>|<span data-ttu-id="85e97-126">application/json</span><span class="sxs-lookup"><span data-stu-id="85e97-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85e97-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="85e97-127">Request body</span></span>
<span data-ttu-id="85e97-128">在请求正文中，提供 androidDeviceOwnerGeneralDeviceConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="85e97-128">In the request body, supply a JSON representation for the androidDeviceOwnerGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="85e97-129">下表显示创建 androidDeviceOwnerGeneralDeviceConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="85e97-129">The following table shows the properties that are required when you create the androidDeviceOwnerGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="85e97-130">属性</span><span class="sxs-lookup"><span data-stu-id="85e97-130">Property</span></span>|<span data-ttu-id="85e97-131">类型</span><span class="sxs-lookup"><span data-stu-id="85e97-131">Type</span></span>|<span data-ttu-id="85e97-132">说明</span><span class="sxs-lookup"><span data-stu-id="85e97-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85e97-133">id</span><span class="sxs-lookup"><span data-stu-id="85e97-133">id</span></span>|<span data-ttu-id="85e97-134">字符串</span><span class="sxs-lookup"><span data-stu-id="85e97-134">String</span></span>|<span data-ttu-id="85e97-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="85e97-135">Key of the entity.</span></span> <span data-ttu-id="85e97-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85e97-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85e97-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="85e97-137">lastModifiedDateTime</span></span>|<span data-ttu-id="85e97-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85e97-138">DateTimeOffset</span></span>|<span data-ttu-id="85e97-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="85e97-139">DateTime the object was last modified.</span></span> <span data-ttu-id="85e97-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85e97-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85e97-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="85e97-141">roleScopeTagIds</span></span>|<span data-ttu-id="85e97-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="85e97-142">String collection</span></span>|<span data-ttu-id="85e97-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="85e97-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="85e97-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85e97-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85e97-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="85e97-145">supportsScopeTags</span></span>|<span data-ttu-id="85e97-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="85e97-146">Boolean</span></span>|<span data-ttu-id="85e97-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="85e97-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="85e97-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="85e97-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="85e97-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="85e97-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="85e97-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="85e97-150">This property is read-only.</span></span> <span data-ttu-id="85e97-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85e97-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85e97-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="85e97-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="85e97-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="85e97-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="85e97-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="85e97-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="85e97-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85e97-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85e97-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="85e97-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="85e97-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="85e97-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="85e97-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="85e97-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="85e97-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85e97-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85e97-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="85e97-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="85e97-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="85e97-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="85e97-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="85e97-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="85e97-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85e97-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85e97-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="85e97-164">createdDateTime</span></span>|<span data-ttu-id="85e97-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85e97-165">DateTimeOffset</span></span>|<span data-ttu-id="85e97-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="85e97-166">DateTime the object was created.</span></span> <span data-ttu-id="85e97-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85e97-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85e97-168">description</span><span class="sxs-lookup"><span data-stu-id="85e97-168">description</span></span>|<span data-ttu-id="85e97-169">String</span><span class="sxs-lookup"><span data-stu-id="85e97-169">String</span></span>|<span data-ttu-id="85e97-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="85e97-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="85e97-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85e97-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85e97-172">displayName</span><span class="sxs-lookup"><span data-stu-id="85e97-172">displayName</span></span>|<span data-ttu-id="85e97-173">String</span><span class="sxs-lookup"><span data-stu-id="85e97-173">String</span></span>|<span data-ttu-id="85e97-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="85e97-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="85e97-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85e97-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85e97-176">version</span><span class="sxs-lookup"><span data-stu-id="85e97-176">version</span></span>|<span data-ttu-id="85e97-177">Int32</span><span class="sxs-lookup"><span data-stu-id="85e97-177">Int32</span></span>|<span data-ttu-id="85e97-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="85e97-178">Version of the device configuration.</span></span> <span data-ttu-id="85e97-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85e97-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85e97-180">accountsBlockModification</span><span class="sxs-lookup"><span data-stu-id="85e97-180">accountsBlockModification</span></span>|<span data-ttu-id="85e97-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="85e97-181">Boolean</span></span>|<span data-ttu-id="85e97-182">指示是否禁用添加或删除帐户。</span><span class="sxs-lookup"><span data-stu-id="85e97-182">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="85e97-183">appsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="85e97-183">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="85e97-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="85e97-184">Boolean</span></span>|<span data-ttu-id="85e97-185">指示是否允许用户启用 "未知源" 设置。</span><span class="sxs-lookup"><span data-stu-id="85e97-185">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="85e97-186">appsAutoUpdatePolicy</span><span class="sxs-lookup"><span data-stu-id="85e97-186">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="85e97-187">androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="85e97-187">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="85e97-188">指示应用程序自动更新策略的值。</span><span class="sxs-lookup"><span data-stu-id="85e97-188">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="85e97-189">可取值为：`notConfigured`、`userChoice`、`never`、`wiFiOnly`、`always`。</span><span class="sxs-lookup"><span data-stu-id="85e97-189">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="85e97-190">appsDefaultPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="85e97-190">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="85e97-191">androidDeviceOwnerDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="85e97-191">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="85e97-192">指示对运行时权限请求的权限策略（如果专门没有为应用程序定义）。</span><span class="sxs-lookup"><span data-stu-id="85e97-192">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="85e97-193">可取值为：`deviceDefault`、`prompt`、`autoGrant`、`autoDeny`。</span><span class="sxs-lookup"><span data-stu-id="85e97-193">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="85e97-194">appsRecommendSkippingFirstUseHints</span><span class="sxs-lookup"><span data-stu-id="85e97-194">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="85e97-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="85e97-195">Boolean</span></span>|<span data-ttu-id="85e97-196">是否建议所有应用都将跳过他们可能已添加的任何首次使用提示。</span><span class="sxs-lookup"><span data-stu-id="85e97-196">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="85e97-197">bluetoothBlockConfiguration</span><span class="sxs-lookup"><span data-stu-id="85e97-197">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="85e97-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="85e97-198">Boolean</span></span>|<span data-ttu-id="85e97-199">指示是否阻止用户配置蓝牙。</span><span class="sxs-lookup"><span data-stu-id="85e97-199">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="85e97-200">bluetoothBlockContactSharing</span><span class="sxs-lookup"><span data-stu-id="85e97-200">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="85e97-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="85e97-201">Boolean</span></span>|<span data-ttu-id="85e97-202">指示是否阻止用户通过蓝牙共享联系人。</span><span class="sxs-lookup"><span data-stu-id="85e97-202">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="85e97-203">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="85e97-203">cameraBlocked</span></span>|<span data-ttu-id="85e97-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="85e97-204">Boolean</span></span>|<span data-ttu-id="85e97-205">指示是否禁用相机的使用。</span><span class="sxs-lookup"><span data-stu-id="85e97-205">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="85e97-206">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="85e97-206">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="85e97-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="85e97-207">Boolean</span></span>|<span data-ttu-id="85e97-208">指示是否阻止 Wi-Fi 网络共享。</span><span class="sxs-lookup"><span data-stu-id="85e97-208">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="85e97-209">certificateCredentialConfigurationDisabled</span><span class="sxs-lookup"><span data-stu-id="85e97-209">certificateCredentialConfigurationDisabled</span></span>|<span data-ttu-id="85e97-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="85e97-210">Boolean</span></span>|<span data-ttu-id="85e97-211">指示是否阻止来自任何证书凭据配置的用户。</span><span class="sxs-lookup"><span data-stu-id="85e97-211">Indicates whether or not to block users from any certificate credential configuration.</span></span>|
|<span data-ttu-id="85e97-212">dataRoamingBlocked</span><span class="sxs-lookup"><span data-stu-id="85e97-212">dataRoamingBlocked</span></span>|<span data-ttu-id="85e97-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="85e97-213">Boolean</span></span>|<span data-ttu-id="85e97-214">指示是否阻止用户使用数据漫游。</span><span class="sxs-lookup"><span data-stu-id="85e97-214">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="85e97-215">dateTimeConfigurationBlocked</span><span class="sxs-lookup"><span data-stu-id="85e97-215">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="85e97-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="85e97-216">Boolean</span></span>|<span data-ttu-id="85e97-217">指示是否阻止用户手动更改设备上的日期或时间</span><span class="sxs-lookup"><span data-stu-id="85e97-217">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="85e97-218">factoryResetDeviceAdministratorEmails</span><span class="sxs-lookup"><span data-stu-id="85e97-218">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="85e97-219">String 集合</span><span class="sxs-lookup"><span data-stu-id="85e97-219">String collection</span></span>|<span data-ttu-id="85e97-220">在设备出厂重置之前，将需要进行身份验证的 Google 帐户电子邮件的列表，然后才能对其进行设置。</span><span class="sxs-lookup"><span data-stu-id="85e97-220">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="85e97-221">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="85e97-221">factoryResetBlocked</span></span>|<span data-ttu-id="85e97-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="85e97-222">Boolean</span></span>|<span data-ttu-id="85e97-223">指示是否禁用了 "设置" 中的 "恢复出厂设置" 选项。</span><span class="sxs-lookup"><span data-stu-id="85e97-223">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="85e97-224">globalProxy</span><span class="sxs-lookup"><span data-stu-id="85e97-224">globalProxy</span></span>|[<span data-ttu-id="85e97-225">androidDeviceOwnerGlobalProxy</span><span class="sxs-lookup"><span data-stu-id="85e97-225">androidDeviceOwnerGlobalProxy</span></span>](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)|<span data-ttu-id="85e97-226">代理是与主机、端口和已排除的主机直接建立的。</span><span class="sxs-lookup"><span data-stu-id="85e97-226">Proxy is set up directly with host, port and excluded hosts.</span></span>|
|<span data-ttu-id="85e97-227">googleAccountsBlocked</span><span class="sxs-lookup"><span data-stu-id="85e97-227">googleAccountsBlocked</span></span>|<span data-ttu-id="85e97-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="85e97-228">Boolean</span></span>|<span data-ttu-id="85e97-229">指示是否将阻止 google 帐户。</span><span class="sxs-lookup"><span data-stu-id="85e97-229">Indicates whether or not google accounts will be blocked.</span></span>|
|<span data-ttu-id="85e97-230">kioskModeScreenSaverConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="85e97-230">kioskModeScreenSaverConfigurationEnabled</span></span>|<span data-ttu-id="85e97-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="85e97-231">Boolean</span></span>|<span data-ttu-id="85e97-232">是否启用屏幕保护程序模式或不启用展台模式。</span><span class="sxs-lookup"><span data-stu-id="85e97-232">Whether or not to enable screen saver mode or not in Kiosk Mode.</span></span>|
|<span data-ttu-id="85e97-233">kioskModeScreenSaverImageUrl</span><span class="sxs-lookup"><span data-stu-id="85e97-233">kioskModeScreenSaverImageUrl</span></span>|<span data-ttu-id="85e97-234">字符串</span><span class="sxs-lookup"><span data-stu-id="85e97-234">String</span></span>|<span data-ttu-id="85e97-235">将作为展台模式下设备的屏幕保护程序的图像的 URL。</span><span class="sxs-lookup"><span data-stu-id="85e97-235">URL for an image that will be the device's screen saver in Kiosk Mode.</span></span>|
|<span data-ttu-id="85e97-236">kioskModeScreenSaverDisplayTimeInSeconds</span><span class="sxs-lookup"><span data-stu-id="85e97-236">kioskModeScreenSaverDisplayTimeInSeconds</span></span>|<span data-ttu-id="85e97-237">Int32</span><span class="sxs-lookup"><span data-stu-id="85e97-237">Int32</span></span>|<span data-ttu-id="85e97-238">设备将在展台模式下显示屏幕保护程序的秒数。</span><span class="sxs-lookup"><span data-stu-id="85e97-238">The number of seconds that the device will display the screen saver for in Kiosk Mode.</span></span> <span data-ttu-id="85e97-239">有效值为0至9999999</span><span class="sxs-lookup"><span data-stu-id="85e97-239">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="85e97-240">kioskModeScreenSaverStartDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="85e97-240">kioskModeScreenSaverStartDelayInSeconds</span></span>|<span data-ttu-id="85e97-241">Int32</span><span class="sxs-lookup"><span data-stu-id="85e97-241">Int32</span></span>|<span data-ttu-id="85e97-242">在 Kiosk 模式下显示屏幕保护程序之前设备需要保持非活动状态的秒数。</span><span class="sxs-lookup"><span data-stu-id="85e97-242">The number of seconds the device needs to be inactive for before the screen saver is shown in Kiosk Mode.</span></span> <span data-ttu-id="85e97-243">有效值为1至9999999</span><span class="sxs-lookup"><span data-stu-id="85e97-243">Valid values 1 to 9999999</span></span>|
|<span data-ttu-id="85e97-244">kioskModeScreenSaverDetectMediaDisabled</span><span class="sxs-lookup"><span data-stu-id="85e97-244">kioskModeScreenSaverDetectMediaDisabled</span></span>|<span data-ttu-id="85e97-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="85e97-245">Boolean</span></span>|<span data-ttu-id="85e97-246">如果音频/视频在展台模式下播放，则设备屏幕是否应显示屏幕保护程序。</span><span class="sxs-lookup"><span data-stu-id="85e97-246">Whether or not the device screen should show the screen saver if audio/video is playing in Kiosk Mode.</span></span>|
|<span data-ttu-id="85e97-247">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="85e97-247">kioskModeApps</span></span>|<span data-ttu-id="85e97-248">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="85e97-248">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="85e97-249">设备处于展台模式时将显示的托管应用列表。</span><span class="sxs-lookup"><span data-stu-id="85e97-249">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="85e97-250">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="85e97-250">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="85e97-251">kioskModeWallpaperUrl</span><span class="sxs-lookup"><span data-stu-id="85e97-251">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="85e97-252">字符串</span><span class="sxs-lookup"><span data-stu-id="85e97-252">String</span></span>|<span data-ttu-id="85e97-253">在设备处于展台模式时用于墙纸的可公开访问图像的 URL。</span><span class="sxs-lookup"><span data-stu-id="85e97-253">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="85e97-254">kioskModeExitCode</span><span class="sxs-lookup"><span data-stu-id="85e97-254">kioskModeExitCode</span></span>|<span data-ttu-id="85e97-255">字符串</span><span class="sxs-lookup"><span data-stu-id="85e97-255">String</span></span>|<span data-ttu-id="85e97-256">退出代码，以允许用户在设备处于展台模式时从展台模式中进行转义。</span><span class="sxs-lookup"><span data-stu-id="85e97-256">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="85e97-257">kioskModeVirtualHomeButtonEnabled</span><span class="sxs-lookup"><span data-stu-id="85e97-257">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="85e97-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="85e97-258">Boolean</span></span>|<span data-ttu-id="85e97-259">设备处于展台模式时是否显示虚拟 "主页" 按钮。</span><span class="sxs-lookup"><span data-stu-id="85e97-259">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="85e97-260">kioskModeVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="85e97-260">kioskModeVirtualHomeButtonType</span></span>|[<span data-ttu-id="85e97-261">androidDeviceOwnerVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="85e97-261">androidDeviceOwnerVirtualHomeButtonType</span></span>](../resources/intune-deviceconfig-androiddeviceownervirtualhomebuttontype.md)|<span data-ttu-id="85e97-262">指示虚拟 home 按钮是否为向上轻扫主页按钮或浮动主页按钮。</span><span class="sxs-lookup"><span data-stu-id="85e97-262">Indicates whether the virtual home button is a swipe up home button or a floating home button.</span></span> <span data-ttu-id="85e97-263">可取值为：`notConfigured`、`swipeUp`、`floating`。</span><span class="sxs-lookup"><span data-stu-id="85e97-263">Possible values are: `notConfigured`, `swipeUp`, `floating`.</span></span>|
|<span data-ttu-id="85e97-264">kioskModeBluetoothConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="85e97-264">kioskModeBluetoothConfigurationEnabled</span></span>|<span data-ttu-id="85e97-265">Boolean</span><span class="sxs-lookup"><span data-stu-id="85e97-265">Boolean</span></span>|<span data-ttu-id="85e97-266">是否允许用户在展台模式下配置蓝牙设置。</span><span class="sxs-lookup"><span data-stu-id="85e97-266">Whether or not to allow a user to configure Bluetooth settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="85e97-267">kioskModeWiFiConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="85e97-267">kioskModeWiFiConfigurationEnabled</span></span>|<span data-ttu-id="85e97-268">Boolean</span><span class="sxs-lookup"><span data-stu-id="85e97-268">Boolean</span></span>|<span data-ttu-id="85e97-269">是否允许用户在展台模式下配置 Wi-fi 设置。</span><span class="sxs-lookup"><span data-stu-id="85e97-269">Whether or not to allow a user to configure Wi-Fi settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="85e97-270">kioskModeFlashlightConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="85e97-270">kioskModeFlashlightConfigurationEnabled</span></span>|<span data-ttu-id="85e97-271">Boolean</span><span class="sxs-lookup"><span data-stu-id="85e97-271">Boolean</span></span>|<span data-ttu-id="85e97-272">是否允许用户在展台模式下使用该模式。</span><span class="sxs-lookup"><span data-stu-id="85e97-272">Whether or not to allow a user to use the flashlight in Kiosk Mode.</span></span>|
|<span data-ttu-id="85e97-273">kioskModeMediaVolumeConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="85e97-273">kioskModeMediaVolumeConfigurationEnabled</span></span>|<span data-ttu-id="85e97-274">Boolean</span><span class="sxs-lookup"><span data-stu-id="85e97-274">Boolean</span></span>|<span data-ttu-id="85e97-275">是否允许用户在展台模式下更改媒体音量。</span><span class="sxs-lookup"><span data-stu-id="85e97-275">Whether or not to allow a user to change the media volume in Kiosk Mode.</span></span>|
|<span data-ttu-id="85e97-276">microphoneForceMute</span><span class="sxs-lookup"><span data-stu-id="85e97-276">microphoneForceMute</span></span>|<span data-ttu-id="85e97-277">Boolean</span><span class="sxs-lookup"><span data-stu-id="85e97-277">Boolean</span></span>|<span data-ttu-id="85e97-278">指示是否阻止观众在设备上的麦克风。</span><span class="sxs-lookup"><span data-stu-id="85e97-278">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="85e97-279">networkEscapeHatchAllowed</span><span class="sxs-lookup"><span data-stu-id="85e97-279">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="85e97-280">Boolean</span><span class="sxs-lookup"><span data-stu-id="85e97-280">Boolean</span></span>|<span data-ttu-id="85e97-281">指示在引导时设备是否允许连接到临时网络连接。</span><span class="sxs-lookup"><span data-stu-id="85e97-281">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="85e97-282">nfcBlockOutgoingBeam</span><span class="sxs-lookup"><span data-stu-id="85e97-282">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="85e97-283">Boolean</span><span class="sxs-lookup"><span data-stu-id="85e97-283">Boolean</span></span>|<span data-ttu-id="85e97-284">指示是否阻止 NFC 传出横梁。</span><span class="sxs-lookup"><span data-stu-id="85e97-284">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="85e97-285">passwordBlockKeyguard</span><span class="sxs-lookup"><span data-stu-id="85e97-285">passwordBlockKeyguard</span></span>|<span data-ttu-id="85e97-286">Boolean</span><span class="sxs-lookup"><span data-stu-id="85e97-286">Boolean</span></span>|<span data-ttu-id="85e97-287">指示是否禁用 keyguard。</span><span class="sxs-lookup"><span data-stu-id="85e97-287">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="85e97-288">passwordBlockKeyguardFeatures</span><span class="sxs-lookup"><span data-stu-id="85e97-288">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="85e97-289">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md)集合</span><span class="sxs-lookup"><span data-stu-id="85e97-289">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="85e97-290">要阻止的设备 keyguard 功能的列表。</span><span class="sxs-lookup"><span data-stu-id="85e97-290">List of device keyguard features to block.</span></span> <span data-ttu-id="85e97-291">该集合最多可包含 7 个元素。</span><span class="sxs-lookup"><span data-stu-id="85e97-291">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="85e97-292">可取值为：`notConfigured`、`camera`、`notifications`、`unredactedNotifications`、`trustAgents`、`fingerprint`、`remoteInput`、`allFeatures`。</span><span class="sxs-lookup"><span data-stu-id="85e97-292">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="85e97-293">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="85e97-293">passwordExpirationDays</span></span>|<span data-ttu-id="85e97-294">Int32</span><span class="sxs-lookup"><span data-stu-id="85e97-294">Int32</span></span>|<span data-ttu-id="85e97-295">指示在密码过期之前可以设置密码的时间量（以秒为单位）以及需要新密码的时间（以秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="85e97-295">Indicates the amount of time in seconds that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="85e97-296">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="85e97-296">Valid values 1 to 365</span></span>|
|<span data-ttu-id="85e97-297">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="85e97-297">passwordMinimumLength</span></span>|<span data-ttu-id="85e97-298">Int32</span><span class="sxs-lookup"><span data-stu-id="85e97-298">Int32</span></span>|<span data-ttu-id="85e97-299">指示设备上所需密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="85e97-299">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="85e97-300">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="85e97-300">Valid values 4 to 16</span></span>|
|<span data-ttu-id="85e97-301">passwordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="85e97-301">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="85e97-302">Int32</span><span class="sxs-lookup"><span data-stu-id="85e97-302">Int32</span></span>|<span data-ttu-id="85e97-303">指示设备密码所需的字母字符的最小数量。</span><span class="sxs-lookup"><span data-stu-id="85e97-303">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="85e97-304">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="85e97-304">Valid values 1 to 16</span></span>|
|<span data-ttu-id="85e97-305">passwordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="85e97-305">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="85e97-306">Int32</span><span class="sxs-lookup"><span data-stu-id="85e97-306">Int32</span></span>|<span data-ttu-id="85e97-307">指示设备密码所需的最小小写字符数。</span><span class="sxs-lookup"><span data-stu-id="85e97-307">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="85e97-308">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="85e97-308">Valid values 1 to 16</span></span>|
|<span data-ttu-id="85e97-309">passwordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="85e97-309">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="85e97-310">Int32</span><span class="sxs-lookup"><span data-stu-id="85e97-310">Int32</span></span>|<span data-ttu-id="85e97-311">指示设备密码所需的最小非字母字符数。</span><span class="sxs-lookup"><span data-stu-id="85e97-311">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="85e97-312">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="85e97-312">Valid values 1 to 16</span></span>|
|<span data-ttu-id="85e97-313">passwordMinimumNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="85e97-313">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="85e97-314">Int32</span><span class="sxs-lookup"><span data-stu-id="85e97-314">Int32</span></span>|<span data-ttu-id="85e97-315">指示设备密码所需的最小数字字符数。</span><span class="sxs-lookup"><span data-stu-id="85e97-315">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="85e97-316">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="85e97-316">Valid values 1 to 16</span></span>|
|<span data-ttu-id="85e97-317">passwordMinimumSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="85e97-317">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="85e97-318">Int32</span><span class="sxs-lookup"><span data-stu-id="85e97-318">Int32</span></span>|<span data-ttu-id="85e97-319">指示设备密码所需的最小符号字符数。</span><span class="sxs-lookup"><span data-stu-id="85e97-319">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="85e97-320">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="85e97-320">Valid values 1 to 16</span></span>|
|<span data-ttu-id="85e97-321">passwordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="85e97-321">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="85e97-322">Int32</span><span class="sxs-lookup"><span data-stu-id="85e97-322">Int32</span></span>|<span data-ttu-id="85e97-323">指示设备密码所需的最小上限 caseletter 字符数。</span><span class="sxs-lookup"><span data-stu-id="85e97-323">Indicates the minimum number of upper caseletter characters required for device password.</span></span> <span data-ttu-id="85e97-324">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="85e97-324">Valid values 1 to 16</span></span>|
|<span data-ttu-id="85e97-325">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="85e97-325">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="85e97-326">Int32</span><span class="sxs-lookup"><span data-stu-id="85e97-326">Int32</span></span>|<span data-ttu-id="85e97-327">屏幕超时之前的不活动时间（毫秒）。</span><span class="sxs-lookup"><span data-stu-id="85e97-327">Milliseconds of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="85e97-328">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="85e97-328">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="85e97-329">Int32</span><span class="sxs-lookup"><span data-stu-id="85e97-329">Int32</span></span>|<span data-ttu-id="85e97-330">指示密码历史记录的长度，其中用户将不能输入与历史记录中的任何密码相同的新密码。</span><span class="sxs-lookup"><span data-stu-id="85e97-330">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="85e97-331">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="85e97-331">Valid values 0 to 24</span></span>|
|<span data-ttu-id="85e97-332">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="85e97-332">passwordRequiredType</span></span>|[<span data-ttu-id="85e97-333">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="85e97-333">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="85e97-334">指示设备上所需的最小密码质量。</span><span class="sxs-lookup"><span data-stu-id="85e97-334">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="85e97-335">可取值为：`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`customPassword`。</span><span class="sxs-lookup"><span data-stu-id="85e97-335">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|
|<span data-ttu-id="85e97-336">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="85e97-336">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="85e97-337">Int32</span><span class="sxs-lookup"><span data-stu-id="85e97-337">Int32</span></span>|<span data-ttu-id="85e97-338">指示用户在擦除设备之前可以输入不正确密码的次数。</span><span class="sxs-lookup"><span data-stu-id="85e97-338">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="85e97-339">有效值为 4 至 11</span><span class="sxs-lookup"><span data-stu-id="85e97-339">Valid values 4 to 11</span></span>|
|<span data-ttu-id="85e97-340">playStoreMode</span><span class="sxs-lookup"><span data-stu-id="85e97-340">playStoreMode</span></span>|[<span data-ttu-id="85e97-341">androidDeviceOwnerPlayStoreMode</span><span class="sxs-lookup"><span data-stu-id="85e97-341">androidDeviceOwnerPlayStoreMode</span></span>](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|<span data-ttu-id="85e97-342">指示设备的播放存储模式。</span><span class="sxs-lookup"><span data-stu-id="85e97-342">Indicates the Play Store mode of the device.</span></span> <span data-ttu-id="85e97-343">可取值为：`notConfigured`、`allowList`、`blockList`。</span><span class="sxs-lookup"><span data-stu-id="85e97-343">Possible values are: `notConfigured`, `allowList`, `blockList`.</span></span>|
|<span data-ttu-id="85e97-344">safeBootBlocked</span><span class="sxs-lookup"><span data-stu-id="85e97-344">safeBootBlocked</span></span>|<span data-ttu-id="85e97-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="85e97-345">Boolean</span></span>|<span data-ttu-id="85e97-346">指示是否禁用重新启动设备到安全启动。</span><span class="sxs-lookup"><span data-stu-id="85e97-346">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="85e97-347">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="85e97-347">screenCaptureBlocked</span></span>|<span data-ttu-id="85e97-348">Boolean</span><span class="sxs-lookup"><span data-stu-id="85e97-348">Boolean</span></span>|<span data-ttu-id="85e97-349">指示是否禁用获取屏幕截图的功能。</span><span class="sxs-lookup"><span data-stu-id="85e97-349">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="85e97-350">securityAllowDebuggingFeatures</span><span class="sxs-lookup"><span data-stu-id="85e97-350">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="85e97-351">Boolean</span><span class="sxs-lookup"><span data-stu-id="85e97-351">Boolean</span></span>|<span data-ttu-id="85e97-352">指示是否阻止用户启用设备上的调试功能。</span><span class="sxs-lookup"><span data-stu-id="85e97-352">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="85e97-353">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="85e97-353">securityRequireVerifyApps</span></span>|<span data-ttu-id="85e97-354">Boolean</span><span class="sxs-lookup"><span data-stu-id="85e97-354">Boolean</span></span>|<span data-ttu-id="85e97-355">指示是否需要验证应用。</span><span class="sxs-lookup"><span data-stu-id="85e97-355">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="85e97-356">statusBarBlocked</span><span class="sxs-lookup"><span data-stu-id="85e97-356">statusBarBlocked</span></span>|<span data-ttu-id="85e97-357">Boolean</span><span class="sxs-lookup"><span data-stu-id="85e97-357">Boolean</span></span>|<span data-ttu-id="85e97-358">指示是否禁用状态栏，包括通知、快速设置和其他屏幕重叠。</span><span class="sxs-lookup"><span data-stu-id="85e97-358">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="85e97-359">stayOnModes</span><span class="sxs-lookup"><span data-stu-id="85e97-359">stayOnModes</span></span>|<span data-ttu-id="85e97-360">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)集合</span><span class="sxs-lookup"><span data-stu-id="85e97-360">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="85e97-361">设备的显示将保持开机状态的模式列表。</span><span class="sxs-lookup"><span data-stu-id="85e97-361">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="85e97-362">此集合最多可包含4个元素。</span><span class="sxs-lookup"><span data-stu-id="85e97-362">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="85e97-363">可取值为：`notConfigured`、`ac`、`usb`、`wireless`。</span><span class="sxs-lookup"><span data-stu-id="85e97-363">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="85e97-364">storageAllowUsb</span><span class="sxs-lookup"><span data-stu-id="85e97-364">storageAllowUsb</span></span>|<span data-ttu-id="85e97-365">Boolean</span><span class="sxs-lookup"><span data-stu-id="85e97-365">Boolean</span></span>|<span data-ttu-id="85e97-366">指示是否允许 USB 大容量存储。</span><span class="sxs-lookup"><span data-stu-id="85e97-366">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="85e97-367">storageBlockExternalMedia</span><span class="sxs-lookup"><span data-stu-id="85e97-367">storageBlockExternalMedia</span></span>|<span data-ttu-id="85e97-368">Boolean</span><span class="sxs-lookup"><span data-stu-id="85e97-368">Boolean</span></span>|<span data-ttu-id="85e97-369">指示是否阻止外部媒体。</span><span class="sxs-lookup"><span data-stu-id="85e97-369">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="85e97-370">storageBlockUsbFileTransfer</span><span class="sxs-lookup"><span data-stu-id="85e97-370">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="85e97-371">Boolean</span><span class="sxs-lookup"><span data-stu-id="85e97-371">Boolean</span></span>|<span data-ttu-id="85e97-372">指示是否阻止 USB 文件传输。</span><span class="sxs-lookup"><span data-stu-id="85e97-372">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="85e97-373">systemUpdateWindowStartMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="85e97-373">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="85e97-374">Int32</span><span class="sxs-lookup"><span data-stu-id="85e97-374">Int32</span></span>|<span data-ttu-id="85e97-375">指示系统更新窗口午夜后启动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="85e97-375">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="85e97-376">有效值为0至1440</span><span class="sxs-lookup"><span data-stu-id="85e97-376">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="85e97-377">systemUpdateWindowEndMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="85e97-377">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="85e97-378">Int32</span><span class="sxs-lookup"><span data-stu-id="85e97-378">Int32</span></span>|<span data-ttu-id="85e97-379">指示系统更新窗口结束后的分钟数。</span><span class="sxs-lookup"><span data-stu-id="85e97-379">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="85e97-380">有效值为0至1440</span><span class="sxs-lookup"><span data-stu-id="85e97-380">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="85e97-381">systemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="85e97-381">systemUpdateInstallType</span></span>|[<span data-ttu-id="85e97-382">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="85e97-382">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="85e97-383">系统更新配置的类型。</span><span class="sxs-lookup"><span data-stu-id="85e97-383">The type of system update configuration.</span></span> <span data-ttu-id="85e97-384">可取值为：`deviceDefault`、`postpone`、`windowed`、`automatic`。</span><span class="sxs-lookup"><span data-stu-id="85e97-384">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="85e97-385">systemWindowsBlocked</span><span class="sxs-lookup"><span data-stu-id="85e97-385">systemWindowsBlocked</span></span>|<span data-ttu-id="85e97-386">Boolean</span><span class="sxs-lookup"><span data-stu-id="85e97-386">Boolean</span></span>|<span data-ttu-id="85e97-387">是否阻止 Android 系统提示符窗口，如 toast、电话活动和系统通知。</span><span class="sxs-lookup"><span data-stu-id="85e97-387">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="85e97-388">usersBlockAdd</span><span class="sxs-lookup"><span data-stu-id="85e97-388">usersBlockAdd</span></span>|<span data-ttu-id="85e97-389">Boolean</span><span class="sxs-lookup"><span data-stu-id="85e97-389">Boolean</span></span>|<span data-ttu-id="85e97-390">指示是否禁用添加用户和配置文件。</span><span class="sxs-lookup"><span data-stu-id="85e97-390">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="85e97-391">usersBlockRemove</span><span class="sxs-lookup"><span data-stu-id="85e97-391">usersBlockRemove</span></span>|<span data-ttu-id="85e97-392">Boolean</span><span class="sxs-lookup"><span data-stu-id="85e97-392">Boolean</span></span>|<span data-ttu-id="85e97-393">指示是否禁用从设备中删除其他用户。</span><span class="sxs-lookup"><span data-stu-id="85e97-393">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="85e97-394">volumeBlockAdjustment</span><span class="sxs-lookup"><span data-stu-id="85e97-394">volumeBlockAdjustment</span></span>|<span data-ttu-id="85e97-395">Boolean</span><span class="sxs-lookup"><span data-stu-id="85e97-395">Boolean</span></span>|<span data-ttu-id="85e97-396">指示是否禁用了调整主音量。</span><span class="sxs-lookup"><span data-stu-id="85e97-396">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="85e97-397">vpnAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="85e97-397">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="85e97-398">Boolean</span><span class="sxs-lookup"><span data-stu-id="85e97-398">Boolean</span></span>|<span data-ttu-id="85e97-399">如果指定了 always on VPN 包名称，则在断开 VPN 连接时是否锁定网络流量。</span><span class="sxs-lookup"><span data-stu-id="85e97-399">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="85e97-400">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="85e97-400">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="85e97-401">字符串</span><span class="sxs-lookup"><span data-stu-id="85e97-401">String</span></span>|<span data-ttu-id="85e97-402">将处理永不启用 VPN 连接的应用程序的 Android 应用程序包名称。</span><span class="sxs-lookup"><span data-stu-id="85e97-402">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="85e97-403">wifiBlockEditConfigurations</span><span class="sxs-lookup"><span data-stu-id="85e97-403">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="85e97-404">Boolean</span><span class="sxs-lookup"><span data-stu-id="85e97-404">Boolean</span></span>|<span data-ttu-id="85e97-405">指示是否阻止用户编辑 wifi 连接设置。</span><span class="sxs-lookup"><span data-stu-id="85e97-405">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="85e97-406">wifiBlockEditPolicyDefinedConfigurations</span><span class="sxs-lookup"><span data-stu-id="85e97-406">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="85e97-407">Boolean</span><span class="sxs-lookup"><span data-stu-id="85e97-407">Boolean</span></span>|<span data-ttu-id="85e97-408">指示是否阻止用户仅编辑策略定义的网络。</span><span class="sxs-lookup"><span data-stu-id="85e97-408">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|



## <a name="response"></a><span data-ttu-id="85e97-409">响应</span><span class="sxs-lookup"><span data-stu-id="85e97-409">Response</span></span>
<span data-ttu-id="85e97-410">如果成功，此方法在响应`201 Created`正文中返回响应代码和[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="85e97-410">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85e97-411">示例</span><span class="sxs-lookup"><span data-stu-id="85e97-411">Example</span></span>

### <a name="request"></a><span data-ttu-id="85e97-412">请求</span><span class="sxs-lookup"><span data-stu-id="85e97-412">Request</span></span>
<span data-ttu-id="85e97-413">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="85e97-413">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="85e97-414">响应</span><span class="sxs-lookup"><span data-stu-id="85e97-414">Response</span></span>
<span data-ttu-id="85e97-p136">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="85e97-p136">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



