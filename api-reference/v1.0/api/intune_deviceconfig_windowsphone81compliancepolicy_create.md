# <a name="create-windowsphone81compliancepolicy"></a><span data-ttu-id="e8e50-101">创建 windowsPhone81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="e8e50-101">Create windowsPhone81CompliancePolicy</span></span>

> <span data-ttu-id="e8e50-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e8e50-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e8e50-103">创建新的 [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e8e50-103">Create a new [plannerBucket](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e8e50-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="e8e50-104">Prerequisites</span></span>
<span data-ttu-id="e8e50-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="e8e50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e8e50-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="e8e50-107">Permission type</span></span>|<span data-ttu-id="e8e50-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e8e50-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8e50-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e8e50-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e8e50-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8e50-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e8e50-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e8e50-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8e50-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="e8e50-112">Not supported.</span></span>|
|<span data-ttu-id="e8e50-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="e8e50-113">Application</span></span>|<span data-ttu-id="e8e50-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e8e50-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8e50-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e8e50-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="e8e50-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="e8e50-116">Request headers</span></span>
|<span data-ttu-id="e8e50-117">标头</span><span class="sxs-lookup"><span data-stu-id="e8e50-117">Header</span></span>|<span data-ttu-id="e8e50-118">值</span><span class="sxs-lookup"><span data-stu-id="e8e50-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8e50-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8e50-119">Authorization</span></span>|<span data-ttu-id="e8e50-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e8e50-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e8e50-121">Accept</span><span class="sxs-lookup"><span data-stu-id="e8e50-121">Accept</span></span>|<span data-ttu-id="e8e50-122">application/json</span><span class="sxs-lookup"><span data-stu-id="e8e50-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8e50-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="e8e50-123">Request body</span></span>
<span data-ttu-id="e8e50-124">在请求正文中，提供 windowsPhone81CompliancePolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e8e50-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="e8e50-125">下表显示创建 windowsPhone81CompliancePolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e8e50-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="e8e50-126">属性</span><span class="sxs-lookup"><span data-stu-id="e8e50-126">Property</span></span>|<span data-ttu-id="e8e50-127">类型</span><span class="sxs-lookup"><span data-stu-id="e8e50-127">Type</span></span>|<span data-ttu-id="e8e50-128">说明</span><span class="sxs-lookup"><span data-stu-id="e8e50-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8e50-129">id</span><span class="sxs-lookup"><span data-stu-id="e8e50-129">id</span></span>|<span data-ttu-id="e8e50-130">String</span><span class="sxs-lookup"><span data-stu-id="e8e50-130">String</span></span>|<span data-ttu-id="e8e50-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e8e50-131">Key of the setting.</span></span> <span data-ttu-id="e8e50-132">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e8e50-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e8e50-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e8e50-133">createdDateTime</span></span>|<span data-ttu-id="e8e50-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8e50-134">DateTimeOffset</span></span>|<span data-ttu-id="e8e50-135">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e8e50-135">DateTime the object was created.</span></span> <span data-ttu-id="e8e50-136">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e8e50-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e8e50-137">description</span><span class="sxs-lookup"><span data-stu-id="e8e50-137">description</span></span>|<span data-ttu-id="e8e50-138">String</span><span class="sxs-lookup"><span data-stu-id="e8e50-138">String</span></span>|<span data-ttu-id="e8e50-139">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="e8e50-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e8e50-140">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e8e50-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e8e50-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e8e50-141">lastModifiedDateTime</span></span>|<span data-ttu-id="e8e50-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8e50-142">DateTimeOffset</span></span>|<span data-ttu-id="e8e50-143">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e8e50-143">Indicates the date the object was last modified.</span></span> <span data-ttu-id="e8e50-144">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e8e50-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e8e50-145">displayName</span><span class="sxs-lookup"><span data-stu-id="e8e50-145">displayName</span></span>|<span data-ttu-id="e8e50-146">String</span><span class="sxs-lookup"><span data-stu-id="e8e50-146">String</span></span>|<span data-ttu-id="e8e50-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="e8e50-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e8e50-148">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e8e50-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e8e50-149">version</span><span class="sxs-lookup"><span data-stu-id="e8e50-149">version</span></span>|<span data-ttu-id="e8e50-150">Int32</span><span class="sxs-lookup"><span data-stu-id="e8e50-150">Int32</span></span>|<span data-ttu-id="e8e50-151">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="e8e50-151">Version of the device configuration.</span></span> <span data-ttu-id="e8e50-152">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e8e50-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e8e50-153">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="e8e50-153">passwordBlockSimple</span></span>|<span data-ttu-id="e8e50-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8e50-154">Boolean</span></span>|<span data-ttu-id="e8e50-155">是否阻止同步日历。</span><span class="sxs-lookup"><span data-stu-id="e8e50-155">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="e8e50-156">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="e8e50-156">passwordExpirationDays</span></span>|<span data-ttu-id="e8e50-157">Int32</span><span class="sxs-lookup"><span data-stu-id="e8e50-157">Int32</span></span>|<span data-ttu-id="e8e50-158">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="e8e50-158">Number of days before the password expires.</span></span>|
|<span data-ttu-id="e8e50-159">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="e8e50-159">passwordMinimumLength</span></span>|<span data-ttu-id="e8e50-160">Int32</span><span class="sxs-lookup"><span data-stu-id="e8e50-160">Int32</span></span>|<span data-ttu-id="e8e50-161">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="e8e50-161">Minimum length of passwords.</span></span>|
|<span data-ttu-id="e8e50-162">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="e8e50-162">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="e8e50-163">Int32</span><span class="sxs-lookup"><span data-stu-id="e8e50-163">Int32</span></span>|<span data-ttu-id="e8e50-164">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="e8e50-164">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="e8e50-165">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="e8e50-165">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="e8e50-166">Int32</span><span class="sxs-lookup"><span data-stu-id="e8e50-166">Int32</span></span>|<span data-ttu-id="e8e50-167">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="e8e50-167">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="e8e50-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="e8e50-168">passwordRequiredType</span></span>|<span data-ttu-id="e8e50-169">String</span><span class="sxs-lookup"><span data-stu-id="e8e50-169">String</span></span>|<span data-ttu-id="e8e50-170">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="e8e50-170">The required password type.</span></span> <span data-ttu-id="e8e50-171">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="e8e50-171">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="e8e50-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="e8e50-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="e8e50-173">Int32</span><span class="sxs-lookup"><span data-stu-id="e8e50-173">Int32</span></span>|<span data-ttu-id="e8e50-174">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="e8e50-174">Number of previous passwords to block.</span></span> <span data-ttu-id="e8e50-175">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="e8e50-175">Valid values 0 to 24</span></span>|
|<span data-ttu-id="e8e50-176">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="e8e50-176">passwordRequired</span></span>|<span data-ttu-id="e8e50-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8e50-177">Boolean</span></span>|<span data-ttu-id="e8e50-178">是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="e8e50-178">Whether or not to require a password.</span></span>|
|<span data-ttu-id="e8e50-179">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="e8e50-179">osMinimumVersion</span></span>|<span data-ttu-id="e8e50-180">String</span><span class="sxs-lookup"><span data-stu-id="e8e50-180">String</span></span>|<span data-ttu-id="e8e50-181">最低 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="e8e50-181">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="e8e50-182">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="e8e50-182">osMaximumVersion</span></span>|<span data-ttu-id="e8e50-183">String</span><span class="sxs-lookup"><span data-stu-id="e8e50-183">String</span></span>|<span data-ttu-id="e8e50-184">最高 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="e8e50-184">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="e8e50-185">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="e8e50-185">storageRequireEncryption</span></span>|<span data-ttu-id="e8e50-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8e50-186">Boolean</span></span>|<span data-ttu-id="e8e50-187">要求对 Windows Phone 设备加密。</span><span class="sxs-lookup"><span data-stu-id="e8e50-187">Require encryption on windows phone devices.</span></span>|



## <a name="response"></a><span data-ttu-id="e8e50-188">响应</span><span class="sxs-lookup"><span data-stu-id="e8e50-188">Response</span></span>
<span data-ttu-id="e8e50-189">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e8e50-189">If successful, this method returns a `201 Created` response code and a [directoryObject](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8e50-190">示例</span><span class="sxs-lookup"><span data-stu-id="e8e50-190">Example</span></span>
### <a name="request"></a><span data-ttu-id="e8e50-191">请求</span><span class="sxs-lookup"><span data-stu-id="e8e50-191">Request</span></span>
<span data-ttu-id="e8e50-192">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e8e50-192">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 671

{
  "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="e8e50-193">响应</span><span class="sxs-lookup"><span data-stu-id="e8e50-193">Response</span></span>
<span data-ttu-id="e8e50-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e8e50-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 779

{
  "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
  "id": "e6021ad4-1ad4-e602-d41a-02e6d41a02e6",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```



