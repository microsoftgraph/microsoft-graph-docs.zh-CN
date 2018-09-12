# <a name="create-ioscompliancepolicy"></a><span data-ttu-id="97483-101">创建 iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="97483-101">Create iosCompliancePolicy</span></span>

> <span data-ttu-id="97483-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="97483-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="97483-103">创建新的 [iosCompliancePolicy](../resources/intune_deviceconfig_ioscompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="97483-103">Create a new [iosCompliancePolicy](../resources/intune_deviceconfig_ioscompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="97483-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="97483-104">Prerequisites</span></span>
<span data-ttu-id="97483-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="97483-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="97483-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="97483-107">Permission type</span></span>|<span data-ttu-id="97483-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="97483-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97483-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="97483-109">Delegated (work or school account)</span></span>|<span data-ttu-id="97483-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97483-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="97483-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="97483-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97483-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="97483-112">Not supported.</span></span>|
|<span data-ttu-id="97483-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="97483-113">Application</span></span>|<span data-ttu-id="97483-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="97483-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="97483-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="97483-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="97483-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="97483-116">Request headers</span></span>
|<span data-ttu-id="97483-117">标头</span><span class="sxs-lookup"><span data-stu-id="97483-117">Header</span></span>|<span data-ttu-id="97483-118">值</span><span class="sxs-lookup"><span data-stu-id="97483-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="97483-119">授权</span><span class="sxs-lookup"><span data-stu-id="97483-119">Authorization</span></span>|<span data-ttu-id="97483-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="97483-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="97483-121">接受</span><span class="sxs-lookup"><span data-stu-id="97483-121">Accept</span></span>|<span data-ttu-id="97483-122">application/json</span><span class="sxs-lookup"><span data-stu-id="97483-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="97483-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="97483-123">Request body</span></span>
<span data-ttu-id="97483-124">在请求正文中，提供 iosCompliancePolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="97483-124">In the request body, supply a JSON representation for the iosCompliancePolicy object.</span></span>

<span data-ttu-id="97483-125">下表显示了创建 iosCompliancePolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="97483-125">The following table shows the properties that are required when you create the iosCompliancePolicy.</span></span>

|<span data-ttu-id="97483-126">属性</span><span class="sxs-lookup"><span data-stu-id="97483-126">Property</span></span>|<span data-ttu-id="97483-127">类型</span><span class="sxs-lookup"><span data-stu-id="97483-127">Type</span></span>|<span data-ttu-id="97483-128">说明</span><span class="sxs-lookup"><span data-stu-id="97483-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97483-129">ID</span><span class="sxs-lookup"><span data-stu-id="97483-129">id</span></span>|<span data-ttu-id="97483-130">字符串</span><span class="sxs-lookup"><span data-stu-id="97483-130">String</span></span>|<span data-ttu-id="97483-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="97483-131">Key of the entity.</span></span> <span data-ttu-id="97483-132">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="97483-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="97483-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="97483-133">createdDateTime</span></span>|<span data-ttu-id="97483-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97483-134">DateTimeOffset</span></span>|<span data-ttu-id="97483-135">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="97483-135">DateTime the object was created.</span></span> <span data-ttu-id="97483-136">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="97483-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="97483-137">说明</span><span class="sxs-lookup"><span data-stu-id="97483-137">description</span></span>|<span data-ttu-id="97483-138">字符串</span><span class="sxs-lookup"><span data-stu-id="97483-138">String</span></span>|<span data-ttu-id="97483-139">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="97483-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="97483-140">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="97483-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="97483-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="97483-141">lastModifiedDateTime</span></span>|<span data-ttu-id="97483-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97483-142">DateTimeOffset</span></span>|<span data-ttu-id="97483-143">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="97483-143">DateTime the object was last modified.</span></span> <span data-ttu-id="97483-144">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="97483-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="97483-145">displayName</span><span class="sxs-lookup"><span data-stu-id="97483-145">displayName</span></span>|<span data-ttu-id="97483-146">字符串</span><span class="sxs-lookup"><span data-stu-id="97483-146">String</span></span>|<span data-ttu-id="97483-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="97483-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="97483-148">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="97483-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="97483-149">version</span><span class="sxs-lookup"><span data-stu-id="97483-149">version</span></span>|<span data-ttu-id="97483-150">Int32</span><span class="sxs-lookup"><span data-stu-id="97483-150">Int32</span></span>|<span data-ttu-id="97483-151">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="97483-151">Version of the device configuration.</span></span> <span data-ttu-id="97483-152">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="97483-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="97483-153">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="97483-153">passcodeBlockSimple</span></span>|<span data-ttu-id="97483-154">布尔值</span><span class="sxs-lookup"><span data-stu-id="97483-154">Boolean</span></span>|<span data-ttu-id="97483-155">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="97483-155">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="97483-156">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="97483-156">passcodeExpirationDays</span></span>|<span data-ttu-id="97483-157">Int32</span><span class="sxs-lookup"><span data-stu-id="97483-157">Int32</span></span>|<span data-ttu-id="97483-158">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="97483-158">Number of days before the passcode expires.</span></span> <span data-ttu-id="97483-159">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="97483-159">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="97483-160">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="97483-160">passcodeMinimumLength</span></span>|<span data-ttu-id="97483-161">Int32</span><span class="sxs-lookup"><span data-stu-id="97483-161">Int32</span></span>|<span data-ttu-id="97483-162">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="97483-162">Minimum length of passcode.</span></span> <span data-ttu-id="97483-163">有效值为 4 至 14</span><span class="sxs-lookup"><span data-stu-id="97483-163">Valid values 4 to 14</span></span>|
|<span data-ttu-id="97483-164">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="97483-164">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="97483-165">Int32</span><span class="sxs-lookup"><span data-stu-id="97483-165">Int32</span></span>|<span data-ttu-id="97483-166">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="97483-166">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="97483-167">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="97483-167">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="97483-168">Int32</span><span class="sxs-lookup"><span data-stu-id="97483-168">Int32</span></span>|<span data-ttu-id="97483-169">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="97483-169">Number of previous passcodes to block.</span></span> <span data-ttu-id="97483-170">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="97483-170">Valid values 1 to 24</span></span>|
|<span data-ttu-id="97483-171">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="97483-171">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="97483-172">Int32</span><span class="sxs-lookup"><span data-stu-id="97483-172">Int32</span></span>|<span data-ttu-id="97483-173">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="97483-173">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="97483-174">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="97483-174">passcodeRequiredType</span></span>|[<span data-ttu-id="97483-175">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="97483-175">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="97483-176">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="97483-176">The required passcode type.</span></span> <span data-ttu-id="97483-177">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="97483-177">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="97483-178">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="97483-178">passcodeRequired</span></span>|<span data-ttu-id="97483-179">布尔值</span><span class="sxs-lookup"><span data-stu-id="97483-179">Boolean</span></span>|<span data-ttu-id="97483-180">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="97483-180">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="97483-181">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="97483-181">osMinimumVersion</span></span>|<span data-ttu-id="97483-182">字符串</span><span class="sxs-lookup"><span data-stu-id="97483-182">String</span></span>|<span data-ttu-id="97483-183">最低 IOS 版本。</span><span class="sxs-lookup"><span data-stu-id="97483-183">Minimum IOS version.</span></span>|
|<span data-ttu-id="97483-184">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="97483-184">osMaximumVersion</span></span>|<span data-ttu-id="97483-185">字符串</span><span class="sxs-lookup"><span data-stu-id="97483-185">String</span></span>|<span data-ttu-id="97483-186">最高 IOS 版本。</span><span class="sxs-lookup"><span data-stu-id="97483-186">Maximum IOS version.</span></span>|
|<span data-ttu-id="97483-187">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="97483-187">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="97483-188">布尔</span><span class="sxs-lookup"><span data-stu-id="97483-188">Boolean</span></span>|<span data-ttu-id="97483-189">设备不得越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="97483-189">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="97483-190">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="97483-190">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="97483-191">布尔值</span><span class="sxs-lookup"><span data-stu-id="97483-191">Boolean</span></span>|<span data-ttu-id="97483-192">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="97483-192">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="97483-193">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="97483-193">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="97483-194">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="97483-194">deviceThreatProtectionLevel</span></span>](../resources/intune_deviceconfig_devicethreatprotectionlevel.md)|<span data-ttu-id="97483-195">要求移动威胁防护最低风险级别来报告不符合情况。</span><span class="sxs-lookup"><span data-stu-id="97483-195">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="97483-196">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="97483-196">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="97483-197">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="97483-197">managedEmailProfileRequired</span></span>|<span data-ttu-id="97483-198">布尔值</span><span class="sxs-lookup"><span data-stu-id="97483-198">Boolean</span></span>|<span data-ttu-id="97483-199">指示是否需要托管电子邮件配置文件。</span><span class="sxs-lookup"><span data-stu-id="97483-199">Indicates whether or not to require a managed email profile.</span></span>|



## <a name="response"></a><span data-ttu-id="97483-200">响应</span><span class="sxs-lookup"><span data-stu-id="97483-200">Response</span></span>
<span data-ttu-id="97483-201">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [iosCompliancePolicy](../resources/intune_deviceconfig_ioscompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="97483-201">If successful, this method returns a `201 Created` response code and a [iosCompliancePolicy](../resources/intune_deviceconfig_ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97483-202">示例</span><span class="sxs-lookup"><span data-stu-id="97483-202">Example</span></span>
### <a name="request"></a><span data-ttu-id="97483-203">请求</span><span class="sxs-lookup"><span data-stu-id="97483-203">Request</span></span>
<span data-ttu-id="97483-204">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="97483-204">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 809

{
  "@odata.type": "#microsoft.graph.iosCompliancePolicy",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "securityBlockJailbrokenDevices": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "managedEmailProfileRequired": true
}
```

### <a name="response"></a><span data-ttu-id="97483-205">响应</span><span class="sxs-lookup"><span data-stu-id="97483-205">Response</span></span>
<span data-ttu-id="97483-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="97483-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 917

{
  "@odata.type": "#microsoft.graph.iosCompliancePolicy",
  "id": "4f501351-1351-4f50-5113-504f5113504f",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "securityBlockJailbrokenDevices": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "managedEmailProfileRequired": true
}
```








