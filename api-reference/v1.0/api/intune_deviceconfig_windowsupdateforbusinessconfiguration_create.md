# <a name="create-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="e1666-101">创建 windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="e1666-101">Create windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="e1666-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e1666-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e1666-103">创建新的 [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e1666-103">Create a new [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e1666-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="e1666-104">Prerequisites</span></span>
<span data-ttu-id="e1666-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="e1666-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e1666-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="e1666-107">Permission type</span></span>|<span data-ttu-id="e1666-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e1666-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1666-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e1666-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e1666-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1666-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e1666-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e1666-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1666-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="e1666-112">Not supported.</span></span>|
|<span data-ttu-id="e1666-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="e1666-113">Application</span></span>|<span data-ttu-id="e1666-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e1666-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1666-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e1666-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e1666-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="e1666-116">Request headers</span></span>
|<span data-ttu-id="e1666-117">标头</span><span class="sxs-lookup"><span data-stu-id="e1666-117">Header</span></span>|<span data-ttu-id="e1666-118">值</span><span class="sxs-lookup"><span data-stu-id="e1666-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1666-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1666-119">Authorization</span></span>|<span data-ttu-id="e1666-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e1666-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1666-121">Accept</span><span class="sxs-lookup"><span data-stu-id="e1666-121">Accept</span></span>|<span data-ttu-id="e1666-122">application/json</span><span class="sxs-lookup"><span data-stu-id="e1666-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1666-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="e1666-123">Request body</span></span>
<span data-ttu-id="e1666-124">在请求正文中，提供 windowsUpdateForBusinessConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e1666-124">In the request body, supply a JSON representation for the windowsUpdateForBusinessConfiguration object.</span></span>

<span data-ttu-id="e1666-125">下表显示创建 windowsUpdateForBusinessConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e1666-125">The following table shows the properties that are required when you create the windowsUpdateForBusinessConfiguration.</span></span>

