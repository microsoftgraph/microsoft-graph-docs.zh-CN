# <a name="update-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="0c2d4-101">更新 windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="0c2d4-101">Update windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="0c2d4-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0c2d4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0c2d4-103">更新 [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0c2d4-103">Update the properties of a [calendar](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0c2d4-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="0c2d4-104">Prerequisites</span></span>
<span data-ttu-id="0c2d4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="0c2d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0c2d4-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="0c2d4-107">Permission type</span></span>|<span data-ttu-id="0c2d4-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0c2d4-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c2d4-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0c2d4-109">Delegated (work or school account)</span></span>|<span data-ttu-id="0c2d4-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c2d4-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0c2d4-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0c2d4-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c2d4-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="0c2d4-112">Not supported.</span></span>|
|<span data-ttu-id="0c2d4-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="0c2d4-113">Application</span></span>|<span data-ttu-id="0c2d4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0c2d4-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c2d4-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0c2d4-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="0c2d4-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="0c2d4-116">Request headers</span></span>
|<span data-ttu-id="0c2d4-117">标头</span><span class="sxs-lookup"><span data-stu-id="0c2d4-117">Header</span></span>|<span data-ttu-id="0c2d4-118">值</span><span class="sxs-lookup"><span data-stu-id="0c2d4-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c2d4-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c2d4-119">Authorization</span></span>|<span data-ttu-id="0c2d4-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0c2d4-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="0c2d4-121">Accept</span><span class="sxs-lookup"><span data-stu-id="0c2d4-121">Accept</span></span>|<span data-ttu-id="0c2d4-122">application/json</span><span class="sxs-lookup"><span data-stu-id="0c2d4-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c2d4-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="0c2d4-123">Request body</span></span>
<span data-ttu-id="0c2d4-124">在请求正文中，提供 [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0c2d4-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="0c2d4-125">下表显示创建 [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0c2d4-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="0c2d4-126">属性</span><span class="sxs-lookup"><span data-stu-id="0c2d4-126">Property</span></span>|<span data-ttu-id="0c2d4-127">类型</span><span class="sxs-lookup"><span data-stu-id="0c2d4-127">Type</span></span>|<span data-ttu-id="0c2d4-128">说明</span><span class="sxs-lookup"><span data-stu-id="0c2d4-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c2d4-129">id</span><span class="sxs-lookup"><span data-stu-id="0c2d4-129">id</span></span>|<span data-ttu-id="0c2d4-130">String</span><span class="sxs-lookup"><span data-stu-id="0c2d4-130">String</span></span>|<span data-ttu-id="0c2d4-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0c2d4-131">Key of the setting.</span></span> <span data-ttu-id="0c2d4-132">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0c2d4-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c2d4-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0c2d4-133">lastModifiedDateTime</span></span>|<span data-ttu-id="0c2d4-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c2d4-134">DateTimeOffset</span></span>|<span data-ttu-id="0c2d4-135">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0c2d4-135">Indicates the date the object was last modified.</span></span> <span data-ttu-id="0c2d4-136">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0c2d4-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c2d4-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0c2d4-137">createdDateTime</span></span>|<span data-ttu-id="0c2d4-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c2d4-138">DateTimeOffset</span></span>|<span data-ttu-id="0c2d4-139">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0c2d4-139">DateTime the object was created.</span></span> <span data-ttu-id="0c2d4-140">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0c2d4-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c2d4-141">description</span><span class="sxs-lookup"><span data-stu-id="0c2d4-141">description</span></span>|<span data-ttu-id="0c2d4-142">String</span><span class="sxs-lookup"><span data-stu-id="0c2d4-142">String</span></span>|<span data-ttu-id="0c2d4-143">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="0c2d4-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0c2d4-144">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0c2d4-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c2d4-145">displayName</span><span class="sxs-lookup"><span data-stu-id="0c2d4-145">displayName</span></span>|<span data-ttu-id="0c2d4-146">String</span><span class="sxs-lookup"><span data-stu-id="0c2d4-146">String</span></span>|<span data-ttu-id="0c2d4-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="0c2d4-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0c2d4-148">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0c2d4-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c2d4-149">version</span><span class="sxs-lookup"><span data-stu-id="0c2d4-149">version</span></span>|<span data-ttu-id="0c2d4-150">Int32</span><span class="sxs-lookup"><span data-stu-id="0c2d4-150">Int32</span></span>|<span data-ttu-id="0c2d4-151">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="0c2d4-151">Version of the device configuration.</span></span> <span data-ttu-id="0c2d4-152">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0c2d4-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c2d4-153">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="0c2d4-153">deliveryOptimizationMode</span></span>|<span data-ttu-id="0c2d4-154">String</span><span class="sxs-lookup"><span data-stu-id="0c2d4-154">String</span></span>|<span data-ttu-id="0c2d4-155">传递优化模式。可取值为：`userDefined`、`httpOnly`、`httpWithPeeringNat`、`httpWithPeeringPrivateGroup`、`httpWithInternetPeering`、`simpleDownload`、`bypassMode`。</span><span class="sxs-lookup"><span data-stu-id="0c2d4-155">Delivery Optimization Mode Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="0c2d4-156">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="0c2d4-156">prereleaseFeatures</span></span>|<span data-ttu-id="0c2d4-157">String</span><span class="sxs-lookup"><span data-stu-id="0c2d4-157">String</span></span>|<span data-ttu-id="0c2d4-158">预发布功能。</span><span class="sxs-lookup"><span data-stu-id="0c2d4-158">The pre-release features.</span></span> <span data-ttu-id="0c2d4-159">可取值为：`userDefined`、`settingsOnly`、`settingsAndExperimentations`、`notAllowed`。</span><span class="sxs-lookup"><span data-stu-id="0c2d4-159">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="0c2d4-160">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="0c2d4-160">automaticUpdateMode</span></span>|<span data-ttu-id="0c2d4-161">String</span><span class="sxs-lookup"><span data-stu-id="0c2d4-161">String</span></span>|<span data-ttu-id="0c2d4-162">自动更新模式。</span><span class="sxs-lookup"><span data-stu-id="0c2d4-162">Automatic update mode.</span></span> <span data-ttu-id="0c2d4-163">可取值为：`userDefined`、`notifyDownload`、`autoInstallAtMaintenanceTime`、`autoInstallAndRebootAtMaintenanceTime`、`autoInstallAndRebootAtScheduledTime`、`autoInstallAndRebootWithoutEndUserControl`。</span><span class="sxs-lookup"><span data-stu-id="0c2d4-163">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`.</span></span>|
|<span data-ttu-id="0c2d4-164">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="0c2d4-164">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="0c2d4-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c2d4-165">Boolean</span></span>|<span data-ttu-id="0c2d4-166">允许 Microsoft 更新服务</span><span class="sxs-lookup"><span data-stu-id="0c2d4-166">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="0c2d4-167">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="0c2d4-167">driversExcluded</span></span>|<span data-ttu-id="0c2d4-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c2d4-168">Boolean</span></span>|<span data-ttu-id="0c2d4-169">排除 Windows 更新驱动程序</span><span class="sxs-lookup"><span data-stu-id="0c2d4-169">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="0c2d4-170">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="0c2d4-170">installationSchedule</span></span>|[<span data-ttu-id="0c2d4-171">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="0c2d4-171">windowsUpdateInstallScheduleType</span></span>](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)|<span data-ttu-id="0c2d4-172">安装计划</span><span class="sxs-lookup"><span data-stu-id="0c2d4-172">Installation schedule</span></span>|
|<span data-ttu-id="0c2d4-173">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="0c2d4-173">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="0c2d4-174">Int32</span><span class="sxs-lookup"><span data-stu-id="0c2d4-174">Int32</span></span>|<span data-ttu-id="0c2d4-175">推迟质量更新的天数</span><span class="sxs-lookup"><span data-stu-id="0c2d4-175">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="0c2d4-176">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="0c2d4-176">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="0c2d4-177">Int32</span><span class="sxs-lookup"><span data-stu-id="0c2d4-177">Int32</span></span>|<span data-ttu-id="0c2d4-178">推迟功能更新的天数</span><span class="sxs-lookup"><span data-stu-id="0c2d4-178">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="0c2d4-179">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="0c2d4-179">qualityUpdatesPaused</span></span>|<span data-ttu-id="0c2d4-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c2d4-180">Boolean</span></span>|<span data-ttu-id="0c2d4-181">暂停质量更新</span><span class="sxs-lookup"><span data-stu-id="0c2d4-181">Pause Quality Updates</span></span>|
|<span data-ttu-id="0c2d4-182">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="0c2d4-182">featureUpdatesPaused</span></span>|<span data-ttu-id="0c2d4-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c2d4-183">Boolean</span></span>|<span data-ttu-id="0c2d4-184">暂停功能更新</span><span class="sxs-lookup"><span data-stu-id="0c2d4-184">Pause Feature Updates</span></span>|
|<span data-ttu-id="0c2d4-185">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="0c2d4-185">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="0c2d4-186">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c2d4-186">DateTimeOffset</span></span>|<span data-ttu-id="0c2d4-187">质量更新暂停到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="0c2d4-187">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="0c2d4-188">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="0c2d4-188">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="0c2d4-189">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c2d4-189">DateTimeOffset</span></span>|<span data-ttu-id="0c2d4-190">功能更新暂停到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="0c2d4-190">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="0c2d4-191">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="0c2d4-191">businessReadyUpdatesOnly</span></span>|<span data-ttu-id="0c2d4-192">String</span><span class="sxs-lookup"><span data-stu-id="0c2d4-192">String</span></span>|<span data-ttu-id="0c2d4-193">确定将从哪些分支设备接收其更新。可取值为：`userDefined`、`all`、`businessReadyOnly`。</span><span class="sxs-lookup"><span data-stu-id="0c2d4-193">Determines which branch devices will receive their updates from Possible values are: `userDefined`, `all`, `businessReadyOnly`.</span></span>|



## <a name="response"></a><span data-ttu-id="0c2d4-194">响应</span><span class="sxs-lookup"><span data-stu-id="0c2d4-194">Response</span></span>
<span data-ttu-id="0c2d4-195">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0c2d4-195">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c2d4-196">示例</span><span class="sxs-lookup"><span data-stu-id="0c2d4-196">Example</span></span>
### <a name="request"></a><span data-ttu-id="0c2d4-197">请求</span><span class="sxs-lookup"><span data-stu-id="0c2d4-197">Request</span></span>
<span data-ttu-id="0c2d4-198">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0c2d4-198">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 898

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="0c2d4-199">响应</span><span class="sxs-lookup"><span data-stu-id="0c2d4-199">Response</span></span>
<span data-ttu-id="0c2d4-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0c2d4-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



