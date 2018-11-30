---
title: 创建 windowsUpdateForBusinessConfiguration
description: 创建新的 windowsUpdateForBusinessConfiguration 对象。
ms.openlocfilehash: 277a90794743c604666d134b26c023fb792c1fb8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008855"
---
# <a name="create-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="16b82-103">创建 windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="16b82-103">Create windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="16b82-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="16b82-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="16b82-105">创建新的 [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="16b82-105">Create a new [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="16b82-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="16b82-106">Prerequisites</span></span>
<span data-ttu-id="16b82-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="16b82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16b82-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="16b82-109">Permission type</span></span>|<span data-ttu-id="16b82-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="16b82-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16b82-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="16b82-111">Delegated (work or school account)</span></span>|<span data-ttu-id="16b82-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16b82-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="16b82-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="16b82-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16b82-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="16b82-114">Not supported.</span></span>|
|<span data-ttu-id="16b82-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="16b82-115">Application</span></span>|<span data-ttu-id="16b82-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="16b82-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="16b82-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="16b82-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="16b82-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="16b82-118">Request headers</span></span>
|<span data-ttu-id="16b82-119">标头</span><span class="sxs-lookup"><span data-stu-id="16b82-119">Header</span></span>|<span data-ttu-id="16b82-120">值</span><span class="sxs-lookup"><span data-stu-id="16b82-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16b82-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="16b82-121">Authorization</span></span>|<span data-ttu-id="16b82-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="16b82-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16b82-123">Accept</span><span class="sxs-lookup"><span data-stu-id="16b82-123">Accept</span></span>|<span data-ttu-id="16b82-124">application/json</span><span class="sxs-lookup"><span data-stu-id="16b82-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16b82-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="16b82-125">Request body</span></span>
<span data-ttu-id="16b82-126">在请求正文中，提供 windowsUpdateForBusinessConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="16b82-126">In the request body, supply a JSON representation for the windowsUpdateForBusinessConfiguration object.</span></span>

<span data-ttu-id="16b82-127">下表显示创建 windowsUpdateForBusinessConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="16b82-127">The following table shows the properties that are required when you create the windowsUpdateForBusinessConfiguration.</span></span>