|<span data-ttu-id="e1666-126">属性</span><span class="sxs-lookup"><span data-stu-id="e1666-126">Property</span></span>|<span data-ttu-id="e1666-127">类型</span><span class="sxs-lookup"><span data-stu-id="e1666-127">Type</span></span>|<span data-ttu-id="e1666-128">说明</span><span class="sxs-lookup"><span data-stu-id="e1666-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1666-129">id</span><span class="sxs-lookup"><span data-stu-id="e1666-129">id</span></span>|<span data-ttu-id="e1666-130">String</span><span class="sxs-lookup"><span data-stu-id="e1666-130">String</span></span>|<span data-ttu-id="e1666-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e1666-131">Key of the entity.</span></span> <span data-ttu-id="e1666-132">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e1666-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e1666-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e1666-133">lastModifiedDateTime</span></span>|<span data-ttu-id="e1666-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1666-134">DateTimeOffset</span></span>|<span data-ttu-id="e1666-135">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e1666-135">DateTime the object was last modified.</span></span> <span data-ttu-id="e1666-136">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e1666-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e1666-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e1666-137">createdDateTime</span></span>|<span data-ttu-id="e1666-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1666-138">DateTimeOffset</span></span>|<span data-ttu-id="e1666-139">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e1666-139">DateTime the object was created.</span></span> <span data-ttu-id="e1666-140">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e1666-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e1666-141">description</span><span class="sxs-lookup"><span data-stu-id="e1666-141">description</span></span>|<span data-ttu-id="e1666-142">String</span><span class="sxs-lookup"><span data-stu-id="e1666-142">String</span></span>|<span data-ttu-id="e1666-143">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="e1666-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e1666-144">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e1666-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e1666-145">displayName</span><span class="sxs-lookup"><span data-stu-id="e1666-145">displayName</span></span>|<span data-ttu-id="e1666-146">String</span><span class="sxs-lookup"><span data-stu-id="e1666-146">String</span></span>|<span data-ttu-id="e1666-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="e1666-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e1666-148">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e1666-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e1666-149">version</span><span class="sxs-lookup"><span data-stu-id="e1666-149">version</span></span>|<span data-ttu-id="e1666-150">Int32</span><span class="sxs-lookup"><span data-stu-id="e1666-150">Int32</span></span>|<span data-ttu-id="e1666-151">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="e1666-151">Version of the device configuration.</span></span> <span data-ttu-id="e1666-152">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e1666-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e1666-153">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="e1666-153">deliveryOptimizationMode</span></span>|[<span data-ttu-id="e1666-154">windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="e1666-154">windowsDeliveryOptimizationMode</span></span>](../resources/intune_deviceconfig_windowsdeliveryoptimizationmode.md)|<span data-ttu-id="e1666-155">传递优化模式。</span><span class="sxs-lookup"><span data-stu-id="e1666-155">Delivery Optimization Mode.</span></span> <span data-ttu-id="e1666-156">可取值为：`userDefined`、`httpOnly`、`httpWithPeeringNat`、`httpWithPeeringPrivateGroup`、`httpWithInternetPeering`、`simpleDownload`、`bypassMode`。</span><span class="sxs-lookup"><span data-stu-id="e1666-156">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="e1666-157">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="e1666-157">prereleaseFeatures</span></span>|[<span data-ttu-id="e1666-158">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="e1666-158">prereleaseFeatures</span></span>](../resources/intune_deviceconfig_prereleasefeatures.md)|<span data-ttu-id="e1666-159">预发布功能。</span><span class="sxs-lookup"><span data-stu-id="e1666-159">The pre-release features.</span></span> <span data-ttu-id="e1666-160">可取值为：`userDefined`、`settingsOnly`、`settingsAndExperimentations`、`notAllowed`。</span><span class="sxs-lookup"><span data-stu-id="e1666-160">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="e1666-161">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="e1666-161">automaticUpdateMode</span></span>|[<span data-ttu-id="e1666-162">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="e1666-162">automaticUpdateMode</span></span>](../resources/intune_deviceconfig_automaticupdatemode.md)|<span data-ttu-id="e1666-163">自动更新模式。</span><span class="sxs-lookup"><span data-stu-id="e1666-163">Automatic update mode.</span></span> <span data-ttu-id="e1666-164">可取值为：`userDefined`、`notifyDownload`、`autoInstallAtMaintenanceTime`、`autoInstallAndRebootAtMaintenanceTime`、`autoInstallAndRebootAtScheduledTime`、`autoInstallAndRebootWithoutEndUserControl`。</span><span class="sxs-lookup"><span data-stu-id="e1666-164">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`.</span></span>|
|<span data-ttu-id="e1666-165">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="e1666-165">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="e1666-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1666-166">Boolean</span></span>|<span data-ttu-id="e1666-167">允许 Microsoft 更新服务</span><span class="sxs-lookup"><span data-stu-id="e1666-167">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="e1666-168">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="e1666-168">driversExcluded</span></span>|<span data-ttu-id="e1666-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1666-169">Boolean</span></span>|<span data-ttu-id="e1666-170">排除 Windows 更新驱动程序</span><span class="sxs-lookup"><span data-stu-id="e1666-170">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="e1666-171">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="e1666-171">installationSchedule</span></span>|[<span data-ttu-id="e1666-172">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="e1666-172">windowsUpdateInstallScheduleType</span></span>](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)|<span data-ttu-id="e1666-173">安装计划</span><span class="sxs-lookup"><span data-stu-id="e1666-173">Installation schedule</span></span>|
|<span data-ttu-id="e1666-174">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="e1666-174">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="e1666-175">Int32</span><span class="sxs-lookup"><span data-stu-id="e1666-175">Int32</span></span>|<span data-ttu-id="e1666-176">推迟质量更新的天数</span><span class="sxs-lookup"><span data-stu-id="e1666-176">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="e1666-177">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="e1666-177">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="e1666-178">Int32</span><span class="sxs-lookup"><span data-stu-id="e1666-178">Int32</span></span>|<span data-ttu-id="e1666-179">推迟功能更新的天数</span><span class="sxs-lookup"><span data-stu-id="e1666-179">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="e1666-180">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="e1666-180">qualityUpdatesPaused</span></span>|<span data-ttu-id="e1666-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1666-181">Boolean</span></span>|<span data-ttu-id="e1666-182">暂停质量更新</span><span class="sxs-lookup"><span data-stu-id="e1666-182">Pause Quality Updates</span></span>|
|<span data-ttu-id="e1666-183">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="e1666-183">featureUpdatesPaused</span></span>|<span data-ttu-id="e1666-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1666-184">Boolean</span></span>|<span data-ttu-id="e1666-185">暂停功能更新</span><span class="sxs-lookup"><span data-stu-id="e1666-185">Pause Feature Updates</span></span>|
|<span data-ttu-id="e1666-186">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="e1666-186">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="e1666-187">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1666-187">DateTimeOffset</span></span>|<span data-ttu-id="e1666-188">质量更新暂停到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="e1666-188">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="e1666-189">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="e1666-189">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="e1666-190">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1666-190">DateTimeOffset</span></span>|<span data-ttu-id="e1666-191">功能更新暂停到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="e1666-191">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="e1666-192">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="e1666-192">businessReadyUpdatesOnly</span></span>|[<span data-ttu-id="e1666-193">windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="e1666-193">windowsUpdateType</span></span>](../resources/intune_deviceconfig_windowsupdatetype.md)|<span data-ttu-id="e1666-194">确定哪些分支设备将接收从其更新。</span><span class="sxs-lookup"><span data-stu-id="e1666-194">Determines which branch devices will receive their updates from.</span></span> <span data-ttu-id="e1666-195">可取值为：`userDefined`、`all`、`businessReadyOnly`、`windowsInsiderBuildFast`、`windowsInsiderBuildSlow`、`windowsInsiderBuildRelease`。</span><span class="sxs-lookup"><span data-stu-id="e1666-195">Possible values are: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span></span>|



## <a name="response"></a><span data-ttu-id="e1666-196">响应</span><span class="sxs-lookup"><span data-stu-id="e1666-196">Response</span></span>
<span data-ttu-id="e1666-197">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e1666-197">If successful, this method returns a `201 Created` response code and a [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1666-198">示例</span><span class="sxs-lookup"><span data-stu-id="e1666-198">Example</span></span>
### <a name="request"></a><span data-ttu-id="e1666-199">请求</span><span class="sxs-lookup"><span data-stu-id="e1666-199">Request</span></span>
<span data-ttu-id="e1666-200">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e1666-200">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e1666-201">响应</span><span class="sxs-lookup"><span data-stu-id="e1666-201">Response</span></span>
<span data-ttu-id="e1666-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e1666-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



