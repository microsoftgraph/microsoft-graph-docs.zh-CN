---
title: 创建 windowsUpdateForBusinessConfiguration
description: 创建新的 windowsUpdateForBusinessConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5166e54fbe7066644b751985b101d1876529ded8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872763"
---
# <a name="create-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="631fa-103">创建 windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="631fa-103">Create windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="631fa-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="631fa-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="631fa-105">创建新的 [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="631fa-105">Create a new [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="631fa-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="631fa-106">Prerequisites</span></span>
<span data-ttu-id="631fa-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="631fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="631fa-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="631fa-109">Permission type</span></span>|<span data-ttu-id="631fa-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="631fa-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="631fa-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="631fa-111">Delegated (work or school account)</span></span>|<span data-ttu-id="631fa-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="631fa-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="631fa-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="631fa-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="631fa-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="631fa-114">Not supported.</span></span>|
|<span data-ttu-id="631fa-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="631fa-115">Application</span></span>|<span data-ttu-id="631fa-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="631fa-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="631fa-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="631fa-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="631fa-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="631fa-118">Request headers</span></span>
|<span data-ttu-id="631fa-119">标头</span><span class="sxs-lookup"><span data-stu-id="631fa-119">Header</span></span>|<span data-ttu-id="631fa-120">值</span><span class="sxs-lookup"><span data-stu-id="631fa-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="631fa-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="631fa-121">Authorization</span></span>|<span data-ttu-id="631fa-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="631fa-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="631fa-123">Accept</span><span class="sxs-lookup"><span data-stu-id="631fa-123">Accept</span></span>|<span data-ttu-id="631fa-124">application/json</span><span class="sxs-lookup"><span data-stu-id="631fa-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="631fa-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="631fa-125">Request body</span></span>
<span data-ttu-id="631fa-126">在请求正文中，提供 windowsUpdateForBusinessConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="631fa-126">In the request body, supply a JSON representation for the windowsUpdateForBusinessConfiguration object.</span></span>

<span data-ttu-id="631fa-127">下表显示创建 windowsUpdateForBusinessConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="631fa-127">The following table shows the properties that are required when you create the windowsUpdateForBusinessConfiguration.</span></span>

