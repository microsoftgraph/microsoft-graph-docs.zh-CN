# <a name="update-iosmobileappconfiguration"></a><span data-ttu-id="6c51a-101">Update iosMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="6c51a-101">Update iosMobileAppConfiguration</span></span>

> <span data-ttu-id="6c51a-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6c51a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6c51a-103">更新 [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6c51a-103">Update the properties of a [windowsInformationProtectionAppLearningSummary](../resources/intune_apps_iosmobileappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6c51a-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="6c51a-104">Prerequisites</span></span>
<span data-ttu-id="6c51a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="6c51a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6c51a-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="6c51a-107">Permission type</span></span>|<span data-ttu-id="6c51a-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6c51a-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c51a-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6c51a-109">Delegated (work or school account)</span></span>|<span data-ttu-id="6c51a-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c51a-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6c51a-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6c51a-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c51a-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="6c51a-112">Not supported.</span></span>|
|<span data-ttu-id="6c51a-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="6c51a-113">Application</span></span>|<span data-ttu-id="6c51a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6c51a-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c51a-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6c51a-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6c51a-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="6c51a-116">Request headers</span></span>
|<span data-ttu-id="6c51a-117">标头</span><span class="sxs-lookup"><span data-stu-id="6c51a-117">Header</span></span>|<span data-ttu-id="6c51a-118">值</span><span class="sxs-lookup"><span data-stu-id="6c51a-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c51a-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c51a-119">Authorization</span></span>|<span data-ttu-id="6c51a-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6c51a-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c51a-121">Accept</span><span class="sxs-lookup"><span data-stu-id="6c51a-121">Accept</span></span>|<span data-ttu-id="6c51a-122">application/json</span><span class="sxs-lookup"><span data-stu-id="6c51a-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c51a-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="6c51a-123">Request body</span></span>
<span data-ttu-id="6c51a-124">在请求正文中，提供 [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6c51a-124">In the request body, supply a JSON representation for the [windows10GeneralConfiguration](../resources/intune_apps_iosmobileappconfiguration.md) object.</span></span>

<span data-ttu-id="6c51a-125">下表显示创建 [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6c51a-125">The following table shows the properties that are required when you create the [iosUpdateDeviceStatus](../resources/intune_apps_iosmobileappconfiguration.md).</span></span>

|<span data-ttu-id="6c51a-126">属性</span><span class="sxs-lookup"><span data-stu-id="6c51a-126">Property</span></span>|<span data-ttu-id="6c51a-127">类型</span><span class="sxs-lookup"><span data-stu-id="6c51a-127">Type</span></span>|<span data-ttu-id="6c51a-128">说明</span><span class="sxs-lookup"><span data-stu-id="6c51a-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c51a-129">id</span><span class="sxs-lookup"><span data-stu-id="6c51a-129">id</span></span>|<span data-ttu-id="6c51a-130">String</span><span class="sxs-lookup"><span data-stu-id="6c51a-130">String</span></span>|<span data-ttu-id="6c51a-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6c51a-131">Key of the entity.</span></span> <span data-ttu-id="6c51a-132">继承自 [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c51a-132">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="6c51a-133">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="6c51a-133">targetedMobileApps</span></span>|<span data-ttu-id="6c51a-134">String 集合</span><span class="sxs-lookup"><span data-stu-id="6c51a-134">String collection</span></span>|<span data-ttu-id="6c51a-135">关联的应用。</span><span class="sxs-lookup"><span data-stu-id="6c51a-135">the associated app.</span></span> <span data-ttu-id="6c51a-136">继承自 [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c51a-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="6c51a-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6c51a-137">createdDateTime</span></span>|<span data-ttu-id="6c51a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c51a-138">DateTimeOffset</span></span>|<span data-ttu-id="6c51a-139">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6c51a-139">DateTime the object was created.</span></span> <span data-ttu-id="6c51a-140">继承自 [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c51a-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="6c51a-141">description</span><span class="sxs-lookup"><span data-stu-id="6c51a-141">description</span></span>|<span data-ttu-id="6c51a-142">String</span><span class="sxs-lookup"><span data-stu-id="6c51a-142">String</span></span>|<span data-ttu-id="6c51a-143">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="6c51a-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6c51a-144">继承自 [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c51a-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="6c51a-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6c51a-145">lastModifiedDateTime</span></span>|<span data-ttu-id="6c51a-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c51a-146">DateTimeOffset</span></span>|<span data-ttu-id="6c51a-147">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6c51a-147">DateTime the object was last modified.</span></span> <span data-ttu-id="6c51a-148">继承自 [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c51a-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="6c51a-149">displayName</span><span class="sxs-lookup"><span data-stu-id="6c51a-149">displayName</span></span>|<span data-ttu-id="6c51a-150">String</span><span class="sxs-lookup"><span data-stu-id="6c51a-150">String</span></span>|<span data-ttu-id="6c51a-151">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="6c51a-151">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6c51a-152">继承自 [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c51a-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="6c51a-153">version</span><span class="sxs-lookup"><span data-stu-id="6c51a-153">version</span></span>|<span data-ttu-id="6c51a-154">Int32</span><span class="sxs-lookup"><span data-stu-id="6c51a-154">Int32</span></span>|<span data-ttu-id="6c51a-155">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="6c51a-155">Version of the device configuration.</span></span> <span data-ttu-id="6c51a-156">继承自 [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c51a-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="6c51a-157">encodedSettingXml</span><span class="sxs-lookup"><span data-stu-id="6c51a-157">encodedSettingXml</span></span>|<span data-ttu-id="6c51a-158">Binary</span><span class="sxs-lookup"><span data-stu-id="6c51a-158">Binary</span></span>|<span data-ttu-id="6c51a-159">mdm 应用配置 Base64 二进制。</span><span class="sxs-lookup"><span data-stu-id="6c51a-159">mdm app configuration Base64 binary.</span></span>|
|<span data-ttu-id="6c51a-160">settings</span><span class="sxs-lookup"><span data-stu-id="6c51a-160">settings</span></span>|<span data-ttu-id="6c51a-161">[appConfigurationSettingItem](../resources/intune_apps_appconfigurationsettingitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6c51a-161">[appConfigurationSettingItem](../resources/intune_apps_appconfigurationsettingitem.md) collection</span></span>|<span data-ttu-id="6c51a-162">应用配置设置项。</span><span class="sxs-lookup"><span data-stu-id="6c51a-162">app configuration setting items.</span></span>|



## <a name="response"></a><span data-ttu-id="6c51a-163">响应</span><span class="sxs-lookup"><span data-stu-id="6c51a-163">Response</span></span>
<span data-ttu-id="6c51a-164">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6c51a-164">If successful, this method returns a `200 OK` response code and an updated [iosManagedAppProtection](../resources/intune_apps_iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c51a-165">示例</span><span class="sxs-lookup"><span data-stu-id="6c51a-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="6c51a-166">请求</span><span class="sxs-lookup"><span data-stu-id="6c51a-166">Request</span></span>
<span data-ttu-id="6c51a-167">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6c51a-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
Content-type: application/json
Content-length: 534

{
  "targetedMobileApps": [
    "Targeted Mobile Apps value"
  ],
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "encodedSettingXml": "ZW5jb2RlZFNldHRpbmdYbWw=",
  "settings": [
    {
      "@odata.type": "microsoft.graph.appConfigurationSettingItem",
      "appConfigKey": "App Config Key value",
      "appConfigKeyType": "integerType",
      "appConfigKeyValue": "App Config Key Value value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="6c51a-168">响应</span><span class="sxs-lookup"><span data-stu-id="6c51a-168">Response</span></span>
<span data-ttu-id="6c51a-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6c51a-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 706

{
  "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
  "id": "b2c33191-3191-b2c3-9131-c3b29131c3b2",
  "targetedMobileApps": [
    "Targeted Mobile Apps value"
  ],
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "encodedSettingXml": "ZW5jb2RlZFNldHRpbmdYbWw=",
  "settings": [
    {
      "@odata.type": "microsoft.graph.appConfigurationSettingItem",
      "appConfigKey": "App Config Key value",
      "appConfigKeyType": "integerType",
      "appConfigKeyValue": "App Config Key Value value"
    }
  ]
}
```



