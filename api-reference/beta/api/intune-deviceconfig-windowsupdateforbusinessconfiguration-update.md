---
title: 更新 windowsUpdateForBusinessConfiguration
description: 更新 windowsUpdateForBusinessConfiguration 对象的属性。
author: tfitzmac
ms.openlocfilehash: b887fe448a574f774cb45cd946cb1bf535c9f3b9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307355"
---
# <a name="update-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="87ac1-103">更新 windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="87ac1-103">Update windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="87ac1-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="87ac1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="87ac1-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="87ac1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="87ac1-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="87ac1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="87ac1-107">更新 [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="87ac1-107">Update the properties of a [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="87ac1-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="87ac1-108">Prerequisites</span></span>
<span data-ttu-id="87ac1-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="87ac1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87ac1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="87ac1-111">Permission type</span></span>|<span data-ttu-id="87ac1-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="87ac1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87ac1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="87ac1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="87ac1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87ac1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="87ac1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="87ac1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87ac1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="87ac1-116">Not supported.</span></span>|
|<span data-ttu-id="87ac1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="87ac1-117">Application</span></span>|<span data-ttu-id="87ac1-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="87ac1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="87ac1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="87ac1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="87ac1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="87ac1-120">Request headers</span></span>
|<span data-ttu-id="87ac1-121">标头</span><span class="sxs-lookup"><span data-stu-id="87ac1-121">Header</span></span>|<span data-ttu-id="87ac1-122">值</span><span class="sxs-lookup"><span data-stu-id="87ac1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87ac1-123">授权</span><span class="sxs-lookup"><span data-stu-id="87ac1-123">Authorization</span></span>|<span data-ttu-id="87ac1-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="87ac1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87ac1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="87ac1-125">Accept</span></span>|<span data-ttu-id="87ac1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="87ac1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87ac1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="87ac1-127">Request body</span></span>
<span data-ttu-id="87ac1-128">在请求正文中，提供 [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="87ac1-128">In the request body, supply a JSON representation for the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="87ac1-129">下表显示创建 [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="87ac1-129">The following table shows the properties that are required when you create the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="87ac1-130">属性</span><span class="sxs-lookup"><span data-stu-id="87ac1-130">Property</span></span>|<span data-ttu-id="87ac1-131">类型</span><span class="sxs-lookup"><span data-stu-id="87ac1-131">Type</span></span>|<span data-ttu-id="87ac1-132">说明</span><span class="sxs-lookup"><span data-stu-id="87ac1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87ac1-133">id</span><span class="sxs-lookup"><span data-stu-id="87ac1-133">id</span></span>|<span data-ttu-id="87ac1-134">String</span><span class="sxs-lookup"><span data-stu-id="87ac1-134">String</span></span>|<span data-ttu-id="87ac1-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="87ac1-135">Key of the entity.</span></span> <span data-ttu-id="87ac1-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="87ac1-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87ac1-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="87ac1-137">lastModifiedDateTime</span></span>|<span data-ttu-id="87ac1-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87ac1-138">DateTimeOffset</span></span>|<span data-ttu-id="87ac1-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="87ac1-139">DateTime the object was last modified.</span></span> <span data-ttu-id="87ac1-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="87ac1-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87ac1-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="87ac1-141">roleScopeTagIds</span></span>|<span data-ttu-id="87ac1-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="87ac1-142">String collection</span></span>|<span data-ttu-id="87ac1-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="87ac1-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="87ac1-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="87ac1-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87ac1-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="87ac1-145">supportsScopeTags</span></span>|<span data-ttu-id="87ac1-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="87ac1-146">Boolean</span></span>|<span data-ttu-id="87ac1-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="87ac1-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="87ac1-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="87ac1-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="87ac1-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="87ac1-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="87ac1-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="87ac1-150">This property is read-only.</span></span> <span data-ttu-id="87ac1-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="87ac1-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87ac1-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="87ac1-152">createdDateTime</span></span>|<span data-ttu-id="87ac1-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87ac1-153">DateTimeOffset</span></span>|<span data-ttu-id="87ac1-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="87ac1-154">DateTime the object was created.</span></span> <span data-ttu-id="87ac1-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="87ac1-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87ac1-156">description</span><span class="sxs-lookup"><span data-stu-id="87ac1-156">description</span></span>|<span data-ttu-id="87ac1-157">String</span><span class="sxs-lookup"><span data-stu-id="87ac1-157">String</span></span>|<span data-ttu-id="87ac1-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="87ac1-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="87ac1-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="87ac1-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87ac1-160">displayName</span><span class="sxs-lookup"><span data-stu-id="87ac1-160">displayName</span></span>|<span data-ttu-id="87ac1-161">String</span><span class="sxs-lookup"><span data-stu-id="87ac1-161">String</span></span>|<span data-ttu-id="87ac1-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="87ac1-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="87ac1-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="87ac1-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87ac1-164">version</span><span class="sxs-lookup"><span data-stu-id="87ac1-164">version</span></span>|<span data-ttu-id="87ac1-165">Int32</span><span class="sxs-lookup"><span data-stu-id="87ac1-165">Int32</span></span>|<span data-ttu-id="87ac1-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="87ac1-166">Version of the device configuration.</span></span> <span data-ttu-id="87ac1-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="87ac1-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87ac1-168">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="87ac1-168">deliveryOptimizationMode</span></span>|[<span data-ttu-id="87ac1-169">windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="87ac1-169">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="87ac1-170">传递优化模式。</span><span class="sxs-lookup"><span data-stu-id="87ac1-170">Delivery Optimization Mode.</span></span> <span data-ttu-id="87ac1-171">可取值为：`userDefined`、`httpOnly`、`httpWithPeeringNat`、`httpWithPeeringPrivateGroup`、`httpWithInternetPeering`、`simpleDownload`、`bypassMode`。</span><span class="sxs-lookup"><span data-stu-id="87ac1-171">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="87ac1-172">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="87ac1-172">prereleaseFeatures</span></span>|[<span data-ttu-id="87ac1-173">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="87ac1-173">prereleaseFeatures</span></span>](../resources/intune-deviceconfig-prereleasefeatures.md)|<span data-ttu-id="87ac1-174">预发布功能。</span><span class="sxs-lookup"><span data-stu-id="87ac1-174">The pre-release features.</span></span> <span data-ttu-id="87ac1-175">可取值为：`userDefined`、`settingsOnly`、`settingsAndExperimentations`、`notAllowed`。</span><span class="sxs-lookup"><span data-stu-id="87ac1-175">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="87ac1-176">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="87ac1-176">automaticUpdateMode</span></span>|[<span data-ttu-id="87ac1-177">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="87ac1-177">automaticUpdateMode</span></span>](../resources/intune-deviceconfig-automaticupdatemode.md)|<span data-ttu-id="87ac1-178">自动更新模式。</span><span class="sxs-lookup"><span data-stu-id="87ac1-178">Automatic update mode.</span></span> <span data-ttu-id="87ac1-179">可取值为：`userDefined`、`notifyDownload`、`autoInstallAtMaintenanceTime`、`autoInstallAndRebootAtMaintenanceTime`、`autoInstallAndRebootAtScheduledTime`、`autoInstallAndRebootWithoutEndUserControl`。</span><span class="sxs-lookup"><span data-stu-id="87ac1-179">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`.</span></span>|
|<span data-ttu-id="87ac1-180">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="87ac1-180">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="87ac1-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="87ac1-181">Boolean</span></span>|<span data-ttu-id="87ac1-182">允许 Microsoft 更新服务</span><span class="sxs-lookup"><span data-stu-id="87ac1-182">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="87ac1-183">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="87ac1-183">driversExcluded</span></span>|<span data-ttu-id="87ac1-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="87ac1-184">Boolean</span></span>|<span data-ttu-id="87ac1-185">排除 Windows 更新驱动程序</span><span class="sxs-lookup"><span data-stu-id="87ac1-185">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="87ac1-186">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="87ac1-186">installationSchedule</span></span>|[<span data-ttu-id="87ac1-187">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="87ac1-187">windowsUpdateInstallScheduleType</span></span>](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)|<span data-ttu-id="87ac1-188">安装计划</span><span class="sxs-lookup"><span data-stu-id="87ac1-188">Installation schedule</span></span>|
|<span data-ttu-id="87ac1-189">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="87ac1-189">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="87ac1-190">Int32</span><span class="sxs-lookup"><span data-stu-id="87ac1-190">Int32</span></span>|<span data-ttu-id="87ac1-191">推迟质量更新的天数</span><span class="sxs-lookup"><span data-stu-id="87ac1-191">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="87ac1-192">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="87ac1-192">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="87ac1-193">Int32</span><span class="sxs-lookup"><span data-stu-id="87ac1-193">Int32</span></span>|<span data-ttu-id="87ac1-194">推迟功能更新的天数</span><span class="sxs-lookup"><span data-stu-id="87ac1-194">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="87ac1-195">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="87ac1-195">qualityUpdatesPaused</span></span>|<span data-ttu-id="87ac1-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="87ac1-196">Boolean</span></span>|<span data-ttu-id="87ac1-197">暂停质量更新</span><span class="sxs-lookup"><span data-stu-id="87ac1-197">Pause Quality Updates</span></span>|
|<span data-ttu-id="87ac1-198">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="87ac1-198">featureUpdatesPaused</span></span>|<span data-ttu-id="87ac1-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="87ac1-199">Boolean</span></span>|<span data-ttu-id="87ac1-200">暂停功能更新</span><span class="sxs-lookup"><span data-stu-id="87ac1-200">Pause Feature Updates</span></span>|
|<span data-ttu-id="87ac1-201">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="87ac1-201">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="87ac1-202">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87ac1-202">DateTimeOffset</span></span>|<span data-ttu-id="87ac1-203">质量更新暂停到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="87ac1-203">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="87ac1-204">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="87ac1-204">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="87ac1-205">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87ac1-205">DateTimeOffset</span></span>|<span data-ttu-id="87ac1-206">功能更新暂停到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="87ac1-206">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="87ac1-207">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="87ac1-207">businessReadyUpdatesOnly</span></span>|[<span data-ttu-id="87ac1-208">windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="87ac1-208">windowsUpdateType</span></span>](../resources/intune-deviceconfig-windowsupdatetype.md)|<span data-ttu-id="87ac1-209">确定哪些分支设备将接收从其更新。</span><span class="sxs-lookup"><span data-stu-id="87ac1-209">Determines which branch devices will receive their updates from.</span></span> <span data-ttu-id="87ac1-210">可取值为：`userDefined`、`all`、`businessReadyOnly`、`windowsInsiderBuildFast`、`windowsInsiderBuildSlow`、`windowsInsiderBuildRelease`。</span><span class="sxs-lookup"><span data-stu-id="87ac1-210">Possible values are: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span></span>|
|<span data-ttu-id="87ac1-211">skipChecksBeforeRestart</span><span class="sxs-lookup"><span data-stu-id="87ac1-211">skipChecksBeforeRestart</span></span>|<span data-ttu-id="87ac1-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="87ac1-212">Boolean</span></span>|<span data-ttu-id="87ac1-213">设置要跳过之前重新启动所有检查： 电池级别 = 40%，用户状态显示需要演示文稿模式下、 全屏幕模式、 电话呼叫状态、 游戏模式等。</span><span class="sxs-lookup"><span data-stu-id="87ac1-213">Set to skip all check before restart: Battery level = 40%, User presence, Display Needed, Presentation mode, Full screen mode, phone call state, game mode etc.</span></span> |
|<span data-ttu-id="87ac1-214">updateWeeks</span><span class="sxs-lookup"><span data-stu-id="87ac1-214">updateWeeks</span></span>|[<span data-ttu-id="87ac1-215">windowsUpdateForBusinessUpdateWeeks</span><span class="sxs-lookup"><span data-stu-id="87ac1-215">windowsUpdateForBusinessUpdateWeeks</span></span>](../resources/intune-deviceconfig-windowsupdateforbusinessupdateweeks.md)|<span data-ttu-id="87ac1-216">计划更新安装在相应月份的周。</span><span class="sxs-lookup"><span data-stu-id="87ac1-216">Scheduled the update installation on the weeks of the month.</span></span> <span data-ttu-id="87ac1-217">可取值为：`userDefined`、`firstWeek`、`secondWeek`、`thirdWeek`、`fourthWeek`、`everyWeek`。</span><span class="sxs-lookup"><span data-stu-id="87ac1-217">Possible values are: `userDefined`, `firstWeek`, `secondWeek`, `thirdWeek`, `fourthWeek`, `everyWeek`.</span></span>|
|<span data-ttu-id="87ac1-218">qualityUpdatesPauseStartDateTime</span><span class="sxs-lookup"><span data-stu-id="87ac1-218">qualityUpdatesPauseStartDateTime</span></span>|<span data-ttu-id="87ac1-219">字符串</span><span class="sxs-lookup"><span data-stu-id="87ac1-219">String</span></span>|<span data-ttu-id="87ac1-220">质量更新暂停开始日期时间</span><span class="sxs-lookup"><span data-stu-id="87ac1-220">Quality Updates Pause Start datetime</span></span>|
|<span data-ttu-id="87ac1-221">featureUpdatesPauseStartDateTime</span><span class="sxs-lookup"><span data-stu-id="87ac1-221">featureUpdatesPauseStartDateTime</span></span>|<span data-ttu-id="87ac1-222">字符串</span><span class="sxs-lookup"><span data-stu-id="87ac1-222">String</span></span>|<span data-ttu-id="87ac1-223">功能更新暂停开始日期时间</span><span class="sxs-lookup"><span data-stu-id="87ac1-223">Feature Updates Pause Start datetime</span></span>|
|<span data-ttu-id="87ac1-224">featureUpdatesRollbackWindowInDays</span><span class="sxs-lookup"><span data-stu-id="87ac1-224">featureUpdatesRollbackWindowInDays</span></span>|<span data-ttu-id="87ac1-225">Int32</span><span class="sxs-lookup"><span data-stu-id="87ac1-225">Int32</span></span>|<span data-ttu-id="87ac1-226">回滚的有效功能更新后的天数</span><span class="sxs-lookup"><span data-stu-id="87ac1-226">The number of days after a Feature Update for which a rollback is valid</span></span>|
|<span data-ttu-id="87ac1-227">qualityUpdatesWillBeRolledBack</span><span class="sxs-lookup"><span data-stu-id="87ac1-227">qualityUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="87ac1-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="87ac1-228">Boolean</span></span>|<span data-ttu-id="87ac1-229">指定是否回滚到下一个设备质量更新签入</span><span class="sxs-lookup"><span data-stu-id="87ac1-229">Specifies whether to rollback Quality Updates on the next device check in</span></span>|
|<span data-ttu-id="87ac1-230">featureUpdatesWillBeRolledBack</span><span class="sxs-lookup"><span data-stu-id="87ac1-230">featureUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="87ac1-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="87ac1-231">Boolean</span></span>|<span data-ttu-id="87ac1-232">指定是否回滚到下一个设备上的功能更新签入</span><span class="sxs-lookup"><span data-stu-id="87ac1-232">Specifies whether to rollback Feature Updates on the next device check in</span></span>|
|<span data-ttu-id="87ac1-233">qualityUpdatesRollbackStartDateTime</span><span class="sxs-lookup"><span data-stu-id="87ac1-233">qualityUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="87ac1-234">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87ac1-234">DateTimeOffset</span></span>|<span data-ttu-id="87ac1-235">质量更新回滚开始日期时间</span><span class="sxs-lookup"><span data-stu-id="87ac1-235">Quality Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="87ac1-236">featureUpdatesRollbackStartDateTime</span><span class="sxs-lookup"><span data-stu-id="87ac1-236">featureUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="87ac1-237">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87ac1-237">DateTimeOffset</span></span>|<span data-ttu-id="87ac1-238">功能更新回滚开始日期时间</span><span class="sxs-lookup"><span data-stu-id="87ac1-238">Feature Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="87ac1-239">engagedRestartDeadlineInDays</span><span class="sxs-lookup"><span data-stu-id="87ac1-239">engagedRestartDeadlineInDays</span></span>|<span data-ttu-id="87ac1-240">Int32</span><span class="sxs-lookup"><span data-stu-id="87ac1-240">Int32</span></span>|<span data-ttu-id="87ac1-241">自动计划并执行挂起的重新启动之外活动的小时，与有效范围为从 2 到 30 天之前的天数的截止日期</span><span class="sxs-lookup"><span data-stu-id="87ac1-241">Deadline in days before automatically scheduling and executing a pending restart outside of active hours, with valid range from 2 to 30 days</span></span>|
|<span data-ttu-id="87ac1-242">engagedRestartSnoozeScheduleInDays</span><span class="sxs-lookup"><span data-stu-id="87ac1-242">engagedRestartSnoozeScheduleInDays</span></span>|<span data-ttu-id="87ac1-243">Int32</span><span class="sxs-lookup"><span data-stu-id="87ac1-243">Int32</span></span>|<span data-ttu-id="87ac1-244">用户可以 snooze 有效范围为从 1 到 3 天具有正在重新启动提醒通知的天数</span><span class="sxs-lookup"><span data-stu-id="87ac1-244">Number of days a user can snooze Engaged Restart reminder notifications with valid range from 1 to 3 days</span></span>|
|<span data-ttu-id="87ac1-245">engagedRestartTransitionScheduleInDays</span><span class="sxs-lookup"><span data-stu-id="87ac1-245">engagedRestartTransitionScheduleInDays</span></span>|<span data-ttu-id="87ac1-246">Int32</span><span class="sxs-lookup"><span data-stu-id="87ac1-246">Int32</span></span>|<span data-ttu-id="87ac1-247">从自动重新启动计划非活动时间正在重新要求用户安排与有效范围为从 0 到 30 天发出转换之前的天数</span><span class="sxs-lookup"><span data-stu-id="87ac1-247">Number of days before transitioning from Auto Restarts scheduled outside of active hours to Engaged Restart, which requires the user to schedule, with valid range from 0 to 30 days</span></span>|
|<span data-ttu-id="87ac1-248">autoRestartNotificationDismissal</span><span class="sxs-lookup"><span data-stu-id="87ac1-248">autoRestartNotificationDismissal</span></span>|[<span data-ttu-id="87ac1-249">autoRestartNotificationDismissalMethod</span><span class="sxs-lookup"><span data-stu-id="87ac1-249">autoRestartNotificationDismissalMethod</span></span>](../resources/intune-deviceconfig-autorestartnotificationdismissalmethod.md)|<span data-ttu-id="87ac1-250">指定按其在自动重新启动所需消除通知的方法。</span><span class="sxs-lookup"><span data-stu-id="87ac1-250">Specify the method by which the auto-restart required notification is dismissed.</span></span> <span data-ttu-id="87ac1-251">可取值为：`notConfigured`、`automatic`、`user`。</span><span class="sxs-lookup"><span data-stu-id="87ac1-251">Possible values are: `notConfigured`, `automatic`, `user`.</span></span>|
|<span data-ttu-id="87ac1-252">scheduleRestartWarningInHours</span><span class="sxs-lookup"><span data-stu-id="87ac1-252">scheduleRestartWarningInHours</span></span>|<span data-ttu-id="87ac1-253">Int32</span><span class="sxs-lookup"><span data-stu-id="87ac1-253">Int32</span></span>|<span data-ttu-id="87ac1-254">指定自动重新启动警告提醒通知的时间段。</span><span class="sxs-lookup"><span data-stu-id="87ac1-254">Specify the period for auto-restart warning reminder notifications.</span></span> <span data-ttu-id="87ac1-255">支持值： 2、 4、 8、 12 或 24 （小时）。</span><span class="sxs-lookup"><span data-stu-id="87ac1-255">Supported values: 2, 4, 8, 12 or 24 (hours).</span></span>|
|<span data-ttu-id="87ac1-256">scheduleImminentRestartWarningInMinutes</span><span class="sxs-lookup"><span data-stu-id="87ac1-256">scheduleImminentRestartWarningInMinutes</span></span>|<span data-ttu-id="87ac1-257">Int32</span><span class="sxs-lookup"><span data-stu-id="87ac1-257">Int32</span></span>|<span data-ttu-id="87ac1-258">指定自动重新启动即将发生警告通知的时间段。</span><span class="sxs-lookup"><span data-stu-id="87ac1-258">Specify the period for auto-restart imminent warning notifications.</span></span> <span data-ttu-id="87ac1-259">支持值： 15、 30 或 60 （分钟）。</span><span class="sxs-lookup"><span data-stu-id="87ac1-259">Supported values: 15, 30 or 60 (minutes).</span></span>|



## <a name="response"></a><span data-ttu-id="87ac1-260">响应</span><span class="sxs-lookup"><span data-stu-id="87ac1-260">Response</span></span>
<span data-ttu-id="87ac1-261">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="87ac1-261">If successful, this method returns a `200 OK` response code and an updated [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87ac1-262">示例</span><span class="sxs-lookup"><span data-stu-id="87ac1-262">Example</span></span>
### <a name="request"></a><span data-ttu-id="87ac1-263">请求</span><span class="sxs-lookup"><span data-stu-id="87ac1-263">Request</span></span>
<span data-ttu-id="87ac1-264">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="87ac1-264">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1787

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
  "qualityUpdatesPauseStartDateTime": "Quality Updates Pause Start Date Time value",
  "featureUpdatesPauseStartDateTime": "Feature Updates Pause Start Date Time value",
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
  "scheduleImminentRestartWarningInMinutes": 7
}
```

### <a name="response"></a><span data-ttu-id="87ac1-265">响应</span><span class="sxs-lookup"><span data-stu-id="87ac1-265">Response</span></span>
<span data-ttu-id="87ac1-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="87ac1-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1971

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
  "qualityUpdatesPauseStartDateTime": "Quality Updates Pause Start Date Time value",
  "featureUpdatesPauseStartDateTime": "Feature Updates Pause Start Date Time value",
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
  "scheduleImminentRestartWarningInMinutes": 7
}
```





