# <a name="update-windows10mobilecompliancepolicy"></a><span data-ttu-id="a77f9-101">更新 windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="a77f9-101">Update windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="a77f9-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a77f9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a77f9-103">更新 [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a77f9-103">Update the properties of a [calendar](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a77f9-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="a77f9-104">Prerequisites</span></span>
<span data-ttu-id="a77f9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a77f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a77f9-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="a77f9-107">Permission type</span></span>|<span data-ttu-id="a77f9-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a77f9-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a77f9-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a77f9-109">Delegated (work or school account)</span></span>|<span data-ttu-id="a77f9-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a77f9-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a77f9-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a77f9-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a77f9-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="a77f9-112">Not supported.</span></span>|
|<span data-ttu-id="a77f9-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="a77f9-113">Application</span></span>|<span data-ttu-id="a77f9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a77f9-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a77f9-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a77f9-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="a77f9-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="a77f9-116">Request headers</span></span>
|<span data-ttu-id="a77f9-117">标头</span><span class="sxs-lookup"><span data-stu-id="a77f9-117">Header</span></span>|<span data-ttu-id="a77f9-118">值</span><span class="sxs-lookup"><span data-stu-id="a77f9-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a77f9-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="a77f9-119">Authorization</span></span>|<span data-ttu-id="a77f9-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a77f9-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a77f9-121">Accept</span><span class="sxs-lookup"><span data-stu-id="a77f9-121">Accept</span></span>|<span data-ttu-id="a77f9-122">application/json</span><span class="sxs-lookup"><span data-stu-id="a77f9-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a77f9-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="a77f9-123">Request body</span></span>
<span data-ttu-id="a77f9-124">在请求正文中，提供 [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a77f9-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md) object.</span></span>

