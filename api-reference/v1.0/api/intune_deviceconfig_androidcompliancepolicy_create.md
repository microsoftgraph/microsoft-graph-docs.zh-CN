# <a name="create-androidcompliancepolicy"></a><span data-ttu-id="5d2c6-101">创建 androidCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="5d2c6-101">Create androidCompliancePolicy</span></span>

> <span data-ttu-id="5d2c6-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5d2c6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5d2c6-103">创建新的 [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5d2c6-103">Create a new [plannerBucket](../resources/intune_deviceconfig_androidcompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5d2c6-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="5d2c6-104">Prerequisites</span></span>
<span data-ttu-id="5d2c6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="5d2c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5d2c6-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="5d2c6-107">Permission type</span></span>|<span data-ttu-id="5d2c6-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5d2c6-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5d2c6-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5d2c6-109">Delegated (work or school account)</span></span>|<span data-ttu-id="5d2c6-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d2c6-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5d2c6-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5d2c6-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5d2c6-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="5d2c6-112">Not supported.</span></span>|
|<span data-ttu-id="5d2c6-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="5d2c6-113">Application</span></span>|<span data-ttu-id="5d2c6-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5d2c6-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5d2c6-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5d2c6-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="5d2c6-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="5d2c6-116">Request headers</span></span>
|<span data-ttu-id="5d2c6-117">标头</span><span class="sxs-lookup"><span data-stu-id="5d2c6-117">Header</span></span>|<span data-ttu-id="5d2c6-118">值</span><span class="sxs-lookup"><span data-stu-id="5d2c6-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5d2c6-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d2c6-119">Authorization</span></span>|<span data-ttu-id="5d2c6-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5d2c6-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5d2c6-121">Accept</span><span class="sxs-lookup"><span data-stu-id="5d2c6-121">Accept</span></span>|<span data-ttu-id="5d2c6-122">application/json</span><span class="sxs-lookup"><span data-stu-id="5d2c6-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d2c6-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="5d2c6-123">Request body</span></span>
<span data-ttu-id="5d2c6-124">在请求正文中，提供 androidCompliancePolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5d2c6-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="5d2c6-125">下表显示了创建 androidCompliancePolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5d2c6-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="5d2c6-126">属性</span><span class="sxs-lookup"><span data-stu-id="5d2c6-126">Property</span></span>|<span data-ttu-id="5d2c6-127">类型</span><span class="sxs-lookup"><span data-stu-id="5d2c6-127">Type</span></span>|<span data-ttu-id="5d2c6-128">说明</span><span class="sxs-lookup"><span data-stu-id="5d2c6-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d2c6-129">id</span><span class="sxs-lookup"><span data-stu-id="5d2c6-129">id</span></span>|<span data-ttu-id="5d2c6-130">String</span><span class="sxs-lookup"><span data-stu-id="5d2c6-130">String</span></span>|<span data-ttu-id="5d2c6-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5d2c6-131">Key of the setting.</span></span> <span data-ttu-id="5d2c6-132">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5d2c6-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5d2c6-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5d2c6-133">createdDateTime</span></span>|<span data-ttu-id="5d2c6-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d2c6-134">DateTimeOffset</span></span>|<span data-ttu-id="5d2c6-135">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="5d2c6-135">DateTime the object was created.</span></span> <span data-ttu-id="5d2c6-136">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5d2c6-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5d2c6-137">description</span><span class="sxs-lookup"><span data-stu-id="5d2c6-137">description</span></span>|<span data-ttu-id="5d2c6-138">String</span><span class="sxs-lookup"><span data-stu-id="5d2c6-138">String</span></span>|<span data-ttu-id="5d2c6-139">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="5d2c6-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5d2c6-140">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5d2c6-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5d2c6-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5d2c6-141">lastModifiedDateTime</span></span>|<span data-ttu-id="5d2c6-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d2c6-142">DateTimeOffset</span></span>|<span data-ttu-id="5d2c6-143">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="5d2c6-143">Indicates the date the object was last modified.</span></span> <span data-ttu-id="5d2c6-144">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5d2c6-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5d2c6-145">displayName</span><span class="sxs-lookup"><span data-stu-id="5d2c6-145">displayName</span></span>|<span data-ttu-id="5d2c6-146">String</span><span class="sxs-lookup"><span data-stu-id="5d2c6-146">String</span></span>|<span data-ttu-id="5d2c6-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="5d2c6-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5d2c6-148">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5d2c6-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5d2c6-149">version</span><span class="sxs-lookup"><span data-stu-id="5d2c6-149">version</span></span>|<span data-ttu-id="5d2c6-150">Int32</span><span class="sxs-lookup"><span data-stu-id="5d2c6-150">Int32</span></span>|<span data-ttu-id="5d2c6-151">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="5d2c6-151">Version of the device configuration.</span></span> <span data-ttu-id="5d2c6-152">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5d2c6-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5d2c6-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="5d2c6-153">passwordRequired</span></span>|<span data-ttu-id="5d2c6-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="5d2c6-154">Boolean</span></span>|<span data-ttu-id="5d2c6-155">需要密码才可解锁设备。</span><span class="sxs-lookup"><span data-stu-id="5d2c6-155">Require a password to unlock device.</span></span>|
|<span data-ttu-id="5d2c6-156">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="5d2c6-156">passwordMinimumLength</span></span>|<span data-ttu-id="5d2c6-157">Int32</span><span class="sxs-lookup"><span data-stu-id="5d2c6-157">Int32</span></span>|<span data-ttu-id="5d2c6-158">最短密码长度。</span><span class="sxs-lookup"><span data-stu-id="5d2c6-158">Minimum password length.</span></span> <span data-ttu-id="5d2c6-159">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="5d2c6-159">Valid values 4 to 16</span></span>|
|<span data-ttu-id="5d2c6-160">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="5d2c6-160">passwordRequiredType</span></span>|<span data-ttu-id="5d2c6-161">String</span><span class="sxs-lookup"><span data-stu-id="5d2c6-161">String</span></span>|<span data-ttu-id="5d2c6-162">密码中的字符类型。可取值为：`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any`。</span><span class="sxs-lookup"><span data-stu-id="5d2c6-162">Type of characters in password Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="5d2c6-163">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="5d2c6-163">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="5d2c6-164">Int32</span><span class="sxs-lookup"><span data-stu-id="5d2c6-164">Int32</span></span>|<span data-ttu-id="5d2c6-165">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="5d2c6-165">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="5d2c6-166">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="5d2c6-166">passwordExpirationDays</span></span>|<span data-ttu-id="5d2c6-167">Int32</span><span class="sxs-lookup"><span data-stu-id="5d2c6-167">Int32</span></span>|<span data-ttu-id="5d2c6-168">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="5d2c6-168">Number of days before the password expires.</span></span> <span data-ttu-id="5d2c6-169">有效值为 1 至 365</span><span class="sxs-lookup"><span data-stu-id="5d2c6-169">Valid values 1 to 365</span></span>|
|<span data-ttu-id="5d2c6-170">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="5d2c6-170">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="5d2c6-171">Int32</span><span class="sxs-lookup"><span data-stu-id="5d2c6-171">Int32</span></span>|<span data-ttu-id="5d2c6-172">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="5d2c6-172">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="5d2c6-173">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="5d2c6-173">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="5d2c6-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="5d2c6-174">Boolean</span></span>|<span data-ttu-id="5d2c6-175">要求设备不允许安装来自未知源的应用。</span><span class="sxs-lookup"><span data-stu-id="5d2c6-175">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="5d2c6-176">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="5d2c6-176">securityDisableUsbDebugging</span></span>|<span data-ttu-id="5d2c6-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="5d2c6-177">Boolean</span></span>|<span data-ttu-id="5d2c6-178">在 Android 设备上禁用 USB 调试。</span><span class="sxs-lookup"><span data-stu-id="5d2c6-178">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="5d2c6-179">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="5d2c6-179">securityRequireVerifyApps</span></span>|<span data-ttu-id="5d2c6-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="5d2c6-180">Boolean</span></span>|<span data-ttu-id="5d2c6-181">要求启用 Android 验证应用功能。</span><span class="sxs-lookup"><span data-stu-id="5d2c6-181">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="5d2c6-182">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="5d2c6-182">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="5d2c6-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="5d2c6-183">Boolean</span></span>|<span data-ttu-id="5d2c6-184">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="5d2c6-184">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="5d2c6-185">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="5d2c6-185">deviceThreatProtectionRequiredSecurityLevel</span></span>|<span data-ttu-id="5d2c6-186">String</span><span class="sxs-lookup"><span data-stu-id="5d2c6-186">String</span></span>|<span data-ttu-id="5d2c6-187">要求移动威胁防护最低风险级别来报告不符合情况。</span><span class="sxs-lookup"><span data-stu-id="5d2c6-187">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="5d2c6-188">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="5d2c6-188">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="5d2c6-189">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="5d2c6-189">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="5d2c6-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="5d2c6-190">Boolean</span></span>|<span data-ttu-id="5d2c6-191">设备不得越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="5d2c6-191">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="5d2c6-192">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="5d2c6-192">osMinimumVersion</span></span>|<span data-ttu-id="5d2c6-193">String</span><span class="sxs-lookup"><span data-stu-id="5d2c6-193">String</span></span>|<span data-ttu-id="5d2c6-194">最低 Android 版本。</span><span class="sxs-lookup"><span data-stu-id="5d2c6-194">Minimum Android version.</span></span>|
|<span data-ttu-id="5d2c6-195">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="5d2c6-195">osMaximumVersion</span></span>|<span data-ttu-id="5d2c6-196">String</span><span class="sxs-lookup"><span data-stu-id="5d2c6-196">String</span></span>|<span data-ttu-id="5d2c6-197">最高 Android 版本。</span><span class="sxs-lookup"><span data-stu-id="5d2c6-197">Maximum Android version.</span></span>|
|<span data-ttu-id="5d2c6-198">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="5d2c6-198">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="5d2c6-199">String</span><span class="sxs-lookup"><span data-stu-id="5d2c6-199">String</span></span>|<span data-ttu-id="5d2c6-200">最低 Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="5d2c6-200">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="5d2c6-201">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="5d2c6-201">storageRequireEncryption</span></span>|<span data-ttu-id="5d2c6-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="5d2c6-202">Boolean</span></span>|<span data-ttu-id="5d2c6-203">要求对 Android 设备加密。</span><span class="sxs-lookup"><span data-stu-id="5d2c6-203">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="5d2c6-204">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="5d2c6-204">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="5d2c6-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="5d2c6-205">Boolean</span></span>|<span data-ttu-id="5d2c6-206">要求设备传递 SafetyNet 基本完整性检查。</span><span class="sxs-lookup"><span data-stu-id="5d2c6-206">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="5d2c6-207">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="5d2c6-207">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="5d2c6-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="5d2c6-208">Boolean</span></span>|<span data-ttu-id="5d2c6-209">要求设备传递 SafetyNet 认证设备检查。</span><span class="sxs-lookup"><span data-stu-id="5d2c6-209">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="5d2c6-210">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="5d2c6-210">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="5d2c6-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="5d2c6-211">Boolean</span></span>|<span data-ttu-id="5d2c6-212">要求在设备上安装并启用 Google Play Services。</span><span class="sxs-lookup"><span data-stu-id="5d2c6-212">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="5d2c6-213">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="5d2c6-213">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="5d2c6-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="5d2c6-214">Boolean</span></span>|<span data-ttu-id="5d2c6-215">要求设备具有最新的安全提供程序。</span><span class="sxs-lookup"><span data-stu-id="5d2c6-215">Require the device to have up to date security providers.</span></span> <span data-ttu-id="5d2c6-216">设备需要启用 Google Play Services 并保持最新状态。</span><span class="sxs-lookup"><span data-stu-id="5d2c6-216">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="5d2c6-217">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="5d2c6-217">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="5d2c6-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="5d2c6-218">Boolean</span></span>|<span data-ttu-id="5d2c6-219">要求设备传递公司门户客户端应用运行时完整性检查。</span><span class="sxs-lookup"><span data-stu-id="5d2c6-219">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="5d2c6-220">响应</span><span class="sxs-lookup"><span data-stu-id="5d2c6-220">Response</span></span>
<span data-ttu-id="5d2c6-221">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5d2c6-221">If successful, this method returns a `201 Created` response code and a [DriveItemVersion](../resources/intune_deviceconfig_androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d2c6-222">示例</span><span class="sxs-lookup"><span data-stu-id="5d2c6-222">Example</span></span>
### <a name="request"></a><span data-ttu-id="5d2c6-223">请求</span><span class="sxs-lookup"><span data-stu-id="5d2c6-223">Request</span></span>
<span data-ttu-id="5d2c6-224">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5d2c6-224">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1223

{
  "@odata.type": "#microsoft.graph.androidCompliancePolicy",
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

### <a name="response"></a><span data-ttu-id="5d2c6-225">响应</span><span class="sxs-lookup"><span data-stu-id="5d2c6-225">Response</span></span>
<span data-ttu-id="5d2c6-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5d2c6-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1331

{
  "@odata.type": "#microsoft.graph.androidCompliancePolicy",
  "id": "752c820f-820f-752c-0f82-2c750f822c75",
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



