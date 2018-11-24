# <a name="update-androidworkprofilecompliancepolicy"></a><span data-ttu-id="136a2-101">更新 androidWorkProfileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="136a2-101">Update androidWorkProfileCompliancePolicy</span></span>

> <span data-ttu-id="136a2-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="136a2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="136a2-103">更新[androidWorkProfileCompliancePolicy](../resources/intune_deviceconfig_androidworkprofilecompliancepolicy.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="136a2-103">Update the properties of a [androidWorkProfileCompliancePolicy](../resources/intune_deviceconfig_androidworkprofilecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="136a2-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="136a2-104">Prerequisites</span></span>
<span data-ttu-id="136a2-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](../../../concepts/permissions_reference.md)。
</span><span class="sxs-lookup"><span data-stu-id="136a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="136a2-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="136a2-107">Permission type</span></span>|<span data-ttu-id="136a2-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="136a2-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="136a2-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="136a2-109">Delegated (work or school account)</span></span>|<span data-ttu-id="136a2-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="136a2-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="136a2-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="136a2-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="136a2-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="136a2-112">Not supported.</span></span>|
|<span data-ttu-id="136a2-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="136a2-113">Application</span></span>|<span data-ttu-id="136a2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="136a2-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="136a2-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="136a2-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="136a2-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="136a2-116">Request headers</span></span>
|<span data-ttu-id="136a2-117">标头</span><span class="sxs-lookup"><span data-stu-id="136a2-117">Header</span></span>|<span data-ttu-id="136a2-118">值</span><span class="sxs-lookup"><span data-stu-id="136a2-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="136a2-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="136a2-119">Authorization</span></span>|<span data-ttu-id="136a2-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="136a2-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="136a2-121">Accept</span><span class="sxs-lookup"><span data-stu-id="136a2-121">Accept</span></span>|<span data-ttu-id="136a2-122">application/json</span><span class="sxs-lookup"><span data-stu-id="136a2-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="136a2-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="136a2-123">Request body</span></span>
<span data-ttu-id="136a2-124">在请求正文中，提供[androidWorkProfileCompliancePolicy](../resources/intune_deviceconfig_androidworkprofilecompliancepolicy.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="136a2-124">In the request body, supply a JSON representation for the [androidWorkProfileCompliancePolicy](../resources/intune_deviceconfig_androidworkprofilecompliancepolicy.md) object.</span></span>

<span data-ttu-id="136a2-125">下表显示时创建[androidWorkProfileCompliancePolicy](../resources/intune_deviceconfig_androidworkprofilecompliancepolicy.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="136a2-125">The following table shows the properties that are required when you create the [androidWorkProfileCompliancePolicy](../resources/intune_deviceconfig_androidworkprofilecompliancepolicy.md).</span></span>

|<span data-ttu-id="136a2-126">属性</span><span class="sxs-lookup"><span data-stu-id="136a2-126">Property</span></span>|<span data-ttu-id="136a2-127">类型</span><span class="sxs-lookup"><span data-stu-id="136a2-127">Type</span></span>|<span data-ttu-id="136a2-128">说明</span><span class="sxs-lookup"><span data-stu-id="136a2-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="136a2-129">id</span><span class="sxs-lookup"><span data-stu-id="136a2-129">id</span></span>|<span data-ttu-id="136a2-130">String</span><span class="sxs-lookup"><span data-stu-id="136a2-130">String</span></span>|<span data-ttu-id="136a2-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="136a2-131">Key of the entity.</span></span> <span data-ttu-id="136a2-132">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="136a2-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="136a2-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="136a2-133">createdDateTime</span></span>|<span data-ttu-id="136a2-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="136a2-134">DateTimeOffset</span></span>|<span data-ttu-id="136a2-135">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="136a2-135">DateTime the object was created.</span></span> <span data-ttu-id="136a2-136">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="136a2-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="136a2-137">description</span><span class="sxs-lookup"><span data-stu-id="136a2-137">description</span></span>|<span data-ttu-id="136a2-138">String</span><span class="sxs-lookup"><span data-stu-id="136a2-138">String</span></span>|<span data-ttu-id="136a2-139">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="136a2-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="136a2-140">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="136a2-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="136a2-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="136a2-141">lastModifiedDateTime</span></span>|<span data-ttu-id="136a2-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="136a2-142">DateTimeOffset</span></span>|<span data-ttu-id="136a2-143">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="136a2-143">DateTime the object was last modified.</span></span> <span data-ttu-id="136a2-144">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="136a2-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="136a2-145">displayName</span><span class="sxs-lookup"><span data-stu-id="136a2-145">displayName</span></span>|<span data-ttu-id="136a2-146">String</span><span class="sxs-lookup"><span data-stu-id="136a2-146">String</span></span>|<span data-ttu-id="136a2-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="136a2-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="136a2-148">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="136a2-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="136a2-149">version</span><span class="sxs-lookup"><span data-stu-id="136a2-149">version</span></span>|<span data-ttu-id="136a2-150">Int32</span><span class="sxs-lookup"><span data-stu-id="136a2-150">Int32</span></span>|<span data-ttu-id="136a2-151">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="136a2-151">Version of the device configuration.</span></span> <span data-ttu-id="136a2-152">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="136a2-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="136a2-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="136a2-153">passwordRequired</span></span>|<span data-ttu-id="136a2-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="136a2-154">Boolean</span></span>|<span data-ttu-id="136a2-155">需要密码才可解锁设备。</span><span class="sxs-lookup"><span data-stu-id="136a2-155">Require a password to unlock device.</span></span>|
|<span data-ttu-id="136a2-156">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="136a2-156">passwordMinimumLength</span></span>|<span data-ttu-id="136a2-157">Int32</span><span class="sxs-lookup"><span data-stu-id="136a2-157">Int32</span></span>|<span data-ttu-id="136a2-158">最短密码长度。</span><span class="sxs-lookup"><span data-stu-id="136a2-158">Minimum password length.</span></span> <span data-ttu-id="136a2-159">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="136a2-159">Valid values 4 to 16</span></span>|
|<span data-ttu-id="136a2-160">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="136a2-160">passwordRequiredType</span></span>|[<span data-ttu-id="136a2-161">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="136a2-161">androidRequiredPasswordType</span></span>](../resources/intune_deviceconfig_androidrequiredpasswordtype.md)|<span data-ttu-id="136a2-162">密码中的字符类型。</span><span class="sxs-lookup"><span data-stu-id="136a2-162">Type of characters in password.</span></span> <span data-ttu-id="136a2-163">可取值为：`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any`。</span><span class="sxs-lookup"><span data-stu-id="136a2-163">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="136a2-164">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="136a2-164">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="136a2-165">Int32</span><span class="sxs-lookup"><span data-stu-id="136a2-165">Int32</span></span>|<span data-ttu-id="136a2-166">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="136a2-166">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="136a2-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="136a2-167">passwordExpirationDays</span></span>|<span data-ttu-id="136a2-168">Int32</span><span class="sxs-lookup"><span data-stu-id="136a2-168">Int32</span></span>|<span data-ttu-id="136a2-169">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="136a2-169">Number of days before the password expires.</span></span> <span data-ttu-id="136a2-170">有效值为 1 至 365</span><span class="sxs-lookup"><span data-stu-id="136a2-170">Valid values 1 to 365</span></span>|
|<span data-ttu-id="136a2-171">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="136a2-171">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="136a2-172">Int32</span><span class="sxs-lookup"><span data-stu-id="136a2-172">Int32</span></span>|<span data-ttu-id="136a2-173">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="136a2-173">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="136a2-174">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="136a2-174">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="136a2-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="136a2-175">Boolean</span></span>|<span data-ttu-id="136a2-176">要求设备不允许安装来自未知源的应用。</span><span class="sxs-lookup"><span data-stu-id="136a2-176">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="136a2-177">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="136a2-177">securityDisableUsbDebugging</span></span>|<span data-ttu-id="136a2-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="136a2-178">Boolean</span></span>|<span data-ttu-id="136a2-179">在 Android 设备上禁用 USB 调试。</span><span class="sxs-lookup"><span data-stu-id="136a2-179">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="136a2-180">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="136a2-180">securityRequireVerifyApps</span></span>|<span data-ttu-id="136a2-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="136a2-181">Boolean</span></span>|<span data-ttu-id="136a2-182">要求启用 Android 验证应用功能。</span><span class="sxs-lookup"><span data-stu-id="136a2-182">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="136a2-183">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="136a2-183">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="136a2-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="136a2-184">Boolean</span></span>|<span data-ttu-id="136a2-185">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="136a2-185">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="136a2-186">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="136a2-186">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="136a2-187">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="136a2-187">deviceThreatProtectionLevel</span></span>](../resources/intune_deviceconfig_devicethreatprotectionlevel.md)|<span data-ttu-id="136a2-188">要求移动威胁防护最低风险级别来报告不符合情况。</span><span class="sxs-lookup"><span data-stu-id="136a2-188">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="136a2-189">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="136a2-189">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="136a2-190">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="136a2-190">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="136a2-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="136a2-191">Boolean</span></span>|<span data-ttu-id="136a2-192">设备不得越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="136a2-192">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="136a2-193">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="136a2-193">osMinimumVersion</span></span>|<span data-ttu-id="136a2-194">String</span><span class="sxs-lookup"><span data-stu-id="136a2-194">String</span></span>|<span data-ttu-id="136a2-195">最低 Android 版本。</span><span class="sxs-lookup"><span data-stu-id="136a2-195">Minimum Android version.</span></span>|
|<span data-ttu-id="136a2-196">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="136a2-196">osMaximumVersion</span></span>|<span data-ttu-id="136a2-197">String</span><span class="sxs-lookup"><span data-stu-id="136a2-197">String</span></span>|<span data-ttu-id="136a2-198">最高 Android 版本。</span><span class="sxs-lookup"><span data-stu-id="136a2-198">Maximum Android version.</span></span>|
|<span data-ttu-id="136a2-199">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="136a2-199">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="136a2-200">String</span><span class="sxs-lookup"><span data-stu-id="136a2-200">String</span></span>|<span data-ttu-id="136a2-201">最低 Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="136a2-201">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="136a2-202">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="136a2-202">storageRequireEncryption</span></span>|<span data-ttu-id="136a2-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="136a2-203">Boolean</span></span>|<span data-ttu-id="136a2-204">要求对 Android 设备加密。</span><span class="sxs-lookup"><span data-stu-id="136a2-204">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="136a2-205">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="136a2-205">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="136a2-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="136a2-206">Boolean</span></span>|<span data-ttu-id="136a2-207">要求设备传递 SafetyNet 基本完整性检查。</span><span class="sxs-lookup"><span data-stu-id="136a2-207">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="136a2-208">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="136a2-208">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="136a2-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="136a2-209">Boolean</span></span>|<span data-ttu-id="136a2-210">要求设备传递 SafetyNet 认证设备检查。</span><span class="sxs-lookup"><span data-stu-id="136a2-210">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="136a2-211">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="136a2-211">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="136a2-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="136a2-212">Boolean</span></span>|<span data-ttu-id="136a2-213">要求在设备上安装并启用 Google Play Services。</span><span class="sxs-lookup"><span data-stu-id="136a2-213">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="136a2-214">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="136a2-214">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="136a2-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="136a2-215">Boolean</span></span>|<span data-ttu-id="136a2-216">要求设备具有最新的安全提供程序。</span><span class="sxs-lookup"><span data-stu-id="136a2-216">Require the device to have up to date security providers.</span></span> <span data-ttu-id="136a2-217">设备将要求启用 Google Play Services 并保持最新状态。</span><span class="sxs-lookup"><span data-stu-id="136a2-217">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="136a2-218">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="136a2-218">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="136a2-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="136a2-219">Boolean</span></span>|<span data-ttu-id="136a2-220">要求设备传递公司门户客户端应用运行时完整性检查。</span><span class="sxs-lookup"><span data-stu-id="136a2-220">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="136a2-221">响应</span><span class="sxs-lookup"><span data-stu-id="136a2-221">Response</span></span>
<span data-ttu-id="136a2-222">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[androidWorkProfileCompliancePolicy](../resources/intune_deviceconfig_androidworkprofilecompliancepolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="136a2-222">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileCompliancePolicy](../resources/intune_deviceconfig_androidworkprofilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="136a2-223">示例</span><span class="sxs-lookup"><span data-stu-id="136a2-223">Example</span></span>
### <a name="request"></a><span data-ttu-id="136a2-224">请求</span><span class="sxs-lookup"><span data-stu-id="136a2-224">Request</span></span>
<span data-ttu-id="136a2-225">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="136a2-225">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1170

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
  "description": "Description value",
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

### <a name="response"></a><span data-ttu-id="136a2-226">响应</span><span class="sxs-lookup"><span data-stu-id="136a2-226">Response</span></span>
<span data-ttu-id="136a2-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="136a2-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



