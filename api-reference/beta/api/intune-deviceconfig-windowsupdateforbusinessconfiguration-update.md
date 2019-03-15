---
title: 更新 windowsUpdateForBusinessConfiguration
description: 更新 windowsUpdateForBusinessConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4ae7af29f9fdf37828548860553a613738333492
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571198"
---
# <a name="update-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="af777-103">更新 windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="af777-103">Update windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="af777-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="af777-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="af777-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="af777-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af777-106">更新 [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="af777-106">Update the properties of a [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="af777-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="af777-107">Prerequisites</span></span>
<span data-ttu-id="af777-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="af777-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="af777-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="af777-110">Permission type</span></span>|<span data-ttu-id="af777-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="af777-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af777-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="af777-112">Delegated (work or school account)</span></span>|<span data-ttu-id="af777-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af777-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="af777-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="af777-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af777-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="af777-115">Not supported.</span></span>|
|<span data-ttu-id="af777-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="af777-116">Application</span></span>|<span data-ttu-id="af777-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="af777-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="af777-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="af777-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="af777-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="af777-119">Request headers</span></span>
|<span data-ttu-id="af777-120">标头</span><span class="sxs-lookup"><span data-stu-id="af777-120">Header</span></span>|<span data-ttu-id="af777-121">值</span><span class="sxs-lookup"><span data-stu-id="af777-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af777-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="af777-122">Authorization</span></span>|<span data-ttu-id="af777-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="af777-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="af777-124">接受</span><span class="sxs-lookup"><span data-stu-id="af777-124">Accept</span></span>|<span data-ttu-id="af777-125">application/json</span><span class="sxs-lookup"><span data-stu-id="af777-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af777-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="af777-126">Request body</span></span>
<span data-ttu-id="af777-127">在请求正文中，提供 [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="af777-127">In the request body, supply a JSON representation for the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="af777-128">下表显示创建 [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="af777-128">The following table shows the properties that are required when you create the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="af777-129">属性</span><span class="sxs-lookup"><span data-stu-id="af777-129">Property</span></span>|<span data-ttu-id="af777-130">类型</span><span class="sxs-lookup"><span data-stu-id="af777-130">Type</span></span>|<span data-ttu-id="af777-131">说明</span><span class="sxs-lookup"><span data-stu-id="af777-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af777-132">id</span><span class="sxs-lookup"><span data-stu-id="af777-132">id</span></span>|<span data-ttu-id="af777-133">String</span><span class="sxs-lookup"><span data-stu-id="af777-133">String</span></span>|<span data-ttu-id="af777-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="af777-134">Key of the entity.</span></span> <span data-ttu-id="af777-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="af777-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="af777-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="af777-136">lastModifiedDateTime</span></span>|<span data-ttu-id="af777-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af777-137">DateTimeOffset</span></span>|<span data-ttu-id="af777-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="af777-138">DateTime the object was last modified.</span></span> <span data-ttu-id="af777-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="af777-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="af777-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="af777-140">roleScopeTagIds</span></span>|<span data-ttu-id="af777-141">String collection</span><span class="sxs-lookup"><span data-stu-id="af777-141">String collection</span></span>|<span data-ttu-id="af777-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="af777-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="af777-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="af777-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="af777-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="af777-144">supportsScopeTags</span></span>|<span data-ttu-id="af777-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="af777-145">Boolean</span></span>|<span data-ttu-id="af777-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="af777-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="af777-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="af777-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="af777-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="af777-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="af777-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="af777-149">This property is read-only.</span></span> <span data-ttu-id="af777-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="af777-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="af777-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="af777-151">createdDateTime</span></span>|<span data-ttu-id="af777-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af777-152">DateTimeOffset</span></span>|<span data-ttu-id="af777-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="af777-153">DateTime the object was created.</span></span> <span data-ttu-id="af777-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="af777-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="af777-155">说明</span><span class="sxs-lookup"><span data-stu-id="af777-155">description</span></span>|<span data-ttu-id="af777-156">String</span><span class="sxs-lookup"><span data-stu-id="af777-156">String</span></span>|<span data-ttu-id="af777-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="af777-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="af777-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="af777-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="af777-159">displayName</span><span class="sxs-lookup"><span data-stu-id="af777-159">displayName</span></span>|<span data-ttu-id="af777-160">String</span><span class="sxs-lookup"><span data-stu-id="af777-160">String</span></span>|<span data-ttu-id="af777-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="af777-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="af777-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="af777-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="af777-163">version</span><span class="sxs-lookup"><span data-stu-id="af777-163">version</span></span>|<span data-ttu-id="af777-164">Int32</span><span class="sxs-lookup"><span data-stu-id="af777-164">Int32</span></span>|<span data-ttu-id="af777-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="af777-165">Version of the device configuration.</span></span> <span data-ttu-id="af777-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="af777-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="af777-167">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="af777-167">deliveryOptimizationMode</span></span>|[<span data-ttu-id="af777-168">windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="af777-168">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="af777-169">传递优化模式。</span><span class="sxs-lookup"><span data-stu-id="af777-169">Delivery Optimization Mode.</span></span> <span data-ttu-id="af777-170">可取值为：`userDefined`、`httpOnly`、`httpWithPeeringNat`、`httpWithPeeringPrivateGroup`、`httpWithInternetPeering`、`simpleDownload` 或 `bypassMode`。</span><span class="sxs-lookup"><span data-stu-id="af777-170">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="af777-171">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="af777-171">prereleaseFeatures</span></span>|[<span data-ttu-id="af777-172">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="af777-172">prereleaseFeatures</span></span>](../resources/intune-deviceconfig-prereleasefeatures.md)|<span data-ttu-id="af777-173">预发布功能。</span><span class="sxs-lookup"><span data-stu-id="af777-173">The pre-release features.</span></span> <span data-ttu-id="af777-174">可取值为：`userDefined`、`settingsOnly`、`settingsAndExperimentations`、`notAllowed`。</span><span class="sxs-lookup"><span data-stu-id="af777-174">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="af777-175">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="af777-175">automaticUpdateMode</span></span>|[<span data-ttu-id="af777-176">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="af777-176">automaticUpdateMode</span></span>](../resources/intune-deviceconfig-automaticupdatemode.md)|<span data-ttu-id="af777-177">自动更新模式。</span><span class="sxs-lookup"><span data-stu-id="af777-177">Automatic update mode.</span></span> <span data-ttu-id="af777-178">可取值为：`userDefined`、`notifyDownload`、`autoInstallAtMaintenanceTime`、`autoInstallAndRebootAtMaintenanceTime`、`autoInstallAndRebootAtScheduledTime`、`autoInstallAndRebootWithoutEndUserControl` 或 `windowsDefault`。</span><span class="sxs-lookup"><span data-stu-id="af777-178">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`, `windowsDefault`.</span></span>|
|<span data-ttu-id="af777-179">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="af777-179">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="af777-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="af777-180">Boolean</span></span>|<span data-ttu-id="af777-181">允许 Microsoft 更新服务</span><span class="sxs-lookup"><span data-stu-id="af777-181">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="af777-182">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="af777-182">driversExcluded</span></span>|<span data-ttu-id="af777-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="af777-183">Boolean</span></span>|<span data-ttu-id="af777-184">排除 Windows 更新驱动程序</span><span class="sxs-lookup"><span data-stu-id="af777-184">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="af777-185">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="af777-185">installationSchedule</span></span>|[<span data-ttu-id="af777-186">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="af777-186">windowsUpdateInstallScheduleType</span></span>](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)|<span data-ttu-id="af777-187">安装计划</span><span class="sxs-lookup"><span data-stu-id="af777-187">Installation schedule</span></span>|
|<span data-ttu-id="af777-188">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="af777-188">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="af777-189">Int32</span><span class="sxs-lookup"><span data-stu-id="af777-189">Int32</span></span>|<span data-ttu-id="af777-190">推迟质量更新的天数</span><span class="sxs-lookup"><span data-stu-id="af777-190">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="af777-191">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="af777-191">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="af777-192">Int32</span><span class="sxs-lookup"><span data-stu-id="af777-192">Int32</span></span>|<span data-ttu-id="af777-193">推迟功能更新的天数</span><span class="sxs-lookup"><span data-stu-id="af777-193">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="af777-194">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="af777-194">qualityUpdatesPaused</span></span>|<span data-ttu-id="af777-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="af777-195">Boolean</span></span>|<span data-ttu-id="af777-196">暂停质量更新</span><span class="sxs-lookup"><span data-stu-id="af777-196">Pause Quality Updates</span></span>|
|<span data-ttu-id="af777-197">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="af777-197">featureUpdatesPaused</span></span>|<span data-ttu-id="af777-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="af777-198">Boolean</span></span>|<span data-ttu-id="af777-199">暂停功能更新</span><span class="sxs-lookup"><span data-stu-id="af777-199">Pause Feature Updates</span></span>|
|<span data-ttu-id="af777-200">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="af777-200">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="af777-201">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af777-201">DateTimeOffset</span></span>|<span data-ttu-id="af777-202">质量更新暂停到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="af777-202">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="af777-203">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="af777-203">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="af777-204">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af777-204">DateTimeOffset</span></span>|<span data-ttu-id="af777-205">功能更新暂停到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="af777-205">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="af777-206">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="af777-206">businessReadyUpdatesOnly</span></span>|[<span data-ttu-id="af777-207">windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="af777-207">windowsUpdateType</span></span>](../resources/intune-deviceconfig-windowsupdatetype.md)|<span data-ttu-id="af777-208">确定将从哪些分支设备接收其更新。</span><span class="sxs-lookup"><span data-stu-id="af777-208">Determines which branch devices will receive their updates from.</span></span> <span data-ttu-id="af777-209">可取值为：`userDefined`、`all`、`businessReadyOnly`、`windowsInsiderBuildFast`、`windowsInsiderBuildSlow`、`windowsInsiderBuildRelease`。</span><span class="sxs-lookup"><span data-stu-id="af777-209">Possible values are: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span></span>|
|<span data-ttu-id="af777-210">skipChecksBeforeRestart</span><span class="sxs-lookup"><span data-stu-id="af777-210">skipChecksBeforeRestart</span></span>|<span data-ttu-id="af777-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="af777-211">Boolean</span></span>|<span data-ttu-id="af777-212">设置为在重新启动之前跳过所有复选: 电池级别 = 40%、用户状态、需要显示、演示模式、全屏模式、电话呼叫状态、游戏模式等。</span><span class="sxs-lookup"><span data-stu-id="af777-212">Set to skip all check before restart: Battery level = 40%, User presence, Display Needed, Presentation mode, Full screen mode, phone call state, game mode etc.</span></span> |
|<span data-ttu-id="af777-213">updateWeeks</span><span class="sxs-lookup"><span data-stu-id="af777-213">updateWeeks</span></span>|[<span data-ttu-id="af777-214">windowsUpdateForBusinessUpdateWeeks</span><span class="sxs-lookup"><span data-stu-id="af777-214">windowsUpdateForBusinessUpdateWeeks</span></span>](../resources/intune-deviceconfig-windowsupdateforbusinessupdateweeks.md)|<span data-ttu-id="af777-215">在每月的几周安排更新安装。</span><span class="sxs-lookup"><span data-stu-id="af777-215">Scheduled the update installation on the weeks of the month.</span></span> <span data-ttu-id="af777-216">可取值为：`userDefined`、`firstWeek`、`secondWeek`、`thirdWeek`、`fourthWeek`、`everyWeek`。</span><span class="sxs-lookup"><span data-stu-id="af777-216">Possible values are: `userDefined`, `firstWeek`, `secondWeek`, `thirdWeek`, `fourthWeek`, `everyWeek`.</span></span>|
|<span data-ttu-id="af777-217">qualityUpdatesPauseStartDate</span><span class="sxs-lookup"><span data-stu-id="af777-217">qualityUpdatesPauseStartDate</span></span>|<span data-ttu-id="af777-218">日期</span><span class="sxs-lookup"><span data-stu-id="af777-218">Date</span></span>|<span data-ttu-id="af777-219">质量更新暂停开始日期。</span><span class="sxs-lookup"><span data-stu-id="af777-219">Quality Updates Pause start date.</span></span> <span data-ttu-id="af777-220">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="af777-220">This property is read-only.</span></span>|
|<span data-ttu-id="af777-221">featureUpdatesPauseStartDate</span><span class="sxs-lookup"><span data-stu-id="af777-221">featureUpdatesPauseStartDate</span></span>|<span data-ttu-id="af777-222">日期</span><span class="sxs-lookup"><span data-stu-id="af777-222">Date</span></span>|<span data-ttu-id="af777-223">功能更新暂停开始日期。</span><span class="sxs-lookup"><span data-stu-id="af777-223">Feature Updates Pause start date.</span></span> <span data-ttu-id="af777-224">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="af777-224">This property is read-only.</span></span>|
|<span data-ttu-id="af777-225">featureUpdatesRollbackWindowInDays</span><span class="sxs-lookup"><span data-stu-id="af777-225">featureUpdatesRollbackWindowInDays</span></span>|<span data-ttu-id="af777-226">Int32</span><span class="sxs-lookup"><span data-stu-id="af777-226">Int32</span></span>|<span data-ttu-id="af777-227">回滚对其有效的功能更新后的天数</span><span class="sxs-lookup"><span data-stu-id="af777-227">The number of days after a Feature Update for which a rollback is valid</span></span>|
|<span data-ttu-id="af777-228">qualityUpdatesWillBeRolledBack</span><span class="sxs-lookup"><span data-stu-id="af777-228">qualityUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="af777-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="af777-229">Boolean</span></span>|<span data-ttu-id="af777-230">指定是否在下一个设备签入时回滚质量更新</span><span class="sxs-lookup"><span data-stu-id="af777-230">Specifies whether to rollback Quality Updates on the next device check in</span></span>|
|<span data-ttu-id="af777-231">featureUpdatesWillBeRolledBack</span><span class="sxs-lookup"><span data-stu-id="af777-231">featureUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="af777-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="af777-232">Boolean</span></span>|<span data-ttu-id="af777-233">指定是否在下一个设备签入时回滚功能更新</span><span class="sxs-lookup"><span data-stu-id="af777-233">Specifies whether to rollback Feature Updates on the next device check in</span></span>|
|<span data-ttu-id="af777-234">qualityUpdatesRollbackStartDateTime</span><span class="sxs-lookup"><span data-stu-id="af777-234">qualityUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="af777-235">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af777-235">DateTimeOffset</span></span>|<span data-ttu-id="af777-236">质量更新回滚开始日期/时间</span><span class="sxs-lookup"><span data-stu-id="af777-236">Quality Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="af777-237">featureUpdatesRollbackStartDateTime</span><span class="sxs-lookup"><span data-stu-id="af777-237">featureUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="af777-238">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af777-238">DateTimeOffset</span></span>|<span data-ttu-id="af777-239">功能更新回滚的开始日期时间</span><span class="sxs-lookup"><span data-stu-id="af777-239">Feature Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="af777-240">engagedRestartDeadlineInDays</span><span class="sxs-lookup"><span data-stu-id="af777-240">engagedRestartDeadlineInDays</span></span>|<span data-ttu-id="af777-241">Int32</span><span class="sxs-lookup"><span data-stu-id="af777-241">Int32</span></span>|<span data-ttu-id="af777-242">在非活动时段自动安排和执行挂起的重启的期限 (以天为单位), 有效范围为2到30天</span><span class="sxs-lookup"><span data-stu-id="af777-242">Deadline in days before automatically scheduling and executing a pending restart outside of active hours, with valid range from 2 to 30 days</span></span>|
|<span data-ttu-id="af777-243">engagedRestartSnoozeScheduleInDays</span><span class="sxs-lookup"><span data-stu-id="af777-243">engagedRestartSnoozeScheduleInDays</span></span>|<span data-ttu-id="af777-244">Int32</span><span class="sxs-lookup"><span data-stu-id="af777-244">Int32</span></span>|<span data-ttu-id="af777-245">用户可推迟预定重启提醒通知的天数, 有效范围为1到3天</span><span class="sxs-lookup"><span data-stu-id="af777-245">Number of days a user can snooze Engaged Restart reminder notifications with valid range from 1 to 3 days</span></span>|
|<span data-ttu-id="af777-246">engagedRestartTransitionScheduleInDays</span><span class="sxs-lookup"><span data-stu-id="af777-246">engagedRestartTransitionScheduleInDays</span></span>|<span data-ttu-id="af777-247">Int32</span><span class="sxs-lookup"><span data-stu-id="af777-247">Int32</span></span>|<span data-ttu-id="af777-248">从主动时段之外的计划的自动重启转换为预定重启 (需要用户进行计划, 有效范围为0到30天) 的天数</span><span class="sxs-lookup"><span data-stu-id="af777-248">Number of days before transitioning from Auto Restarts scheduled outside of active hours to Engaged Restart, which requires the user to schedule, with valid range from 0 to 30 days</span></span>|
|<span data-ttu-id="af777-249">autoRestartNotificationDismissal</span><span class="sxs-lookup"><span data-stu-id="af777-249">autoRestartNotificationDismissal</span></span>|[<span data-ttu-id="af777-250">autoRestartNotificationDismissalMethod</span><span class="sxs-lookup"><span data-stu-id="af777-250">autoRestartNotificationDismissalMethod</span></span>](../resources/intune-deviceconfig-autorestartnotificationdismissalmethod.md)|<span data-ttu-id="af777-251">指定用于消除 "需要自动重新启动" 通知的方法。</span><span class="sxs-lookup"><span data-stu-id="af777-251">Specify the method by which the auto-restart required notification is dismissed.</span></span> <span data-ttu-id="af777-252">可取值为：`notConfigured`、`automatic`、`user`。</span><span class="sxs-lookup"><span data-stu-id="af777-252">Possible values are: `notConfigured`, `automatic`, `user`.</span></span>|
|<span data-ttu-id="af777-253">scheduleRestartWarningInHours</span><span class="sxs-lookup"><span data-stu-id="af777-253">scheduleRestartWarningInHours</span></span>|<span data-ttu-id="af777-254">Int32</span><span class="sxs-lookup"><span data-stu-id="af777-254">Int32</span></span>|<span data-ttu-id="af777-255">指定自动重新启动警告提醒通知的期限。</span><span class="sxs-lookup"><span data-stu-id="af777-255">Specify the period for auto-restart warning reminder notifications.</span></span> <span data-ttu-id="af777-256">支持的值: 2、4、8、12或 24 (小时)。</span><span class="sxs-lookup"><span data-stu-id="af777-256">Supported values: 2, 4, 8, 12 or 24 (hours).</span></span>|
|<span data-ttu-id="af777-257">scheduleImminentRestartWarningInMinutes</span><span class="sxs-lookup"><span data-stu-id="af777-257">scheduleImminentRestartWarningInMinutes</span></span>|<span data-ttu-id="af777-258">Int32</span><span class="sxs-lookup"><span data-stu-id="af777-258">Int32</span></span>|<span data-ttu-id="af777-259">指定自动重启即将发生的警告通知的期限。</span><span class="sxs-lookup"><span data-stu-id="af777-259">Specify the period for auto-restart imminent warning notifications.</span></span> <span data-ttu-id="af777-260">支持的值:15、30或 60 (分钟)。</span><span class="sxs-lookup"><span data-stu-id="af777-260">Supported values: 15, 30 or 60 (minutes).</span></span>|
|<span data-ttu-id="af777-261">userPauseAccess</span><span class="sxs-lookup"><span data-stu-id="af777-261">userPauseAccess</span></span>|[<span data-ttu-id="af777-262">启用</span><span class="sxs-lookup"><span data-stu-id="af777-262">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="af777-263">指定是否允许最终用户访问暂停软件更新。</span><span class="sxs-lookup"><span data-stu-id="af777-263">Specifies whether to enable end user’s access to pause software updates.</span></span> <span data-ttu-id="af777-264">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="af777-264">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="af777-265">userWindowsUpdateScanAccess</span><span class="sxs-lookup"><span data-stu-id="af777-265">userWindowsUpdateScanAccess</span></span>|[<span data-ttu-id="af777-266">启用</span><span class="sxs-lookup"><span data-stu-id="af777-266">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="af777-267">指定是否禁用用户对扫描 Windows 更新的访问权限。</span><span class="sxs-lookup"><span data-stu-id="af777-267">Specifies whether to disable user’s access to scan Windows Update.</span></span> <span data-ttu-id="af777-268">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="af777-268">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="af777-269">updateNotificationLevel</span><span class="sxs-lookup"><span data-stu-id="af777-269">updateNotificationLevel</span></span>|[<span data-ttu-id="af777-270">windowsUpdateNotificationDisplayOption</span><span class="sxs-lookup"><span data-stu-id="af777-270">windowsUpdateNotificationDisplayOption</span></span>](../resources/intune-deviceconfig-windowsupdatenotificationdisplayoption.md)|<span data-ttu-id="af777-271">指定用户看到的 Windows 更新通知的具体内容。</span><span class="sxs-lookup"><span data-stu-id="af777-271">Specifies what Windows Update notifications users see.</span></span> <span data-ttu-id="af777-272">可取值为：`notConfigured`、`defaultNotifications`、`restartWarningsOnly`、`disableAllNotifications`。</span><span class="sxs-lookup"><span data-stu-id="af777-272">Possible values are: `notConfigured`, `defaultNotifications`, `restartWarningsOnly`, `disableAllNotifications`.</span></span>|



## <a name="response"></a><span data-ttu-id="af777-273">响应</span><span class="sxs-lookup"><span data-stu-id="af777-273">Response</span></span>
<span data-ttu-id="af777-274">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="af777-274">If successful, this method returns a `200 OK` response code and an updated [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af777-275">示例</span><span class="sxs-lookup"><span data-stu-id="af777-275">Example</span></span>

### <a name="request"></a><span data-ttu-id="af777-276">请求</span><span class="sxs-lookup"><span data-stu-id="af777-276">Request</span></span>
<span data-ttu-id="af777-277">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="af777-277">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1903

{
  "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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

### <a name="response"></a><span data-ttu-id="af777-278">响应</span><span class="sxs-lookup"><span data-stu-id="af777-278">Response</span></span>
<span data-ttu-id="af777-p123">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="af777-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2075

{
  "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
  "id": "4928dd6a-dd6a-4928-6add-28496add2849",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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




