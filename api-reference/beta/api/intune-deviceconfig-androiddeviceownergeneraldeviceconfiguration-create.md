---
title: 创建 androidDeviceOwnerGeneralDeviceConfiguration
description: 创建新的 androidDeviceOwnerGeneralDeviceConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 06e2bae6e729fa76fef88be33b30b5de0c6cb4fa
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49240934"
---
# <a name="create-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="1a30d-103">创建 androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="1a30d-103">Create androidDeviceOwnerGeneralDeviceConfiguration</span></span>

<span data-ttu-id="1a30d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a30d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1a30d-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1a30d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a30d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1a30d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a30d-107">创建新的 [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1a30d-107">Create a new [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1a30d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="1a30d-108">Prerequisites</span></span>
<span data-ttu-id="1a30d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1a30d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a30d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1a30d-111">Permission type</span></span>|<span data-ttu-id="1a30d-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1a30d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a30d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1a30d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1a30d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a30d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1a30d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1a30d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a30d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a30d-116">Not supported.</span></span>|
|<span data-ttu-id="1a30d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1a30d-117">Application</span></span>|<span data-ttu-id="1a30d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a30d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a30d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1a30d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1a30d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1a30d-120">Request headers</span></span>
|<span data-ttu-id="1a30d-121">标头</span><span class="sxs-lookup"><span data-stu-id="1a30d-121">Header</span></span>|<span data-ttu-id="1a30d-122">值</span><span class="sxs-lookup"><span data-stu-id="1a30d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a30d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a30d-123">Authorization</span></span>|<span data-ttu-id="1a30d-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1a30d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a30d-125">接受</span><span class="sxs-lookup"><span data-stu-id="1a30d-125">Accept</span></span>|<span data-ttu-id="1a30d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1a30d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a30d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1a30d-127">Request body</span></span>
<span data-ttu-id="1a30d-128">在请求正文中，提供 androidDeviceOwnerGeneralDeviceConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1a30d-128">In the request body, supply a JSON representation for the androidDeviceOwnerGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="1a30d-129">下表显示创建 androidDeviceOwnerGeneralDeviceConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1a30d-129">The following table shows the properties that are required when you create the androidDeviceOwnerGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="1a30d-130">属性</span><span class="sxs-lookup"><span data-stu-id="1a30d-130">Property</span></span>|<span data-ttu-id="1a30d-131">类型</span><span class="sxs-lookup"><span data-stu-id="1a30d-131">Type</span></span>|<span data-ttu-id="1a30d-132">说明</span><span class="sxs-lookup"><span data-stu-id="1a30d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a30d-133">id</span><span class="sxs-lookup"><span data-stu-id="1a30d-133">id</span></span>|<span data-ttu-id="1a30d-134">String</span><span class="sxs-lookup"><span data-stu-id="1a30d-134">String</span></span>|<span data-ttu-id="1a30d-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1a30d-135">Key of the entity.</span></span> <span data-ttu-id="1a30d-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a30d-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a30d-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1a30d-137">lastModifiedDateTime</span></span>|<span data-ttu-id="1a30d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a30d-138">DateTimeOffset</span></span>|<span data-ttu-id="1a30d-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1a30d-139">DateTime the object was last modified.</span></span> <span data-ttu-id="1a30d-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a30d-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a30d-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1a30d-141">roleScopeTagIds</span></span>|<span data-ttu-id="1a30d-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="1a30d-142">String collection</span></span>|<span data-ttu-id="1a30d-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="1a30d-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1a30d-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a30d-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a30d-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1a30d-145">supportsScopeTags</span></span>|<span data-ttu-id="1a30d-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-146">Boolean</span></span>|<span data-ttu-id="1a30d-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="1a30d-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1a30d-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="1a30d-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1a30d-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="1a30d-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1a30d-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="1a30d-150">This property is read-only.</span></span> <span data-ttu-id="1a30d-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a30d-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a30d-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1a30d-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="1a30d-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1a30d-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="1a30d-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="1a30d-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="1a30d-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a30d-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a30d-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1a30d-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="1a30d-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1a30d-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="1a30d-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="1a30d-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="1a30d-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a30d-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a30d-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="1a30d-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="1a30d-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="1a30d-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="1a30d-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="1a30d-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="1a30d-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a30d-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a30d-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1a30d-164">createdDateTime</span></span>|<span data-ttu-id="1a30d-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a30d-165">DateTimeOffset</span></span>|<span data-ttu-id="1a30d-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1a30d-166">DateTime the object was created.</span></span> <span data-ttu-id="1a30d-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a30d-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a30d-168">description</span><span class="sxs-lookup"><span data-stu-id="1a30d-168">description</span></span>|<span data-ttu-id="1a30d-169">String</span><span class="sxs-lookup"><span data-stu-id="1a30d-169">String</span></span>|<span data-ttu-id="1a30d-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="1a30d-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1a30d-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a30d-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a30d-172">displayName</span><span class="sxs-lookup"><span data-stu-id="1a30d-172">displayName</span></span>|<span data-ttu-id="1a30d-173">String</span><span class="sxs-lookup"><span data-stu-id="1a30d-173">String</span></span>|<span data-ttu-id="1a30d-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="1a30d-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1a30d-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a30d-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a30d-176">version</span><span class="sxs-lookup"><span data-stu-id="1a30d-176">version</span></span>|<span data-ttu-id="1a30d-177">Int32</span><span class="sxs-lookup"><span data-stu-id="1a30d-177">Int32</span></span>|<span data-ttu-id="1a30d-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="1a30d-178">Version of the device configuration.</span></span> <span data-ttu-id="1a30d-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a30d-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a30d-180">accountsBlockModification</span><span class="sxs-lookup"><span data-stu-id="1a30d-180">accountsBlockModification</span></span>|<span data-ttu-id="1a30d-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-181">Boolean</span></span>|<span data-ttu-id="1a30d-182">指示是否禁用添加或删除帐户。</span><span class="sxs-lookup"><span data-stu-id="1a30d-182">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="1a30d-183">appsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="1a30d-183">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="1a30d-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-184">Boolean</span></span>|<span data-ttu-id="1a30d-185">指示是否允许用户启用 "未知源" 设置。</span><span class="sxs-lookup"><span data-stu-id="1a30d-185">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="1a30d-186">appsAutoUpdatePolicy</span><span class="sxs-lookup"><span data-stu-id="1a30d-186">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="1a30d-187">androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="1a30d-187">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="1a30d-188">指示应用程序自动更新策略的值。</span><span class="sxs-lookup"><span data-stu-id="1a30d-188">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="1a30d-189">可取值为：`notConfigured`、`userChoice`、`never`、`wiFiOnly`、`always`。</span><span class="sxs-lookup"><span data-stu-id="1a30d-189">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="1a30d-190">appsDefaultPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="1a30d-190">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="1a30d-191">androidDeviceOwnerDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="1a30d-191">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="1a30d-192">指示对运行时权限请求的权限策略（如果专门没有为应用程序定义）。</span><span class="sxs-lookup"><span data-stu-id="1a30d-192">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="1a30d-193">可取值为：`deviceDefault`、`prompt`、`autoGrant`、`autoDeny`。</span><span class="sxs-lookup"><span data-stu-id="1a30d-193">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="1a30d-194">appsRecommendSkippingFirstUseHints</span><span class="sxs-lookup"><span data-stu-id="1a30d-194">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="1a30d-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-195">Boolean</span></span>|<span data-ttu-id="1a30d-196">是否建议所有应用都将跳过他们可能已添加的任何首次使用提示。</span><span class="sxs-lookup"><span data-stu-id="1a30d-196">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="1a30d-197">bluetoothBlockConfiguration</span><span class="sxs-lookup"><span data-stu-id="1a30d-197">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="1a30d-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-198">Boolean</span></span>|<span data-ttu-id="1a30d-199">指示是否阻止用户配置蓝牙。</span><span class="sxs-lookup"><span data-stu-id="1a30d-199">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="1a30d-200">bluetoothBlockContactSharing</span><span class="sxs-lookup"><span data-stu-id="1a30d-200">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="1a30d-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-201">Boolean</span></span>|<span data-ttu-id="1a30d-202">指示是否阻止用户通过蓝牙共享联系人。</span><span class="sxs-lookup"><span data-stu-id="1a30d-202">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="1a30d-203">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="1a30d-203">cameraBlocked</span></span>|<span data-ttu-id="1a30d-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-204">Boolean</span></span>|<span data-ttu-id="1a30d-205">指示是否禁用相机的使用。</span><span class="sxs-lookup"><span data-stu-id="1a30d-205">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="1a30d-206">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="1a30d-206">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="1a30d-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-207">Boolean</span></span>|<span data-ttu-id="1a30d-208">指示是否阻止 Wi-Fi 网络共享。</span><span class="sxs-lookup"><span data-stu-id="1a30d-208">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="1a30d-209">certificateCredentialConfigurationDisabled</span><span class="sxs-lookup"><span data-stu-id="1a30d-209">certificateCredentialConfigurationDisabled</span></span>|<span data-ttu-id="1a30d-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-210">Boolean</span></span>|<span data-ttu-id="1a30d-211">指示是否阻止来自任何证书凭据配置的用户。</span><span class="sxs-lookup"><span data-stu-id="1a30d-211">Indicates whether or not to block users from any certificate credential configuration.</span></span>|
|<span data-ttu-id="1a30d-212">microsoftLauncherConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="1a30d-212">microsoftLauncherConfigurationEnabled</span></span>|<span data-ttu-id="1a30d-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-213">Boolean</span></span>|<span data-ttu-id="1a30d-214">指示是否要配置 Microsoft 启动器。</span><span class="sxs-lookup"><span data-stu-id="1a30d-214">Indicates whether or not to you want configure Microsoft Launcher.</span></span>|
|<span data-ttu-id="1a30d-215">microsoftLauncherCustomWallpaperEnabled</span><span class="sxs-lookup"><span data-stu-id="1a30d-215">microsoftLauncherCustomWallpaperEnabled</span></span>|<span data-ttu-id="1a30d-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-216">Boolean</span></span>|<span data-ttu-id="1a30d-217">指示是否在目标设备上配置墙纸。</span><span class="sxs-lookup"><span data-stu-id="1a30d-217">Indicates whether or not to configure the wallpaper on the targeted devices.</span></span>|
|<span data-ttu-id="1a30d-218">microsoftLauncherCustomWallpaperImageUrl</span><span class="sxs-lookup"><span data-stu-id="1a30d-218">microsoftLauncherCustomWallpaperImageUrl</span></span>|<span data-ttu-id="1a30d-219">String</span><span class="sxs-lookup"><span data-stu-id="1a30d-219">String</span></span>|<span data-ttu-id="1a30d-220">指示用作目标设备墙纸的图像文件的 URL。</span><span class="sxs-lookup"><span data-stu-id="1a30d-220">Indicates the URL for the image file to use as the wallpaper on the targeted devices.</span></span>|
|<span data-ttu-id="1a30d-221">microsoftLauncherCustomWallpaperAllowUserModification</span><span class="sxs-lookup"><span data-stu-id="1a30d-221">microsoftLauncherCustomWallpaperAllowUserModification</span></span>|<span data-ttu-id="1a30d-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-222">Boolean</span></span>|<span data-ttu-id="1a30d-223">指示用户是否可以修改墙纸以个性化设置其设备。</span><span class="sxs-lookup"><span data-stu-id="1a30d-223">Indicates whether or not the user can modify the wallpaper to personalize their device.</span></span>|
|<span data-ttu-id="1a30d-224">microsoftLauncherFeedEnabled</span><span class="sxs-lookup"><span data-stu-id="1a30d-224">microsoftLauncherFeedEnabled</span></span>|<span data-ttu-id="1a30d-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-225">Boolean</span></span>|<span data-ttu-id="1a30d-226">指示是否要在设备上启用启动器源。</span><span class="sxs-lookup"><span data-stu-id="1a30d-226">Indicates whether or not you want to enable the launcher feed on the device.</span></span>|
|<span data-ttu-id="1a30d-227">microsoftLauncherFeedAllowUserModification</span><span class="sxs-lookup"><span data-stu-id="1a30d-227">microsoftLauncherFeedAllowUserModification</span></span>|<span data-ttu-id="1a30d-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-228">Boolean</span></span>|<span data-ttu-id="1a30d-229">指示用户是否可以修改设备上的启动器源。</span><span class="sxs-lookup"><span data-stu-id="1a30d-229">Indicates whether or not the user can modify the launcher feed on the device.</span></span>|
|<span data-ttu-id="1a30d-230">microsoftLauncherDockPresenceConfiguration</span><span class="sxs-lookup"><span data-stu-id="1a30d-230">microsoftLauncherDockPresenceConfiguration</span></span>|[<span data-ttu-id="1a30d-231">microsoftLauncherDockPresence</span><span class="sxs-lookup"><span data-stu-id="1a30d-231">microsoftLauncherDockPresence</span></span>](../resources/intune-deviceconfig-microsoftlauncherdockpresence.md)|<span data-ttu-id="1a30d-232">指示是否要配置设备停靠。</span><span class="sxs-lookup"><span data-stu-id="1a30d-232">Indicates whether or not you want to configure the device dock.</span></span> <span data-ttu-id="1a30d-233">可取值为：`notConfigured`、`show`、`hide`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="1a30d-233">Possible values are: `notConfigured`, `show`, `hide`, `disabled`.</span></span>|
|<span data-ttu-id="1a30d-234">microsoftLauncherDockPresenceAllowUserModification</span><span class="sxs-lookup"><span data-stu-id="1a30d-234">microsoftLauncherDockPresenceAllowUserModification</span></span>|<span data-ttu-id="1a30d-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-235">Boolean</span></span>|<span data-ttu-id="1a30d-236">指示用户是否可以修改设备上的设备停靠配置。</span><span class="sxs-lookup"><span data-stu-id="1a30d-236">Indicates whether or not the user can modify the device dock configuration on the device.</span></span>|
|<span data-ttu-id="1a30d-237">microsoftLauncherSearchBarPlacementConfiguration</span><span class="sxs-lookup"><span data-stu-id="1a30d-237">microsoftLauncherSearchBarPlacementConfiguration</span></span>|[<span data-ttu-id="1a30d-238">microsoftLauncherSearchBarPlacement</span><span class="sxs-lookup"><span data-stu-id="1a30d-238">microsoftLauncherSearchBarPlacement</span></span>](../resources/intune-deviceconfig-microsoftlaunchersearchbarplacement.md)|<span data-ttu-id="1a30d-239">指示设备上的搜索栏的布局配置。</span><span class="sxs-lookup"><span data-stu-id="1a30d-239">Indicates the search bar placement configuration on the device.</span></span> <span data-ttu-id="1a30d-240">可取值为：`notConfigured`、`top`、`bottom`、`hide`。</span><span class="sxs-lookup"><span data-stu-id="1a30d-240">Possible values are: `notConfigured`, `top`, `bottom`, `hide`.</span></span>|
|<span data-ttu-id="1a30d-241">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="1a30d-241">enrollmentProfile</span></span>|[<span data-ttu-id="1a30d-242">androidDeviceOwnerEnrollmentProfileType</span><span class="sxs-lookup"><span data-stu-id="1a30d-242">androidDeviceOwnerEnrollmentProfileType</span></span>](../resources/intune-deviceconfig-androiddeviceownerenrollmentprofiletype.md)|<span data-ttu-id="1a30d-243">指示要配置的注册配置文件。</span><span class="sxs-lookup"><span data-stu-id="1a30d-243">Indicates which enrollment profile you want to configure.</span></span> <span data-ttu-id="1a30d-244">可取值为：`notConfigured`、`dedicatedDevice`、`fullyManaged`。</span><span class="sxs-lookup"><span data-stu-id="1a30d-244">Possible values are: `notConfigured`, `dedicatedDevice`, `fullyManaged`.</span></span>|
|<span data-ttu-id="1a30d-245">dataRoamingBlocked</span><span class="sxs-lookup"><span data-stu-id="1a30d-245">dataRoamingBlocked</span></span>|<span data-ttu-id="1a30d-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-246">Boolean</span></span>|<span data-ttu-id="1a30d-247">指示是否阻止用户使用数据漫游。</span><span class="sxs-lookup"><span data-stu-id="1a30d-247">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="1a30d-248">dateTimeConfigurationBlocked</span><span class="sxs-lookup"><span data-stu-id="1a30d-248">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="1a30d-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-249">Boolean</span></span>|<span data-ttu-id="1a30d-250">指示是否阻止用户手动更改设备上的日期或时间</span><span class="sxs-lookup"><span data-stu-id="1a30d-250">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="1a30d-251">factoryResetDeviceAdministratorEmails</span><span class="sxs-lookup"><span data-stu-id="1a30d-251">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="1a30d-252">String 集合</span><span class="sxs-lookup"><span data-stu-id="1a30d-252">String collection</span></span>|<span data-ttu-id="1a30d-253">在设备出厂重置之前，将需要进行身份验证的 Google 帐户电子邮件的列表，然后才能对其进行设置。</span><span class="sxs-lookup"><span data-stu-id="1a30d-253">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="1a30d-254">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="1a30d-254">factoryResetBlocked</span></span>|<span data-ttu-id="1a30d-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-255">Boolean</span></span>|<span data-ttu-id="1a30d-256">指示是否禁用了 "设置" 中的 "恢复出厂设置" 选项。</span><span class="sxs-lookup"><span data-stu-id="1a30d-256">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="1a30d-257">globalProxy</span><span class="sxs-lookup"><span data-stu-id="1a30d-257">globalProxy</span></span>|[<span data-ttu-id="1a30d-258">androidDeviceOwnerGlobalProxy</span><span class="sxs-lookup"><span data-stu-id="1a30d-258">androidDeviceOwnerGlobalProxy</span></span>](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)|<span data-ttu-id="1a30d-259">代理是与主机、端口和已排除的主机直接建立的。</span><span class="sxs-lookup"><span data-stu-id="1a30d-259">Proxy is set up directly with host, port and excluded hosts.</span></span>|
|<span data-ttu-id="1a30d-260">googleAccountsBlocked</span><span class="sxs-lookup"><span data-stu-id="1a30d-260">googleAccountsBlocked</span></span>|<span data-ttu-id="1a30d-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-261">Boolean</span></span>|<span data-ttu-id="1a30d-262">指示是否将阻止 google 帐户。</span><span class="sxs-lookup"><span data-stu-id="1a30d-262">Indicates whether or not google accounts will be blocked.</span></span>|
|<span data-ttu-id="1a30d-263">kioskCustomizationDeviceSettingsBlocked</span><span class="sxs-lookup"><span data-stu-id="1a30d-263">kioskCustomizationDeviceSettingsBlocked</span></span>|<span data-ttu-id="1a30d-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-264">Boolean</span></span>|<span data-ttu-id="1a30d-265">指示用户是否可以在展台模式下访问设备的 "设置" 应用程序。</span><span class="sxs-lookup"><span data-stu-id="1a30d-265">Indicates whether a user can access the device's Settings app while in Kiosk Mode.</span></span>|
|<span data-ttu-id="1a30d-266">kioskCustomizationPowerButtonActionsBlocked</span><span class="sxs-lookup"><span data-stu-id="1a30d-266">kioskCustomizationPowerButtonActionsBlocked</span></span>|<span data-ttu-id="1a30d-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-267">Boolean</span></span>|<span data-ttu-id="1a30d-268">用户长按展台模式下设备的电源按钮时是否显示电源菜单。</span><span class="sxs-lookup"><span data-stu-id="1a30d-268">Whether the power menu is shown when a user long presses the Power button of a device in Kiosk Mode.</span></span>|
|<span data-ttu-id="1a30d-269">kioskCustomizationStatusBar</span><span class="sxs-lookup"><span data-stu-id="1a30d-269">kioskCustomizationStatusBar</span></span>|[<span data-ttu-id="1a30d-270">androidDeviceOwnerKioskCustomizationStatusBar</span><span class="sxs-lookup"><span data-stu-id="1a30d-270">androidDeviceOwnerKioskCustomizationStatusBar</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskcustomizationstatusbar.md)|<span data-ttu-id="1a30d-271">指示是否在展台模式下禁用系统信息和通知。</span><span class="sxs-lookup"><span data-stu-id="1a30d-271">Indicates whether system info and notifications are disabled in Kiosk Mode.</span></span> <span data-ttu-id="1a30d-272">可取值为：`notConfigured`、`notificationsAndSystemInfoEnabled`、`systemInfoOnly`。</span><span class="sxs-lookup"><span data-stu-id="1a30d-272">Possible values are: `notConfigured`, `notificationsAndSystemInfoEnabled`, `systemInfoOnly`.</span></span>|
|<span data-ttu-id="1a30d-273">kioskCustomizationSystemErrorWarnings</span><span class="sxs-lookup"><span data-stu-id="1a30d-273">kioskCustomizationSystemErrorWarnings</span></span>|<span data-ttu-id="1a30d-274">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-274">Boolean</span></span>|<span data-ttu-id="1a30d-275">指示在展台模式下是否显示崩溃的或未响应的应用程序的系统错误对话框。</span><span class="sxs-lookup"><span data-stu-id="1a30d-275">Indicates whether system error dialogs for crashed or unresponsive apps are shown in Kiosk Mode.</span></span>|
|<span data-ttu-id="1a30d-276">kioskCustomizationSystemNavigation</span><span class="sxs-lookup"><span data-stu-id="1a30d-276">kioskCustomizationSystemNavigation</span></span>|[<span data-ttu-id="1a30d-277">androidDeviceOwnerKioskCustomizationSystemNavigation</span><span class="sxs-lookup"><span data-stu-id="1a30d-277">androidDeviceOwnerKioskCustomizationSystemNavigation</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskcustomizationsystemnavigation.md)|<span data-ttu-id="1a30d-278">指示在展台模式下启用的导航功能。</span><span class="sxs-lookup"><span data-stu-id="1a30d-278">Indicates which navigation features are enabled in Kiosk Mode.</span></span> <span data-ttu-id="1a30d-279">可取值为：`notConfigured`、`navigationEnabled`、`homeButtonOnly`。</span><span class="sxs-lookup"><span data-stu-id="1a30d-279">Possible values are: `notConfigured`, `navigationEnabled`, `homeButtonOnly`.</span></span>|
|<span data-ttu-id="1a30d-280">kioskModeScreenSaverConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="1a30d-280">kioskModeScreenSaverConfigurationEnabled</span></span>|<span data-ttu-id="1a30d-281">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-281">Boolean</span></span>|<span data-ttu-id="1a30d-282">是否启用屏幕保护程序模式或不启用展台模式。</span><span class="sxs-lookup"><span data-stu-id="1a30d-282">Whether or not to enable screen saver mode or not in Kiosk Mode.</span></span>|
|<span data-ttu-id="1a30d-283">kioskModeScreenSaverImageUrl</span><span class="sxs-lookup"><span data-stu-id="1a30d-283">kioskModeScreenSaverImageUrl</span></span>|<span data-ttu-id="1a30d-284">String</span><span class="sxs-lookup"><span data-stu-id="1a30d-284">String</span></span>|<span data-ttu-id="1a30d-285">将作为展台模式下设备的屏幕保护程序的图像的 URL。</span><span class="sxs-lookup"><span data-stu-id="1a30d-285">URL for an image that will be the device's screen saver in Kiosk Mode.</span></span>|
|<span data-ttu-id="1a30d-286">kioskModeScreenSaverDisplayTimeInSeconds</span><span class="sxs-lookup"><span data-stu-id="1a30d-286">kioskModeScreenSaverDisplayTimeInSeconds</span></span>|<span data-ttu-id="1a30d-287">Int32</span><span class="sxs-lookup"><span data-stu-id="1a30d-287">Int32</span></span>|<span data-ttu-id="1a30d-288">设备将在展台模式下显示屏幕保护程序的秒数。</span><span class="sxs-lookup"><span data-stu-id="1a30d-288">The number of seconds that the device will display the screen saver for in Kiosk Mode.</span></span> <span data-ttu-id="1a30d-289">有效值为0至9999999</span><span class="sxs-lookup"><span data-stu-id="1a30d-289">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="1a30d-290">kioskModeScreenSaverStartDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="1a30d-290">kioskModeScreenSaverStartDelayInSeconds</span></span>|<span data-ttu-id="1a30d-291">Int32</span><span class="sxs-lookup"><span data-stu-id="1a30d-291">Int32</span></span>|<span data-ttu-id="1a30d-292">在 Kiosk 模式下显示屏幕保护程序之前设备需要保持非活动状态的秒数。</span><span class="sxs-lookup"><span data-stu-id="1a30d-292">The number of seconds the device needs to be inactive for before the screen saver is shown in Kiosk Mode.</span></span> <span data-ttu-id="1a30d-293">有效值为1至9999999</span><span class="sxs-lookup"><span data-stu-id="1a30d-293">Valid values 1 to 9999999</span></span>|
|<span data-ttu-id="1a30d-294">kioskModeScreenSaverDetectMediaDisabled</span><span class="sxs-lookup"><span data-stu-id="1a30d-294">kioskModeScreenSaverDetectMediaDisabled</span></span>|<span data-ttu-id="1a30d-295">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-295">Boolean</span></span>|<span data-ttu-id="1a30d-296">如果音频/视频在展台模式下播放，则设备屏幕是否应显示屏幕保护程序。</span><span class="sxs-lookup"><span data-stu-id="1a30d-296">Whether or not the device screen should show the screen saver if audio/video is playing in Kiosk Mode.</span></span>|
|<span data-ttu-id="1a30d-297">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="1a30d-297">kioskModeApps</span></span>|<span data-ttu-id="1a30d-298">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1a30d-298">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="1a30d-299">设备处于展台模式时将显示的托管应用列表。</span><span class="sxs-lookup"><span data-stu-id="1a30d-299">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="1a30d-300">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="1a30d-300">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="1a30d-301">kioskModeWallpaperUrl</span><span class="sxs-lookup"><span data-stu-id="1a30d-301">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="1a30d-302">String</span><span class="sxs-lookup"><span data-stu-id="1a30d-302">String</span></span>|<span data-ttu-id="1a30d-303">在设备处于展台模式时用于墙纸的可公开访问图像的 URL。</span><span class="sxs-lookup"><span data-stu-id="1a30d-303">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="1a30d-304">kioskModeExitCode</span><span class="sxs-lookup"><span data-stu-id="1a30d-304">kioskModeExitCode</span></span>|<span data-ttu-id="1a30d-305">String</span><span class="sxs-lookup"><span data-stu-id="1a30d-305">String</span></span>|<span data-ttu-id="1a30d-306">退出代码，以允许用户在设备处于展台模式时从展台模式中进行转义。</span><span class="sxs-lookup"><span data-stu-id="1a30d-306">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="1a30d-307">kioskModeVirtualHomeButtonEnabled</span><span class="sxs-lookup"><span data-stu-id="1a30d-307">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="1a30d-308">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-308">Boolean</span></span>|<span data-ttu-id="1a30d-309">设备处于展台模式时是否显示虚拟 "主页" 按钮。</span><span class="sxs-lookup"><span data-stu-id="1a30d-309">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="1a30d-310">kioskModeVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="1a30d-310">kioskModeVirtualHomeButtonType</span></span>|[<span data-ttu-id="1a30d-311">androidDeviceOwnerVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="1a30d-311">androidDeviceOwnerVirtualHomeButtonType</span></span>](../resources/intune-deviceconfig-androiddeviceownervirtualhomebuttontype.md)|<span data-ttu-id="1a30d-312">指示虚拟 home 按钮是否为向上轻扫主页按钮或浮动主页按钮。</span><span class="sxs-lookup"><span data-stu-id="1a30d-312">Indicates whether the virtual home button is a swipe up home button or a floating home button.</span></span> <span data-ttu-id="1a30d-313">可取值为：`notConfigured`、`swipeUp`、`floating`。</span><span class="sxs-lookup"><span data-stu-id="1a30d-313">Possible values are: `notConfigured`, `swipeUp`, `floating`.</span></span>|
|<span data-ttu-id="1a30d-314">kioskModeBluetoothConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="1a30d-314">kioskModeBluetoothConfigurationEnabled</span></span>|<span data-ttu-id="1a30d-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-315">Boolean</span></span>|<span data-ttu-id="1a30d-316">是否允许用户在展台模式下配置蓝牙设置。</span><span class="sxs-lookup"><span data-stu-id="1a30d-316">Whether or not to allow a user to configure Bluetooth settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="1a30d-317">kioskModeWiFiConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="1a30d-317">kioskModeWiFiConfigurationEnabled</span></span>|<span data-ttu-id="1a30d-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-318">Boolean</span></span>|<span data-ttu-id="1a30d-319">是否允许用户在展台模式下配置 Wi-Fi 设置。</span><span class="sxs-lookup"><span data-stu-id="1a30d-319">Whether or not to allow a user to configure Wi-Fi settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="1a30d-320">kioskModeFlashlightConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="1a30d-320">kioskModeFlashlightConfigurationEnabled</span></span>|<span data-ttu-id="1a30d-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-321">Boolean</span></span>|<span data-ttu-id="1a30d-322">是否允许用户在展台模式下使用该模式。</span><span class="sxs-lookup"><span data-stu-id="1a30d-322">Whether or not to allow a user to use the flashlight in Kiosk Mode.</span></span>|
|<span data-ttu-id="1a30d-323">kioskModeMediaVolumeConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="1a30d-323">kioskModeMediaVolumeConfigurationEnabled</span></span>|<span data-ttu-id="1a30d-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-324">Boolean</span></span>|<span data-ttu-id="1a30d-325">是否允许用户在展台模式下更改媒体音量。</span><span class="sxs-lookup"><span data-stu-id="1a30d-325">Whether or not to allow a user to change the media volume in Kiosk Mode.</span></span>|
|<span data-ttu-id="1a30d-326">kioskModeShowDeviceInfo</span><span class="sxs-lookup"><span data-stu-id="1a30d-326">kioskModeShowDeviceInfo</span></span>|<span data-ttu-id="1a30d-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-327">Boolean</span></span>|<span data-ttu-id="1a30d-328">是否允许用户访问基本设备信息。</span><span class="sxs-lookup"><span data-stu-id="1a30d-328">Whether or not to allow a user to access basic device information.</span></span>|
|<span data-ttu-id="1a30d-329">kioskModeManagedSettingsEntryDisabled</span><span class="sxs-lookup"><span data-stu-id="1a30d-329">kioskModeManagedSettingsEntryDisabled</span></span>|<span data-ttu-id="1a30d-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-330">Boolean</span></span>|<span data-ttu-id="1a30d-331">是否在展台模式下在托管的主屏幕上显示托管设置入口点。</span><span class="sxs-lookup"><span data-stu-id="1a30d-331">Whether or not to display the Managed Settings entry point on the managed home screen in Kiosk Mode.</span></span>|
|<span data-ttu-id="1a30d-332">kioskModeDebugMenuEasyAccessEnabled</span><span class="sxs-lookup"><span data-stu-id="1a30d-332">kioskModeDebugMenuEasyAccessEnabled</span></span>|<span data-ttu-id="1a30d-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-333">Boolean</span></span>|<span data-ttu-id="1a30d-334">是否允许用户在展台模式下轻松访问 "调试" 菜单。</span><span class="sxs-lookup"><span data-stu-id="1a30d-334">Whether or not to allow a user to easy access to the debug menu in Kiosk Mode.</span></span>|
|<span data-ttu-id="1a30d-335">kioskModeShowAppNotificationBadge</span><span class="sxs-lookup"><span data-stu-id="1a30d-335">kioskModeShowAppNotificationBadge</span></span>|<span data-ttu-id="1a30d-336">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-336">Boolean</span></span>|<span data-ttu-id="1a30d-337">是否在展台模式下显示应用程序通知徽章。</span><span class="sxs-lookup"><span data-stu-id="1a30d-337">Whether or not to display application notification badges in Kiosk Mode.</span></span>|
|<span data-ttu-id="1a30d-338">kioskModeScreenOrientation</span><span class="sxs-lookup"><span data-stu-id="1a30d-338">kioskModeScreenOrientation</span></span>|[<span data-ttu-id="1a30d-339">androidDeviceOwnerKioskModeScreenOrientation</span><span class="sxs-lookup"><span data-stu-id="1a30d-339">androidDeviceOwnerKioskModeScreenOrientation</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskmodescreenorientation.md)|<span data-ttu-id="1a30d-340">在展台模式下管理的主屏幕的屏幕方向配置。</span><span class="sxs-lookup"><span data-stu-id="1a30d-340">Screen orientation configuration for managed home screen in Kiosk Mode.</span></span> <span data-ttu-id="1a30d-341">可取值为：`notConfigured`、`portrait`、`landscape`、`autoRotate`。</span><span class="sxs-lookup"><span data-stu-id="1a30d-341">Possible values are: `notConfigured`, `portrait`, `landscape`, `autoRotate`.</span></span>|
|<span data-ttu-id="1a30d-342">kioskModeIconSize</span><span class="sxs-lookup"><span data-stu-id="1a30d-342">kioskModeIconSize</span></span>|[<span data-ttu-id="1a30d-343">androidDeviceOwnerKioskModeIconSize</span><span class="sxs-lookup"><span data-stu-id="1a30d-343">androidDeviceOwnerKioskModeIconSize</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskmodeiconsize.md)|<span data-ttu-id="1a30d-344">在展台模式下，管理的主屏幕的图标大小配置。</span><span class="sxs-lookup"><span data-stu-id="1a30d-344">Icon size configuration for managed home screen in Kiosk Mode.</span></span> <span data-ttu-id="1a30d-345">可取值为：`notConfigured`、`smallest`、`small`、`regular`、`large`、`largest`。</span><span class="sxs-lookup"><span data-stu-id="1a30d-345">Possible values are: `notConfigured`, `smallest`, `small`, `regular`, `large`, `largest`.</span></span>|
|<span data-ttu-id="1a30d-346">kioskModeFolderIcon</span><span class="sxs-lookup"><span data-stu-id="1a30d-346">kioskModeFolderIcon</span></span>|[<span data-ttu-id="1a30d-347">androidDeviceOwnerKioskModeFolderIcon</span><span class="sxs-lookup"><span data-stu-id="1a30d-347">androidDeviceOwnerKioskModeFolderIcon</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskmodefoldericon.md)|<span data-ttu-id="1a30d-348">展台模式下的托管主屏幕的文件夹图标配置。</span><span class="sxs-lookup"><span data-stu-id="1a30d-348">Folder icon configuration for managed home screen in Kiosk Mode.</span></span> <span data-ttu-id="1a30d-349">可取值为：`notConfigured`、`darkSquare`、`darkCircle`、`lightSquare`、`lightCircle`。</span><span class="sxs-lookup"><span data-stu-id="1a30d-349">Possible values are: `notConfigured`, `darkSquare`, `darkCircle`, `lightSquare`, `lightCircle`.</span></span>|
|<span data-ttu-id="1a30d-350">kioskModeWifiAllowedSsids</span><span class="sxs-lookup"><span data-stu-id="1a30d-350">kioskModeWifiAllowedSsids</span></span>|<span data-ttu-id="1a30d-351">String 集合</span><span class="sxs-lookup"><span data-stu-id="1a30d-351">String collection</span></span>|<span data-ttu-id="1a30d-352">可供用户在展台模式下进行配置的受限制的 WIFI Ssid 集。</span><span class="sxs-lookup"><span data-stu-id="1a30d-352">The restricted set of WIFI SSIDs available for the user to configure in Kiosk Mode.</span></span> <span data-ttu-id="1a30d-353">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="1a30d-353">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="1a30d-354">microphoneForceMute</span><span class="sxs-lookup"><span data-stu-id="1a30d-354">microphoneForceMute</span></span>|<span data-ttu-id="1a30d-355">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-355">Boolean</span></span>|<span data-ttu-id="1a30d-356">指示是否阻止观众在设备上的麦克风。</span><span class="sxs-lookup"><span data-stu-id="1a30d-356">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="1a30d-357">networkEscapeHatchAllowed</span><span class="sxs-lookup"><span data-stu-id="1a30d-357">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="1a30d-358">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-358">Boolean</span></span>|<span data-ttu-id="1a30d-359">指示在引导时设备是否允许连接到临时网络连接。</span><span class="sxs-lookup"><span data-stu-id="1a30d-359">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="1a30d-360">nfcBlockOutgoingBeam</span><span class="sxs-lookup"><span data-stu-id="1a30d-360">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="1a30d-361">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-361">Boolean</span></span>|<span data-ttu-id="1a30d-362">指示是否阻止 NFC 传出横梁。</span><span class="sxs-lookup"><span data-stu-id="1a30d-362">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="1a30d-363">passwordBlockKeyguard</span><span class="sxs-lookup"><span data-stu-id="1a30d-363">passwordBlockKeyguard</span></span>|<span data-ttu-id="1a30d-364">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-364">Boolean</span></span>|<span data-ttu-id="1a30d-365">指示是否禁用 keyguard。</span><span class="sxs-lookup"><span data-stu-id="1a30d-365">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="1a30d-366">passwordBlockKeyguardFeatures</span><span class="sxs-lookup"><span data-stu-id="1a30d-366">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="1a30d-367">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1a30d-367">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="1a30d-368">要阻止的设备 keyguard 功能的列表。</span><span class="sxs-lookup"><span data-stu-id="1a30d-368">List of device keyguard features to block.</span></span> <span data-ttu-id="1a30d-369">该集合最多可包含 7 个元素。</span><span class="sxs-lookup"><span data-stu-id="1a30d-369">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="1a30d-370">可取值为：`notConfigured`、`camera`、`notifications`、`unredactedNotifications`、`trustAgents`、`fingerprint`、`remoteInput`、`allFeatures`。</span><span class="sxs-lookup"><span data-stu-id="1a30d-370">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="1a30d-371">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="1a30d-371">passwordExpirationDays</span></span>|<span data-ttu-id="1a30d-372">Int32</span><span class="sxs-lookup"><span data-stu-id="1a30d-372">Int32</span></span>|<span data-ttu-id="1a30d-373">指示密码在过期之前可以设置的时间量，并需要新密码。</span><span class="sxs-lookup"><span data-stu-id="1a30d-373">Indicates the amount of time that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="1a30d-374">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="1a30d-374">Valid values 1 to 365</span></span>|
|<span data-ttu-id="1a30d-375">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="1a30d-375">passwordMinimumLength</span></span>|<span data-ttu-id="1a30d-376">Int32</span><span class="sxs-lookup"><span data-stu-id="1a30d-376">Int32</span></span>|<span data-ttu-id="1a30d-377">指示设备上所需密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="1a30d-377">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="1a30d-378">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="1a30d-378">Valid values 4 to 16</span></span>|
|<span data-ttu-id="1a30d-379">passwordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="1a30d-379">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="1a30d-380">Int32</span><span class="sxs-lookup"><span data-stu-id="1a30d-380">Int32</span></span>|<span data-ttu-id="1a30d-381">指示设备密码所需的字母字符的最小数量。</span><span class="sxs-lookup"><span data-stu-id="1a30d-381">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="1a30d-382">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="1a30d-382">Valid values 1 to 16</span></span>|
|<span data-ttu-id="1a30d-383">passwordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="1a30d-383">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="1a30d-384">Int32</span><span class="sxs-lookup"><span data-stu-id="1a30d-384">Int32</span></span>|<span data-ttu-id="1a30d-385">指示设备密码所需的最小小写字符数。</span><span class="sxs-lookup"><span data-stu-id="1a30d-385">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="1a30d-386">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="1a30d-386">Valid values 1 to 16</span></span>|
|<span data-ttu-id="1a30d-387">passwordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="1a30d-387">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="1a30d-388">Int32</span><span class="sxs-lookup"><span data-stu-id="1a30d-388">Int32</span></span>|<span data-ttu-id="1a30d-389">指示设备密码所需的最小非字母字符数。</span><span class="sxs-lookup"><span data-stu-id="1a30d-389">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="1a30d-390">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="1a30d-390">Valid values 1 to 16</span></span>|
|<span data-ttu-id="1a30d-391">passwordMinimumNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="1a30d-391">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="1a30d-392">Int32</span><span class="sxs-lookup"><span data-stu-id="1a30d-392">Int32</span></span>|<span data-ttu-id="1a30d-393">指示设备密码所需的最小数字字符数。</span><span class="sxs-lookup"><span data-stu-id="1a30d-393">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="1a30d-394">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="1a30d-394">Valid values 1 to 16</span></span>|
|<span data-ttu-id="1a30d-395">passwordMinimumSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="1a30d-395">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="1a30d-396">Int32</span><span class="sxs-lookup"><span data-stu-id="1a30d-396">Int32</span></span>|<span data-ttu-id="1a30d-397">指示设备密码所需的最小符号字符数。</span><span class="sxs-lookup"><span data-stu-id="1a30d-397">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="1a30d-398">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="1a30d-398">Valid values 1 to 16</span></span>|
|<span data-ttu-id="1a30d-399">passwordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="1a30d-399">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="1a30d-400">Int32</span><span class="sxs-lookup"><span data-stu-id="1a30d-400">Int32</span></span>|<span data-ttu-id="1a30d-401">指示设备密码所需的大写字母字符的最小数量。</span><span class="sxs-lookup"><span data-stu-id="1a30d-401">Indicates the minimum number of upper case letter characters required for device password.</span></span> <span data-ttu-id="1a30d-402">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="1a30d-402">Valid values 1 to 16</span></span>|
|<span data-ttu-id="1a30d-403">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="1a30d-403">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="1a30d-404">Int32</span><span class="sxs-lookup"><span data-stu-id="1a30d-404">Int32</span></span>|<span data-ttu-id="1a30d-405">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="1a30d-405">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="1a30d-406">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="1a30d-406">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="1a30d-407">Int32</span><span class="sxs-lookup"><span data-stu-id="1a30d-407">Int32</span></span>|<span data-ttu-id="1a30d-408">指示密码历史记录的长度，其中用户将不能输入与历史记录中的任何密码相同的新密码。</span><span class="sxs-lookup"><span data-stu-id="1a30d-408">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="1a30d-409">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="1a30d-409">Valid values 0 to 24</span></span>|
|<span data-ttu-id="1a30d-410">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="1a30d-410">passwordRequiredType</span></span>|[<span data-ttu-id="1a30d-411">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="1a30d-411">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="1a30d-412">指示设备上所需的最小密码质量。</span><span class="sxs-lookup"><span data-stu-id="1a30d-412">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="1a30d-413">可取值为：`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`customPassword`。</span><span class="sxs-lookup"><span data-stu-id="1a30d-413">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|
|<span data-ttu-id="1a30d-414">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="1a30d-414">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="1a30d-415">Int32</span><span class="sxs-lookup"><span data-stu-id="1a30d-415">Int32</span></span>|<span data-ttu-id="1a30d-416">指示用户在擦除设备之前可以输入不正确密码的次数。</span><span class="sxs-lookup"><span data-stu-id="1a30d-416">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="1a30d-417">有效值为 4 至 11</span><span class="sxs-lookup"><span data-stu-id="1a30d-417">Valid values 4 to 11</span></span>|
|<span data-ttu-id="1a30d-418">playStoreMode</span><span class="sxs-lookup"><span data-stu-id="1a30d-418">playStoreMode</span></span>|[<span data-ttu-id="1a30d-419">androidDeviceOwnerPlayStoreMode</span><span class="sxs-lookup"><span data-stu-id="1a30d-419">androidDeviceOwnerPlayStoreMode</span></span>](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|<span data-ttu-id="1a30d-420">指示设备的播放存储模式。</span><span class="sxs-lookup"><span data-stu-id="1a30d-420">Indicates the Play Store mode of the device.</span></span> <span data-ttu-id="1a30d-421">可取值为：`notConfigured`、`allowList`、`blockList`。</span><span class="sxs-lookup"><span data-stu-id="1a30d-421">Possible values are: `notConfigured`, `allowList`, `blockList`.</span></span>|
|<span data-ttu-id="1a30d-422">safeBootBlocked</span><span class="sxs-lookup"><span data-stu-id="1a30d-422">safeBootBlocked</span></span>|<span data-ttu-id="1a30d-423">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-423">Boolean</span></span>|<span data-ttu-id="1a30d-424">指示是否禁用重新启动设备到安全启动。</span><span class="sxs-lookup"><span data-stu-id="1a30d-424">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="1a30d-425">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="1a30d-425">screenCaptureBlocked</span></span>|<span data-ttu-id="1a30d-426">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-426">Boolean</span></span>|<span data-ttu-id="1a30d-427">指示是否禁用获取屏幕截图的功能。</span><span class="sxs-lookup"><span data-stu-id="1a30d-427">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="1a30d-428">securityAllowDebuggingFeatures</span><span class="sxs-lookup"><span data-stu-id="1a30d-428">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="1a30d-429">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-429">Boolean</span></span>|<span data-ttu-id="1a30d-430">指示是否阻止用户启用设备上的调试功能。</span><span class="sxs-lookup"><span data-stu-id="1a30d-430">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="1a30d-431">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="1a30d-431">securityRequireVerifyApps</span></span>|<span data-ttu-id="1a30d-432">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-432">Boolean</span></span>|<span data-ttu-id="1a30d-433">指示是否需要验证应用。</span><span class="sxs-lookup"><span data-stu-id="1a30d-433">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="1a30d-434">statusBarBlocked</span><span class="sxs-lookup"><span data-stu-id="1a30d-434">statusBarBlocked</span></span>|<span data-ttu-id="1a30d-435">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-435">Boolean</span></span>|<span data-ttu-id="1a30d-436">指示是否禁用状态栏，包括通知、快速设置和其他屏幕重叠。</span><span class="sxs-lookup"><span data-stu-id="1a30d-436">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="1a30d-437">stayOnModes</span><span class="sxs-lookup"><span data-stu-id="1a30d-437">stayOnModes</span></span>|<span data-ttu-id="1a30d-438">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1a30d-438">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="1a30d-439">设备的显示将保持开机状态的模式列表。</span><span class="sxs-lookup"><span data-stu-id="1a30d-439">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="1a30d-440">此集合最多可包含4个元素。</span><span class="sxs-lookup"><span data-stu-id="1a30d-440">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="1a30d-441">可取值为：`notConfigured`、`ac`、`usb`、`wireless`。</span><span class="sxs-lookup"><span data-stu-id="1a30d-441">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="1a30d-442">storageAllowUsb</span><span class="sxs-lookup"><span data-stu-id="1a30d-442">storageAllowUsb</span></span>|<span data-ttu-id="1a30d-443">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-443">Boolean</span></span>|<span data-ttu-id="1a30d-444">指示是否允许 USB 大容量存储。</span><span class="sxs-lookup"><span data-stu-id="1a30d-444">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="1a30d-445">storageBlockExternalMedia</span><span class="sxs-lookup"><span data-stu-id="1a30d-445">storageBlockExternalMedia</span></span>|<span data-ttu-id="1a30d-446">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-446">Boolean</span></span>|<span data-ttu-id="1a30d-447">指示是否阻止外部媒体。</span><span class="sxs-lookup"><span data-stu-id="1a30d-447">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="1a30d-448">storageBlockUsbFileTransfer</span><span class="sxs-lookup"><span data-stu-id="1a30d-448">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="1a30d-449">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-449">Boolean</span></span>|<span data-ttu-id="1a30d-450">指示是否阻止 USB 文件传输。</span><span class="sxs-lookup"><span data-stu-id="1a30d-450">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="1a30d-451">systemUpdateWindowStartMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="1a30d-451">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="1a30d-452">Int32</span><span class="sxs-lookup"><span data-stu-id="1a30d-452">Int32</span></span>|<span data-ttu-id="1a30d-453">指示系统更新窗口午夜后启动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="1a30d-453">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="1a30d-454">有效值为0至1440</span><span class="sxs-lookup"><span data-stu-id="1a30d-454">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="1a30d-455">systemUpdateWindowEndMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="1a30d-455">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="1a30d-456">Int32</span><span class="sxs-lookup"><span data-stu-id="1a30d-456">Int32</span></span>|<span data-ttu-id="1a30d-457">指示系统更新窗口结束后的分钟数。</span><span class="sxs-lookup"><span data-stu-id="1a30d-457">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="1a30d-458">有效值为0至1440</span><span class="sxs-lookup"><span data-stu-id="1a30d-458">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="1a30d-459">systemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="1a30d-459">systemUpdateInstallType</span></span>|[<span data-ttu-id="1a30d-460">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="1a30d-460">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="1a30d-461">系统更新配置的类型。</span><span class="sxs-lookup"><span data-stu-id="1a30d-461">The type of system update configuration.</span></span> <span data-ttu-id="1a30d-462">可取值为：`deviceDefault`、`postpone`、`windowed`、`automatic`。</span><span class="sxs-lookup"><span data-stu-id="1a30d-462">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="1a30d-463">systemWindowsBlocked</span><span class="sxs-lookup"><span data-stu-id="1a30d-463">systemWindowsBlocked</span></span>|<span data-ttu-id="1a30d-464">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-464">Boolean</span></span>|<span data-ttu-id="1a30d-465">是否阻止 Android 系统提示符窗口，如 toast、电话活动和系统通知。</span><span class="sxs-lookup"><span data-stu-id="1a30d-465">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="1a30d-466">usersBlockAdd</span><span class="sxs-lookup"><span data-stu-id="1a30d-466">usersBlockAdd</span></span>|<span data-ttu-id="1a30d-467">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-467">Boolean</span></span>|<span data-ttu-id="1a30d-468">指示是否禁用添加用户和配置文件。</span><span class="sxs-lookup"><span data-stu-id="1a30d-468">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="1a30d-469">usersBlockRemove</span><span class="sxs-lookup"><span data-stu-id="1a30d-469">usersBlockRemove</span></span>|<span data-ttu-id="1a30d-470">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-470">Boolean</span></span>|<span data-ttu-id="1a30d-471">指示是否禁用从设备中删除其他用户。</span><span class="sxs-lookup"><span data-stu-id="1a30d-471">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="1a30d-472">volumeBlockAdjustment</span><span class="sxs-lookup"><span data-stu-id="1a30d-472">volumeBlockAdjustment</span></span>|<span data-ttu-id="1a30d-473">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-473">Boolean</span></span>|<span data-ttu-id="1a30d-474">指示是否禁用了调整主音量。</span><span class="sxs-lookup"><span data-stu-id="1a30d-474">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="1a30d-475">vpnAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="1a30d-475">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="1a30d-476">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-476">Boolean</span></span>|<span data-ttu-id="1a30d-477">如果指定了 always on VPN 包名称，则在断开 VPN 连接时是否锁定网络流量。</span><span class="sxs-lookup"><span data-stu-id="1a30d-477">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="1a30d-478">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="1a30d-478">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="1a30d-479">String</span><span class="sxs-lookup"><span data-stu-id="1a30d-479">String</span></span>|<span data-ttu-id="1a30d-480">将处理永不启用 VPN 连接的应用程序的 Android 应用程序包名称。</span><span class="sxs-lookup"><span data-stu-id="1a30d-480">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="1a30d-481">wifiBlockEditConfigurations</span><span class="sxs-lookup"><span data-stu-id="1a30d-481">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="1a30d-482">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-482">Boolean</span></span>|<span data-ttu-id="1a30d-483">指示是否阻止用户编辑 wifi 连接设置。</span><span class="sxs-lookup"><span data-stu-id="1a30d-483">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="1a30d-484">wifiBlockEditPolicyDefinedConfigurations</span><span class="sxs-lookup"><span data-stu-id="1a30d-484">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="1a30d-485">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-485">Boolean</span></span>|<span data-ttu-id="1a30d-486">指示是否阻止用户仅编辑策略定义的网络。</span><span class="sxs-lookup"><span data-stu-id="1a30d-486">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|
|<span data-ttu-id="1a30d-487">personalProfileAppsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="1a30d-487">personalProfileAppsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="1a30d-488">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-488">Boolean</span></span>|<span data-ttu-id="1a30d-489">指示用户是否可以在个人配置文件上安装来自未知源的应用程序。</span><span class="sxs-lookup"><span data-stu-id="1a30d-489">Indicates whether the user can install apps from unknown sources on the personal profile.</span></span>|
|<span data-ttu-id="1a30d-490">personalProfileCameraBlocked</span><span class="sxs-lookup"><span data-stu-id="1a30d-490">personalProfileCameraBlocked</span></span>|<span data-ttu-id="1a30d-491">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-491">Boolean</span></span>|<span data-ttu-id="1a30d-492">指示是否禁用个人配置文件上的摄像头的使用。</span><span class="sxs-lookup"><span data-stu-id="1a30d-492">Indicates whether to disable the use of the camera on the personal profile.</span></span>|
|<span data-ttu-id="1a30d-493">personalProfileScreenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="1a30d-493">personalProfileScreenCaptureBlocked</span></span>|<span data-ttu-id="1a30d-494">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a30d-494">Boolean</span></span>|<span data-ttu-id="1a30d-495">指示是否禁用在个人配置文件上采用屏幕截图的功能。</span><span class="sxs-lookup"><span data-stu-id="1a30d-495">Indicates whether to disable the capability to take screenshots on the personal profile.</span></span>|
|<span data-ttu-id="1a30d-496">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="1a30d-496">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="1a30d-497">Int32</span><span class="sxs-lookup"><span data-stu-id="1a30d-497">Int32</span></span>|<span data-ttu-id="1a30d-498">指示工作配置文件密码在过期之前可以设置的天数，并将需要新密码。</span><span class="sxs-lookup"><span data-stu-id="1a30d-498">Indicates the number of days that a work profile password can be set before it expires and a new password will be required.</span></span> <span data-ttu-id="1a30d-499">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="1a30d-499">Valid values 1 to 365</span></span>|
|<span data-ttu-id="1a30d-500">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="1a30d-500">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="1a30d-501">Int32</span><span class="sxs-lookup"><span data-stu-id="1a30d-501">Int32</span></span>|<span data-ttu-id="1a30d-502">指示工作配置文件密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="1a30d-502">Indicates the minimum length of the work profile password.</span></span> <span data-ttu-id="1a30d-503">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="1a30d-503">Valid values 4 to 16</span></span>|
|<span data-ttu-id="1a30d-504">workProfilePasswordMinimumNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="1a30d-504">workProfilePasswordMinimumNumericCharacters</span></span>|<span data-ttu-id="1a30d-505">Int32</span><span class="sxs-lookup"><span data-stu-id="1a30d-505">Int32</span></span>|<span data-ttu-id="1a30d-506">指示工作配置文件密码所需的最小数字字符数。</span><span class="sxs-lookup"><span data-stu-id="1a30d-506">Indicates the minimum number of numeric characters required for the work profile password.</span></span> <span data-ttu-id="1a30d-507">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="1a30d-507">Valid values 1 to 16</span></span>|
|<span data-ttu-id="1a30d-508">workProfilePasswordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="1a30d-508">workProfilePasswordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="1a30d-509">Int32</span><span class="sxs-lookup"><span data-stu-id="1a30d-509">Int32</span></span>|<span data-ttu-id="1a30d-510">指示工作配置文件密码所需的最小非字母字符数。</span><span class="sxs-lookup"><span data-stu-id="1a30d-510">Indicates the minimum number of non-letter characters required for the work profile password.</span></span> <span data-ttu-id="1a30d-511">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="1a30d-511">Valid values 1 to 16</span></span>|
|<span data-ttu-id="1a30d-512">workProfilePasswordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="1a30d-512">workProfilePasswordMinimumLetterCharacters</span></span>|<span data-ttu-id="1a30d-513">Int32</span><span class="sxs-lookup"><span data-stu-id="1a30d-513">Int32</span></span>|<span data-ttu-id="1a30d-514">指示工作配置文件密码所需的字母字符的最小数量。</span><span class="sxs-lookup"><span data-stu-id="1a30d-514">Indicates the minimum number of letter characters required for the work profile password.</span></span> <span data-ttu-id="1a30d-515">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="1a30d-515">Valid values 1 to 16</span></span>|
|<span data-ttu-id="1a30d-516">workProfilePasswordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="1a30d-516">workProfilePasswordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="1a30d-517">Int32</span><span class="sxs-lookup"><span data-stu-id="1a30d-517">Int32</span></span>|<span data-ttu-id="1a30d-518">指示工作配置文件密码所需的最小小写字符数。</span><span class="sxs-lookup"><span data-stu-id="1a30d-518">Indicates the minimum number of lower-case characters required for the work profile password.</span></span> <span data-ttu-id="1a30d-519">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="1a30d-519">Valid values 1 to 16</span></span>|
|<span data-ttu-id="1a30d-520">workProfilePasswordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="1a30d-520">workProfilePasswordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="1a30d-521">Int32</span><span class="sxs-lookup"><span data-stu-id="1a30d-521">Int32</span></span>|<span data-ttu-id="1a30d-522">指示工作配置文件密码所需的大写字母字符的最小数量。</span><span class="sxs-lookup"><span data-stu-id="1a30d-522">Indicates the minimum number of upper-case letter characters required for the work profile password.</span></span> <span data-ttu-id="1a30d-523">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="1a30d-523">Valid values 1 to 16</span></span>|
|<span data-ttu-id="1a30d-524">workProfilePasswordMinimumSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="1a30d-524">workProfilePasswordMinimumSymbolCharacters</span></span>|<span data-ttu-id="1a30d-525">Int32</span><span class="sxs-lookup"><span data-stu-id="1a30d-525">Int32</span></span>|<span data-ttu-id="1a30d-526">指示工作配置文件密码所需的最小符号字符数。</span><span class="sxs-lookup"><span data-stu-id="1a30d-526">Indicates the minimum number of symbol characters required for the work profile password.</span></span> <span data-ttu-id="1a30d-527">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="1a30d-527">Valid values 1 to 16</span></span>|
|<span data-ttu-id="1a30d-528">workProfilePasswordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="1a30d-528">workProfilePasswordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="1a30d-529">Int32</span><span class="sxs-lookup"><span data-stu-id="1a30d-529">Int32</span></span>|<span data-ttu-id="1a30d-530">指示工作配置文件密码历史记录的长度，其中用户将不能输入与历史记录中的任何密码相同的新密码。</span><span class="sxs-lookup"><span data-stu-id="1a30d-530">Indicates the length of the work profile password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="1a30d-531">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="1a30d-531">Valid values 0 to 24</span></span>|
|<span data-ttu-id="1a30d-532">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="1a30d-532">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="1a30d-533">Int32</span><span class="sxs-lookup"><span data-stu-id="1a30d-533">Int32</span></span>|<span data-ttu-id="1a30d-534">指示用户在擦除设备之前可以输入不正确的工作配置文件密码的次数。</span><span class="sxs-lookup"><span data-stu-id="1a30d-534">Indicates the number of times a user can enter an incorrect work profile password before the device is wiped.</span></span> <span data-ttu-id="1a30d-535">有效值为 4 至 11</span><span class="sxs-lookup"><span data-stu-id="1a30d-535">Valid values 4 to 11</span></span>|
|<span data-ttu-id="1a30d-536">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="1a30d-536">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="1a30d-537">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="1a30d-537">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="1a30d-538">指示工作配置文件密码所需的最小密码质量。</span><span class="sxs-lookup"><span data-stu-id="1a30d-538">Indicates the minimum password quality required on the work profile password.</span></span> <span data-ttu-id="1a30d-539">可取值为：`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`customPassword`。</span><span class="sxs-lookup"><span data-stu-id="1a30d-539">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|



## <a name="response"></a><span data-ttu-id="1a30d-540">响应</span><span class="sxs-lookup"><span data-stu-id="1a30d-540">Response</span></span>
<span data-ttu-id="1a30d-541">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1a30d-541">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a30d-542">示例</span><span class="sxs-lookup"><span data-stu-id="1a30d-542">Example</span></span>

### <a name="request"></a><span data-ttu-id="1a30d-543">请求</span><span class="sxs-lookup"><span data-stu-id="1a30d-543">Request</span></span>
<span data-ttu-id="1a30d-544">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1a30d-544">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="1a30d-545">响应</span><span class="sxs-lookup"><span data-stu-id="1a30d-545">Response</span></span>
<span data-ttu-id="1a30d-p156">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1a30d-p156">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




