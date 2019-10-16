---
title: 更新 windowsUpdateForBusinessConfiguration
description: 更新 windowsUpdateForBusinessConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 33261dc3283512887c612a3a35ce0400a0aea8e3
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37532160"
---
# <a name="update-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="86ae9-103">更新 windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="86ae9-103">Update windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="86ae9-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="86ae9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86ae9-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="86ae9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86ae9-106">更新 [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="86ae9-106">Update the properties of a [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="86ae9-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="86ae9-107">Prerequisites</span></span>
<span data-ttu-id="86ae9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="86ae9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86ae9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="86ae9-110">Permission type</span></span>|<span data-ttu-id="86ae9-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="86ae9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86ae9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="86ae9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="86ae9-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86ae9-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="86ae9-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="86ae9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86ae9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="86ae9-115">Not supported.</span></span>|
|<span data-ttu-id="86ae9-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="86ae9-116">Application</span></span>|<span data-ttu-id="86ae9-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86ae9-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="86ae9-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="86ae9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="86ae9-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="86ae9-119">Request headers</span></span>
|<span data-ttu-id="86ae9-120">标头</span><span class="sxs-lookup"><span data-stu-id="86ae9-120">Header</span></span>|<span data-ttu-id="86ae9-121">值</span><span class="sxs-lookup"><span data-stu-id="86ae9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86ae9-122">授权</span><span class="sxs-lookup"><span data-stu-id="86ae9-122">Authorization</span></span>|<span data-ttu-id="86ae9-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="86ae9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86ae9-124">接受</span><span class="sxs-lookup"><span data-stu-id="86ae9-124">Accept</span></span>|<span data-ttu-id="86ae9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="86ae9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86ae9-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="86ae9-126">Request body</span></span>
<span data-ttu-id="86ae9-127">在请求正文中，提供 [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="86ae9-127">In the request body, supply a JSON representation for the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="86ae9-128">下表显示创建 [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="86ae9-128">The following table shows the properties that are required when you create the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="86ae9-129">属性</span><span class="sxs-lookup"><span data-stu-id="86ae9-129">Property</span></span>|<span data-ttu-id="86ae9-130">类型</span><span class="sxs-lookup"><span data-stu-id="86ae9-130">Type</span></span>|<span data-ttu-id="86ae9-131">说明</span><span class="sxs-lookup"><span data-stu-id="86ae9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86ae9-132">id</span><span class="sxs-lookup"><span data-stu-id="86ae9-132">id</span></span>|<span data-ttu-id="86ae9-133">字符串</span><span class="sxs-lookup"><span data-stu-id="86ae9-133">String</span></span>|<span data-ttu-id="86ae9-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="86ae9-134">Key of the entity.</span></span> <span data-ttu-id="86ae9-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86ae9-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86ae9-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="86ae9-136">lastModifiedDateTime</span></span>|<span data-ttu-id="86ae9-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86ae9-137">DateTimeOffset</span></span>|<span data-ttu-id="86ae9-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="86ae9-138">DateTime the object was last modified.</span></span> <span data-ttu-id="86ae9-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86ae9-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86ae9-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="86ae9-140">roleScopeTagIds</span></span>|<span data-ttu-id="86ae9-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="86ae9-141">String collection</span></span>|<span data-ttu-id="86ae9-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="86ae9-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="86ae9-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86ae9-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86ae9-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="86ae9-144">supportsScopeTags</span></span>|<span data-ttu-id="86ae9-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="86ae9-145">Boolean</span></span>|<span data-ttu-id="86ae9-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="86ae9-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="86ae9-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="86ae9-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="86ae9-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="86ae9-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="86ae9-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="86ae9-149">This property is read-only.</span></span> <span data-ttu-id="86ae9-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86ae9-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86ae9-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="86ae9-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="86ae9-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="86ae9-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="86ae9-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="86ae9-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="86ae9-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86ae9-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86ae9-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="86ae9-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="86ae9-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="86ae9-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="86ae9-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="86ae9-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="86ae9-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86ae9-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86ae9-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="86ae9-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="86ae9-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="86ae9-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="86ae9-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="86ae9-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="86ae9-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86ae9-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86ae9-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="86ae9-163">createdDateTime</span></span>|<span data-ttu-id="86ae9-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86ae9-164">DateTimeOffset</span></span>|<span data-ttu-id="86ae9-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="86ae9-165">DateTime the object was created.</span></span> <span data-ttu-id="86ae9-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86ae9-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86ae9-167">说明</span><span class="sxs-lookup"><span data-stu-id="86ae9-167">description</span></span>|<span data-ttu-id="86ae9-168">String</span><span class="sxs-lookup"><span data-stu-id="86ae9-168">String</span></span>|<span data-ttu-id="86ae9-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="86ae9-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="86ae9-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86ae9-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86ae9-171">displayName</span><span class="sxs-lookup"><span data-stu-id="86ae9-171">displayName</span></span>|<span data-ttu-id="86ae9-172">String</span><span class="sxs-lookup"><span data-stu-id="86ae9-172">String</span></span>|<span data-ttu-id="86ae9-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="86ae9-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="86ae9-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86ae9-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86ae9-175">version</span><span class="sxs-lookup"><span data-stu-id="86ae9-175">version</span></span>|<span data-ttu-id="86ae9-176">Int32</span><span class="sxs-lookup"><span data-stu-id="86ae9-176">Int32</span></span>|<span data-ttu-id="86ae9-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="86ae9-177">Version of the device configuration.</span></span> <span data-ttu-id="86ae9-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86ae9-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86ae9-179">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="86ae9-179">deliveryOptimizationMode</span></span>|[<span data-ttu-id="86ae9-180">windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="86ae9-180">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="86ae9-181">传递优化模式。</span><span class="sxs-lookup"><span data-stu-id="86ae9-181">Delivery Optimization Mode.</span></span> <span data-ttu-id="86ae9-182">可取值为：`userDefined`、`httpOnly`、`httpWithPeeringNat`、`httpWithPeeringPrivateGroup`、`httpWithInternetPeering`、`simpleDownload` 或 `bypassMode`。</span><span class="sxs-lookup"><span data-stu-id="86ae9-182">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="86ae9-183">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="86ae9-183">prereleaseFeatures</span></span>|[<span data-ttu-id="86ae9-184">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="86ae9-184">prereleaseFeatures</span></span>](../resources/intune-deviceconfig-prereleasefeatures.md)|<span data-ttu-id="86ae9-185">预发布功能。</span><span class="sxs-lookup"><span data-stu-id="86ae9-185">The pre-release features.</span></span> <span data-ttu-id="86ae9-186">可取值为：`userDefined`、`settingsOnly`、`settingsAndExperimentations`、`notAllowed`。</span><span class="sxs-lookup"><span data-stu-id="86ae9-186">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="86ae9-187">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="86ae9-187">automaticUpdateMode</span></span>|[<span data-ttu-id="86ae9-188">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="86ae9-188">automaticUpdateMode</span></span>](../resources/intune-deviceconfig-automaticupdatemode.md)|<span data-ttu-id="86ae9-189">自动更新模式。</span><span class="sxs-lookup"><span data-stu-id="86ae9-189">Automatic update mode.</span></span> <span data-ttu-id="86ae9-190">可取值为：`userDefined`、`notifyDownload`、`autoInstallAtMaintenanceTime`、`autoInstallAndRebootAtMaintenanceTime`、`autoInstallAndRebootAtScheduledTime`、`autoInstallAndRebootWithoutEndUserControl` 或 `windowsDefault`。</span><span class="sxs-lookup"><span data-stu-id="86ae9-190">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`, `windowsDefault`.</span></span>|
|<span data-ttu-id="86ae9-191">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="86ae9-191">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="86ae9-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="86ae9-192">Boolean</span></span>|<span data-ttu-id="86ae9-193">允许 Microsoft 更新服务</span><span class="sxs-lookup"><span data-stu-id="86ae9-193">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="86ae9-194">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="86ae9-194">driversExcluded</span></span>|<span data-ttu-id="86ae9-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="86ae9-195">Boolean</span></span>|<span data-ttu-id="86ae9-196">排除 Windows 更新驱动程序</span><span class="sxs-lookup"><span data-stu-id="86ae9-196">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="86ae9-197">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="86ae9-197">installationSchedule</span></span>|[<span data-ttu-id="86ae9-198">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="86ae9-198">windowsUpdateInstallScheduleType</span></span>](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)|<span data-ttu-id="86ae9-199">安装计划</span><span class="sxs-lookup"><span data-stu-id="86ae9-199">Installation schedule</span></span>|
|<span data-ttu-id="86ae9-200">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="86ae9-200">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="86ae9-201">Int32</span><span class="sxs-lookup"><span data-stu-id="86ae9-201">Int32</span></span>|<span data-ttu-id="86ae9-202">推迟质量更新的天数</span><span class="sxs-lookup"><span data-stu-id="86ae9-202">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="86ae9-203">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="86ae9-203">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="86ae9-204">Int32</span><span class="sxs-lookup"><span data-stu-id="86ae9-204">Int32</span></span>|<span data-ttu-id="86ae9-205">推迟功能更新的天数</span><span class="sxs-lookup"><span data-stu-id="86ae9-205">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="86ae9-206">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="86ae9-206">qualityUpdatesPaused</span></span>|<span data-ttu-id="86ae9-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="86ae9-207">Boolean</span></span>|<span data-ttu-id="86ae9-208">暂停质量更新</span><span class="sxs-lookup"><span data-stu-id="86ae9-208">Pause Quality Updates</span></span>|
|<span data-ttu-id="86ae9-209">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="86ae9-209">featureUpdatesPaused</span></span>|<span data-ttu-id="86ae9-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="86ae9-210">Boolean</span></span>|<span data-ttu-id="86ae9-211">暂停功能更新</span><span class="sxs-lookup"><span data-stu-id="86ae9-211">Pause Feature Updates</span></span>|
|<span data-ttu-id="86ae9-212">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="86ae9-212">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="86ae9-213">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86ae9-213">DateTimeOffset</span></span>|<span data-ttu-id="86ae9-214">质量更新暂停到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="86ae9-214">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="86ae9-215">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="86ae9-215">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="86ae9-216">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86ae9-216">DateTimeOffset</span></span>|<span data-ttu-id="86ae9-217">功能更新暂停到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="86ae9-217">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="86ae9-218">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="86ae9-218">businessReadyUpdatesOnly</span></span>|[<span data-ttu-id="86ae9-219">windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="86ae9-219">windowsUpdateType</span></span>](../resources/intune-deviceconfig-windowsupdatetype.md)|<span data-ttu-id="86ae9-220">确定将从哪些分支设备接收其更新。</span><span class="sxs-lookup"><span data-stu-id="86ae9-220">Determines which branch devices will receive their updates from.</span></span> <span data-ttu-id="86ae9-221">可取值为：`userDefined`、`all`、`businessReadyOnly`、`windowsInsiderBuildFast`、`windowsInsiderBuildSlow`、`windowsInsiderBuildRelease`。</span><span class="sxs-lookup"><span data-stu-id="86ae9-221">Possible values are: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span></span>|
|<span data-ttu-id="86ae9-222">skipChecksBeforeRestart</span><span class="sxs-lookup"><span data-stu-id="86ae9-222">skipChecksBeforeRestart</span></span>|<span data-ttu-id="86ae9-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="86ae9-223">Boolean</span></span>|<span data-ttu-id="86ae9-224">设置为在重新启动之前跳过所有复选：电池级别 = 40%、用户状态、需要显示、演示模式、全屏模式、电话呼叫状态、游戏模式等。</span><span class="sxs-lookup"><span data-stu-id="86ae9-224">Set to skip all check before restart: Battery level = 40%, User presence, Display Needed, Presentation mode, Full screen mode, phone call state, game mode etc.</span></span> |
|<span data-ttu-id="86ae9-225">updateWeeks</span><span class="sxs-lookup"><span data-stu-id="86ae9-225">updateWeeks</span></span>|[<span data-ttu-id="86ae9-226">windowsUpdateForBusinessUpdateWeeks</span><span class="sxs-lookup"><span data-stu-id="86ae9-226">windowsUpdateForBusinessUpdateWeeks</span></span>](../resources/intune-deviceconfig-windowsupdateforbusinessupdateweeks.md)|<span data-ttu-id="86ae9-227">在每月的几周安排更新安装。</span><span class="sxs-lookup"><span data-stu-id="86ae9-227">Scheduled the update installation on the weeks of the month.</span></span> <span data-ttu-id="86ae9-228">可取值为：`userDefined`、`firstWeek`、`secondWeek`、`thirdWeek`、`fourthWeek`、`everyWeek`。</span><span class="sxs-lookup"><span data-stu-id="86ae9-228">Possible values are: `userDefined`, `firstWeek`, `secondWeek`, `thirdWeek`, `fourthWeek`, `everyWeek`.</span></span>|
|<span data-ttu-id="86ae9-229">qualityUpdatesPauseStartDate</span><span class="sxs-lookup"><span data-stu-id="86ae9-229">qualityUpdatesPauseStartDate</span></span>|<span data-ttu-id="86ae9-230">日期</span><span class="sxs-lookup"><span data-stu-id="86ae9-230">Date</span></span>|<span data-ttu-id="86ae9-231">质量更新暂停开始日期。</span><span class="sxs-lookup"><span data-stu-id="86ae9-231">Quality Updates Pause start date.</span></span> <span data-ttu-id="86ae9-232">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="86ae9-232">This property is read-only.</span></span>|
|<span data-ttu-id="86ae9-233">featureUpdatesPauseStartDate</span><span class="sxs-lookup"><span data-stu-id="86ae9-233">featureUpdatesPauseStartDate</span></span>|<span data-ttu-id="86ae9-234">日期</span><span class="sxs-lookup"><span data-stu-id="86ae9-234">Date</span></span>|<span data-ttu-id="86ae9-235">功能更新暂停开始日期。</span><span class="sxs-lookup"><span data-stu-id="86ae9-235">Feature Updates Pause start date.</span></span> <span data-ttu-id="86ae9-236">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="86ae9-236">This property is read-only.</span></span>|
|<span data-ttu-id="86ae9-237">featureUpdatesRollbackWindowInDays</span><span class="sxs-lookup"><span data-stu-id="86ae9-237">featureUpdatesRollbackWindowInDays</span></span>|<span data-ttu-id="86ae9-238">Int32</span><span class="sxs-lookup"><span data-stu-id="86ae9-238">Int32</span></span>|<span data-ttu-id="86ae9-239">回滚对其有效的功能更新后的天数</span><span class="sxs-lookup"><span data-stu-id="86ae9-239">The number of days after a Feature Update for which a rollback is valid</span></span>|
|<span data-ttu-id="86ae9-240">qualityUpdatesWillBeRolledBack</span><span class="sxs-lookup"><span data-stu-id="86ae9-240">qualityUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="86ae9-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="86ae9-241">Boolean</span></span>|<span data-ttu-id="86ae9-242">指定是否在下一个设备签入时回滚质量更新</span><span class="sxs-lookup"><span data-stu-id="86ae9-242">Specifies whether to rollback Quality Updates on the next device check in</span></span>|
|<span data-ttu-id="86ae9-243">featureUpdatesWillBeRolledBack</span><span class="sxs-lookup"><span data-stu-id="86ae9-243">featureUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="86ae9-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="86ae9-244">Boolean</span></span>|<span data-ttu-id="86ae9-245">指定是否在下一个设备签入时回滚功能更新</span><span class="sxs-lookup"><span data-stu-id="86ae9-245">Specifies whether to rollback Feature Updates on the next device check in</span></span>|
|<span data-ttu-id="86ae9-246">qualityUpdatesRollbackStartDateTime</span><span class="sxs-lookup"><span data-stu-id="86ae9-246">qualityUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="86ae9-247">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86ae9-247">DateTimeOffset</span></span>|<span data-ttu-id="86ae9-248">质量更新回滚开始日期/时间</span><span class="sxs-lookup"><span data-stu-id="86ae9-248">Quality Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="86ae9-249">featureUpdatesRollbackStartDateTime</span><span class="sxs-lookup"><span data-stu-id="86ae9-249">featureUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="86ae9-250">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86ae9-250">DateTimeOffset</span></span>|<span data-ttu-id="86ae9-251">功能更新回滚的开始日期时间</span><span class="sxs-lookup"><span data-stu-id="86ae9-251">Feature Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="86ae9-252">engagedRestartDeadlineInDays</span><span class="sxs-lookup"><span data-stu-id="86ae9-252">engagedRestartDeadlineInDays</span></span>|<span data-ttu-id="86ae9-253">Int32</span><span class="sxs-lookup"><span data-stu-id="86ae9-253">Int32</span></span>|<span data-ttu-id="86ae9-254">在非活动时段自动安排和执行挂起的重启的期限（以天为单位），有效范围为2到30天</span><span class="sxs-lookup"><span data-stu-id="86ae9-254">Deadline in days before automatically scheduling and executing a pending restart outside of active hours, with valid range from 2 to 30 days</span></span>|
|<span data-ttu-id="86ae9-255">engagedRestartSnoozeScheduleInDays</span><span class="sxs-lookup"><span data-stu-id="86ae9-255">engagedRestartSnoozeScheduleInDays</span></span>|<span data-ttu-id="86ae9-256">Int32</span><span class="sxs-lookup"><span data-stu-id="86ae9-256">Int32</span></span>|<span data-ttu-id="86ae9-257">用户可推迟预定重启提醒通知的天数，有效范围为1到3天</span><span class="sxs-lookup"><span data-stu-id="86ae9-257">Number of days a user can snooze Engaged Restart reminder notifications with valid range from 1 to 3 days</span></span>|
|<span data-ttu-id="86ae9-258">engagedRestartTransitionScheduleInDays</span><span class="sxs-lookup"><span data-stu-id="86ae9-258">engagedRestartTransitionScheduleInDays</span></span>|<span data-ttu-id="86ae9-259">Int32</span><span class="sxs-lookup"><span data-stu-id="86ae9-259">Int32</span></span>|<span data-ttu-id="86ae9-260">从主动时段之外的计划的自动重启转换为预定重启（需要用户进行计划，有效范围为0到30天）的天数</span><span class="sxs-lookup"><span data-stu-id="86ae9-260">Number of days before transitioning from Auto Restarts scheduled outside of active hours to Engaged Restart, which requires the user to schedule, with valid range from 0 to 30 days</span></span>|
|<span data-ttu-id="86ae9-261">deadlineForFeatureUpdatesInDays</span><span class="sxs-lookup"><span data-stu-id="86ae9-261">deadlineForFeatureUpdatesInDays</span></span>|<span data-ttu-id="86ae9-262">Int32</span><span class="sxs-lookup"><span data-stu-id="86ae9-262">Int32</span></span>|<span data-ttu-id="86ae9-263">自动安装具有介于2到30天的有效范围的功能更新之前的天数</span><span class="sxs-lookup"><span data-stu-id="86ae9-263">Number of days before feature updates are installed automatically with valid range from 2 to 30 days</span></span>|
|<span data-ttu-id="86ae9-264">deadlineForQualityUpdatesInDays</span><span class="sxs-lookup"><span data-stu-id="86ae9-264">deadlineForQualityUpdatesInDays</span></span>|<span data-ttu-id="86ae9-265">Int32</span><span class="sxs-lookup"><span data-stu-id="86ae9-265">Int32</span></span>|<span data-ttu-id="86ae9-266">自动安装质量更新前的天数介于2到30天的有效范围内</span><span class="sxs-lookup"><span data-stu-id="86ae9-266">Number of days before quality updates are installed automatically with valid range from 2 to 30 days</span></span>|
|<span data-ttu-id="86ae9-267">deadlineGracePeriodInDays</span><span class="sxs-lookup"><span data-stu-id="86ae9-267">deadlineGracePeriodInDays</span></span>|<span data-ttu-id="86ae9-268">Int32</span><span class="sxs-lookup"><span data-stu-id="86ae9-268">Int32</span></span>|<span data-ttu-id="86ae9-269">使用有效范围（范围为0到7天）自动重新启动之前的最后期限的天数</span><span class="sxs-lookup"><span data-stu-id="86ae9-269">Number of days after deadline  until restarts occur automatically with valid range from 0 to 7 days</span></span>|
|<span data-ttu-id="86ae9-270">postponeRebootUntilAfterDeadline</span><span class="sxs-lookup"><span data-stu-id="86ae9-270">postponeRebootUntilAfterDeadline</span></span>|<span data-ttu-id="86ae9-271">Boolean</span><span class="sxs-lookup"><span data-stu-id="86ae9-271">Boolean</span></span>|<span data-ttu-id="86ae9-272">指定设备是否应等到最后期限结束后才能在 active 时段之外进行重新启动</span><span class="sxs-lookup"><span data-stu-id="86ae9-272">Specifies if the device should wait until deadline for rebooting outside of active hours</span></span>|
|<span data-ttu-id="86ae9-273">autoRestartNotificationDismissal</span><span class="sxs-lookup"><span data-stu-id="86ae9-273">autoRestartNotificationDismissal</span></span>|[<span data-ttu-id="86ae9-274">autoRestartNotificationDismissalMethod</span><span class="sxs-lookup"><span data-stu-id="86ae9-274">autoRestartNotificationDismissalMethod</span></span>](../resources/intune-deviceconfig-autorestartnotificationdismissalmethod.md)|<span data-ttu-id="86ae9-275">指定用于消除 "需要自动重新启动" 通知的方法。</span><span class="sxs-lookup"><span data-stu-id="86ae9-275">Specify the method by which the auto-restart required notification is dismissed.</span></span> <span data-ttu-id="86ae9-276">可取值为：`notConfigured`、`automatic`、`user`。</span><span class="sxs-lookup"><span data-stu-id="86ae9-276">Possible values are: `notConfigured`, `automatic`, `user`.</span></span>|
|<span data-ttu-id="86ae9-277">scheduleRestartWarningInHours</span><span class="sxs-lookup"><span data-stu-id="86ae9-277">scheduleRestartWarningInHours</span></span>|<span data-ttu-id="86ae9-278">Int32</span><span class="sxs-lookup"><span data-stu-id="86ae9-278">Int32</span></span>|<span data-ttu-id="86ae9-279">指定自动重新启动警告提醒通知的期限。</span><span class="sxs-lookup"><span data-stu-id="86ae9-279">Specify the period for auto-restart warning reminder notifications.</span></span> <span data-ttu-id="86ae9-280">支持的值：2、4、8、12或24（小时）。</span><span class="sxs-lookup"><span data-stu-id="86ae9-280">Supported values: 2, 4, 8, 12 or 24 (hours).</span></span>|
|<span data-ttu-id="86ae9-281">scheduleImminentRestartWarningInMinutes</span><span class="sxs-lookup"><span data-stu-id="86ae9-281">scheduleImminentRestartWarningInMinutes</span></span>|<span data-ttu-id="86ae9-282">Int32</span><span class="sxs-lookup"><span data-stu-id="86ae9-282">Int32</span></span>|<span data-ttu-id="86ae9-283">指定自动重启即将发生的警告通知的期限。</span><span class="sxs-lookup"><span data-stu-id="86ae9-283">Specify the period for auto-restart imminent warning notifications.</span></span> <span data-ttu-id="86ae9-284">支持的值：15、30或60（分钟）。</span><span class="sxs-lookup"><span data-stu-id="86ae9-284">Supported values: 15, 30 or 60 (minutes).</span></span>|
|<span data-ttu-id="86ae9-285">userPauseAccess</span><span class="sxs-lookup"><span data-stu-id="86ae9-285">userPauseAccess</span></span>|[<span data-ttu-id="86ae9-286">启用</span><span class="sxs-lookup"><span data-stu-id="86ae9-286">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="86ae9-287">指定是否允许最终用户访问暂停软件更新。</span><span class="sxs-lookup"><span data-stu-id="86ae9-287">Specifies whether to enable end user’s access to pause software updates.</span></span> <span data-ttu-id="86ae9-288">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="86ae9-288">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="86ae9-289">userWindowsUpdateScanAccess</span><span class="sxs-lookup"><span data-stu-id="86ae9-289">userWindowsUpdateScanAccess</span></span>|[<span data-ttu-id="86ae9-290">启用</span><span class="sxs-lookup"><span data-stu-id="86ae9-290">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="86ae9-291">指定是否禁用用户对扫描 Windows 更新的访问权限。</span><span class="sxs-lookup"><span data-stu-id="86ae9-291">Specifies whether to disable user’s access to scan Windows Update.</span></span> <span data-ttu-id="86ae9-292">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="86ae9-292">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="86ae9-293">updateNotificationLevel</span><span class="sxs-lookup"><span data-stu-id="86ae9-293">updateNotificationLevel</span></span>|[<span data-ttu-id="86ae9-294">windowsUpdateNotificationDisplayOption</span><span class="sxs-lookup"><span data-stu-id="86ae9-294">windowsUpdateNotificationDisplayOption</span></span>](../resources/intune-deviceconfig-windowsupdatenotificationdisplayoption.md)|<span data-ttu-id="86ae9-295">指定用户看到的 Windows 更新通知的具体内容。</span><span class="sxs-lookup"><span data-stu-id="86ae9-295">Specifies what Windows Update notifications users see.</span></span> <span data-ttu-id="86ae9-296">可取值为：`notConfigured`、`defaultNotifications`、`restartWarningsOnly`、`disableAllNotifications`。</span><span class="sxs-lookup"><span data-stu-id="86ae9-296">Possible values are: `notConfigured`, `defaultNotifications`, `restartWarningsOnly`, `disableAllNotifications`.</span></span>|



## <a name="response"></a><span data-ttu-id="86ae9-297">响应</span><span class="sxs-lookup"><span data-stu-id="86ae9-297">Response</span></span>
<span data-ttu-id="86ae9-298">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="86ae9-298">If successful, this method returns a `200 OK` response code and an updated [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86ae9-299">示例</span><span class="sxs-lookup"><span data-stu-id="86ae9-299">Example</span></span>

### <a name="request"></a><span data-ttu-id="86ae9-300">请求</span><span class="sxs-lookup"><span data-stu-id="86ae9-300">Request</span></span>
<span data-ttu-id="86ae9-301">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="86ae9-301">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2840

{
  "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
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
  "deliveryOptimizationMode": "httpOnly",
  "prereleaseFeatures": "settingsOnly",
  "automaticUpdateMode": "notifyDownload",
  "microsoftUpdateServiceAllowed": true,
  "driversExcluded": true,
  "installationSchedule": {
    "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall",
    "scheduledInstallDay": "everyday",
    "scheduledInstallTime": "11:59:31.3170000"
  },
  "qualityUpdatesDeferralPeriodInDays": 2,
  "featureUpdatesDeferralPeriodInDays": 2,
  "qualityUpdatesPaused": true,
  "featureUpdatesPaused": true,
  "qualityUpdatesPauseExpiryDateTime": "2017-01-01T00:00:22.9594683-08:00",
  "featureUpdatesPauseExpiryDateTime": "2016-12-31T23:58:08.068669-08:00",
  "businessReadyUpdatesOnly": "all",
  "skipChecksBeforeRestart": true,
  "updateWeeks": "firstWeek",
  "qualityUpdatesPauseStartDate": "<Unknown Primitive Type Edm.Date>",
  "featureUpdatesPauseStartDate": "<Unknown Primitive Type Edm.Date>",
  "featureUpdatesRollbackWindowInDays": 2,
  "qualityUpdatesWillBeRolledBack": true,
  "featureUpdatesWillBeRolledBack": true,
  "qualityUpdatesRollbackStartDateTime": "2016-12-31T23:57:01.05526-08:00",
  "featureUpdatesRollbackStartDateTime": "2017-01-01T00:03:21.6080517-08:00",
  "engagedRestartDeadlineInDays": 12,
  "engagedRestartSnoozeScheduleInDays": 2,
  "engagedRestartTransitionScheduleInDays": 6,
  "deadlineForFeatureUpdatesInDays": 15,
  "deadlineForQualityUpdatesInDays": 15,
  "deadlineGracePeriodInDays": 9,
  "postponeRebootUntilAfterDeadline": true,
  "autoRestartNotificationDismissal": "automatic",
  "scheduleRestartWarningInHours": 13,
  "scheduleImminentRestartWarningInMinutes": 7,
  "userPauseAccess": "enabled",
  "userWindowsUpdateScanAccess": "enabled",
  "updateNotificationLevel": "defaultNotifications"
}
```

### <a name="response"></a><span data-ttu-id="86ae9-302">响应</span><span class="sxs-lookup"><span data-stu-id="86ae9-302">Response</span></span>
<span data-ttu-id="86ae9-p126">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="86ae9-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3012

{
  "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
  "id": "4928dd6a-dd6a-4928-6add-28496add2849",
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
  "deliveryOptimizationMode": "httpOnly",
  "prereleaseFeatures": "settingsOnly",
  "automaticUpdateMode": "notifyDownload",
  "microsoftUpdateServiceAllowed": true,
  "driversExcluded": true,
  "installationSchedule": {
    "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall",
    "scheduledInstallDay": "everyday",
    "scheduledInstallTime": "11:59:31.3170000"
  },
  "qualityUpdatesDeferralPeriodInDays": 2,
  "featureUpdatesDeferralPeriodInDays": 2,
  "qualityUpdatesPaused": true,
  "featureUpdatesPaused": true,
  "qualityUpdatesPauseExpiryDateTime": "2017-01-01T00:00:22.9594683-08:00",
  "featureUpdatesPauseExpiryDateTime": "2016-12-31T23:58:08.068669-08:00",
  "businessReadyUpdatesOnly": "all",
  "skipChecksBeforeRestart": true,
  "updateWeeks": "firstWeek",
  "qualityUpdatesPauseStartDate": "<Unknown Primitive Type Edm.Date>",
  "featureUpdatesPauseStartDate": "<Unknown Primitive Type Edm.Date>",
  "featureUpdatesRollbackWindowInDays": 2,
  "qualityUpdatesWillBeRolledBack": true,
  "featureUpdatesWillBeRolledBack": true,
  "qualityUpdatesRollbackStartDateTime": "2016-12-31T23:57:01.05526-08:00",
  "featureUpdatesRollbackStartDateTime": "2017-01-01T00:03:21.6080517-08:00",
  "engagedRestartDeadlineInDays": 12,
  "engagedRestartSnoozeScheduleInDays": 2,
  "engagedRestartTransitionScheduleInDays": 6,
  "deadlineForFeatureUpdatesInDays": 15,
  "deadlineForQualityUpdatesInDays": 15,
  "deadlineGracePeriodInDays": 9,
  "postponeRebootUntilAfterDeadline": true,
  "autoRestartNotificationDismissal": "automatic",
  "scheduleRestartWarningInHours": 13,
  "scheduleImminentRestartWarningInMinutes": 7,
  "userPauseAccess": "enabled",
  "userWindowsUpdateScanAccess": "enabled",
  "updateNotificationLevel": "defaultNotifications"
}
```






