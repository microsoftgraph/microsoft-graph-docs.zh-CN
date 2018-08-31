# <a name="update-windows10compliancepolicy"></a><span data-ttu-id="f95c0-101">更新 windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="f95c0-101">Update windows10CompliancePolicy</span></span>

> <span data-ttu-id="f95c0-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f95c0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f95c0-103">更新 [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f95c0-103">Update the properties of a [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f95c0-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="f95c0-104">Prerequisites</span></span>
<span data-ttu-id="f95c0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="f95c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f95c0-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="f95c0-107">Permission type</span></span>|<span data-ttu-id="f95c0-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f95c0-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f95c0-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f95c0-109">Delegated (work or school account)</span></span>|<span data-ttu-id="f95c0-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f95c0-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f95c0-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f95c0-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f95c0-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="f95c0-112">Not supported.</span></span>|
|<span data-ttu-id="f95c0-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="f95c0-113">Application</span></span>|<span data-ttu-id="f95c0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f95c0-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f95c0-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f95c0-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="f95c0-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="f95c0-116">Request headers</span></span>
|<span data-ttu-id="f95c0-117">标头</span><span class="sxs-lookup"><span data-stu-id="f95c0-117">Header</span></span>|<span data-ttu-id="f95c0-118">值</span><span class="sxs-lookup"><span data-stu-id="f95c0-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f95c0-119">授权</span><span class="sxs-lookup"><span data-stu-id="f95c0-119">Authorization</span></span>|<span data-ttu-id="f95c0-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f95c0-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f95c0-121">接受</span><span class="sxs-lookup"><span data-stu-id="f95c0-121">Accept</span></span>|<span data-ttu-id="f95c0-122">application/json</span><span class="sxs-lookup"><span data-stu-id="f95c0-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f95c0-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="f95c0-123">Request body</span></span>
<span data-ttu-id="f95c0-124">在请求正文中，提供 [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f95c0-124">In the request body, supply a JSON representation for the [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md) object.</span></span>

<span data-ttu-id="f95c0-125">下表显示创建 [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f95c0-125">The following table shows the properties that are required when you create the [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md).</span></span>

|<span data-ttu-id="f95c0-126">属性</span><span class="sxs-lookup"><span data-stu-id="f95c0-126">Property</span></span>|<span data-ttu-id="f95c0-127">类型</span><span class="sxs-lookup"><span data-stu-id="f95c0-127">Type</span></span>|<span data-ttu-id="f95c0-128">说明</span><span class="sxs-lookup"><span data-stu-id="f95c0-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f95c0-129">id</span><span class="sxs-lookup"><span data-stu-id="f95c0-129">id</span></span>|<span data-ttu-id="f95c0-130">字符串</span><span class="sxs-lookup"><span data-stu-id="f95c0-130">String</span></span>|<span data-ttu-id="f95c0-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f95c0-131">Key of the entity.</span></span> <span data-ttu-id="f95c0-132">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f95c0-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f95c0-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f95c0-133">createdDateTime</span></span>|<span data-ttu-id="f95c0-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f95c0-134">DateTimeOffset</span></span>|<span data-ttu-id="f95c0-135">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f95c0-135">DateTime the object was created.</span></span> <span data-ttu-id="f95c0-136">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f95c0-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f95c0-137">description</span><span class="sxs-lookup"><span data-stu-id="f95c0-137">description</span></span>|<span data-ttu-id="f95c0-138">String</span><span class="sxs-lookup"><span data-stu-id="f95c0-138">String</span></span>|<span data-ttu-id="f95c0-139">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="f95c0-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f95c0-140">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f95c0-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f95c0-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f95c0-141">lastModifiedDateTime</span></span>|<span data-ttu-id="f95c0-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f95c0-142">DateTimeOffset</span></span>|<span data-ttu-id="f95c0-143">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f95c0-143">DateTime the object was last modified.</span></span> <span data-ttu-id="f95c0-144">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f95c0-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f95c0-145">displayName</span><span class="sxs-lookup"><span data-stu-id="f95c0-145">displayName</span></span>|<span data-ttu-id="f95c0-146">String</span><span class="sxs-lookup"><span data-stu-id="f95c0-146">String</span></span>|<span data-ttu-id="f95c0-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="f95c0-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f95c0-148">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f95c0-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f95c0-149">version</span><span class="sxs-lookup"><span data-stu-id="f95c0-149">version</span></span>|<span data-ttu-id="f95c0-150">Int32</span><span class="sxs-lookup"><span data-stu-id="f95c0-150">Int32</span></span>|<span data-ttu-id="f95c0-151">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="f95c0-151">Version of the device configuration.</span></span> <span data-ttu-id="f95c0-152">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f95c0-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f95c0-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="f95c0-153">passwordRequired</span></span>|<span data-ttu-id="f95c0-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="f95c0-154">Boolean</span></span>|<span data-ttu-id="f95c0-155">需要密码才可解锁 Windows 设备。</span><span class="sxs-lookup"><span data-stu-id="f95c0-155">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="f95c0-156">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="f95c0-156">passwordBlockSimple</span></span>|<span data-ttu-id="f95c0-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="f95c0-157">Boolean</span></span>|<span data-ttu-id="f95c0-158">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="f95c0-158">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="f95c0-159">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="f95c0-159">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="f95c0-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="f95c0-160">Boolean</span></span>|<span data-ttu-id="f95c0-161">需要密码才可解锁空闲设备。</span><span class="sxs-lookup"><span data-stu-id="f95c0-161">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="f95c0-162">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="f95c0-162">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="f95c0-163">Int32</span><span class="sxs-lookup"><span data-stu-id="f95c0-163">Int32</span></span>|<span data-ttu-id="f95c0-164">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="f95c0-164">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="f95c0-165">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="f95c0-165">passwordExpirationDays</span></span>|<span data-ttu-id="f95c0-166">Int32</span><span class="sxs-lookup"><span data-stu-id="f95c0-166">Int32</span></span>|<span data-ttu-id="f95c0-167">密码过期天数。</span><span class="sxs-lookup"><span data-stu-id="f95c0-167">The password expiration in days.</span></span>|
|<span data-ttu-id="f95c0-168">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="f95c0-168">passwordMinimumLength</span></span>|<span data-ttu-id="f95c0-169">Int32</span><span class="sxs-lookup"><span data-stu-id="f95c0-169">Int32</span></span>|<span data-ttu-id="f95c0-170">密码最短长度。</span><span class="sxs-lookup"><span data-stu-id="f95c0-170">The minimum password length.</span></span>|
|<span data-ttu-id="f95c0-171">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="f95c0-171">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="f95c0-172">Int32</span><span class="sxs-lookup"><span data-stu-id="f95c0-172">Int32</span></span>|<span data-ttu-id="f95c0-173">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="f95c0-173">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="f95c0-174">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="f95c0-174">passwordRequiredType</span></span>|[<span data-ttu-id="f95c0-175">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="f95c0-175">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="f95c0-176">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="f95c0-176">The required password type.</span></span> <span data-ttu-id="f95c0-177">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="f95c0-177">The possible values are `deviceDefault`, `alphanumeric`, `numeric`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="f95c0-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="f95c0-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="f95c0-179">Int32</span><span class="sxs-lookup"><span data-stu-id="f95c0-179">Int32</span></span>|<span data-ttu-id="f95c0-180">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="f95c0-180">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="f95c0-181">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="f95c0-181">requireHealthyDeviceReport</span></span>|<span data-ttu-id="f95c0-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="f95c0-182">Boolean</span></span>|<span data-ttu-id="f95c0-183">要求设备由 Windows 设备运行状况证明报告为正常。</span><span class="sxs-lookup"><span data-stu-id="f95c0-183">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="f95c0-184">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="f95c0-184">osMinimumVersion</span></span>|<span data-ttu-id="f95c0-185">String</span><span class="sxs-lookup"><span data-stu-id="f95c0-185">String</span></span>|<span data-ttu-id="f95c0-186">最低 Windows 10 版本。</span><span class="sxs-lookup"><span data-stu-id="f95c0-186">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="f95c0-187">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="f95c0-187">osMaximumVersion</span></span>|<span data-ttu-id="f95c0-188">String</span><span class="sxs-lookup"><span data-stu-id="f95c0-188">String</span></span>|<span data-ttu-id="f95c0-189">最高 Windows 10 版本。</span><span class="sxs-lookup"><span data-stu-id="f95c0-189">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="f95c0-190">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="f95c0-190">mobileOsMinimumVersion</span></span>|<span data-ttu-id="f95c0-191">String</span><span class="sxs-lookup"><span data-stu-id="f95c0-191">String</span></span>|<span data-ttu-id="f95c0-192">最低 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="f95c0-192">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="f95c0-193">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="f95c0-193">mobileOsMaximumVersion</span></span>|<span data-ttu-id="f95c0-194">String</span><span class="sxs-lookup"><span data-stu-id="f95c0-194">String</span></span>|<span data-ttu-id="f95c0-195">最高 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="f95c0-195">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="f95c0-196">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="f95c0-196">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="f95c0-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="f95c0-197">Boolean</span></span>|<span data-ttu-id="f95c0-198">要求设备由 Windows 设备运行状况证明报告为正常 - 提前启动反恶意驱动程序已启用。</span><span class="sxs-lookup"><span data-stu-id="f95c0-198">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="f95c0-199">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="f95c0-199">bitLockerEnabled</span></span>|<span data-ttu-id="f95c0-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="f95c0-200">Boolean</span></span>|<span data-ttu-id="f95c0-201">要求设备由 Windows 设备运行状况证明报告为正常 - bit locker 已启用。</span><span class="sxs-lookup"><span data-stu-id="f95c0-201">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="f95c0-202">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="f95c0-202">secureBootEnabled</span></span>|<span data-ttu-id="f95c0-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="f95c0-203">Boolean</span></span>|<span data-ttu-id="f95c0-204">要求设备由 Windows 设备运行状况证明报告为正常 - 安全启动已启用。</span><span class="sxs-lookup"><span data-stu-id="f95c0-204">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="f95c0-205">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="f95c0-205">codeIntegrityEnabled</span></span>|<span data-ttu-id="f95c0-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="f95c0-206">Boolean</span></span>|<span data-ttu-id="f95c0-207">要求设备由 Windows 设备运行状况证明报告为正常。</span><span class="sxs-lookup"><span data-stu-id="f95c0-207">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="f95c0-208">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="f95c0-208">storageRequireEncryption</span></span>|<span data-ttu-id="f95c0-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="f95c0-209">Boolean</span></span>|<span data-ttu-id="f95c0-210">要求对 Windows 设备加密。</span><span class="sxs-lookup"><span data-stu-id="f95c0-210">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="f95c0-211">响应</span><span class="sxs-lookup"><span data-stu-id="f95c0-211">Response</span></span>
<span data-ttu-id="f95c0-212">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f95c0-212">If successful, this method returns a `200 OK` response code and an updated [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f95c0-213">示例</span><span class="sxs-lookup"><span data-stu-id="f95c0-213">Example</span></span>
### <a name="request"></a><span data-ttu-id="f95c0-214">请求</span><span class="sxs-lookup"><span data-stu-id="f95c0-214">Request</span></span>
<span data-ttu-id="f95c0-215">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f95c0-215">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 954

{
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordRequiredToUnlockFromIdle": true,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "requireHealthyDeviceReport": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "mobileOsMinimumVersion": "Mobile Os Minimum Version value",
  "mobileOsMaximumVersion": "Mobile Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="f95c0-216">响应</span><span class="sxs-lookup"><span data-stu-id="f95c0-216">Response</span></span>
<span data-ttu-id="f95c0-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f95c0-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1126

{
  "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
  "id": "2919ae62-ae62-2919-62ae-192962ae1929",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordRequiredToUnlockFromIdle": true,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "requireHealthyDeviceReport": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "mobileOsMinimumVersion": "Mobile Os Minimum Version value",
  "mobileOsMaximumVersion": "Mobile Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true
}
```



