---
title: 创建 windowsUpdateForBusinessConfiguration
description: 创建新的 windowsUpdateForBusinessConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8f874b495e177417842b01806d19fbaa239b5418
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33917391"
---
# <a name="create-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="9503c-103">创建 windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="9503c-103">Create windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="9503c-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9503c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9503c-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9503c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9503c-106">创建新的 [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9503c-106">Create a new [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9503c-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="9503c-107">Prerequisites</span></span>
<span data-ttu-id="9503c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9503c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9503c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9503c-110">Permission type</span></span>|<span data-ttu-id="9503c-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9503c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9503c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9503c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9503c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9503c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9503c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9503c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9503c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9503c-115">Not supported.</span></span>|
|<span data-ttu-id="9503c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9503c-116">Application</span></span>|<span data-ttu-id="9503c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="9503c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9503c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9503c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9503c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9503c-119">Request headers</span></span>
|<span data-ttu-id="9503c-120">标头</span><span class="sxs-lookup"><span data-stu-id="9503c-120">Header</span></span>|<span data-ttu-id="9503c-121">值</span><span class="sxs-lookup"><span data-stu-id="9503c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9503c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9503c-122">Authorization</span></span>|<span data-ttu-id="9503c-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9503c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9503c-124">接受</span><span class="sxs-lookup"><span data-stu-id="9503c-124">Accept</span></span>|<span data-ttu-id="9503c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9503c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9503c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9503c-126">Request body</span></span>
<span data-ttu-id="9503c-127">在请求正文中，提供 windowsUpdateForBusinessConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9503c-127">In the request body, supply a JSON representation for the windowsUpdateForBusinessConfiguration object.</span></span>

<span data-ttu-id="9503c-128">下表显示创建 windowsUpdateForBusinessConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9503c-128">The following table shows the properties that are required when you create the windowsUpdateForBusinessConfiguration.</span></span>

