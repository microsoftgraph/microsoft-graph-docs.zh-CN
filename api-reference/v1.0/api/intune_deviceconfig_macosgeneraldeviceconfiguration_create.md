# <a name="create-macosgeneraldeviceconfiguration"></a><span data-ttu-id="f4e21-101">创建 macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="f4e21-101">Create macOSGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="f4e21-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f4e21-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f4e21-103">创建新的 [macOSGeneralDeviceConfiguration](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f4e21-103">Create a new [plannerBucket](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f4e21-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="f4e21-104">Prerequisites</span></span>
<span data-ttu-id="f4e21-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="f4e21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f4e21-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="f4e21-107">Permission type</span></span>|<span data-ttu-id="f4e21-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f4e21-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4e21-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f4e21-109">Delegated (work or school account)</span></span>|<span data-ttu-id="f4e21-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4e21-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f4e21-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f4e21-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4e21-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="f4e21-112">Not supported.</span></span>|
|<span data-ttu-id="f4e21-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="f4e21-113">Application</span></span>|<span data-ttu-id="f4e21-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f4e21-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4e21-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f4e21-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f4e21-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="f4e21-116">Request headers</span></span>
|<span data-ttu-id="f4e21-117">标头</span><span class="sxs-lookup"><span data-stu-id="f4e21-117">Header</span></span>|<span data-ttu-id="f4e21-118">值</span><span class="sxs-lookup"><span data-stu-id="f4e21-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4e21-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4e21-119">Authorization</span></span>|<span data-ttu-id="f4e21-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f4e21-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f4e21-121">Accept</span><span class="sxs-lookup"><span data-stu-id="f4e21-121">Accept</span></span>|<span data-ttu-id="f4e21-122">application/json</span><span class="sxs-lookup"><span data-stu-id="f4e21-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4e21-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="f4e21-123">Request body</span></span>
<span data-ttu-id="f4e21-124">在请求正文中，提供 macOSGeneralDeviceConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f4e21-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="f4e21-125">下表显示创建 macOSGeneralDeviceConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f4e21-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="f4e21-126">属性</span><span class="sxs-lookup"><span data-stu-id="f4e21-126">Property</span></span>|<span data-ttu-id="f4e21-127">类型</span><span class="sxs-lookup"><span data-stu-id="f4e21-127">Type</span></span>|<span data-ttu-id="f4e21-128">说明</span><span class="sxs-lookup"><span data-stu-id="f4e21-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4e21-129">id</span><span class="sxs-lookup"><span data-stu-id="f4e21-129">id</span></span>|<span data-ttu-id="f4e21-130">String</span><span class="sxs-lookup"><span data-stu-id="f4e21-130">String</span></span>|<span data-ttu-id="f4e21-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f4e21-131">Key of the setting.</span></span> <span data-ttu-id="f4e21-132">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4e21-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4e21-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f4e21-133">lastModifiedDateTime</span></span>|<span data-ttu-id="f4e21-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4e21-134">DateTimeOffset</span></span>|<span data-ttu-id="f4e21-135">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f4e21-135">Indicates the date the object was last modified.</span></span> <span data-ttu-id="f4e21-136">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4e21-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4e21-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f4e21-137">createdDateTime</span></span>|<span data-ttu-id="f4e21-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4e21-138">DateTimeOffset</span></span>|<span data-ttu-id="f4e21-139">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f4e21-139">DateTime the object was created.</span></span> <span data-ttu-id="f4e21-140">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4e21-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4e21-141">description</span><span class="sxs-lookup"><span data-stu-id="f4e21-141">description</span></span>|<span data-ttu-id="f4e21-142">String</span><span class="sxs-lookup"><span data-stu-id="f4e21-142">String</span></span>|<span data-ttu-id="f4e21-143">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="f4e21-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f4e21-144">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4e21-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4e21-145">displayName</span><span class="sxs-lookup"><span data-stu-id="f4e21-145">displayName</span></span>|<span data-ttu-id="f4e21-146">String</span><span class="sxs-lookup"><span data-stu-id="f4e21-146">String</span></span>|<span data-ttu-id="f4e21-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="f4e21-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f4e21-148">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4e21-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4e21-149">version</span><span class="sxs-lookup"><span data-stu-id="f4e21-149">version</span></span>|<span data-ttu-id="f4e21-150">Int32</span><span class="sxs-lookup"><span data-stu-id="f4e21-150">Int32</span></span>|<span data-ttu-id="f4e21-151">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="f4e21-151">Version of the device configuration.</span></span> <span data-ttu-id="f4e21-152">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4e21-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4e21-153">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="f4e21-153">compliantAppsList</span></span>|<span data-ttu-id="f4e21-154">[appListItem](../resources/intune_deviceconfig_applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f4e21-154">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="f4e21-155">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="f4e21-155">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="f4e21-156">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="f4e21-156">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="f4e21-157">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="f4e21-157">compliantAppListType</span></span>|<span data-ttu-id="f4e21-158">String</span><span class="sxs-lookup"><span data-stu-id="f4e21-158">String</span></span>|<span data-ttu-id="f4e21-159">位于 CompliantAppsList 中的列表。</span><span class="sxs-lookup"><span data-stu-id="f4e21-159">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="f4e21-160">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="f4e21-160">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="f4e21-161">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="f4e21-161">emailInDomainSuffixes</span></span>|<span data-ttu-id="f4e21-162">String 集合</span><span class="sxs-lookup"><span data-stu-id="f4e21-162">String collection</span></span>|<span data-ttu-id="f4e21-163">缺少匹配任何这些字符串的后缀的电子邮件地址将被视为超出域范围。</span><span class="sxs-lookup"><span data-stu-id="f4e21-163">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="f4e21-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="f4e21-164">passwordBlockSimple</span></span>|<span data-ttu-id="f4e21-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4e21-165">Boolean</span></span>|<span data-ttu-id="f4e21-166">阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="f4e21-166">Block simple passwords.</span></span>|
|<span data-ttu-id="f4e21-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="f4e21-167">passwordExpirationDays</span></span>|<span data-ttu-id="f4e21-168">Int32</span><span class="sxs-lookup"><span data-stu-id="f4e21-168">Int32</span></span>|<span data-ttu-id="f4e21-169">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="f4e21-169">Number of days before the password expires.</span></span>|
|<span data-ttu-id="f4e21-170">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="f4e21-170">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="f4e21-171">Int32</span><span class="sxs-lookup"><span data-stu-id="f4e21-171">Int32</span></span>|<span data-ttu-id="f4e21-172">密码必须包含的字符集数。</span><span class="sxs-lookup"><span data-stu-id="f4e21-172">Number of character sets a password must contain.</span></span> <span data-ttu-id="f4e21-173">有效值为 0 至 4</span><span class="sxs-lookup"><span data-stu-id="f4e21-173">Valid values 0 to 4</span></span>|
|<span data-ttu-id="f4e21-174">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="f4e21-174">passwordMinimumLength</span></span>|<span data-ttu-id="f4e21-175">Int32</span><span class="sxs-lookup"><span data-stu-id="f4e21-175">Int32</span></span>|<span data-ttu-id="f4e21-176">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="f4e21-176">Minimum length of passwords.</span></span>|
|<span data-ttu-id="f4e21-177">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="f4e21-177">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="f4e21-178">Int32</span><span class="sxs-lookup"><span data-stu-id="f4e21-178">Int32</span></span>|<span data-ttu-id="f4e21-179">在需要密码之前需要不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="f4e21-179">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="f4e21-180">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="f4e21-180">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="f4e21-181">Int32</span><span class="sxs-lookup"><span data-stu-id="f4e21-181">Int32</span></span>|<span data-ttu-id="f4e21-182">在屏幕超时之前需要不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="f4e21-182">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="f4e21-183">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="f4e21-183">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="f4e21-184">Int32</span><span class="sxs-lookup"><span data-stu-id="f4e21-184">Int32</span></span>|<span data-ttu-id="f4e21-185">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="f4e21-185">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="f4e21-186">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="f4e21-186">passwordRequiredType</span></span>|<span data-ttu-id="f4e21-187">String</span><span class="sxs-lookup"><span data-stu-id="f4e21-187">String</span></span>|<span data-ttu-id="f4e21-188">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="f4e21-188">Type of password that is required.</span></span> <span data-ttu-id="f4e21-189">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="f4e21-189">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="f4e21-190">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="f4e21-190">passwordRequired</span></span>|<span data-ttu-id="f4e21-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4e21-191">Boolean</span></span>|<span data-ttu-id="f4e21-192">是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="f4e21-192">Whether or not to require a password.</span></span>|



## <a name="response"></a><span data-ttu-id="f4e21-193">响应</span><span class="sxs-lookup"><span data-stu-id="f4e21-193">Response</span></span>
<span data-ttu-id="f4e21-194">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [macOSGeneralDeviceConfiguration](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f4e21-194">If successful, this method returns a `201 Created` response code and a [directoryObject](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4e21-195">示例</span><span class="sxs-lookup"><span data-stu-id="f4e21-195">Example</span></span>
### <a name="request"></a><span data-ttu-id="f4e21-196">请求</span><span class="sxs-lookup"><span data-stu-id="f4e21-196">Request</span></span>
<span data-ttu-id="f4e21-197">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f4e21-197">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 970

{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumCharacterSetCount": 0,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true
}
```

### <a name="response"></a><span data-ttu-id="f4e21-198">响应</span><span class="sxs-lookup"><span data-stu-id="f4e21-198">Response</span></span>
<span data-ttu-id="f4e21-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f4e21-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1078

{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
  "id": "dc356aee-6aee-dc35-ee6a-35dcee6a35dc",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumCharacterSetCount": 0,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true
}
```