<span data-ttu-id="a77f9-125">下表显示了创建 [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a77f9-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="a77f9-126">属性</span><span class="sxs-lookup"><span data-stu-id="a77f9-126">Property</span></span>|<span data-ttu-id="a77f9-127">类型</span><span class="sxs-lookup"><span data-stu-id="a77f9-127">Type</span></span>|<span data-ttu-id="a77f9-128">说明</span><span class="sxs-lookup"><span data-stu-id="a77f9-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a77f9-129">id</span><span class="sxs-lookup"><span data-stu-id="a77f9-129">id</span></span>|<span data-ttu-id="a77f9-130">String</span><span class="sxs-lookup"><span data-stu-id="a77f9-130">String</span></span>|<span data-ttu-id="a77f9-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a77f9-131">Key of the setting.</span></span> <span data-ttu-id="a77f9-132">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a77f9-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a77f9-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a77f9-133">createdDateTime</span></span>|<span data-ttu-id="a77f9-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a77f9-134">DateTimeOffset</span></span>|<span data-ttu-id="a77f9-135">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a77f9-135">DateTime the object was created.</span></span> <span data-ttu-id="a77f9-136">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a77f9-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a77f9-137">description</span><span class="sxs-lookup"><span data-stu-id="a77f9-137">description</span></span>|<span data-ttu-id="a77f9-138">String</span><span class="sxs-lookup"><span data-stu-id="a77f9-138">String</span></span>|<span data-ttu-id="a77f9-139">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="a77f9-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a77f9-140">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a77f9-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a77f9-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a77f9-141">lastModifiedDateTime</span></span>|<span data-ttu-id="a77f9-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a77f9-142">DateTimeOffset</span></span>|<span data-ttu-id="a77f9-143">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a77f9-143">Indicates the date the object was last modified.</span></span> <span data-ttu-id="a77f9-144">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a77f9-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a77f9-145">displayName</span><span class="sxs-lookup"><span data-stu-id="a77f9-145">displayName</span></span>|<span data-ttu-id="a77f9-146">String</span><span class="sxs-lookup"><span data-stu-id="a77f9-146">String</span></span>|<span data-ttu-id="a77f9-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="a77f9-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a77f9-148">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a77f9-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a77f9-149">version</span><span class="sxs-lookup"><span data-stu-id="a77f9-149">version</span></span>|<span data-ttu-id="a77f9-150">Int32</span><span class="sxs-lookup"><span data-stu-id="a77f9-150">Int32</span></span>|<span data-ttu-id="a77f9-151">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="a77f9-151">Version of the device configuration.</span></span> <span data-ttu-id="a77f9-152">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a77f9-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a77f9-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="a77f9-153">passwordRequired</span></span>|<span data-ttu-id="a77f9-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="a77f9-154">Boolean</span></span>|<span data-ttu-id="a77f9-155">需要密码才可解锁 Windows Phone 设备。</span><span class="sxs-lookup"><span data-stu-id="a77f9-155">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="a77f9-156">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="a77f9-156">passwordBlockSimple</span></span>|<span data-ttu-id="a77f9-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="a77f9-157">Boolean</span></span>|<span data-ttu-id="a77f9-158">是否阻止同步日历。</span><span class="sxs-lookup"><span data-stu-id="a77f9-158">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="a77f9-159">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="a77f9-159">passwordMinimumLength</span></span>|<span data-ttu-id="a77f9-160">Int32</span><span class="sxs-lookup"><span data-stu-id="a77f9-160">Int32</span></span>|<span data-ttu-id="a77f9-161">最短密码长度。</span><span class="sxs-lookup"><span data-stu-id="a77f9-161">Minimum password length.</span></span> <span data-ttu-id="a77f9-162">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="a77f9-162">Valid values 4 to 16</span></span>|
|<span data-ttu-id="a77f9-163">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="a77f9-163">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="a77f9-164">Int32</span><span class="sxs-lookup"><span data-stu-id="a77f9-164">Int32</span></span>|<span data-ttu-id="a77f9-165">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="a77f9-165">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="a77f9-166">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="a77f9-166">passwordRequiredType</span></span>|<span data-ttu-id="a77f9-167">String</span><span class="sxs-lookup"><span data-stu-id="a77f9-167">String</span></span>|<span data-ttu-id="a77f9-168">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="a77f9-168">The required password type.</span></span> <span data-ttu-id="a77f9-169">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="a77f9-169">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="a77f9-170">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="a77f9-170">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="a77f9-171">Int32</span><span class="sxs-lookup"><span data-stu-id="a77f9-171">Int32</span></span>|<span data-ttu-id="a77f9-172">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="a77f9-172">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="a77f9-173">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="a77f9-173">passwordExpirationDays</span></span>|<span data-ttu-id="a77f9-174">Int32</span><span class="sxs-lookup"><span data-stu-id="a77f9-174">Int32</span></span>|<span data-ttu-id="a77f9-175">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="a77f9-175">Number of days before password expiration.</span></span> <span data-ttu-id="a77f9-176">有效值为 1 至 255</span><span class="sxs-lookup"><span data-stu-id="a77f9-176">Valid values 1 to 255</span></span>|
|<span data-ttu-id="a77f9-177">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="a77f9-177">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="a77f9-178">Int32</span><span class="sxs-lookup"><span data-stu-id="a77f9-178">Int32</span></span>|<span data-ttu-id="a77f9-179">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="a77f9-179">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="a77f9-180">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="a77f9-180">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="a77f9-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="a77f9-181">Boolean</span></span>|<span data-ttu-id="a77f9-182">需要密码才可解锁空闲设备。</span><span class="sxs-lookup"><span data-stu-id="a77f9-182">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="a77f9-183">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="a77f9-183">osMinimumVersion</span></span>|<span data-ttu-id="a77f9-184">String</span><span class="sxs-lookup"><span data-stu-id="a77f9-184">String</span></span>|<span data-ttu-id="a77f9-185">最低 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="a77f9-185">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="a77f9-186">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="a77f9-186">osMaximumVersion</span></span>|<span data-ttu-id="a77f9-187">String</span><span class="sxs-lookup"><span data-stu-id="a77f9-187">String</span></span>|<span data-ttu-id="a77f9-188">最高 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="a77f9-188">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="a77f9-189">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="a77f9-189">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="a77f9-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="a77f9-190">Boolean</span></span>|<span data-ttu-id="a77f9-191">要求设备由 Windows 设备运行状况证明报告为正常 - 提前启动反恶意驱动程序已启用。</span><span class="sxs-lookup"><span data-stu-id="a77f9-191">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="a77f9-192">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="a77f9-192">bitLockerEnabled</span></span>|<span data-ttu-id="a77f9-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="a77f9-193">Boolean</span></span>|<span data-ttu-id="a77f9-194">要求设备由 Windows 设备运行状况证明报告为正常 - bit locker 已启用。</span><span class="sxs-lookup"><span data-stu-id="a77f9-194">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="a77f9-195">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="a77f9-195">secureBootEnabled</span></span>|<span data-ttu-id="a77f9-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="a77f9-196">Boolean</span></span>|<span data-ttu-id="a77f9-197">要求设备由 Windows 设备运行状况证明报告为正常 - 安全启动已启用。</span><span class="sxs-lookup"><span data-stu-id="a77f9-197">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="a77f9-198">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="a77f9-198">codeIntegrityEnabled</span></span>|<span data-ttu-id="a77f9-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="a77f9-199">Boolean</span></span>|<span data-ttu-id="a77f9-200">要求设备由 Windows 设备运行状况证明报告为正常。</span><span class="sxs-lookup"><span data-stu-id="a77f9-200">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="a77f9-201">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="a77f9-201">storageRequireEncryption</span></span>|<span data-ttu-id="a77f9-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="a77f9-202">Boolean</span></span>|<span data-ttu-id="a77f9-203">要求对 Windows 设备加密。</span><span class="sxs-lookup"><span data-stu-id="a77f9-203">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="a77f9-204">响应</span><span class="sxs-lookup"><span data-stu-id="a77f9-204">Response</span></span>
<span data-ttu-id="a77f9-205">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a77f9-205">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a77f9-206">示例</span><span class="sxs-lookup"><span data-stu-id="a77f9-206">Example</span></span>
### <a name="request"></a><span data-ttu-id="a77f9-207">请求</span><span class="sxs-lookup"><span data-stu-id="a77f9-207">Request</span></span>
<span data-ttu-id="a77f9-208">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a77f9-208">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 786

{
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordExpirationDays": 6,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordRequireToUnlockFromIdle": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="a77f9-209">响应</span><span class="sxs-lookup"><span data-stu-id="a77f9-209">Response</span></span>
<span data-ttu-id="a77f9-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a77f9-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 964

{
  "@odata.type": "#microsoft.graph.windows10MobileCompliancePolicy",
  "id": "3d4237b0-37b0-3d42-b037-423db037423d",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordExpirationDays": 6,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordRequireToUnlockFromIdle": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true
}
```