|<span data-ttu-id="16b82-128">属性</span><span class="sxs-lookup"><span data-stu-id="16b82-128">Property</span></span>|<span data-ttu-id="16b82-129">类型</span><span class="sxs-lookup"><span data-stu-id="16b82-129">Type</span></span>|<span data-ttu-id="16b82-130">说明</span><span class="sxs-lookup"><span data-stu-id="16b82-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16b82-131">id</span><span class="sxs-lookup"><span data-stu-id="16b82-131">id</span></span>|<span data-ttu-id="16b82-132">String</span><span class="sxs-lookup"><span data-stu-id="16b82-132">String</span></span>|<span data-ttu-id="16b82-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="16b82-133">Key of the entity.</span></span> <span data-ttu-id="16b82-134">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16b82-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16b82-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="16b82-135">lastModifiedDateTime</span></span>|<span data-ttu-id="16b82-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16b82-136">DateTimeOffset</span></span>|<span data-ttu-id="16b82-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="16b82-137">DateTime the object was last modified.</span></span> <span data-ttu-id="16b82-138">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16b82-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16b82-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="16b82-139">createdDateTime</span></span>|<span data-ttu-id="16b82-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16b82-140">DateTimeOffset</span></span>|<span data-ttu-id="16b82-141">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="16b82-141">DateTime the object was created.</span></span> <span data-ttu-id="16b82-142">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16b82-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16b82-143">description</span><span class="sxs-lookup"><span data-stu-id="16b82-143">description</span></span>|<span data-ttu-id="16b82-144">String</span><span class="sxs-lookup"><span data-stu-id="16b82-144">String</span></span>|<span data-ttu-id="16b82-145">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="16b82-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="16b82-146">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16b82-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16b82-147">displayName</span><span class="sxs-lookup"><span data-stu-id="16b82-147">displayName</span></span>|<span data-ttu-id="16b82-148">String</span><span class="sxs-lookup"><span data-stu-id="16b82-148">String</span></span>|<span data-ttu-id="16b82-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="16b82-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="16b82-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16b82-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16b82-151">version</span><span class="sxs-lookup"><span data-stu-id="16b82-151">version</span></span>|<span data-ttu-id="16b82-152">Int32</span><span class="sxs-lookup"><span data-stu-id="16b82-152">Int32</span></span>|<span data-ttu-id="16b82-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="16b82-153">Version of the device configuration.</span></span> <span data-ttu-id="16b82-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16b82-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16b82-155">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="16b82-155">deliveryOptimizationMode</span></span>|[<span data-ttu-id="16b82-156">windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="16b82-156">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="16b82-157">传递优化模式。</span><span class="sxs-lookup"><span data-stu-id="16b82-157">Delivery Optimization Mode.</span></span> <span data-ttu-id="16b82-158">可取值为：`userDefined`、`httpOnly`、`httpWithPeeringNat`、`httpWithPeeringPrivateGroup`、`httpWithInternetPeering`、`simpleDownload`、`bypassMode`。</span><span class="sxs-lookup"><span data-stu-id="16b82-158">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="16b82-159">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="16b82-159">prereleaseFeatures</span></span>|[<span data-ttu-id="16b82-160">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="16b82-160">prereleaseFeatures</span></span>](../resources/intune-deviceconfig-prereleasefeatures.md)|<span data-ttu-id="16b82-161">预发布功能。</span><span class="sxs-lookup"><span data-stu-id="16b82-161">The pre-release features.</span></span> <span data-ttu-id="16b82-162">可取值为：`userDefined`、`settingsOnly`、`settingsAndExperimentations`、`notAllowed`。</span><span class="sxs-lookup"><span data-stu-id="16b82-162">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="16b82-163">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="16b82-163">automaticUpdateMode</span></span>|[<span data-ttu-id="16b82-164">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="16b82-164">automaticUpdateMode</span></span>](../resources/intune-deviceconfig-automaticupdatemode.md)|<span data-ttu-id="16b82-165">自动更新模式。</span><span class="sxs-lookup"><span data-stu-id="16b82-165">Automatic update mode.</span></span> <span data-ttu-id="16b82-166">可取值为：`userDefined`、`notifyDownload`、`autoInstallAtMaintenanceTime`、`autoInstallAndRebootAtMaintenanceTime`、`autoInstallAndRebootAtScheduledTime`、`autoInstallAndRebootWithoutEndUserControl`。</span><span class="sxs-lookup"><span data-stu-id="16b82-166">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`.</span></span>|
|<span data-ttu-id="16b82-167">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="16b82-167">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="16b82-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="16b82-168">Boolean</span></span>|<span data-ttu-id="16b82-169">允许 Microsoft 更新服务</span><span class="sxs-lookup"><span data-stu-id="16b82-169">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="16b82-170">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="16b82-170">driversExcluded</span></span>|<span data-ttu-id="16b82-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="16b82-171">Boolean</span></span>|<span data-ttu-id="16b82-172">排除 Windows 更新驱动程序</span><span class="sxs-lookup"><span data-stu-id="16b82-172">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="16b82-173">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="16b82-173">installationSchedule</span></span>|[<span data-ttu-id="16b82-174">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="16b82-174">windowsUpdateInstallScheduleType</span></span>](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)|<span data-ttu-id="16b82-175">安装计划</span><span class="sxs-lookup"><span data-stu-id="16b82-175">Installation schedule</span></span>|
|<span data-ttu-id="16b82-176">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="16b82-176">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="16b82-177">Int32</span><span class="sxs-lookup"><span data-stu-id="16b82-177">Int32</span></span>|<span data-ttu-id="16b82-178">推迟质量更新的天数</span><span class="sxs-lookup"><span data-stu-id="16b82-178">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="16b82-179">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="16b82-179">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="16b82-180">Int32</span><span class="sxs-lookup"><span data-stu-id="16b82-180">Int32</span></span>|<span data-ttu-id="16b82-181">推迟功能更新的天数</span><span class="sxs-lookup"><span data-stu-id="16b82-181">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="16b82-182">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="16b82-182">qualityUpdatesPaused</span></span>|<span data-ttu-id="16b82-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="16b82-183">Boolean</span></span>|<span data-ttu-id="16b82-184">暂停质量更新</span><span class="sxs-lookup"><span data-stu-id="16b82-184">Pause Quality Updates</span></span>|
|<span data-ttu-id="16b82-185">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="16b82-185">featureUpdatesPaused</span></span>|<span data-ttu-id="16b82-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="16b82-186">Boolean</span></span>|<span data-ttu-id="16b82-187">暂停功能更新</span><span class="sxs-lookup"><span data-stu-id="16b82-187">Pause Feature Updates</span></span>|
|<span data-ttu-id="16b82-188">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="16b82-188">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="16b82-189">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16b82-189">DateTimeOffset</span></span>|<span data-ttu-id="16b82-190">质量更新暂停到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="16b82-190">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="16b82-191">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="16b82-191">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="16b82-192">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16b82-192">DateTimeOffset</span></span>|<span data-ttu-id="16b82-193">功能更新暂停到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="16b82-193">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="16b82-194">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="16b82-194">businessReadyUpdatesOnly</span></span>|[<span data-ttu-id="16b82-195">windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="16b82-195">windowsUpdateType</span></span>](../resources/intune-deviceconfig-windowsupdatetype.md)|<span data-ttu-id="16b82-196">确定哪些分支设备将接收从其更新。</span><span class="sxs-lookup"><span data-stu-id="16b82-196">Determines which branch devices will receive their updates from.</span></span> <span data-ttu-id="16b82-197">可取值为：`userDefined`、`all`、`businessReadyOnly`、`windowsInsiderBuildFast`、`windowsInsiderBuildSlow`、`windowsInsiderBuildRelease`。</span><span class="sxs-lookup"><span data-stu-id="16b82-197">Possible values are: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span></span>|



## <a name="response"></a><span data-ttu-id="16b82-198">响应</span><span class="sxs-lookup"><span data-stu-id="16b82-198">Response</span></span>
<span data-ttu-id="16b82-199">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="16b82-199">If successful, this method returns a `201 Created` response code and a [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16b82-200">示例</span><span class="sxs-lookup"><span data-stu-id="16b82-200">Example</span></span>
### <a name="request"></a><span data-ttu-id="16b82-201">请求</span><span class="sxs-lookup"><span data-stu-id="16b82-201">Request</span></span>
<span data-ttu-id="16b82-202">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="16b82-202">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 910

{
  "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
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
  "businessReadyUpdatesOnly": "all"
}
```

### <a name="response"></a><span data-ttu-id="16b82-203">响应</span><span class="sxs-lookup"><span data-stu-id="16b82-203">Response</span></span>
<span data-ttu-id="16b82-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="16b82-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1082

{
  "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
  "id": "4928dd6a-dd6a-4928-6add-28496add2849",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
  "businessReadyUpdatesOnly": "all"
}
```



