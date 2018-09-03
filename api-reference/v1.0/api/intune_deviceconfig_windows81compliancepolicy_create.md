# <a name="create-windows81compliancepolicy"></a><span data-ttu-id="e84a0-101">创建 windows81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="e84a0-101">Create windows81CompliancePolicy</span></span>

> <span data-ttu-id="e84a0-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e84a0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e84a0-103">创建新的 [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e84a0-103">Create a new [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e84a0-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="e84a0-104">Prerequisites</span></span>
<span data-ttu-id="e84a0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="e84a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e84a0-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="e84a0-107">Permission type</span></span>|<span data-ttu-id="e84a0-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e84a0-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e84a0-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e84a0-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e84a0-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e84a0-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e84a0-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e84a0-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e84a0-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="e84a0-112">Not supported.</span></span>|
|<span data-ttu-id="e84a0-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="e84a0-113">Application</span></span>|<span data-ttu-id="e84a0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e84a0-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e84a0-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e84a0-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="e84a0-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="e84a0-116">Request headers</span></span>
|<span data-ttu-id="e84a0-117">标头</span><span class="sxs-lookup"><span data-stu-id="e84a0-117">Header</span></span>|<span data-ttu-id="e84a0-118">值</span><span class="sxs-lookup"><span data-stu-id="e84a0-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e84a0-119">授权</span><span class="sxs-lookup"><span data-stu-id="e84a0-119">Authorization</span></span>|<span data-ttu-id="e84a0-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e84a0-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e84a0-121">接受</span><span class="sxs-lookup"><span data-stu-id="e84a0-121">Accept</span></span>|<span data-ttu-id="e84a0-122">application/json</span><span class="sxs-lookup"><span data-stu-id="e84a0-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e84a0-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="e84a0-123">Request body</span></span>
<span data-ttu-id="e84a0-124">在请求正文中，提供 windows81CompliancePolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e84a0-124">In the request body, supply a JSON representation for the windows81CompliancePolicy object.</span></span>

<span data-ttu-id="e84a0-125">下表显示创建 windows81CompliancePolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e84a0-125">The following table shows the properties that are required when you create the windows81CompliancePolicy.</span></span>

|<span data-ttu-id="e84a0-126">属性</span><span class="sxs-lookup"><span data-stu-id="e84a0-126">Property</span></span>|<span data-ttu-id="e84a0-127">类型</span><span class="sxs-lookup"><span data-stu-id="e84a0-127">Type</span></span>|<span data-ttu-id="e84a0-128">说明</span><span class="sxs-lookup"><span data-stu-id="e84a0-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e84a0-129">id</span><span class="sxs-lookup"><span data-stu-id="e84a0-129">id</span></span>|<span data-ttu-id="e84a0-130">字符串</span><span class="sxs-lookup"><span data-stu-id="e84a0-130">String</span></span>|<span data-ttu-id="e84a0-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e84a0-131">Key of the entity.</span></span> <span data-ttu-id="e84a0-132">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e84a0-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e84a0-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e84a0-133">createdDateTime</span></span>|<span data-ttu-id="e84a0-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e84a0-134">DateTimeOffset</span></span>|<span data-ttu-id="e84a0-135">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e84a0-135">DateTime the object was created.</span></span> <span data-ttu-id="e84a0-136">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e84a0-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e84a0-137">说明</span><span class="sxs-lookup"><span data-stu-id="e84a0-137">description</span></span>|<span data-ttu-id="e84a0-138">String</span><span class="sxs-lookup"><span data-stu-id="e84a0-138">String</span></span>|<span data-ttu-id="e84a0-139">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="e84a0-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e84a0-140">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e84a0-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e84a0-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e84a0-141">lastModifiedDateTime</span></span>|<span data-ttu-id="e84a0-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e84a0-142">DateTimeOffset</span></span>|<span data-ttu-id="e84a0-143">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e84a0-143">DateTime the object was last modified.</span></span> <span data-ttu-id="e84a0-144">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e84a0-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e84a0-145">displayName</span><span class="sxs-lookup"><span data-stu-id="e84a0-145">displayName</span></span>|<span data-ttu-id="e84a0-146">String</span><span class="sxs-lookup"><span data-stu-id="e84a0-146">String</span></span>|<span data-ttu-id="e84a0-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="e84a0-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e84a0-148">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e84a0-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e84a0-149">版本</span><span class="sxs-lookup"><span data-stu-id="e84a0-149">version</span></span>|<span data-ttu-id="e84a0-150">Int32</span><span class="sxs-lookup"><span data-stu-id="e84a0-150">Int32</span></span>|<span data-ttu-id="e84a0-151">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="e84a0-151">Version of the device configuration.</span></span> <span data-ttu-id="e84a0-152">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e84a0-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e84a0-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="e84a0-153">passwordRequired</span></span>|<span data-ttu-id="e84a0-154">布尔值</span><span class="sxs-lookup"><span data-stu-id="e84a0-154">Boolean</span></span>|<span data-ttu-id="e84a0-155">需要密码才可解锁 Windows 设备。</span><span class="sxs-lookup"><span data-stu-id="e84a0-155">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="e84a0-156">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="e84a0-156">passwordBlockSimple</span></span>|<span data-ttu-id="e84a0-157">布尔值</span><span class="sxs-lookup"><span data-stu-id="e84a0-157">Boolean</span></span>|<span data-ttu-id="e84a0-158">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="e84a0-158">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="e84a0-159">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="e84a0-159">passwordExpirationDays</span></span>|<span data-ttu-id="e84a0-160">Int32</span><span class="sxs-lookup"><span data-stu-id="e84a0-160">Int32</span></span>|<span data-ttu-id="e84a0-161">密码过期天数。</span><span class="sxs-lookup"><span data-stu-id="e84a0-161">Password expiration in days.</span></span>|
|<span data-ttu-id="e84a0-162">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="e84a0-162">passwordMinimumLength</span></span>|<span data-ttu-id="e84a0-163">Int32</span><span class="sxs-lookup"><span data-stu-id="e84a0-163">Int32</span></span>|<span data-ttu-id="e84a0-164">密码最短长度。</span><span class="sxs-lookup"><span data-stu-id="e84a0-164">The minimum password length.</span></span>|
|<span data-ttu-id="e84a0-165">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="e84a0-165">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="e84a0-166">Int32</span><span class="sxs-lookup"><span data-stu-id="e84a0-166">Int32</span></span>|<span data-ttu-id="e84a0-167">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="e84a0-167">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="e84a0-168">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="e84a0-168">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="e84a0-169">Int32</span><span class="sxs-lookup"><span data-stu-id="e84a0-169">Int32</span></span>|<span data-ttu-id="e84a0-170">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="e84a0-170">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="e84a0-171">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="e84a0-171">passwordRequiredType</span></span>|[<span data-ttu-id="e84a0-172">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="e84a0-172">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="e84a0-173">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="e84a0-173">The required password type.</span></span> <span data-ttu-id="e84a0-174">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="e84a0-174">The possible values are `deviceDefault`, `alphanumeric`, `numeric`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="e84a0-175">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="e84a0-175">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="e84a0-176">Int32</span><span class="sxs-lookup"><span data-stu-id="e84a0-176">Int32</span></span>|<span data-ttu-id="e84a0-177">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="e84a0-177">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="e84a0-178">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="e84a0-178">Valid values 0 to 24</span></span>|
|<span data-ttu-id="e84a0-179">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="e84a0-179">osMinimumVersion</span></span>|<span data-ttu-id="e84a0-180">String</span><span class="sxs-lookup"><span data-stu-id="e84a0-180">String</span></span>|<span data-ttu-id="e84a0-181">最低 Windows 8.1 版本。</span><span class="sxs-lookup"><span data-stu-id="e84a0-181">Minimum Windows 8.1 version.</span></span>|
|<span data-ttu-id="e84a0-182">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="e84a0-182">osMaximumVersion</span></span>|<span data-ttu-id="e84a0-183">String</span><span class="sxs-lookup"><span data-stu-id="e84a0-183">String</span></span>|<span data-ttu-id="e84a0-184">最高 Windows 8.1 版本。</span><span class="sxs-lookup"><span data-stu-id="e84a0-184">Maximum Windows 8.1 version.</span></span>|
|<span data-ttu-id="e84a0-185">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="e84a0-185">storageRequireEncryption</span></span>|<span data-ttu-id="e84a0-186">布尔值</span><span class="sxs-lookup"><span data-stu-id="e84a0-186">Boolean</span></span>|<span data-ttu-id="e84a0-187">指示是否要求对 Windows 8.1 设备加密。</span><span class="sxs-lookup"><span data-stu-id="e84a0-187">Indicates whether or not to require encryption on a windows 8.1 device.</span></span>|



## <a name="response"></a><span data-ttu-id="e84a0-188">响应</span><span class="sxs-lookup"><span data-stu-id="e84a0-188">Response</span></span>
<span data-ttu-id="e84a0-189">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e84a0-189">If successful, this method returns a `201 Created` response code and a [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e84a0-190">示例</span><span class="sxs-lookup"><span data-stu-id="e84a0-190">Example</span></span>
### <a name="request"></a><span data-ttu-id="e84a0-191">请求</span><span class="sxs-lookup"><span data-stu-id="e84a0-191">Request</span></span>
<span data-ttu-id="e84a0-192">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e84a0-192">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 666

{
  "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="e84a0-193">响应</span><span class="sxs-lookup"><span data-stu-id="e84a0-193">Response</span></span>
<span data-ttu-id="e84a0-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e84a0-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 774

{
  "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
  "id": "6bb4b7e0-b7e0-6bb4-e0b7-b46be0b7b46b",
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
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```



