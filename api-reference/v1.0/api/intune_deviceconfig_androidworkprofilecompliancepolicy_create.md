# <a name="create-androidworkprofilecompliancepolicy"></a><span data-ttu-id="73219-101">创建 androidWorkProfileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="73219-101">Create androidWorkProfileCompliancePolicy</span></span>

> <span data-ttu-id="73219-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="73219-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="73219-103">创建新的 [androidWorkProfileCompliancePolicy](../resources/intune_deviceconfig_androidworkprofilecompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="73219-103">Create a new [editionUpgradeConfiguration](../resources/intune_deviceconfig_androidworkprofilecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="73219-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="73219-104">Prerequisites</span></span>
<span data-ttu-id="73219-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="73219-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="73219-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="73219-107">Permission type</span></span>|<span data-ttu-id="73219-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="73219-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73219-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="73219-109">Delegated (work or school account)</span></span>|<span data-ttu-id="73219-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73219-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="73219-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="73219-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73219-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="73219-112">Not supported.</span></span>|
|<span data-ttu-id="73219-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="73219-113">Application</span></span>|<span data-ttu-id="73219-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="73219-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="73219-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="73219-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="73219-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="73219-116">Request headers</span></span>
|<span data-ttu-id="73219-117">标头</span><span class="sxs-lookup"><span data-stu-id="73219-117">Header</span></span>|<span data-ttu-id="73219-118">值</span><span class="sxs-lookup"><span data-stu-id="73219-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73219-119">授权</span><span class="sxs-lookup"><span data-stu-id="73219-119">Authorization</span></span>|<span data-ttu-id="73219-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="73219-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73219-121">接受</span><span class="sxs-lookup"><span data-stu-id="73219-121">Accept</span></span>|<span data-ttu-id="73219-122">application/json</span><span class="sxs-lookup"><span data-stu-id="73219-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73219-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="73219-123">Request body</span></span>
<span data-ttu-id="73219-124">在请求正文中，为 androidWorkProfileCompliancePolicy 对象提供 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="73219-124">In the request body, supply a JSON representation for the deviceConfigurationAssignment object.</span></span>

<span data-ttu-id="73219-125">下表显示当你创建  androidWorkProfileCompliancePolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="73219-125">The following table shows the properties that are required when you create the deviceComplianceUserOverview.</span></span>

|<span data-ttu-id="73219-126">属性</span><span class="sxs-lookup"><span data-stu-id="73219-126">Property</span></span>|<span data-ttu-id="73219-127">类型</span><span class="sxs-lookup"><span data-stu-id="73219-127">Type</span></span>|<span data-ttu-id="73219-128">说明</span><span class="sxs-lookup"><span data-stu-id="73219-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73219-129">ID</span><span class="sxs-lookup"><span data-stu-id="73219-129">id</span></span>|<span data-ttu-id="73219-130">字符串</span><span class="sxs-lookup"><span data-stu-id="73219-130">String</span></span>|<span data-ttu-id="73219-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="73219-131">Key of the entity.</span></span> <span data-ttu-id="73219-132">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="73219-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="73219-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="73219-133">createdDateTime</span></span>|<span data-ttu-id="73219-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73219-134">DateTimeOffset</span></span>|<span data-ttu-id="73219-135">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="73219-135">DateTime the object was created.</span></span> <span data-ttu-id="73219-136">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="73219-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="73219-137">说明</span><span class="sxs-lookup"><span data-stu-id="73219-137">description</span></span>|<span data-ttu-id="73219-138">字符串</span><span class="sxs-lookup"><span data-stu-id="73219-138">String</span></span>|<span data-ttu-id="73219-139">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="73219-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="73219-140">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="73219-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="73219-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="73219-141">lastModifiedDateTime</span></span>|<span data-ttu-id="73219-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73219-142">DateTimeOffset</span></span>|<span data-ttu-id="73219-143">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="73219-143">DateTime the object was last modified.</span></span> <span data-ttu-id="73219-144">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="73219-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="73219-145">displayName</span><span class="sxs-lookup"><span data-stu-id="73219-145">displayName</span></span>|<span data-ttu-id="73219-146">字符串</span><span class="sxs-lookup"><span data-stu-id="73219-146">String</span></span>|<span data-ttu-id="73219-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="73219-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="73219-148">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="73219-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="73219-149">版本</span><span class="sxs-lookup"><span data-stu-id="73219-149">version</span></span>|<span data-ttu-id="73219-150">Int32</span><span class="sxs-lookup"><span data-stu-id="73219-150">Int32</span></span>|<span data-ttu-id="73219-151">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="73219-151">Version of the device configuration.</span></span> <span data-ttu-id="73219-152">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="73219-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="73219-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="73219-153">passwordRequired</span></span>|<span data-ttu-id="73219-154">布尔</span><span class="sxs-lookup"><span data-stu-id="73219-154">Boolean</span></span>|<span data-ttu-id="73219-155">需要密码才可解锁设备。</span><span class="sxs-lookup"><span data-stu-id="73219-155">Require a password to unlock device.</span></span>|
|<span data-ttu-id="73219-156">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="73219-156">passwordMinimumLength</span></span>|<span data-ttu-id="73219-157">Int32</span><span class="sxs-lookup"><span data-stu-id="73219-157">Int32</span></span>|<span data-ttu-id="73219-158">最短密码长度。</span><span class="sxs-lookup"><span data-stu-id="73219-158">Minimum password length.</span></span> <span data-ttu-id="73219-159">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="73219-159">Valid values 4 to 16</span></span>|
|<span data-ttu-id="73219-160">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="73219-160">passwordRequiredType</span></span>|[<span data-ttu-id="73219-161">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="73219-161">androidRequiredPasswordType</span></span>](../resources/intune_deviceconfig_androidrequiredpasswordtype.md)|<span data-ttu-id="73219-162">密码中字符的类型。</span><span class="sxs-lookup"><span data-stu-id="73219-162">Type of characters in password Possible values are: , , , , , , , .</span></span> <span data-ttu-id="73219-163">可取值为：`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any`。</span><span class="sxs-lookup"><span data-stu-id="73219-163">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="73219-164">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="73219-164">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="73219-165">Int32</span><span class="sxs-lookup"><span data-stu-id="73219-165">Int32</span></span>|<span data-ttu-id="73219-166">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="73219-166">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="73219-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="73219-167">passwordExpirationDays</span></span>|<span data-ttu-id="73219-168">Int32</span><span class="sxs-lookup"><span data-stu-id="73219-168">Int32</span></span>|<span data-ttu-id="73219-169">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="73219-169">Number of days before the password expires.</span></span> <span data-ttu-id="73219-170">有效值为 1 至 365</span><span class="sxs-lookup"><span data-stu-id="73219-170">Valid values 1 to 365</span></span>|
|<span data-ttu-id="73219-171">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="73219-171">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="73219-172">Int32</span><span class="sxs-lookup"><span data-stu-id="73219-172">Int32</span></span>|<span data-ttu-id="73219-173">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="73219-173">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="73219-174">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="73219-174">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="73219-175">布尔</span><span class="sxs-lookup"><span data-stu-id="73219-175">Boolean</span></span>|<span data-ttu-id="73219-176">要求设备不允许安装来自未知源的应用。</span><span class="sxs-lookup"><span data-stu-id="73219-176">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="73219-177">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="73219-177">securityDisableUsbDebugging</span></span>|<span data-ttu-id="73219-178">布尔</span><span class="sxs-lookup"><span data-stu-id="73219-178">Boolean</span></span>|<span data-ttu-id="73219-179">在 Android 设备上禁用 USB 调试。</span><span class="sxs-lookup"><span data-stu-id="73219-179">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="73219-180">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="73219-180">securityRequireVerifyApps</span></span>|<span data-ttu-id="73219-181">布尔</span><span class="sxs-lookup"><span data-stu-id="73219-181">Boolean</span></span>|<span data-ttu-id="73219-182">要求启用 Android 验证应用功能。</span><span class="sxs-lookup"><span data-stu-id="73219-182">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="73219-183">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="73219-183">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="73219-184">布尔</span><span class="sxs-lookup"><span data-stu-id="73219-184">Boolean</span></span>|<span data-ttu-id="73219-185">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="73219-185">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="73219-186">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="73219-186">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="73219-187">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="73219-187">deviceThreatProtectionLevel</span></span>](../resources/intune_deviceconfig_devicethreatprotectionlevel.md)|<span data-ttu-id="73219-188">要求移动威胁防护最低风险级别来报告不符合情况。</span><span class="sxs-lookup"><span data-stu-id="73219-188">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="73219-189">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="73219-189">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="73219-190">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="73219-190">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="73219-191">布尔</span><span class="sxs-lookup"><span data-stu-id="73219-191">Boolean</span></span>|<span data-ttu-id="73219-192">设备不得越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="73219-192">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="73219-193">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="73219-193">osMinimumVersion</span></span>|<span data-ttu-id="73219-194">字符串</span><span class="sxs-lookup"><span data-stu-id="73219-194">String</span></span>|<span data-ttu-id="73219-195">最低 Android 版本。</span><span class="sxs-lookup"><span data-stu-id="73219-195">Minimum Android version.</span></span>|
|<span data-ttu-id="73219-196">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="73219-196">osMaximumVersion</span></span>|<span data-ttu-id="73219-197">字符串</span><span class="sxs-lookup"><span data-stu-id="73219-197">String</span></span>|<span data-ttu-id="73219-198">最高 Android 版本。</span><span class="sxs-lookup"><span data-stu-id="73219-198">Maximum Android version.</span></span>|
|<span data-ttu-id="73219-199">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="73219-199">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="73219-200">字符串</span><span class="sxs-lookup"><span data-stu-id="73219-200">String</span></span>|<span data-ttu-id="73219-201">最低 Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="73219-201">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="73219-202">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="73219-202">storageRequireEncryption</span></span>|<span data-ttu-id="73219-203">布尔</span><span class="sxs-lookup"><span data-stu-id="73219-203">Boolean</span></span>|<span data-ttu-id="73219-204">要求对 Android 设备加密。</span><span class="sxs-lookup"><span data-stu-id="73219-204">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="73219-205">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="73219-205">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="73219-206">布尔</span><span class="sxs-lookup"><span data-stu-id="73219-206">Boolean</span></span>|<span data-ttu-id="73219-207">要求设备传递 SafetyNet 基本完整性检查。</span><span class="sxs-lookup"><span data-stu-id="73219-207">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="73219-208">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="73219-208">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="73219-209">布尔</span><span class="sxs-lookup"><span data-stu-id="73219-209">Boolean</span></span>|<span data-ttu-id="73219-210">要求设备传递 SafetyNet 认证设备检查。</span><span class="sxs-lookup"><span data-stu-id="73219-210">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="73219-211">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="73219-211">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="73219-212">布尔</span><span class="sxs-lookup"><span data-stu-id="73219-212">Boolean</span></span>|<span data-ttu-id="73219-213">要求在设备上安装并启用 Google Play Services。</span><span class="sxs-lookup"><span data-stu-id="73219-213">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="73219-214">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="73219-214">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="73219-215">布尔</span><span class="sxs-lookup"><span data-stu-id="73219-215">Boolean</span></span>|<span data-ttu-id="73219-216">要求设备具有最新的安全提供程序。</span><span class="sxs-lookup"><span data-stu-id="73219-216">Require the device to have up to date security providers.</span></span> <span data-ttu-id="73219-217">设备将要求启用 Google Play Services 并保持最新状态。</span><span class="sxs-lookup"><span data-stu-id="73219-217">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="73219-218">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="73219-218">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="73219-219">布尔</span><span class="sxs-lookup"><span data-stu-id="73219-219">Boolean</span></span>|<span data-ttu-id="73219-220">要求设备传递公司门户客户端应用运行时完整性检查。</span><span class="sxs-lookup"><span data-stu-id="73219-220">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="73219-221">响应</span><span class="sxs-lookup"><span data-stu-id="73219-221">Response</span></span>
<span data-ttu-id="73219-222">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [androidWorkProfileCompliancePolicy](../resources/intune_deviceconfig_androidworkprofilecompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="73219-222">If successful, this method returns a `201 Created` response code and a [ListItemVersion](../resources/intune_deviceconfig_androidworkprofilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73219-223">示例</span><span class="sxs-lookup"><span data-stu-id="73219-223">Example</span></span>
### <a name="request"></a><span data-ttu-id="73219-224">请求</span><span class="sxs-lookup"><span data-stu-id="73219-224">Request</span></span>
<span data-ttu-id="73219-225">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="73219-225">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1234

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordRequiredType": "alphabetic",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordPreviousPasswordBlockCount": 2,
  "securityPreventInstallAppsFromUnknownSources": true,
  "securityDisableUsbDebugging": true,
  "securityRequireVerifyApps": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "securityBlockJailbrokenDevices": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "storageRequireEncryption": true,
  "securityRequireSafetyNetAttestationBasicIntegrity": true,
  "securityRequireSafetyNetAttestationCertifiedDevice": true,
  "securityRequireGooglePlayServices": true,
  "securityRequireUpToDateSecurityProviders": true,
  "securityRequireCompanyPortalAppIntegrity": true
}
```

### <a name="response"></a><span data-ttu-id="73219-226">响应</span><span class="sxs-lookup"><span data-stu-id="73219-226">Response</span></span>
<span data-ttu-id="73219-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="73219-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1342

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
  "id": "4e385271-5271-4e38-7152-384e7152384e",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordRequiredType": "alphabetic",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordPreviousPasswordBlockCount": 2,
  "securityPreventInstallAppsFromUnknownSources": true,
  "securityDisableUsbDebugging": true,
  "securityRequireVerifyApps": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "securityBlockJailbrokenDevices": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "storageRequireEncryption": true,
  "securityRequireSafetyNetAttestationBasicIntegrity": true,
  "securityRequireSafetyNetAttestationCertifiedDevice": true,
  "securityRequireGooglePlayServices": true,
  "securityRequireUpToDateSecurityProviders": true,
  "securityRequireCompanyPortalAppIntegrity": true
}
```