|<span data-ttu-id="9503c-129">属性</span><span class="sxs-lookup"><span data-stu-id="9503c-129">Property</span></span>|<span data-ttu-id="9503c-130">类型</span><span class="sxs-lookup"><span data-stu-id="9503c-130">Type</span></span>|<span data-ttu-id="9503c-131">说明</span><span class="sxs-lookup"><span data-stu-id="9503c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9503c-132">id</span><span class="sxs-lookup"><span data-stu-id="9503c-132">id</span></span>|<span data-ttu-id="9503c-133">字符串</span><span class="sxs-lookup"><span data-stu-id="9503c-133">String</span></span>|<span data-ttu-id="9503c-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9503c-134">Key of the entity.</span></span> <span data-ttu-id="9503c-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9503c-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9503c-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9503c-136">lastModifiedDateTime</span></span>|<span data-ttu-id="9503c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9503c-137">DateTimeOffset</span></span>|<span data-ttu-id="9503c-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="9503c-138">DateTime the object was last modified.</span></span> <span data-ttu-id="9503c-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9503c-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9503c-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9503c-140">roleScopeTagIds</span></span>|<span data-ttu-id="9503c-141">String collection</span><span class="sxs-lookup"><span data-stu-id="9503c-141">String collection</span></span>|<span data-ttu-id="9503c-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="9503c-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9503c-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9503c-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9503c-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9503c-144">supportsScopeTags</span></span>|<span data-ttu-id="9503c-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="9503c-145">Boolean</span></span>|<span data-ttu-id="9503c-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="9503c-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9503c-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="9503c-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9503c-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="9503c-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9503c-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9503c-149">This property is read-only.</span></span> <span data-ttu-id="9503c-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9503c-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9503c-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9503c-151">createdDateTime</span></span>|<span data-ttu-id="9503c-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9503c-152">DateTimeOffset</span></span>|<span data-ttu-id="9503c-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="9503c-153">DateTime the object was created.</span></span> <span data-ttu-id="9503c-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9503c-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9503c-155">说明</span><span class="sxs-lookup"><span data-stu-id="9503c-155">description</span></span>|<span data-ttu-id="9503c-156">String</span><span class="sxs-lookup"><span data-stu-id="9503c-156">String</span></span>|<span data-ttu-id="9503c-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="9503c-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9503c-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9503c-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9503c-159">displayName</span><span class="sxs-lookup"><span data-stu-id="9503c-159">displayName</span></span>|<span data-ttu-id="9503c-160">String</span><span class="sxs-lookup"><span data-stu-id="9503c-160">String</span></span>|<span data-ttu-id="9503c-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="9503c-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9503c-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9503c-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9503c-163">version</span><span class="sxs-lookup"><span data-stu-id="9503c-163">version</span></span>|<span data-ttu-id="9503c-164">Int32</span><span class="sxs-lookup"><span data-stu-id="9503c-164">Int32</span></span>|<span data-ttu-id="9503c-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="9503c-165">Version of the device configuration.</span></span> <span data-ttu-id="9503c-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9503c-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9503c-167">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="9503c-167">deliveryOptimizationMode</span></span>|[<span data-ttu-id="9503c-168">windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="9503c-168">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="9503c-169">传递优化模式。</span><span class="sxs-lookup"><span data-stu-id="9503c-169">Delivery Optimization Mode.</span></span> <span data-ttu-id="9503c-170">可取值为：`userDefined`、`httpOnly`、`httpWithPeeringNat`、`httpWithPeeringPrivateGroup`、`httpWithInternetPeering`、`simpleDownload` 或 `bypassMode`。</span><span class="sxs-lookup"><span data-stu-id="9503c-170">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="9503c-171">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="9503c-171">prereleaseFeatures</span></span>|[<span data-ttu-id="9503c-172">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="9503c-172">prereleaseFeatures</span></span>](../resources/intune-deviceconfig-prereleasefeatures.md)|<span data-ttu-id="9503c-173">预发布功能。</span><span class="sxs-lookup"><span data-stu-id="9503c-173">The pre-release features.</span></span> <span data-ttu-id="9503c-174">可取值为：`userDefined`、`settingsOnly`、`settingsAndExperimentations`、`notAllowed`。</span><span class="sxs-lookup"><span data-stu-id="9503c-174">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="9503c-175">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="9503c-175">automaticUpdateMode</span></span>|[<span data-ttu-id="9503c-176">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="9503c-176">automaticUpdateMode</span></span>](../resources/intune-deviceconfig-automaticupdatemode.md)|<span data-ttu-id="9503c-177">自动更新模式。</span><span class="sxs-lookup"><span data-stu-id="9503c-177">Automatic update mode.</span></span> <span data-ttu-id="9503c-178">可取值为：`userDefined`、`notifyDownload`、`autoInstallAtMaintenanceTime`、`autoInstallAndRebootAtMaintenanceTime`、`autoInstallAndRebootAtScheduledTime`、`autoInstallAndRebootWithoutEndUserControl` 或 `windowsDefault`。</span><span class="sxs-lookup"><span data-stu-id="9503c-178">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`, `windowsDefault`.</span></span>|
|<span data-ttu-id="9503c-179">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="9503c-179">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="9503c-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="9503c-180">Boolean</span></span>|<span data-ttu-id="9503c-181">允许 Microsoft 更新服务</span><span class="sxs-lookup"><span data-stu-id="9503c-181">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="9503c-182">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="9503c-182">driversExcluded</span></span>|<span data-ttu-id="9503c-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="9503c-183">Boolean</span></span>|<span data-ttu-id="9503c-184">排除 Windows 更新驱动程序</span><span class="sxs-lookup"><span data-stu-id="9503c-184">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="9503c-185">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="9503c-185">installationSchedule</span></span>|[<span data-ttu-id="9503c-186">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="9503c-186">windowsUpdateInstallScheduleType</span></span>](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)|<span data-ttu-id="9503c-187">安装计划</span><span class="sxs-lookup"><span data-stu-id="9503c-187">Installation schedule</span></span>|
|<span data-ttu-id="9503c-188">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="9503c-188">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="9503c-189">Int32</span><span class="sxs-lookup"><span data-stu-id="9503c-189">Int32</span></span>|<span data-ttu-id="9503c-190">推迟质量更新的天数</span><span class="sxs-lookup"><span data-stu-id="9503c-190">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="9503c-191">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="9503c-191">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="9503c-192">Int32</span><span class="sxs-lookup"><span data-stu-id="9503c-192">Int32</span></span>|<span data-ttu-id="9503c-193">推迟功能更新的天数</span><span class="sxs-lookup"><span data-stu-id="9503c-193">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="9503c-194">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="9503c-194">qualityUpdatesPaused</span></span>|<span data-ttu-id="9503c-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="9503c-195">Boolean</span></span>|<span data-ttu-id="9503c-196">暂停质量更新</span><span class="sxs-lookup"><span data-stu-id="9503c-196">Pause Quality Updates</span></span>|
|<span data-ttu-id="9503c-197">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="9503c-197">featureUpdatesPaused</span></span>|<span data-ttu-id="9503c-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="9503c-198">Boolean</span></span>|<span data-ttu-id="9503c-199">暂停功能更新</span><span class="sxs-lookup"><span data-stu-id="9503c-199">Pause Feature Updates</span></span>|
|<span data-ttu-id="9503c-200">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="9503c-200">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="9503c-201">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9503c-201">DateTimeOffset</span></span>|<span data-ttu-id="9503c-202">质量更新暂停到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="9503c-202">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="9503c-203">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="9503c-203">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="9503c-204">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9503c-204">DateTimeOffset</span></span>|<span data-ttu-id="9503c-205">功能更新暂停到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="9503c-205">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="9503c-206">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="9503c-206">businessReadyUpdatesOnly</span></span>|[<span data-ttu-id="9503c-207">windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="9503c-207">windowsUpdateType</span></span>](../resources/intune-deviceconfig-windowsupdatetype.md)|<span data-ttu-id="9503c-208">确定将从哪些分支设备接收其更新。</span><span class="sxs-lookup"><span data-stu-id="9503c-208">Determines which branch devices will receive their updates from.</span></span> <span data-ttu-id="9503c-209">可取值为：`userDefined`、`all`、`businessReadyOnly`、`windowsInsiderBuildFast`、`windowsInsiderBuildSlow`、`windowsInsiderBuildRelease`。</span><span class="sxs-lookup"><span data-stu-id="9503c-209">Possible values are: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span></span>|
|<span data-ttu-id="9503c-210">skipChecksBeforeRestart</span><span class="sxs-lookup"><span data-stu-id="9503c-210">skipChecksBeforeRestart</span></span>|<span data-ttu-id="9503c-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="9503c-211">Boolean</span></span>|<span data-ttu-id="9503c-212">设置为在重新启动之前跳过所有复选: 电池级别 = 40%、用户状态、需要显示、演示模式、全屏模式、电话呼叫状态、游戏模式等。</span><span class="sxs-lookup"><span data-stu-id="9503c-212">Set to skip all check before restart: Battery level = 40%, User presence, Display Needed, Presentation mode, Full screen mode, phone call state, game mode etc.</span></span> |
|<span data-ttu-id="9503c-213">updateWeeks</span><span class="sxs-lookup"><span data-stu-id="9503c-213">updateWeeks</span></span>|[<span data-ttu-id="9503c-214">windowsUpdateForBusinessUpdateWeeks</span><span class="sxs-lookup"><span data-stu-id="9503c-214">windowsUpdateForBusinessUpdateWeeks</span></span>](../resources/intune-deviceconfig-windowsupdateforbusinessupdateweeks.md)|<span data-ttu-id="9503c-215">在每月的几周安排更新安装。</span><span class="sxs-lookup"><span data-stu-id="9503c-215">Scheduled the update installation on the weeks of the month.</span></span> <span data-ttu-id="9503c-216">可取值为：`userDefined`、`firstWeek`、`secondWeek`、`thirdWeek`、`fourthWeek`、`everyWeek`。</span><span class="sxs-lookup"><span data-stu-id="9503c-216">Possible values are: `userDefined`, `firstWeek`, `secondWeek`, `thirdWeek`, `fourthWeek`, `everyWeek`.</span></span>|
|<span data-ttu-id="9503c-217">qualityUpdatesPauseStartDate</span><span class="sxs-lookup"><span data-stu-id="9503c-217">qualityUpdatesPauseStartDate</span></span>|<span data-ttu-id="9503c-218">日期</span><span class="sxs-lookup"><span data-stu-id="9503c-218">Date</span></span>|<span data-ttu-id="9503c-219">质量更新暂停开始日期。</span><span class="sxs-lookup"><span data-stu-id="9503c-219">Quality Updates Pause start date.</span></span> <span data-ttu-id="9503c-220">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9503c-220">This property is read-only.</span></span>|
|<span data-ttu-id="9503c-221">featureUpdatesPauseStartDate</span><span class="sxs-lookup"><span data-stu-id="9503c-221">featureUpdatesPauseStartDate</span></span>|<span data-ttu-id="9503c-222">日期</span><span class="sxs-lookup"><span data-stu-id="9503c-222">Date</span></span>|<span data-ttu-id="9503c-223">功能更新暂停开始日期。</span><span class="sxs-lookup"><span data-stu-id="9503c-223">Feature Updates Pause start date.</span></span> <span data-ttu-id="9503c-224">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9503c-224">This property is read-only.</span></span>|
|<span data-ttu-id="9503c-225">featureUpdatesRollbackWindowInDays</span><span class="sxs-lookup"><span data-stu-id="9503c-225">featureUpdatesRollbackWindowInDays</span></span>|<span data-ttu-id="9503c-226">Int32</span><span class="sxs-lookup"><span data-stu-id="9503c-226">Int32</span></span>|<span data-ttu-id="9503c-227">回滚对其有效的功能更新后的天数</span><span class="sxs-lookup"><span data-stu-id="9503c-227">The number of days after a Feature Update for which a rollback is valid</span></span>|
|<span data-ttu-id="9503c-228">qualityUpdatesWillBeRolledBack</span><span class="sxs-lookup"><span data-stu-id="9503c-228">qualityUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="9503c-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="9503c-229">Boolean</span></span>|<span data-ttu-id="9503c-230">指定是否在下一个设备签入时回滚质量更新</span><span class="sxs-lookup"><span data-stu-id="9503c-230">Specifies whether to rollback Quality Updates on the next device check in</span></span>|
|<span data-ttu-id="9503c-231">featureUpdatesWillBeRolledBack</span><span class="sxs-lookup"><span data-stu-id="9503c-231">featureUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="9503c-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="9503c-232">Boolean</span></span>|<span data-ttu-id="9503c-233">指定是否在下一个设备签入时回滚功能更新</span><span class="sxs-lookup"><span data-stu-id="9503c-233">Specifies whether to rollback Feature Updates on the next device check in</span></span>|
|<span data-ttu-id="9503c-234">qualityUpdatesRollbackStartDateTime</span><span class="sxs-lookup"><span data-stu-id="9503c-234">qualityUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="9503c-235">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9503c-235">DateTimeOffset</span></span>|<span data-ttu-id="9503c-236">质量更新回滚开始日期/时间</span><span class="sxs-lookup"><span data-stu-id="9503c-236">Quality Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="9503c-237">featureUpdatesRollbackStartDateTime</span><span class="sxs-lookup"><span data-stu-id="9503c-237">featureUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="9503c-238">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9503c-238">DateTimeOffset</span></span>|<span data-ttu-id="9503c-239">功能更新回滚的开始日期时间</span><span class="sxs-lookup"><span data-stu-id="9503c-239">Feature Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="9503c-240">engagedRestartDeadlineInDays</span><span class="sxs-lookup"><span data-stu-id="9503c-240">engagedRestartDeadlineInDays</span></span>|<span data-ttu-id="9503c-241">Int32</span><span class="sxs-lookup"><span data-stu-id="9503c-241">Int32</span></span>|<span data-ttu-id="9503c-242">在非活动时段自动安排和执行挂起的重启的期限 (以天为单位), 有效范围为2到30天</span><span class="sxs-lookup"><span data-stu-id="9503c-242">Deadline in days before automatically scheduling and executing a pending restart outside of active hours, with valid range from 2 to 30 days</span></span>|
|<span data-ttu-id="9503c-243">engagedRestartSnoozeScheduleInDays</span><span class="sxs-lookup"><span data-stu-id="9503c-243">engagedRestartSnoozeScheduleInDays</span></span>|<span data-ttu-id="9503c-244">Int32</span><span class="sxs-lookup"><span data-stu-id="9503c-244">Int32</span></span>|<span data-ttu-id="9503c-245">用户可推迟预定重启提醒通知的天数, 有效范围为1到3天</span><span class="sxs-lookup"><span data-stu-id="9503c-245">Number of days a user can snooze Engaged Restart reminder notifications with valid range from 1 to 3 days</span></span>|
|<span data-ttu-id="9503c-246">engagedRestartTransitionScheduleInDays</span><span class="sxs-lookup"><span data-stu-id="9503c-246">engagedRestartTransitionScheduleInDays</span></span>|<span data-ttu-id="9503c-247">Int32</span><span class="sxs-lookup"><span data-stu-id="9503c-247">Int32</span></span>|<span data-ttu-id="9503c-248">从主动时段之外的计划的自动重启转换为预定重启 (需要用户进行计划, 有效范围为0到30天) 的天数</span><span class="sxs-lookup"><span data-stu-id="9503c-248">Number of days before transitioning from Auto Restarts scheduled outside of active hours to Engaged Restart, which requires the user to schedule, with valid range from 0 to 30 days</span></span>|
|<span data-ttu-id="9503c-249">autoRestartNotificationDismissal</span><span class="sxs-lookup"><span data-stu-id="9503c-249">autoRestartNotificationDismissal</span></span>|[<span data-ttu-id="9503c-250">autoRestartNotificationDismissalMethod</span><span class="sxs-lookup"><span data-stu-id="9503c-250">autoRestartNotificationDismissalMethod</span></span>](../resources/intune-deviceconfig-autorestartnotificationdismissalmethod.md)|<span data-ttu-id="9503c-251">指定用于消除 "需要自动重新启动" 通知的方法。</span><span class="sxs-lookup"><span data-stu-id="9503c-251">Specify the method by which the auto-restart required notification is dismissed.</span></span> <span data-ttu-id="9503c-252">可取值为：`notConfigured`、`automatic`、`user`。</span><span class="sxs-lookup"><span data-stu-id="9503c-252">Possible values are: `notConfigured`, `automatic`, `user`.</span></span>|
|<span data-ttu-id="9503c-253">scheduleRestartWarningInHours</span><span class="sxs-lookup"><span data-stu-id="9503c-253">scheduleRestartWarningInHours</span></span>|<span data-ttu-id="9503c-254">Int32</span><span class="sxs-lookup"><span data-stu-id="9503c-254">Int32</span></span>|<span data-ttu-id="9503c-255">指定自动重新启动警告提醒通知的期限。</span><span class="sxs-lookup"><span data-stu-id="9503c-255">Specify the period for auto-restart warning reminder notifications.</span></span> <span data-ttu-id="9503c-256">支持的值: 2、4、8、12或 24 (小时)。</span><span class="sxs-lookup"><span data-stu-id="9503c-256">Supported values: 2, 4, 8, 12 or 24 (hours).</span></span>|
|<span data-ttu-id="9503c-257">scheduleImminentRestartWarningInMinutes</span><span class="sxs-lookup"><span data-stu-id="9503c-257">scheduleImminentRestartWarningInMinutes</span></span>|<span data-ttu-id="9503c-258">Int32</span><span class="sxs-lookup"><span data-stu-id="9503c-258">Int32</span></span>|<span data-ttu-id="9503c-259">指定自动重启即将发生的警告通知的期限。</span><span class="sxs-lookup"><span data-stu-id="9503c-259">Specify the period for auto-restart imminent warning notifications.</span></span> <span data-ttu-id="9503c-260">支持的值:15、30或 60 (分钟)。</span><span class="sxs-lookup"><span data-stu-id="9503c-260">Supported values: 15, 30 or 60 (minutes).</span></span>|
|<span data-ttu-id="9503c-261">userPauseAccess</span><span class="sxs-lookup"><span data-stu-id="9503c-261">userPauseAccess</span></span>|[<span data-ttu-id="9503c-262">启用</span><span class="sxs-lookup"><span data-stu-id="9503c-262">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="9503c-263">指定是否允许最终用户访问暂停软件更新。</span><span class="sxs-lookup"><span data-stu-id="9503c-263">Specifies whether to enable end user’s access to pause software updates.</span></span> <span data-ttu-id="9503c-264">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="9503c-264">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="9503c-265">userWindowsUpdateScanAccess</span><span class="sxs-lookup"><span data-stu-id="9503c-265">userWindowsUpdateScanAccess</span></span>|[<span data-ttu-id="9503c-266">启用</span><span class="sxs-lookup"><span data-stu-id="9503c-266">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="9503c-267">指定是否禁用用户对扫描 Windows 更新的访问权限。</span><span class="sxs-lookup"><span data-stu-id="9503c-267">Specifies whether to disable user’s access to scan Windows Update.</span></span> <span data-ttu-id="9503c-268">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="9503c-268">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="9503c-269">updateNotificationLevel</span><span class="sxs-lookup"><span data-stu-id="9503c-269">updateNotificationLevel</span></span>|[<span data-ttu-id="9503c-270">windowsUpdateNotificationDisplayOption</span><span class="sxs-lookup"><span data-stu-id="9503c-270">windowsUpdateNotificationDisplayOption</span></span>](../resources/intune-deviceconfig-windowsupdatenotificationdisplayoption.md)|<span data-ttu-id="9503c-271">指定用户看到的 Windows 更新通知的具体内容。</span><span class="sxs-lookup"><span data-stu-id="9503c-271">Specifies what Windows Update notifications users see.</span></span> <span data-ttu-id="9503c-272">可取值为：`notConfigured`、`defaultNotifications`、`restartWarningsOnly`、`disableAllNotifications`。</span><span class="sxs-lookup"><span data-stu-id="9503c-272">Possible values are: `notConfigured`, `defaultNotifications`, `restartWarningsOnly`, `disableAllNotifications`.</span></span>|



## <a name="response"></a><span data-ttu-id="9503c-273">响应</span><span class="sxs-lookup"><span data-stu-id="9503c-273">Response</span></span>
<span data-ttu-id="9503c-274">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9503c-274">If successful, this method returns a `201 Created` response code and a [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9503c-275">示例</span><span class="sxs-lookup"><span data-stu-id="9503c-275">Example</span></span>

### <a name="request"></a><span data-ttu-id="9503c-276">请求</span><span class="sxs-lookup"><span data-stu-id="9503c-276">Request</span></span>
<span data-ttu-id="9503c-277">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9503c-277">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="9503c-278">响应</span><span class="sxs-lookup"><span data-stu-id="9503c-278">Response</span></span>
<span data-ttu-id="9503c-p123">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9503c-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




