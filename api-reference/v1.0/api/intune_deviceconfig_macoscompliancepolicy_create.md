# <a name="create-macoscompliancepolicy"></a><span data-ttu-id="8f05e-101">创建 macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="8f05e-101">Create macOSCompliancePolicy</span></span>

> <span data-ttu-id="8f05e-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8f05e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8f05e-103">创建新的 [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8f05e-103">Create a new [plannerBucket](../resources/intune_deviceconfig_macoscompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8f05e-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="8f05e-104">Prerequisites</span></span>
<span data-ttu-id="8f05e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="8f05e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8f05e-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="8f05e-107">Permission type</span></span>|<span data-ttu-id="8f05e-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8f05e-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f05e-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8f05e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="8f05e-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f05e-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8f05e-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8f05e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f05e-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="8f05e-112">Not supported.</span></span>|
|<span data-ttu-id="8f05e-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="8f05e-113">Application</span></span>|<span data-ttu-id="8f05e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8f05e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8f05e-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8f05e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="8f05e-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="8f05e-116">Request headers</span></span>
|<span data-ttu-id="8f05e-117">标头</span><span class="sxs-lookup"><span data-stu-id="8f05e-117">Header</span></span>|<span data-ttu-id="8f05e-118">值</span><span class="sxs-lookup"><span data-stu-id="8f05e-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8f05e-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f05e-119">Authorization</span></span>|<span data-ttu-id="8f05e-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8f05e-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8f05e-121">Accept</span><span class="sxs-lookup"><span data-stu-id="8f05e-121">Accept</span></span>|<span data-ttu-id="8f05e-122">application/json</span><span class="sxs-lookup"><span data-stu-id="8f05e-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f05e-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="8f05e-123">Request body</span></span>
<span data-ttu-id="8f05e-124">在请求正文中，提供 macOSCompliancePolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8f05e-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="8f05e-125">下表显示创建 macOSCompliancePolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8f05e-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="8f05e-126">属性</span><span class="sxs-lookup"><span data-stu-id="8f05e-126">Property</span></span>|<span data-ttu-id="8f05e-127">类型</span><span class="sxs-lookup"><span data-stu-id="8f05e-127">Type</span></span>|<span data-ttu-id="8f05e-128">说明</span><span class="sxs-lookup"><span data-stu-id="8f05e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f05e-129">id</span><span class="sxs-lookup"><span data-stu-id="8f05e-129">id</span></span>|<span data-ttu-id="8f05e-130">String</span><span class="sxs-lookup"><span data-stu-id="8f05e-130">String</span></span>|<span data-ttu-id="8f05e-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="8f05e-131">Key of the setting.</span></span> <span data-ttu-id="8f05e-132">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8f05e-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8f05e-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8f05e-133">createdDateTime</span></span>|<span data-ttu-id="8f05e-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f05e-134">DateTimeOffset</span></span>|<span data-ttu-id="8f05e-135">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="8f05e-135">DateTime the object was created.</span></span> <span data-ttu-id="8f05e-136">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8f05e-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8f05e-137">description</span><span class="sxs-lookup"><span data-stu-id="8f05e-137">description</span></span>|<span data-ttu-id="8f05e-138">String</span><span class="sxs-lookup"><span data-stu-id="8f05e-138">String</span></span>|<span data-ttu-id="8f05e-139">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="8f05e-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8f05e-140">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8f05e-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8f05e-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8f05e-141">lastModifiedDateTime</span></span>|<span data-ttu-id="8f05e-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f05e-142">DateTimeOffset</span></span>|<span data-ttu-id="8f05e-143">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="8f05e-143">Indicates the date the object was last modified.</span></span> <span data-ttu-id="8f05e-144">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8f05e-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8f05e-145">displayName</span><span class="sxs-lookup"><span data-stu-id="8f05e-145">displayName</span></span>|<span data-ttu-id="8f05e-146">String</span><span class="sxs-lookup"><span data-stu-id="8f05e-146">String</span></span>|<span data-ttu-id="8f05e-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="8f05e-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8f05e-148">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8f05e-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8f05e-149">version</span><span class="sxs-lookup"><span data-stu-id="8f05e-149">version</span></span>|<span data-ttu-id="8f05e-150">Int32</span><span class="sxs-lookup"><span data-stu-id="8f05e-150">Int32</span></span>|<span data-ttu-id="8f05e-151">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="8f05e-151">Version of the device configuration.</span></span> <span data-ttu-id="8f05e-152">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8f05e-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8f05e-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="8f05e-153">passwordRequired</span></span>|<span data-ttu-id="8f05e-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f05e-154">Boolean</span></span>|<span data-ttu-id="8f05e-155">是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="8f05e-155">Whether or not to require a password.</span></span>|
|<span data-ttu-id="8f05e-156">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="8f05e-156">passwordBlockSimple</span></span>|<span data-ttu-id="8f05e-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f05e-157">Boolean</span></span>|<span data-ttu-id="8f05e-158">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="8f05e-158">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="8f05e-159">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="8f05e-159">passwordExpirationDays</span></span>|<span data-ttu-id="8f05e-160">Int32</span><span class="sxs-lookup"><span data-stu-id="8f05e-160">Int32</span></span>|<span data-ttu-id="8f05e-161">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="8f05e-161">Number of days before the password expires.</span></span> <span data-ttu-id="8f05e-162">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="8f05e-162">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="8f05e-163">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="8f05e-163">passwordMinimumLength</span></span>|<span data-ttu-id="8f05e-164">Int32</span><span class="sxs-lookup"><span data-stu-id="8f05e-164">Int32</span></span>|<span data-ttu-id="8f05e-165">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="8f05e-165">Minimum length of password.</span></span> <span data-ttu-id="8f05e-166">有效值为 4 至 14</span><span class="sxs-lookup"><span data-stu-id="8f05e-166">Valid values 4 to 14</span></span>|
|<span data-ttu-id="8f05e-167">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="8f05e-167">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="8f05e-168">Int32</span><span class="sxs-lookup"><span data-stu-id="8f05e-168">Int32</span></span>|<span data-ttu-id="8f05e-169">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="8f05e-169">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="8f05e-170">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="8f05e-170">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="8f05e-171">Int32</span><span class="sxs-lookup"><span data-stu-id="8f05e-171">Int32</span></span>|<span data-ttu-id="8f05e-172">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="8f05e-172">Number of previous passwords to block.</span></span> <span data-ttu-id="8f05e-173">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="8f05e-173">Valid values 1 to 24</span></span>|
|<span data-ttu-id="8f05e-174">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="8f05e-174">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="8f05e-175">Int32</span><span class="sxs-lookup"><span data-stu-id="8f05e-175">Int32</span></span>|<span data-ttu-id="8f05e-176">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="8f05e-176">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="8f05e-177">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="8f05e-177">passwordRequiredType</span></span>|<span data-ttu-id="8f05e-178">String</span><span class="sxs-lookup"><span data-stu-id="8f05e-178">String</span></span>|<span data-ttu-id="8f05e-179">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="8f05e-179">The required password type.</span></span> <span data-ttu-id="8f05e-180">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="8f05e-180">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="8f05e-181">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="8f05e-181">osMinimumVersion</span></span>|<span data-ttu-id="8f05e-182">String</span><span class="sxs-lookup"><span data-stu-id="8f05e-182">String</span></span>|<span data-ttu-id="8f05e-183">最低 IOS 版本。</span><span class="sxs-lookup"><span data-stu-id="8f05e-183">Minimum IOS version.</span></span>|
|<span data-ttu-id="8f05e-184">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="8f05e-184">osMaximumVersion</span></span>|<span data-ttu-id="8f05e-185">String</span><span class="sxs-lookup"><span data-stu-id="8f05e-185">String</span></span>|<span data-ttu-id="8f05e-186">最高 IOS 版本。</span><span class="sxs-lookup"><span data-stu-id="8f05e-186">Maximum IOS version.</span></span>|
|<span data-ttu-id="8f05e-187">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="8f05e-187">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="8f05e-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f05e-188">Boolean</span></span>|<span data-ttu-id="8f05e-189">要求设备已启用系统完整性保护。</span><span class="sxs-lookup"><span data-stu-id="8f05e-189">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="8f05e-190">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="8f05e-190">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="8f05e-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f05e-191">Boolean</span></span>|<span data-ttu-id="8f05e-192">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="8f05e-192">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="8f05e-193">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="8f05e-193">deviceThreatProtectionRequiredSecurityLevel</span></span>|<span data-ttu-id="8f05e-194">String</span><span class="sxs-lookup"><span data-stu-id="8f05e-194">String</span></span>|<span data-ttu-id="8f05e-195">要求移动威胁防护最低风险级别来报告不符合情况。</span><span class="sxs-lookup"><span data-stu-id="8f05e-195">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="8f05e-196">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="8f05e-196">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="8f05e-197">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="8f05e-197">storageRequireEncryption</span></span>|<span data-ttu-id="8f05e-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f05e-198">Boolean</span></span>|<span data-ttu-id="8f05e-199">要求对 Mac OS 设备加密。</span><span class="sxs-lookup"><span data-stu-id="8f05e-199">Require encryption on Mac OS devices.</span></span>|



## <a name="response"></a><span data-ttu-id="8f05e-200">响应</span><span class="sxs-lookup"><span data-stu-id="8f05e-200">Response</span></span>
<span data-ttu-id="8f05e-201">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8f05e-201">If successful, this method returns a `201 Created` response code and a [DriveItemVersion](../resources/intune_deviceconfig_macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f05e-202">示例</span><span class="sxs-lookup"><span data-stu-id="8f05e-202">Example</span></span>
### <a name="request"></a><span data-ttu-id="8f05e-203">请求</span><span class="sxs-lookup"><span data-stu-id="8f05e-203">Request</span></span>
<span data-ttu-id="8f05e-204">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8f05e-204">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 810

{
  "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "systemIntegrityProtectionEnabled": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="8f05e-205">响应</span><span class="sxs-lookup"><span data-stu-id="8f05e-205">Response</span></span>
<span data-ttu-id="8f05e-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8f05e-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 918

{
  "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
  "id": "ddbadff3-dff3-ddba-f3df-baddf3dfbadd",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "systemIntegrityProtectionEnabled": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "storageRequireEncryption": true
}
```



