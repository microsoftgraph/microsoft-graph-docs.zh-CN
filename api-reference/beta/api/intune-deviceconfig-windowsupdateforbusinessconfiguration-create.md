---
title: 创建 windowsUpdateForBusinessConfiguration
description: 创建新的 windowsUpdateForBusinessConfiguration 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: dade72412a64b5703fa253eda0a40829f2475549
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406190"
---
# <a name="create-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="d17d6-103">创建 windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="d17d6-103">Create windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="d17d6-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="d17d6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d17d6-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d17d6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d17d6-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d17d6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d17d6-107">创建新的 [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d17d6-107">Create a new [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d17d6-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d17d6-108">Prerequisites</span></span>
<span data-ttu-id="d17d6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="d17d6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d17d6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d17d6-111">Permission type</span></span>|<span data-ttu-id="d17d6-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d17d6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d17d6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d17d6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d17d6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d17d6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d17d6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d17d6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d17d6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d17d6-116">Not supported.</span></span>|
|<span data-ttu-id="d17d6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d17d6-117">Application</span></span>|<span data-ttu-id="d17d6-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="d17d6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d17d6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d17d6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d17d6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d17d6-120">Request headers</span></span>
|<span data-ttu-id="d17d6-121">标头</span><span class="sxs-lookup"><span data-stu-id="d17d6-121">Header</span></span>|<span data-ttu-id="d17d6-122">值</span><span class="sxs-lookup"><span data-stu-id="d17d6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d17d6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d17d6-123">Authorization</span></span>|<span data-ttu-id="d17d6-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d17d6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d17d6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d17d6-125">Accept</span></span>|<span data-ttu-id="d17d6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d17d6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d17d6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d17d6-127">Request body</span></span>
<span data-ttu-id="d17d6-128">在请求正文中，提供 windowsUpdateForBusinessConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d17d6-128">In the request body, supply a JSON representation for the windowsUpdateForBusinessConfiguration object.</span></span>

<span data-ttu-id="d17d6-129">下表显示创建 windowsUpdateForBusinessConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d17d6-129">The following table shows the properties that are required when you create the windowsUpdateForBusinessConfiguration.</span></span>

