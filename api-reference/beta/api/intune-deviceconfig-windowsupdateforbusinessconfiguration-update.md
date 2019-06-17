---
title: 更新 windowsUpdateForBusinessConfiguration
description: 更新 windowsUpdateForBusinessConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b178b614f12ae193b1e2369a9c71e337978dde93
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34961285"
---
# <a name="update-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="237d5-103">更新 windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="237d5-103">Update windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="237d5-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="237d5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="237d5-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="237d5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="237d5-106">更新 [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="237d5-106">Update the properties of a [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="237d5-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="237d5-107">Prerequisites</span></span>
<span data-ttu-id="237d5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="237d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="237d5-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="237d5-110">Permission type</span></span>|<span data-ttu-id="237d5-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="237d5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="237d5-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="237d5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="237d5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="237d5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="237d5-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="237d5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="237d5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="237d5-115">Not supported.</span></span>|
|<span data-ttu-id="237d5-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="237d5-116">Application</span></span>|<span data-ttu-id="237d5-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="237d5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="237d5-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="237d5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="237d5-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="237d5-119">Request headers</span></span>
|<span data-ttu-id="237d5-120">标头</span><span class="sxs-lookup"><span data-stu-id="237d5-120">Header</span></span>|<span data-ttu-id="237d5-121">值</span><span class="sxs-lookup"><span data-stu-id="237d5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="237d5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="237d5-122">Authorization</span></span>|<span data-ttu-id="237d5-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="237d5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="237d5-124">接受</span><span class="sxs-lookup"><span data-stu-id="237d5-124">Accept</span></span>|<span data-ttu-id="237d5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="237d5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="237d5-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="237d5-126">Request body</span></span>
<span data-ttu-id="237d5-127">在请求正文中，提供 [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="237d5-127">In the request body, supply a JSON representation for the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="237d5-128">下表显示创建 [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="237d5-128">The following table shows the properties that are required when you create the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="237d5-129">属性</span><span class="sxs-lookup"><span data-stu-id="237d5-129">Property</span></span>|<span data-ttu-id="237d5-130">类型</span><span class="sxs-lookup"><span data-stu-id="237d5-130">Type</span></span>|<span data-ttu-id="237d5-131">说明</span><span class="sxs-lookup"><span data-stu-id="237d5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="237d5-132">id</span><span class="sxs-lookup"><span data-stu-id="237d5-132">id</span></span>|<span data-ttu-id="237d5-133">字符串</span><span class="sxs-lookup"><span data-stu-id="237d5-133">String</span></span>|<span data-ttu-id="237d5-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="237d5-134">Key of the entity.</span></span> <span data-ttu-id="237d5-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="237d5-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="237d5-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="237d5-136">lastModifiedDateTime</span></span>|<span data-ttu-id="237d5-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="237d5-137">DateTimeOffset</span></span>|<span data-ttu-id="237d5-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="237d5-138">DateTime the object was last modified.</span></span> <span data-ttu-id="237d5-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="237d5-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="237d5-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="237d5-140">roleScopeTagIds</span></span>|<span data-ttu-id="237d5-141">String collection</span><span class="sxs-lookup"><span data-stu-id="237d5-141">String collection</span></span>|<span data-ttu-id="237d5-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="237d5-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="237d5-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="237d5-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="237d5-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="237d5-144">supportsScopeTags</span></span>|<span data-ttu-id="237d5-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="237d5-145">Boolean</span></span>|<span data-ttu-id="237d5-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="237d5-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="237d5-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="237d5-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="237d5-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="237d5-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="237d5-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="237d5-149">This property is read-only.</span></span> <span data-ttu-id="237d5-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="237d5-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="237d5-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="237d5-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="237d5-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="237d5-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="237d5-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="237d5-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="237d5-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="237d5-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="237d5-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="237d5-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="237d5-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="237d5-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="237d5-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="237d5-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="237d5-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="237d5-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="237d5-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="237d5-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="237d5-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="237d5-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="237d5-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="237d5-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="237d5-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="237d5-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="237d5-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="237d5-163">createdDateTime</span></span>|<span data-ttu-id="237d5-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="237d5-164">DateTimeOffset</span></span>|<span data-ttu-id="237d5-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="237d5-165">DateTime the object was created.</span></span> <span data-ttu-id="237d5-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="237d5-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="237d5-167">说明</span><span class="sxs-lookup"><span data-stu-id="237d5-167">description</span></span>|<span data-ttu-id="237d5-168">String</span><span class="sxs-lookup"><span data-stu-id="237d5-168">String</span></span>|<span data-ttu-id="237d5-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="237d5-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="237d5-170">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="237d5-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="237d5-171">displayName</span><span class="sxs-lookup"><span data-stu-id="237d5-171">displayName</span></span>|<span data-ttu-id="237d5-172">String</span><span class="sxs-lookup"><span data-stu-id="237d5-172">String</span></span>|<span data-ttu-id="237d5-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="237d5-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="237d5-174">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="237d5-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="237d5-175">version</span><span class="sxs-lookup"><span data-stu-id="237d5-175">version</span></span>|<span data-ttu-id="237d5-176">Int32</span><span class="sxs-lookup"><span data-stu-id="237d5-176">Int32</span></span>|<span data-ttu-id="237d5-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="237d5-177">Version of the device configuration.</span></span> <span data-ttu-id="237d5-178">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="237d5-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="237d5-179">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="237d5-179">deliveryOptimizationMode</span></span>|[<span data-ttu-id="237d5-180">windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="237d5-180">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="237d5-181">传递优化模式。</span><span class="sxs-lookup"><span data-stu-id="237d5-181">Delivery Optimization Mode.</span></span> <span data-ttu-id="237d5-182">可取值为：`userDefined`、`httpOnly`、`httpWithPeeringNat`、`httpWithPeeringPrivateGroup`、`httpWithInternetPeering`、`simpleDownload` 或 `bypassMode`。</span><span class="sxs-lookup"><span data-stu-id="237d5-182">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="237d5-183">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="237d5-183">prereleaseFeatures</span></span>|[<span data-ttu-id="237d5-184">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="237d5-184">prereleaseFeatures</span></span>](../resources/intune-deviceconfig-prereleasefeatures.md)|<span data-ttu-id="237d5-185">预发布功能。</span><span class="sxs-lookup"><span data-stu-id="237d5-185">The pre-release features.</span></span> <span data-ttu-id="237d5-186">可取值为：`userDefined`、`settingsOnly`、`settingsAndExperimentations`、`notAllowed`。</span><span class="sxs-lookup"><span data-stu-id="237d5-186">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="237d5-187">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="237d5-187">automaticUpdateMode</span></span>|[<span data-ttu-id="237d5-188">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="237d5-188">automaticUpdateMode</span></span>](../resources/intune-deviceconfig-automaticupdatemode.md)|<span data-ttu-id="237d5-189">自动更新模式。</span><span class="sxs-lookup"><span data-stu-id="237d5-189">Automatic update mode.</span></span> <span data-ttu-id="237d5-190">可取值为：`userDefined`、`notifyDownload`、`autoInstallAtMaintenanceTime`、`autoInstallAndRebootAtMaintenanceTime`、`autoInstallAndRebootAtScheduledTime`、`autoInstallAndRebootWithoutEndUserControl` 或 `windowsDefault`。</span><span class="sxs-lookup"><span data-stu-id="237d5-190">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`, `windowsDefault`.</span></span>|
|<span data-ttu-id="237d5-191">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="237d5-191">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="237d5-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="237d5-192">Boolean</span></span>|<span data-ttu-id="237d5-193">允许 Microsoft 更新服务</span><span class="sxs-lookup"><span data-stu-id="237d5-193">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="237d5-194">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="237d5-194">driversExcluded</span></span>|<span data-ttu-id="237d5-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="237d5-195">Boolean</span></span>|<span data-ttu-id="237d5-196">排除 Windows 更新驱动程序</span><span class="sxs-lookup"><span data-stu-id="237d5-196">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="237d5-197">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="237d5-197">installationSchedule</span></span>|[<span data-ttu-id="237d5-198">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="237d5-198">windowsUpdateInstallScheduleType</span></span>](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)|<span data-ttu-id="237d5-199">安装计划</span><span class="sxs-lookup"><span data-stu-id="237d5-199">Installation schedule</span></span>|
|<span data-ttu-id="237d5-200">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="237d5-200">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="237d5-201">Int32</span><span class="sxs-lookup"><span data-stu-id="237d5-201">Int32</span></span>|<span data-ttu-id="237d5-202">推迟质量更新的天数</span><span class="sxs-lookup"><span data-stu-id="237d5-202">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="237d5-203">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="237d5-203">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="237d5-204">Int32</span><span class="sxs-lookup"><span data-stu-id="237d5-204">Int32</span></span>|<span data-ttu-id="237d5-205">推迟功能更新的天数</span><span class="sxs-lookup"><span data-stu-id="237d5-205">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="237d5-206">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="237d5-206">qualityUpdatesPaused</span></span>|<span data-ttu-id="237d5-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="237d5-207">Boolean</span></span>|<span data-ttu-id="237d5-208">暂停质量更新</span><span class="sxs-lookup"><span data-stu-id="237d5-208">Pause Quality Updates</span></span>|
|<span data-ttu-id="237d5-209">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="237d5-209">featureUpdatesPaused</span></span>|<span data-ttu-id="237d5-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="237d5-210">Boolean</span></span>|<span data-ttu-id="237d5-211">暂停功能更新</span><span class="sxs-lookup"><span data-stu-id="237d5-211">Pause Feature Updates</span></span>|
|<span data-ttu-id="237d5-212">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="237d5-212">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="237d5-213">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="237d5-213">DateTimeOffset</span></span>|<span data-ttu-id="237d5-214">质量更新暂停到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="237d5-214">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="237d5-215">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="237d5-215">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="237d5-216">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="237d5-216">DateTimeOffset</span></span>|<span data-ttu-id="237d5-217">功能更新暂停到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="237d5-217">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="237d5-218">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="237d5-218">businessReadyUpdatesOnly</span></span>|[<span data-ttu-id="237d5-219">windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="237d5-219">windowsUpdateType</span></span>](../resources/intune-deviceconfig-windowsupdatetype.md)|<span data-ttu-id="237d5-220">确定将从哪些分支设备接收其更新。</span><span class="sxs-lookup"><span data-stu-id="237d5-220">Determines which branch devices will receive their updates from.</span></span> <span data-ttu-id="237d5-221">可取值为：`userDefined`、`all`、`businessReadyOnly`、`windowsInsiderBuildFast`、`windowsInsiderBuildSlow`、`windowsInsiderBuildRelease`。</span><span class="sxs-lookup"><span data-stu-id="237d5-221">Possible values are: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span></span>|
|<span data-ttu-id="237d5-222">skipChecksBeforeRestart</span><span class="sxs-lookup"><span data-stu-id="237d5-222">skipChecksBeforeRestart</span></span>|<span data-ttu-id="237d5-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="237d5-223">Boolean</span></span>|<span data-ttu-id="237d5-224">设置为在重新启动之前跳过所有复选: 电池级别 = 40%、用户状态、需要显示、演示模式、全屏模式、电话呼叫状态、游戏模式等。</span><span class="sxs-lookup"><span data-stu-id="237d5-224">Set to skip all check before restart: Battery level = 40%, User presence, Display Needed, Presentation mode, Full screen mode, phone call state, game mode etc.</span></span> |
|<span data-ttu-id="237d5-225">updateWeeks</span><span class="sxs-lookup"><span data-stu-id="237d5-225">updateWeeks</span></span>|[<span data-ttu-id="237d5-226">windowsUpdateForBusinessUpdateWeeks</span><span class="sxs-lookup"><span data-stu-id="237d5-226">windowsUpdateForBusinessUpdateWeeks</span></span>](../resources/intune-deviceconfig-windowsupdateforbusinessupdateweeks.md)|<span data-ttu-id="237d5-227">在每月的几周安排更新安装。</span><span class="sxs-lookup"><span data-stu-id="237d5-227">Scheduled the update installation on the weeks of the month.</span></span> <span data-ttu-id="237d5-228">可取值为：`userDefined`、`firstWeek`、`secondWeek`、`thirdWeek`、`fourthWeek`、`everyWeek`。</span><span class="sxs-lookup"><span data-stu-id="237d5-228">Possible values are: `userDefined`, `firstWeek`, `secondWeek`, `thirdWeek`, `fourthWeek`, `everyWeek`.</span></span>|
|<span data-ttu-id="237d5-229">qualityUpdatesPauseStartDate</span><span class="sxs-lookup"><span data-stu-id="237d5-229">qualityUpdatesPauseStartDate</span></span>|<span data-ttu-id="237d5-230">日期</span><span class="sxs-lookup"><span data-stu-id="237d5-230">Date</span></span>|<span data-ttu-id="237d5-231">质量更新暂停开始日期。</span><span class="sxs-lookup"><span data-stu-id="237d5-231">Quality Updates Pause start date.</span></span> <span data-ttu-id="237d5-232">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="237d5-232">This property is read-only.</span></span>|
|<span data-ttu-id="237d5-233">featureUpdatesPauseStartDate</span><span class="sxs-lookup"><span data-stu-id="237d5-233">featureUpdatesPauseStartDate</span></span>|<span data-ttu-id="237d5-234">日期</span><span class="sxs-lookup"><span data-stu-id="237d5-234">Date</span></span>|<span data-ttu-id="237d5-235">功能更新暂停开始日期。</span><span class="sxs-lookup"><span data-stu-id="237d5-235">Feature Updates Pause start date.</span></span> <span data-ttu-id="237d5-236">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="237d5-236">This property is read-only.</span></span>|
|<span data-ttu-id="237d5-237">featureUpdatesRollbackWindowInDays</span><span class="sxs-lookup"><span data-stu-id="237d5-237">featureUpdatesRollbackWindowInDays</span></span>|<span data-ttu-id="237d5-238">Int32</span><span class="sxs-lookup"><span data-stu-id="237d5-238">Int32</span></span>|<span data-ttu-id="237d5-239">回滚对其有效的功能更新后的天数</span><span class="sxs-lookup"><span data-stu-id="237d5-239">The number of days after a Feature Update for which a rollback is valid</span></span>|
|<span data-ttu-id="237d5-240">qualityUpdatesWillBeRolledBack</span><span class="sxs-lookup"><span data-stu-id="237d5-240">qualityUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="237d5-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="237d5-241">Boolean</span></span>|<span data-ttu-id="237d5-242">指定是否在下一个设备签入时回滚质量更新</span><span class="sxs-lookup"><span data-stu-id="237d5-242">Specifies whether to rollback Quality Updates on the next device check in</span></span>|
|<span data-ttu-id="237d5-243">featureUpdatesWillBeRolledBack</span><span class="sxs-lookup"><span data-stu-id="237d5-243">featureUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="237d5-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="237d5-244">Boolean</span></span>|<span data-ttu-id="237d5-245">指定是否在下一个设备签入时回滚功能更新</span><span class="sxs-lookup"><span data-stu-id="237d5-245">Specifies whether to rollback Feature Updates on the next device check in</span></span>|
|<span data-ttu-id="237d5-246">qualityUpdatesRollbackStartDateTime</span><span class="sxs-lookup"><span data-stu-id="237d5-246">qualityUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="237d5-247">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="237d5-247">DateTimeOffset</span></span>|<span data-ttu-id="237d5-248">质量更新回滚开始日期/时间</span><span class="sxs-lookup"><span data-stu-id="237d5-248">Quality Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="237d5-249">featureUpdatesRollbackStartDateTime</span><span class="sxs-lookup"><span data-stu-id="237d5-249">featureUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="237d5-250">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="237d5-250">DateTimeOffset</span></span>|<span data-ttu-id="237d5-251">功能更新回滚的开始日期时间</span><span class="sxs-lookup"><span data-stu-id="237d5-251">Feature Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="237d5-252">engagedRestartDeadlineInDays</span><span class="sxs-lookup"><span data-stu-id="237d5-252">engagedRestartDeadlineInDays</span></span>|<span data-ttu-id="237d5-253">Int32</span><span class="sxs-lookup"><span data-stu-id="237d5-253">Int32</span></span>|<span data-ttu-id="237d5-254">在非活动时段自动安排和执行挂起的重启的期限 (以天为单位), 有效范围为2到30天</span><span class="sxs-lookup"><span data-stu-id="237d5-254">Deadline in days before automatically scheduling and executing a pending restart outside of active hours, with valid range from 2 to 30 days</span></span>|
|<span data-ttu-id="237d5-255">engagedRestartSnoozeScheduleInDays</span><span class="sxs-lookup"><span data-stu-id="237d5-255">engagedRestartSnoozeScheduleInDays</span></span>|<span data-ttu-id="237d5-256">Int32</span><span class="sxs-lookup"><span data-stu-id="237d5-256">Int32</span></span>|<span data-ttu-id="237d5-257">用户可推迟预定重启提醒通知的天数, 有效范围为1到3天</span><span class="sxs-lookup"><span data-stu-id="237d5-257">Number of days a user can snooze Engaged Restart reminder notifications with valid range from 1 to 3 days</span></span>|
|<span data-ttu-id="237d5-258">engagedRestartTransitionScheduleInDays</span><span class="sxs-lookup"><span data-stu-id="237d5-258">engagedRestartTransitionScheduleInDays</span></span>|<span data-ttu-id="237d5-259">Int32</span><span class="sxs-lookup"><span data-stu-id="237d5-259">Int32</span></span>|<span data-ttu-id="237d5-260">从主动时段之外的计划的自动重启转换为预定重启 (需要用户进行计划, 有效范围为0到30天) 的天数</span><span class="sxs-lookup"><span data-stu-id="237d5-260">Number of days before transitioning from Auto Restarts scheduled outside of active hours to Engaged Restart, which requires the user to schedule, with valid range from 0 to 30 days</span></span>|
|<span data-ttu-id="237d5-261">autoRestartNotificationDismissal</span><span class="sxs-lookup"><span data-stu-id="237d5-261">autoRestartNotificationDismissal</span></span>|[<span data-ttu-id="237d5-262">autoRestartNotificationDismissalMethod</span><span class="sxs-lookup"><span data-stu-id="237d5-262">autoRestartNotificationDismissalMethod</span></span>](../resources/intune-deviceconfig-autorestartnotificationdismissalmethod.md)|<span data-ttu-id="237d5-263">指定用于消除 "需要自动重新启动" 通知的方法。</span><span class="sxs-lookup"><span data-stu-id="237d5-263">Specify the method by which the auto-restart required notification is dismissed.</span></span> <span data-ttu-id="237d5-264">可取值为：`notConfigured`、`automatic`、`user`。</span><span class="sxs-lookup"><span data-stu-id="237d5-264">Possible values are: `notConfigured`, `automatic`, `user`.</span></span>|
|<span data-ttu-id="237d5-265">scheduleRestartWarningInHours</span><span class="sxs-lookup"><span data-stu-id="237d5-265">scheduleRestartWarningInHours</span></span>|<span data-ttu-id="237d5-266">Int32</span><span class="sxs-lookup"><span data-stu-id="237d5-266">Int32</span></span>|<span data-ttu-id="237d5-267">指定自动重新启动警告提醒通知的期限。</span><span class="sxs-lookup"><span data-stu-id="237d5-267">Specify the period for auto-restart warning reminder notifications.</span></span> <span data-ttu-id="237d5-268">支持的值: 2、4、8、12或 24 (小时)。</span><span class="sxs-lookup"><span data-stu-id="237d5-268">Supported values: 2, 4, 8, 12 or 24 (hours).</span></span>|
|<span data-ttu-id="237d5-269">scheduleImminentRestartWarningInMinutes</span><span class="sxs-lookup"><span data-stu-id="237d5-269">scheduleImminentRestartWarningInMinutes</span></span>|<span data-ttu-id="237d5-270">Int32</span><span class="sxs-lookup"><span data-stu-id="237d5-270">Int32</span></span>|<span data-ttu-id="237d5-271">指定自动重启即将发生的警告通知的期限。</span><span class="sxs-lookup"><span data-stu-id="237d5-271">Specify the period for auto-restart imminent warning notifications.</span></span> <span data-ttu-id="237d5-272">支持的值:15、30或 60 (分钟)。</span><span class="sxs-lookup"><span data-stu-id="237d5-272">Supported values: 15, 30 or 60 (minutes).</span></span>|
|<span data-ttu-id="237d5-273">userPauseAccess</span><span class="sxs-lookup"><span data-stu-id="237d5-273">userPauseAccess</span></span>|[<span data-ttu-id="237d5-274">启用</span><span class="sxs-lookup"><span data-stu-id="237d5-274">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="237d5-275">指定是否允许最终用户访问暂停软件更新。</span><span class="sxs-lookup"><span data-stu-id="237d5-275">Specifies whether to enable end user’s access to pause software updates.</span></span> <span data-ttu-id="237d5-276">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="237d5-276">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="237d5-277">userWindowsUpdateScanAccess</span><span class="sxs-lookup"><span data-stu-id="237d5-277">userWindowsUpdateScanAccess</span></span>|[<span data-ttu-id="237d5-278">启用</span><span class="sxs-lookup"><span data-stu-id="237d5-278">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="237d5-279">指定是否禁用用户对扫描 Windows 更新的访问权限。</span><span class="sxs-lookup"><span data-stu-id="237d5-279">Specifies whether to disable user’s access to scan Windows Update.</span></span> <span data-ttu-id="237d5-280">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="237d5-280">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="237d5-281">updateNotificationLevel</span><span class="sxs-lookup"><span data-stu-id="237d5-281">updateNotificationLevel</span></span>|[<span data-ttu-id="237d5-282">windowsUpdateNotificationDisplayOption</span><span class="sxs-lookup"><span data-stu-id="237d5-282">windowsUpdateNotificationDisplayOption</span></span>](../resources/intune-deviceconfig-windowsupdatenotificationdisplayoption.md)|<span data-ttu-id="237d5-283">指定用户看到的 Windows 更新通知的具体内容。</span><span class="sxs-lookup"><span data-stu-id="237d5-283">Specifies what Windows Update notifications users see.</span></span> <span data-ttu-id="237d5-284">可取值为：`notConfigured`、`defaultNotifications`、`restartWarningsOnly`、`disableAllNotifications`。</span><span class="sxs-lookup"><span data-stu-id="237d5-284">Possible values are: `notConfigured`, `defaultNotifications`, `restartWarningsOnly`, `disableAllNotifications`.</span></span>|



## <a name="response"></a><span data-ttu-id="237d5-285">响应</span><span class="sxs-lookup"><span data-stu-id="237d5-285">Response</span></span>
<span data-ttu-id="237d5-286">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="237d5-286">If successful, this method returns a `200 OK` response code and an updated [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="237d5-287">示例</span><span class="sxs-lookup"><span data-stu-id="237d5-287">Example</span></span>

### <a name="request"></a><span data-ttu-id="237d5-288">请求</span><span class="sxs-lookup"><span data-stu-id="237d5-288">Request</span></span>
<span data-ttu-id="237d5-289">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="237d5-289">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2676

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
  "autoRestartNotificationDismissal": "automatic",
  "scheduleRestartWarningInHours": 13,
  "scheduleImminentRestartWarningInMinutes": 7,
  "userPauseAccess": "enabled",
  "userWindowsUpdateScanAccess": "enabled",
  "updateNotificationLevel": "defaultNotifications"
}
```

### <a name="response"></a><span data-ttu-id="237d5-290">响应</span><span class="sxs-lookup"><span data-stu-id="237d5-290">Response</span></span>
<span data-ttu-id="237d5-p126">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="237d5-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2848

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
  "autoRestartNotificationDismissal": "automatic",
  "scheduleRestartWarningInHours": 13,
  "scheduleImminentRestartWarningInMinutes": 7,
  "userPauseAccess": "enabled",
  "userWindowsUpdateScanAccess": "enabled",
  "updateNotificationLevel": "defaultNotifications"
}
```





