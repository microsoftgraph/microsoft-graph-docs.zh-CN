# <a name="update-windows81compliancepolicy"></a><span data-ttu-id="87c39-101">更新 windows81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="87c39-101">Update windows81CompliancePolicy</span></span>

> <span data-ttu-id="87c39-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="87c39-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="87c39-103">更新 [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="87c39-103">Update the properties of a [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="87c39-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="87c39-104">Prerequisites</span></span>
<span data-ttu-id="87c39-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="87c39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="87c39-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="87c39-107">Permission type</span></span>|<span data-ttu-id="87c39-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="87c39-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87c39-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="87c39-109">Delegated (work or school account)</span></span>|<span data-ttu-id="87c39-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87c39-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="87c39-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="87c39-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87c39-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="87c39-112">Not supported.</span></span>|
|<span data-ttu-id="87c39-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="87c39-113">Application</span></span>|<span data-ttu-id="87c39-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="87c39-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="87c39-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="87c39-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="87c39-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="87c39-116">Request headers</span></span>
|<span data-ttu-id="87c39-117">标头</span><span class="sxs-lookup"><span data-stu-id="87c39-117">Header</span></span>|<span data-ttu-id="87c39-118">值</span><span class="sxs-lookup"><span data-stu-id="87c39-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87c39-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="87c39-119">Authorization</span></span>|<span data-ttu-id="87c39-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="87c39-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87c39-121">Accept</span><span class="sxs-lookup"><span data-stu-id="87c39-121">Accept</span></span>|<span data-ttu-id="87c39-122">application/json</span><span class="sxs-lookup"><span data-stu-id="87c39-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87c39-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="87c39-123">Request body</span></span>
<span data-ttu-id="87c39-124">在请求正文中，提供 [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="87c39-124">In the request body, supply a JSON representation for the [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md) object.</span></span>

<span data-ttu-id="87c39-125">下表显示创建 [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="87c39-125">The following table shows the properties that are required when you create the [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md).</span></span>

|<span data-ttu-id="87c39-126">属性</span><span class="sxs-lookup"><span data-stu-id="87c39-126">Property</span></span>|<span data-ttu-id="87c39-127">类型</span><span class="sxs-lookup"><span data-stu-id="87c39-127">Type</span></span>|<span data-ttu-id="87c39-128">说明</span><span class="sxs-lookup"><span data-stu-id="87c39-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87c39-129">id</span><span class="sxs-lookup"><span data-stu-id="87c39-129">id</span></span>|<span data-ttu-id="87c39-130">String</span><span class="sxs-lookup"><span data-stu-id="87c39-130">String</span></span>|<span data-ttu-id="87c39-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="87c39-131">Key of the entity.</span></span> <span data-ttu-id="87c39-132">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="87c39-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="87c39-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="87c39-133">createdDateTime</span></span>|<span data-ttu-id="87c39-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87c39-134">DateTimeOffset</span></span>|<span data-ttu-id="87c39-135">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="87c39-135">DateTime the object was created.</span></span> <span data-ttu-id="87c39-136">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="87c39-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="87c39-137">description</span><span class="sxs-lookup"><span data-stu-id="87c39-137">description</span></span>|<span data-ttu-id="87c39-138">String</span><span class="sxs-lookup"><span data-stu-id="87c39-138">String</span></span>|<span data-ttu-id="87c39-139">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="87c39-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="87c39-140">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="87c39-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="87c39-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="87c39-141">lastModifiedDateTime</span></span>|<span data-ttu-id="87c39-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87c39-142">DateTimeOffset</span></span>|<span data-ttu-id="87c39-143">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="87c39-143">DateTime the object was last modified.</span></span> <span data-ttu-id="87c39-144">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="87c39-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="87c39-145">displayName</span><span class="sxs-lookup"><span data-stu-id="87c39-145">displayName</span></span>|<span data-ttu-id="87c39-146">String</span><span class="sxs-lookup"><span data-stu-id="87c39-146">String</span></span>|<span data-ttu-id="87c39-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="87c39-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="87c39-148">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="87c39-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="87c39-149">version</span><span class="sxs-lookup"><span data-stu-id="87c39-149">version</span></span>|<span data-ttu-id="87c39-150">Int32</span><span class="sxs-lookup"><span data-stu-id="87c39-150">Int32</span></span>|<span data-ttu-id="87c39-151">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="87c39-151">Version of the device configuration.</span></span> <span data-ttu-id="87c39-152">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="87c39-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="87c39-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="87c39-153">passwordRequired</span></span>|<span data-ttu-id="87c39-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="87c39-154">Boolean</span></span>|<span data-ttu-id="87c39-155">需要密码才可解锁 Windows 设备。</span><span class="sxs-lookup"><span data-stu-id="87c39-155">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="87c39-156">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="87c39-156">passwordBlockSimple</span></span>|<span data-ttu-id="87c39-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="87c39-157">Boolean</span></span>|<span data-ttu-id="87c39-158">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="87c39-158">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="87c39-159">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="87c39-159">passwordExpirationDays</span></span>|<span data-ttu-id="87c39-160">Int32</span><span class="sxs-lookup"><span data-stu-id="87c39-160">Int32</span></span>|<span data-ttu-id="87c39-161">密码过期天数。</span><span class="sxs-lookup"><span data-stu-id="87c39-161">Password expiration in days.</span></span>|
|<span data-ttu-id="87c39-162">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="87c39-162">passwordMinimumLength</span></span>|<span data-ttu-id="87c39-163">Int32</span><span class="sxs-lookup"><span data-stu-id="87c39-163">Int32</span></span>|<span data-ttu-id="87c39-164">密码最短长度。</span><span class="sxs-lookup"><span data-stu-id="87c39-164">The minimum password length.</span></span>|
|<span data-ttu-id="87c39-165">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="87c39-165">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="87c39-166">Int32</span><span class="sxs-lookup"><span data-stu-id="87c39-166">Int32</span></span>|<span data-ttu-id="87c39-167">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="87c39-167">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="87c39-168">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="87c39-168">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="87c39-169">Int32</span><span class="sxs-lookup"><span data-stu-id="87c39-169">Int32</span></span>|<span data-ttu-id="87c39-170">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="87c39-170">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="87c39-171">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="87c39-171">passwordRequiredType</span></span>|[<span data-ttu-id="87c39-172">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="87c39-172">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="87c39-173">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="87c39-173">The required password type.</span></span> <span data-ttu-id="87c39-174">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="87c39-174">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="87c39-175">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="87c39-175">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="87c39-176">Int32</span><span class="sxs-lookup"><span data-stu-id="87c39-176">Int32</span></span>|<span data-ttu-id="87c39-177">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="87c39-177">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="87c39-178">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="87c39-178">Valid values 0 to 24</span></span>|
|<span data-ttu-id="87c39-179">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="87c39-179">osMinimumVersion</span></span>|<span data-ttu-id="87c39-180">String</span><span class="sxs-lookup"><span data-stu-id="87c39-180">String</span></span>|<span data-ttu-id="87c39-181">最低 Windows 8.1 版本。</span><span class="sxs-lookup"><span data-stu-id="87c39-181">Minimum Windows 8.1 version.</span></span>|
|<span data-ttu-id="87c39-182">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="87c39-182">osMaximumVersion</span></span>|<span data-ttu-id="87c39-183">String</span><span class="sxs-lookup"><span data-stu-id="87c39-183">String</span></span>|<span data-ttu-id="87c39-184">最高 Windows 8.1 版本。</span><span class="sxs-lookup"><span data-stu-id="87c39-184">Maximum Windows 8.1 version.</span></span>|
|<span data-ttu-id="87c39-185">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="87c39-185">storageRequireEncryption</span></span>|<span data-ttu-id="87c39-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="87c39-186">Boolean</span></span>|<span data-ttu-id="87c39-187">指示是否要求对 Windows 8.1 设备加密。</span><span class="sxs-lookup"><span data-stu-id="87c39-187">Indicates whether or not to require encryption on a windows 8.1 device.</span></span>|



## <a name="response"></a><span data-ttu-id="87c39-188">响应</span><span class="sxs-lookup"><span data-stu-id="87c39-188">Response</span></span>
<span data-ttu-id="87c39-189">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="87c39-189">If successful, this method returns a `200 OK` response code and an updated [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87c39-190">示例</span><span class="sxs-lookup"><span data-stu-id="87c39-190">Example</span></span>
### <a name="request"></a><span data-ttu-id="87c39-191">请求</span><span class="sxs-lookup"><span data-stu-id="87c39-191">Request</span></span>
<span data-ttu-id="87c39-192">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="87c39-192">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 602

{
  "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
  "description": "Description value",
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

### <a name="response"></a><span data-ttu-id="87c39-193">响应</span><span class="sxs-lookup"><span data-stu-id="87c39-193">Response</span></span>
<span data-ttu-id="87c39-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="87c39-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