|<span data-ttu-id="d17d6-130">属性</span><span class="sxs-lookup"><span data-stu-id="d17d6-130">Property</span></span>|<span data-ttu-id="d17d6-131">类型</span><span class="sxs-lookup"><span data-stu-id="d17d6-131">Type</span></span>|<span data-ttu-id="d17d6-132">说明</span><span class="sxs-lookup"><span data-stu-id="d17d6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d17d6-133">id</span><span class="sxs-lookup"><span data-stu-id="d17d6-133">id</span></span>|<span data-ttu-id="d17d6-134">String</span><span class="sxs-lookup"><span data-stu-id="d17d6-134">String</span></span>|<span data-ttu-id="d17d6-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d17d6-135">Key of the entity.</span></span> <span data-ttu-id="d17d6-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d17d6-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d17d6-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d17d6-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d17d6-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d17d6-138">DateTimeOffset</span></span>|<span data-ttu-id="d17d6-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d17d6-139">DateTime the object was last modified.</span></span> <span data-ttu-id="d17d6-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d17d6-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d17d6-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d17d6-141">roleScopeTagIds</span></span>|<span data-ttu-id="d17d6-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="d17d6-142">String collection</span></span>|<span data-ttu-id="d17d6-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="d17d6-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d17d6-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d17d6-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d17d6-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d17d6-145">supportsScopeTags</span></span>|<span data-ttu-id="d17d6-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="d17d6-146">Boolean</span></span>|<span data-ttu-id="d17d6-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="d17d6-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d17d6-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="d17d6-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d17d6-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="d17d6-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d17d6-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="d17d6-150">This property is read-only.</span></span> <span data-ttu-id="d17d6-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d17d6-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d17d6-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d17d6-152">createdDateTime</span></span>|<span data-ttu-id="d17d6-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d17d6-153">DateTimeOffset</span></span>|<span data-ttu-id="d17d6-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d17d6-154">DateTime the object was created.</span></span> <span data-ttu-id="d17d6-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d17d6-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d17d6-156">description</span><span class="sxs-lookup"><span data-stu-id="d17d6-156">description</span></span>|<span data-ttu-id="d17d6-157">String</span><span class="sxs-lookup"><span data-stu-id="d17d6-157">String</span></span>|<span data-ttu-id="d17d6-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="d17d6-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d17d6-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d17d6-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d17d6-160">displayName</span><span class="sxs-lookup"><span data-stu-id="d17d6-160">displayName</span></span>|<span data-ttu-id="d17d6-161">String</span><span class="sxs-lookup"><span data-stu-id="d17d6-161">String</span></span>|<span data-ttu-id="d17d6-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="d17d6-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d17d6-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d17d6-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d17d6-164">version</span><span class="sxs-lookup"><span data-stu-id="d17d6-164">version</span></span>|<span data-ttu-id="d17d6-165">Int32</span><span class="sxs-lookup"><span data-stu-id="d17d6-165">Int32</span></span>|<span data-ttu-id="d17d6-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="d17d6-166">Version of the device configuration.</span></span> <span data-ttu-id="d17d6-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d17d6-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d17d6-168">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="d17d6-168">deliveryOptimizationMode</span></span>|[<span data-ttu-id="d17d6-169">windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="d17d6-169">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="d17d6-170">传递优化模式。</span><span class="sxs-lookup"><span data-stu-id="d17d6-170">Delivery Optimization Mode.</span></span> <span data-ttu-id="d17d6-171">可取值为：`userDefined`、`httpOnly`、`httpWithPeeringNat`、`httpWithPeeringPrivateGroup`、`httpWithInternetPeering`、`simpleDownload`、`bypassMode`。</span><span class="sxs-lookup"><span data-stu-id="d17d6-171">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="d17d6-172">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="d17d6-172">prereleaseFeatures</span></span>|[<span data-ttu-id="d17d6-173">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="d17d6-173">prereleaseFeatures</span></span>](../resources/intune-deviceconfig-prereleasefeatures.md)|<span data-ttu-id="d17d6-174">预发布功能。</span><span class="sxs-lookup"><span data-stu-id="d17d6-174">The pre-release features.</span></span> <span data-ttu-id="d17d6-175">可取值为：`userDefined`、`settingsOnly`、`settingsAndExperimentations`、`notAllowed`。</span><span class="sxs-lookup"><span data-stu-id="d17d6-175">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="d17d6-176">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="d17d6-176">automaticUpdateMode</span></span>|[<span data-ttu-id="d17d6-177">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="d17d6-177">automaticUpdateMode</span></span>](../resources/intune-deviceconfig-automaticupdatemode.md)|<span data-ttu-id="d17d6-178">自动更新模式。</span><span class="sxs-lookup"><span data-stu-id="d17d6-178">Automatic update mode.</span></span> <span data-ttu-id="d17d6-179">可取值为：`userDefined`、`notifyDownload`、`autoInstallAtMaintenanceTime`、`autoInstallAndRebootAtMaintenanceTime`、`autoInstallAndRebootAtScheduledTime`、`autoInstallAndRebootWithoutEndUserControl`、`windowsDefault`。</span><span class="sxs-lookup"><span data-stu-id="d17d6-179">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`, `windowsDefault`.</span></span>|
|<span data-ttu-id="d17d6-180">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="d17d6-180">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="d17d6-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="d17d6-181">Boolean</span></span>|<span data-ttu-id="d17d6-182">允许 Microsoft 更新服务</span><span class="sxs-lookup"><span data-stu-id="d17d6-182">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="d17d6-183">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="d17d6-183">driversExcluded</span></span>|<span data-ttu-id="d17d6-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="d17d6-184">Boolean</span></span>|<span data-ttu-id="d17d6-185">排除 Windows 更新驱动程序</span><span class="sxs-lookup"><span data-stu-id="d17d6-185">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="d17d6-186">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="d17d6-186">installationSchedule</span></span>|[<span data-ttu-id="d17d6-187">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="d17d6-187">windowsUpdateInstallScheduleType</span></span>](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)|<span data-ttu-id="d17d6-188">安装计划</span><span class="sxs-lookup"><span data-stu-id="d17d6-188">Installation schedule</span></span>|
|<span data-ttu-id="d17d6-189">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="d17d6-189">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="d17d6-190">Int32</span><span class="sxs-lookup"><span data-stu-id="d17d6-190">Int32</span></span>|<span data-ttu-id="d17d6-191">推迟质量更新的天数</span><span class="sxs-lookup"><span data-stu-id="d17d6-191">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="d17d6-192">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="d17d6-192">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="d17d6-193">Int32</span><span class="sxs-lookup"><span data-stu-id="d17d6-193">Int32</span></span>|<span data-ttu-id="d17d6-194">推迟功能更新的天数</span><span class="sxs-lookup"><span data-stu-id="d17d6-194">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="d17d6-195">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="d17d6-195">qualityUpdatesPaused</span></span>|<span data-ttu-id="d17d6-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="d17d6-196">Boolean</span></span>|<span data-ttu-id="d17d6-197">暂停质量更新</span><span class="sxs-lookup"><span data-stu-id="d17d6-197">Pause Quality Updates</span></span>|
|<span data-ttu-id="d17d6-198">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="d17d6-198">featureUpdatesPaused</span></span>|<span data-ttu-id="d17d6-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="d17d6-199">Boolean</span></span>|<span data-ttu-id="d17d6-200">暂停功能更新</span><span class="sxs-lookup"><span data-stu-id="d17d6-200">Pause Feature Updates</span></span>|
|<span data-ttu-id="d17d6-201">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="d17d6-201">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="d17d6-202">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d17d6-202">DateTimeOffset</span></span>|<span data-ttu-id="d17d6-203">质量更新暂停到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="d17d6-203">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="d17d6-204">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="d17d6-204">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="d17d6-205">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d17d6-205">DateTimeOffset</span></span>|<span data-ttu-id="d17d6-206">功能更新暂停到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="d17d6-206">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="d17d6-207">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="d17d6-207">businessReadyUpdatesOnly</span></span>|[<span data-ttu-id="d17d6-208">windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="d17d6-208">windowsUpdateType</span></span>](../resources/intune-deviceconfig-windowsupdatetype.md)|<span data-ttu-id="d17d6-209">确定哪些分支设备将接收从其更新。</span><span class="sxs-lookup"><span data-stu-id="d17d6-209">Determines which branch devices will receive their updates from.</span></span> <span data-ttu-id="d17d6-210">可取值为：`userDefined`、`all`、`businessReadyOnly`、`windowsInsiderBuildFast`、`windowsInsiderBuildSlow`、`windowsInsiderBuildRelease`。</span><span class="sxs-lookup"><span data-stu-id="d17d6-210">Possible values are: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span></span>|
|<span data-ttu-id="d17d6-211">skipChecksBeforeRestart</span><span class="sxs-lookup"><span data-stu-id="d17d6-211">skipChecksBeforeRestart</span></span>|<span data-ttu-id="d17d6-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="d17d6-212">Boolean</span></span>|<span data-ttu-id="d17d6-213">设置要跳过之前重新启动所有检查： 电池级别 = 40%，用户状态显示需要演示文稿模式下、 全屏幕模式、 电话呼叫状态、 游戏模式等。</span><span class="sxs-lookup"><span data-stu-id="d17d6-213">Set to skip all check before restart: Battery level = 40%, User presence, Display Needed, Presentation mode, Full screen mode, phone call state, game mode etc.</span></span> |
|<span data-ttu-id="d17d6-214">updateWeeks</span><span class="sxs-lookup"><span data-stu-id="d17d6-214">updateWeeks</span></span>|[<span data-ttu-id="d17d6-215">windowsUpdateForBusinessUpdateWeeks</span><span class="sxs-lookup"><span data-stu-id="d17d6-215">windowsUpdateForBusinessUpdateWeeks</span></span>](../resources/intune-deviceconfig-windowsupdateforbusinessupdateweeks.md)|<span data-ttu-id="d17d6-216">计划更新安装在相应月份的周。</span><span class="sxs-lookup"><span data-stu-id="d17d6-216">Scheduled the update installation on the weeks of the month.</span></span> <span data-ttu-id="d17d6-217">可取值为：`userDefined`、`firstWeek`、`secondWeek`、`thirdWeek`、`fourthWeek`、`everyWeek`。</span><span class="sxs-lookup"><span data-stu-id="d17d6-217">Possible values are: `userDefined`, `firstWeek`, `secondWeek`, `thirdWeek`, `fourthWeek`, `everyWeek`.</span></span>|
|<span data-ttu-id="d17d6-218">qualityUpdatesPauseStartDate</span><span class="sxs-lookup"><span data-stu-id="d17d6-218">qualityUpdatesPauseStartDate</span></span>|<span data-ttu-id="d17d6-219">日期</span><span class="sxs-lookup"><span data-stu-id="d17d6-219">Date</span></span>|<span data-ttu-id="d17d6-220">质量更新暂停的开始日期。</span><span class="sxs-lookup"><span data-stu-id="d17d6-220">Quality Updates Pause start date.</span></span> <span data-ttu-id="d17d6-221">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="d17d6-221">This property is read-only.</span></span>|
|<span data-ttu-id="d17d6-222">featureUpdatesPauseStartDate</span><span class="sxs-lookup"><span data-stu-id="d17d6-222">featureUpdatesPauseStartDate</span></span>|<span data-ttu-id="d17d6-223">日期</span><span class="sxs-lookup"><span data-stu-id="d17d6-223">Date</span></span>|<span data-ttu-id="d17d6-224">功能更新暂停的开始日期。</span><span class="sxs-lookup"><span data-stu-id="d17d6-224">Feature Updates Pause start date.</span></span> <span data-ttu-id="d17d6-225">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="d17d6-225">This property is read-only.</span></span>|
|<span data-ttu-id="d17d6-226">featureUpdatesRollbackWindowInDays</span><span class="sxs-lookup"><span data-stu-id="d17d6-226">featureUpdatesRollbackWindowInDays</span></span>|<span data-ttu-id="d17d6-227">Int32</span><span class="sxs-lookup"><span data-stu-id="d17d6-227">Int32</span></span>|<span data-ttu-id="d17d6-228">回滚的有效功能更新后的天数</span><span class="sxs-lookup"><span data-stu-id="d17d6-228">The number of days after a Feature Update for which a rollback is valid</span></span>|
|<span data-ttu-id="d17d6-229">qualityUpdatesWillBeRolledBack</span><span class="sxs-lookup"><span data-stu-id="d17d6-229">qualityUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="d17d6-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="d17d6-230">Boolean</span></span>|<span data-ttu-id="d17d6-231">指定是否回滚到下一个设备质量更新签入</span><span class="sxs-lookup"><span data-stu-id="d17d6-231">Specifies whether to rollback Quality Updates on the next device check in</span></span>|
|<span data-ttu-id="d17d6-232">featureUpdatesWillBeRolledBack</span><span class="sxs-lookup"><span data-stu-id="d17d6-232">featureUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="d17d6-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="d17d6-233">Boolean</span></span>|<span data-ttu-id="d17d6-234">指定是否回滚到下一个设备上的功能更新签入</span><span class="sxs-lookup"><span data-stu-id="d17d6-234">Specifies whether to rollback Feature Updates on the next device check in</span></span>|
|<span data-ttu-id="d17d6-235">qualityUpdatesRollbackStartDateTime</span><span class="sxs-lookup"><span data-stu-id="d17d6-235">qualityUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="d17d6-236">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d17d6-236">DateTimeOffset</span></span>|<span data-ttu-id="d17d6-237">质量更新回滚开始日期时间</span><span class="sxs-lookup"><span data-stu-id="d17d6-237">Quality Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="d17d6-238">featureUpdatesRollbackStartDateTime</span><span class="sxs-lookup"><span data-stu-id="d17d6-238">featureUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="d17d6-239">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d17d6-239">DateTimeOffset</span></span>|<span data-ttu-id="d17d6-240">功能更新回滚开始日期时间</span><span class="sxs-lookup"><span data-stu-id="d17d6-240">Feature Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="d17d6-241">engagedRestartDeadlineInDays</span><span class="sxs-lookup"><span data-stu-id="d17d6-241">engagedRestartDeadlineInDays</span></span>|<span data-ttu-id="d17d6-242">Int32</span><span class="sxs-lookup"><span data-stu-id="d17d6-242">Int32</span></span>|<span data-ttu-id="d17d6-243">自动计划并执行挂起的重新启动之外活动的小时，与有效范围为从 2 到 30 天之前的天数的截止日期</span><span class="sxs-lookup"><span data-stu-id="d17d6-243">Deadline in days before automatically scheduling and executing a pending restart outside of active hours, with valid range from 2 to 30 days</span></span>|
|<span data-ttu-id="d17d6-244">engagedRestartSnoozeScheduleInDays</span><span class="sxs-lookup"><span data-stu-id="d17d6-244">engagedRestartSnoozeScheduleInDays</span></span>|<span data-ttu-id="d17d6-245">Int32</span><span class="sxs-lookup"><span data-stu-id="d17d6-245">Int32</span></span>|<span data-ttu-id="d17d6-246">用户可以 snooze 有效范围为从 1 到 3 天具有正在重新启动提醒通知的天数</span><span class="sxs-lookup"><span data-stu-id="d17d6-246">Number of days a user can snooze Engaged Restart reminder notifications with valid range from 1 to 3 days</span></span>|
|<span data-ttu-id="d17d6-247">engagedRestartTransitionScheduleInDays</span><span class="sxs-lookup"><span data-stu-id="d17d6-247">engagedRestartTransitionScheduleInDays</span></span>|<span data-ttu-id="d17d6-248">Int32</span><span class="sxs-lookup"><span data-stu-id="d17d6-248">Int32</span></span>|<span data-ttu-id="d17d6-249">从自动重新启动计划非活动时间正在重新要求用户安排与有效范围为从 0 到 30 天发出转换之前的天数</span><span class="sxs-lookup"><span data-stu-id="d17d6-249">Number of days before transitioning from Auto Restarts scheduled outside of active hours to Engaged Restart, which requires the user to schedule, with valid range from 0 to 30 days</span></span>|
|<span data-ttu-id="d17d6-250">autoRestartNotificationDismissal</span><span class="sxs-lookup"><span data-stu-id="d17d6-250">autoRestartNotificationDismissal</span></span>|[<span data-ttu-id="d17d6-251">autoRestartNotificationDismissalMethod</span><span class="sxs-lookup"><span data-stu-id="d17d6-251">autoRestartNotificationDismissalMethod</span></span>](../resources/intune-deviceconfig-autorestartnotificationdismissalmethod.md)|<span data-ttu-id="d17d6-252">指定按其在自动重新启动所需消除通知的方法。</span><span class="sxs-lookup"><span data-stu-id="d17d6-252">Specify the method by which the auto-restart required notification is dismissed.</span></span> <span data-ttu-id="d17d6-253">可取值为：`notConfigured`、`automatic`、`user`。</span><span class="sxs-lookup"><span data-stu-id="d17d6-253">Possible values are: `notConfigured`, `automatic`, `user`.</span></span>|
|<span data-ttu-id="d17d6-254">scheduleRestartWarningInHours</span><span class="sxs-lookup"><span data-stu-id="d17d6-254">scheduleRestartWarningInHours</span></span>|<span data-ttu-id="d17d6-255">Int32</span><span class="sxs-lookup"><span data-stu-id="d17d6-255">Int32</span></span>|<span data-ttu-id="d17d6-256">指定自动重新启动警告提醒通知的时间段。</span><span class="sxs-lookup"><span data-stu-id="d17d6-256">Specify the period for auto-restart warning reminder notifications.</span></span> <span data-ttu-id="d17d6-257">支持值： 2、 4、 8、 12 或 24 （小时）。</span><span class="sxs-lookup"><span data-stu-id="d17d6-257">Supported values: 2, 4, 8, 12 or 24 (hours).</span></span>|
|<span data-ttu-id="d17d6-258">scheduleImminentRestartWarningInMinutes</span><span class="sxs-lookup"><span data-stu-id="d17d6-258">scheduleImminentRestartWarningInMinutes</span></span>|<span data-ttu-id="d17d6-259">Int32</span><span class="sxs-lookup"><span data-stu-id="d17d6-259">Int32</span></span>|<span data-ttu-id="d17d6-260">指定自动重新启动即将发生警告通知的时间段。</span><span class="sxs-lookup"><span data-stu-id="d17d6-260">Specify the period for auto-restart imminent warning notifications.</span></span> <span data-ttu-id="d17d6-261">支持值： 15、 30 或 60 （分钟）。</span><span class="sxs-lookup"><span data-stu-id="d17d6-261">Supported values: 15, 30 or 60 (minutes).</span></span>|
|<span data-ttu-id="d17d6-262">userPauseAccess</span><span class="sxs-lookup"><span data-stu-id="d17d6-262">userPauseAccess</span></span>|<span data-ttu-id="d17d6-263">[启用](../resources/intune-shared-enablement</span><span class="sxs-lookup"><span data-stu-id="d17d6-263">[enablement](../resources/intune-shared-enablement</span></span>
<span data-ttu-id="d17d6-264">.md)</span><span class="sxs-lookup"><span data-stu-id="d17d6-264">.md)</span></span>|<span data-ttu-id="d17d6-265">指定是否启用要暂停软件更新的最终用户的访问。</span><span class="sxs-lookup"><span data-stu-id="d17d6-265">Specifies whether to enable end user’s access to pause software updates.</span></span> <span data-ttu-id="d17d6-266">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="d17d6-266">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="d17d6-267">响应</span><span class="sxs-lookup"><span data-stu-id="d17d6-267">Response</span></span>
<span data-ttu-id="d17d6-268">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d17d6-268">If successful, this method returns a `201 Created` response code and a [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d17d6-269">示例</span><span class="sxs-lookup"><span data-stu-id="d17d6-269">Example</span></span>

### <a name="request"></a><span data-ttu-id="d17d6-270">请求</span><span class="sxs-lookup"><span data-stu-id="d17d6-270">Request</span></span>
<span data-ttu-id="d17d6-271">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d17d6-271">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1804

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
  "userPauseAccess": "enabled"
}
```

### <a name="response"></a><span data-ttu-id="d17d6-272">响应</span><span class="sxs-lookup"><span data-stu-id="d17d6-272">Response</span></span>
<span data-ttu-id="d17d6-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d17d6-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1976

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
  "userPauseAccess": "enabled"
}
```