|<span data-ttu-id="631fa-128">属性</span><span class="sxs-lookup"><span data-stu-id="631fa-128">Property</span></span>|<span data-ttu-id="631fa-129">类型</span><span class="sxs-lookup"><span data-stu-id="631fa-129">Type</span></span>|<span data-ttu-id="631fa-130">说明</span><span class="sxs-lookup"><span data-stu-id="631fa-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="631fa-131">id</span><span class="sxs-lookup"><span data-stu-id="631fa-131">id</span></span>|<span data-ttu-id="631fa-132">String</span><span class="sxs-lookup"><span data-stu-id="631fa-132">String</span></span>|<span data-ttu-id="631fa-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="631fa-133">Key of the entity.</span></span> <span data-ttu-id="631fa-134">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="631fa-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="631fa-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="631fa-135">lastModifiedDateTime</span></span>|<span data-ttu-id="631fa-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="631fa-136">DateTimeOffset</span></span>|<span data-ttu-id="631fa-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="631fa-137">DateTime the object was last modified.</span></span> <span data-ttu-id="631fa-138">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="631fa-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="631fa-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="631fa-139">createdDateTime</span></span>|<span data-ttu-id="631fa-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="631fa-140">DateTimeOffset</span></span>|<span data-ttu-id="631fa-141">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="631fa-141">DateTime the object was created.</span></span> <span data-ttu-id="631fa-142">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="631fa-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="631fa-143">description</span><span class="sxs-lookup"><span data-stu-id="631fa-143">description</span></span>|<span data-ttu-id="631fa-144">String</span><span class="sxs-lookup"><span data-stu-id="631fa-144">String</span></span>|<span data-ttu-id="631fa-145">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="631fa-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="631fa-146">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="631fa-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="631fa-147">displayName</span><span class="sxs-lookup"><span data-stu-id="631fa-147">displayName</span></span>|<span data-ttu-id="631fa-148">String</span><span class="sxs-lookup"><span data-stu-id="631fa-148">String</span></span>|<span data-ttu-id="631fa-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="631fa-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="631fa-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="631fa-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="631fa-151">version</span><span class="sxs-lookup"><span data-stu-id="631fa-151">version</span></span>|<span data-ttu-id="631fa-152">Int32</span><span class="sxs-lookup"><span data-stu-id="631fa-152">Int32</span></span>|<span data-ttu-id="631fa-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="631fa-153">Version of the device configuration.</span></span> <span data-ttu-id="631fa-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="631fa-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="631fa-155">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="631fa-155">deliveryOptimizationMode</span></span>|[<span data-ttu-id="631fa-156">windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="631fa-156">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="631fa-157">传递优化模式。</span><span class="sxs-lookup"><span data-stu-id="631fa-157">Delivery Optimization Mode.</span></span> <span data-ttu-id="631fa-158">可取值为：`userDefined`、`httpOnly`、`httpWithPeeringNat`、`httpWithPeeringPrivateGroup`、`httpWithInternetPeering`、`simpleDownload`、`bypassMode`。</span><span class="sxs-lookup"><span data-stu-id="631fa-158">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="631fa-159">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="631fa-159">prereleaseFeatures</span></span>|[<span data-ttu-id="631fa-160">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="631fa-160">prereleaseFeatures</span></span>](../resources/intune-deviceconfig-prereleasefeatures.md)|<span data-ttu-id="631fa-161">预发布功能。</span><span class="sxs-lookup"><span data-stu-id="631fa-161">The pre-release features.</span></span> <span data-ttu-id="631fa-162">可取值为：`userDefined`、`settingsOnly`、`settingsAndExperimentations`、`notAllowed`。</span><span class="sxs-lookup"><span data-stu-id="631fa-162">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="631fa-163">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="631fa-163">automaticUpdateMode</span></span>|[<span data-ttu-id="631fa-164">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="631fa-164">automaticUpdateMode</span></span>](../resources/intune-deviceconfig-automaticupdatemode.md)|<span data-ttu-id="631fa-165">自动更新模式。</span><span class="sxs-lookup"><span data-stu-id="631fa-165">Automatic update mode.</span></span> <span data-ttu-id="631fa-166">可取值为：`userDefined`、`notifyDownload`、`autoInstallAtMaintenanceTime`、`autoInstallAndRebootAtMaintenanceTime`、`autoInstallAndRebootAtScheduledTime`、`autoInstallAndRebootWithoutEndUserControl`。</span><span class="sxs-lookup"><span data-stu-id="631fa-166">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`.</span></span>|
|<span data-ttu-id="631fa-167">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="631fa-167">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="631fa-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="631fa-168">Boolean</span></span>|<span data-ttu-id="631fa-169">允许 Microsoft 更新服务</span><span class="sxs-lookup"><span data-stu-id="631fa-169">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="631fa-170">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="631fa-170">driversExcluded</span></span>|<span data-ttu-id="631fa-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="631fa-171">Boolean</span></span>|<span data-ttu-id="631fa-172">排除 Windows 更新驱动程序</span><span class="sxs-lookup"><span data-stu-id="631fa-172">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="631fa-173">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="631fa-173">installationSchedule</span></span>|[<span data-ttu-id="631fa-174">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="631fa-174">windowsUpdateInstallScheduleType</span></span>](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)|<span data-ttu-id="631fa-175">安装计划</span><span class="sxs-lookup"><span data-stu-id="631fa-175">Installation schedule</span></span>|
|<span data-ttu-id="631fa-176">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="631fa-176">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="631fa-177">Int32</span><span class="sxs-lookup"><span data-stu-id="631fa-177">Int32</span></span>|<span data-ttu-id="631fa-178">推迟质量更新的天数</span><span class="sxs-lookup"><span data-stu-id="631fa-178">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="631fa-179">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="631fa-179">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="631fa-180">Int32</span><span class="sxs-lookup"><span data-stu-id="631fa-180">Int32</span></span>|<span data-ttu-id="631fa-181">推迟功能更新的天数</span><span class="sxs-lookup"><span data-stu-id="631fa-181">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="631fa-182">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="631fa-182">qualityUpdatesPaused</span></span>|<span data-ttu-id="631fa-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="631fa-183">Boolean</span></span>|<span data-ttu-id="631fa-184">暂停质量更新</span><span class="sxs-lookup"><span data-stu-id="631fa-184">Pause Quality Updates</span></span>|
|<span data-ttu-id="631fa-185">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="631fa-185">featureUpdatesPaused</span></span>|<span data-ttu-id="631fa-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="631fa-186">Boolean</span></span>|<span data-ttu-id="631fa-187">暂停功能更新</span><span class="sxs-lookup"><span data-stu-id="631fa-187">Pause Feature Updates</span></span>|
|<span data-ttu-id="631fa-188">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="631fa-188">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="631fa-189">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="631fa-189">DateTimeOffset</span></span>|<span data-ttu-id="631fa-190">质量更新暂停到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="631fa-190">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="631fa-191">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="631fa-191">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="631fa-192">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="631fa-192">DateTimeOffset</span></span>|<span data-ttu-id="631fa-193">功能更新暂停到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="631fa-193">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="631fa-194">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="631fa-194">businessReadyUpdatesOnly</span></span>|[<span data-ttu-id="631fa-195">windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="631fa-195">windowsUpdateType</span></span>](../resources/intune-deviceconfig-windowsupdatetype.md)|<span data-ttu-id="631fa-196">确定哪些分支设备将接收从其更新。</span><span class="sxs-lookup"><span data-stu-id="631fa-196">Determines which branch devices will receive their updates from.</span></span> <span data-ttu-id="631fa-197">可取值为：`userDefined`、`all`、`businessReadyOnly`、`windowsInsiderBuildFast`、`windowsInsiderBuildSlow`、`windowsInsiderBuildRelease`。</span><span class="sxs-lookup"><span data-stu-id="631fa-197">Possible values are: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span></span>|



## <a name="response"></a><span data-ttu-id="631fa-198">响应</span><span class="sxs-lookup"><span data-stu-id="631fa-198">Response</span></span>
<span data-ttu-id="631fa-199">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="631fa-199">If successful, this method returns a `201 Created` response code and a [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="631fa-200">示例</span><span class="sxs-lookup"><span data-stu-id="631fa-200">Example</span></span>
### <a name="request"></a><span data-ttu-id="631fa-201">请求</span><span class="sxs-lookup"><span data-stu-id="631fa-201">Request</span></span>
<span data-ttu-id="631fa-202">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="631fa-202">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="631fa-203">响应</span><span class="sxs-lookup"><span data-stu-id="631fa-203">Response</span></span>
<span data-ttu-id="631fa-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="631fa-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



