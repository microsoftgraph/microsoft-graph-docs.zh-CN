# <a name="update-sharedpcconfiguration"></a><span data-ttu-id="5ab91-101">更新 sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="5ab91-101">Update sharedPCConfiguration</span></span>

> <span data-ttu-id="5ab91-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5ab91-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5ab91-103">更新 [sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5ab91-103">Update the properties of a [calendar](../resources/intune_deviceconfig_sharedpcconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5ab91-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="5ab91-104">Prerequisites</span></span>
<span data-ttu-id="5ab91-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="5ab91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5ab91-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="5ab91-107">Permission type</span></span>|<span data-ttu-id="5ab91-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5ab91-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ab91-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5ab91-109">Delegated (work or school account)</span></span>|<span data-ttu-id="5ab91-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ab91-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5ab91-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5ab91-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ab91-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="5ab91-112">Not supported.</span></span>|
|<span data-ttu-id="5ab91-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="5ab91-113">Application</span></span>|<span data-ttu-id="5ab91-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5ab91-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ab91-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5ab91-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="5ab91-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="5ab91-116">Request headers</span></span>
|<span data-ttu-id="5ab91-117">标头</span><span class="sxs-lookup"><span data-stu-id="5ab91-117">Header</span></span>|<span data-ttu-id="5ab91-118">值</span><span class="sxs-lookup"><span data-stu-id="5ab91-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5ab91-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ab91-119">Authorization</span></span>|<span data-ttu-id="5ab91-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5ab91-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5ab91-121">Accept</span><span class="sxs-lookup"><span data-stu-id="5ab91-121">Accept</span></span>|<span data-ttu-id="5ab91-122">application/json</span><span class="sxs-lookup"><span data-stu-id="5ab91-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ab91-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="5ab91-123">Request body</span></span>
<span data-ttu-id="5ab91-124">在请求正文中，提供 [sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5ab91-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_sharedpcconfiguration.md) object.</span></span>

<span data-ttu-id="5ab91-125">下表显示创建 [sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5ab91-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="5ab91-126">属性</span><span class="sxs-lookup"><span data-stu-id="5ab91-126">Property</span></span>|<span data-ttu-id="5ab91-127">类型</span><span class="sxs-lookup"><span data-stu-id="5ab91-127">Type</span></span>|<span data-ttu-id="5ab91-128">说明</span><span class="sxs-lookup"><span data-stu-id="5ab91-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ab91-129">id</span><span class="sxs-lookup"><span data-stu-id="5ab91-129">id</span></span>|<span data-ttu-id="5ab91-130">String</span><span class="sxs-lookup"><span data-stu-id="5ab91-130">String</span></span>|<span data-ttu-id="5ab91-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5ab91-131">Key of the setting.</span></span> <span data-ttu-id="5ab91-132">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ab91-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ab91-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5ab91-133">lastModifiedDateTime</span></span>|<span data-ttu-id="5ab91-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ab91-134">DateTimeOffset</span></span>|<span data-ttu-id="5ab91-135">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="5ab91-135">Indicates the date the object was last modified.</span></span> <span data-ttu-id="5ab91-136">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ab91-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ab91-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5ab91-137">createdDateTime</span></span>|<span data-ttu-id="5ab91-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ab91-138">DateTimeOffset</span></span>|<span data-ttu-id="5ab91-139">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="5ab91-139">DateTime the object was created.</span></span> <span data-ttu-id="5ab91-140">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ab91-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ab91-141">description</span><span class="sxs-lookup"><span data-stu-id="5ab91-141">description</span></span>|<span data-ttu-id="5ab91-142">String</span><span class="sxs-lookup"><span data-stu-id="5ab91-142">String</span></span>|<span data-ttu-id="5ab91-143">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="5ab91-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5ab91-144">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ab91-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ab91-145">displayName</span><span class="sxs-lookup"><span data-stu-id="5ab91-145">displayName</span></span>|<span data-ttu-id="5ab91-146">String</span><span class="sxs-lookup"><span data-stu-id="5ab91-146">String</span></span>|<span data-ttu-id="5ab91-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="5ab91-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5ab91-148">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ab91-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ab91-149">version</span><span class="sxs-lookup"><span data-stu-id="5ab91-149">version</span></span>|<span data-ttu-id="5ab91-150">Int32</span><span class="sxs-lookup"><span data-stu-id="5ab91-150">Int32</span></span>|<span data-ttu-id="5ab91-151">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="5ab91-151">Version of the device configuration.</span></span> <span data-ttu-id="5ab91-152">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ab91-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ab91-153">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="5ab91-153">accountManagerPolicy</span></span>|[<span data-ttu-id="5ab91-154">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="5ab91-154">sharedPCAccountManagerPolicy</span></span>](../resources/intune_deviceconfig_sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="5ab91-155">指定在共享电脑上管理帐户的方式。</span><span class="sxs-lookup"><span data-stu-id="5ab91-155">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="5ab91-156">仅当 disableAccountManager 为 false 时适用。</span><span class="sxs-lookup"><span data-stu-id="5ab91-156">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="5ab91-157">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="5ab91-157">allowedAccounts</span></span>|<span data-ttu-id="5ab91-158">String</span><span class="sxs-lookup"><span data-stu-id="5ab91-158">String</span></span>|<span data-ttu-id="5ab91-159">指示允许在共享电脑上使用哪种类型的帐户。</span><span class="sxs-lookup"><span data-stu-id="5ab91-159">Indicates which type of accounts are allowed to use on a shared PC.</span></span> <span data-ttu-id="5ab91-160">可取值为：`guest`、`domain`。</span><span class="sxs-lookup"><span data-stu-id="5ab91-160">Possible values are: `guest`, `domain`.</span></span>|
|<span data-ttu-id="5ab91-161">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="5ab91-161">allowLocalStorage</span></span>|<span data-ttu-id="5ab91-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ab91-162">Boolean</span></span>|<span data-ttu-id="5ab91-163">指定在共享电脑上是否允许本地存储。</span><span class="sxs-lookup"><span data-stu-id="5ab91-163">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="5ab91-164">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="5ab91-164">disableAccountManager</span></span>|<span data-ttu-id="5ab91-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ab91-165">Boolean</span></span>|<span data-ttu-id="5ab91-166">禁用共享电脑模式的帐户管理器。</span><span class="sxs-lookup"><span data-stu-id="5ab91-166">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="5ab91-167">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="5ab91-167">disableEduPolicies</span></span>|<span data-ttu-id="5ab91-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ab91-168">Boolean</span></span>|<span data-ttu-id="5ab91-169">指定是否应禁用默认的共享电脑教育环境策略。</span><span class="sxs-lookup"><span data-stu-id="5ab91-169">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="5ab91-170">对于 Windows 10 RS2 及更高版本，将应用此策略而不将 Enabled 设置为 true。</span><span class="sxs-lookup"><span data-stu-id="5ab91-170">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="5ab91-171">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="5ab91-171">disablePowerPolicies</span></span>|<span data-ttu-id="5ab91-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ab91-172">Boolean</span></span>|<span data-ttu-id="5ab91-173">指定是否应禁用默认的共享电脑电源策略。</span><span class="sxs-lookup"><span data-stu-id="5ab91-173">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="5ab91-174">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="5ab91-174">disableSignInOnResume</span></span>|<span data-ttu-id="5ab91-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ab91-175">Boolean</span></span>|<span data-ttu-id="5ab91-176">禁用每当设备从睡眠模式唤醒时需要登录的要求。</span><span class="sxs-lookup"><span data-stu-id="5ab91-176">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="5ab91-177">enabled</span><span class="sxs-lookup"><span data-stu-id="5ab91-177">enabled</span></span>|<span data-ttu-id="5ab91-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ab91-178">Boolean</span></span>|<span data-ttu-id="5ab91-179">启用共享的电脑模式并应用共享的电脑策略。</span><span class="sxs-lookup"><span data-stu-id="5ab91-179">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="5ab91-180">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="5ab91-180">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="5ab91-181">Int32</span><span class="sxs-lookup"><span data-stu-id="5ab91-181">Int32</span></span>|<span data-ttu-id="5ab91-182">指定电脑进入睡眠状态之前设备必须保持空闲状态的时间（以秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="5ab91-182">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="5ab91-183">将此值设置为 0 可防止发生睡眠超时。</span><span class="sxs-lookup"><span data-stu-id="5ab91-183">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="5ab91-184">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="5ab91-184">kioskAppDisplayName</span></span>|<span data-ttu-id="5ab91-185">String</span><span class="sxs-lookup"><span data-stu-id="5ab91-185">String</span></span>|<span data-ttu-id="5ab91-186">指定启动由 SetKioskAppUserModelId 指定的应用的登录屏幕上显示的帐户的显示文本。</span><span class="sxs-lookup"><span data-stu-id="5ab91-186">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="5ab91-187">仅在设置 KioskAppUserModelId 后适用。</span><span class="sxs-lookup"><span data-stu-id="5ab91-187">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="5ab91-188">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="5ab91-188">kioskAppUserModelId</span></span>|<span data-ttu-id="5ab91-189">String</span><span class="sxs-lookup"><span data-stu-id="5ab91-189">String</span></span>|<span data-ttu-id="5ab91-190">指定要与分配的访问权限结合使用的应用的应用程序用户模型 ID。</span><span class="sxs-lookup"><span data-stu-id="5ab91-190">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="5ab91-191">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="5ab91-191">maintenanceStartTime</span></span>|<span data-ttu-id="5ab91-192">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="5ab91-192">TimeOfDay</span></span>|<span data-ttu-id="5ab91-193">指定维护小时的每日开始时间。</span><span class="sxs-lookup"><span data-stu-id="5ab91-193">Specifies the daily start time of maintenance hour.</span></span>|



## <a name="response"></a><span data-ttu-id="5ab91-194">响应</span><span class="sxs-lookup"><span data-stu-id="5ab91-194">Response</span></span>
<span data-ttu-id="5ab91-195">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5ab91-195">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ab91-196">示例</span><span class="sxs-lookup"><span data-stu-id="5ab91-196">Example</span></span>
### <a name="request"></a><span data-ttu-id="5ab91-197">请求</span><span class="sxs-lookup"><span data-stu-id="5ab91-197">Request</span></span>
<span data-ttu-id="5ab91-198">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5ab91-198">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 864

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountManagerPolicy": {
    "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy",
    "accountDeletionPolicy": "diskSpaceThreshold",
    "cacheAccountsAboveDiskFreePercentage": 4,
    "inactiveThresholdDays": 5,
    "removeAccountsBelowDiskFreePercentage": 5
  },
  "allowedAccounts": "domain",
  "allowLocalStorage": true,
  "disableAccountManager": true,
  "disableEduPolicies": true,
  "disablePowerPolicies": true,
  "disableSignInOnResume": true,
  "enabled": true,
  "idleTimeBeforeSleepInSeconds": 12,
  "kioskAppDisplayName": "Kiosk App Display Name value",
  "kioskAppUserModelId": "Kiosk App User Model Id value",
  "maintenanceStartTime": "11:59:24.7240000"
}
```

### <a name="response"></a><span data-ttu-id="5ab91-199">响应</span><span class="sxs-lookup"><span data-stu-id="5ab91-199">Response</span></span>
<span data-ttu-id="5ab91-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5ab91-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1032

{
  "@odata.type": "#microsoft.graph.sharedPCConfiguration",
  "id": "5206be3b-be3b-5206-3bbe-06523bbe0652",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountManagerPolicy": {
    "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy",
    "accountDeletionPolicy": "diskSpaceThreshold",
    "cacheAccountsAboveDiskFreePercentage": 4,
    "inactiveThresholdDays": 5,
    "removeAccountsBelowDiskFreePercentage": 5
  },
  "allowedAccounts": "domain",
  "allowLocalStorage": true,
  "disableAccountManager": true,
  "disableEduPolicies": true,
  "disablePowerPolicies": true,
  "disableSignInOnResume": true,
  "enabled": true,
  "idleTimeBeforeSleepInSeconds": 12,
  "kioskAppDisplayName": "Kiosk App Display Name value",
  "kioskAppUserModelId": "Kiosk App User Model Id value",
  "maintenanceStartTime": "11:59:24.7240000"
}
```



