# <a name="create-iosmobileappconfiguration"></a><span data-ttu-id="ef6d8-101">创建 iosMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="ef6d8-101">Create iosMobileAppConfiguration</span></span>

> <span data-ttu-id="ef6d8-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ef6d8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ef6d8-103">创建新的 [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ef6d8-103">Create a new [managedMobileApp](../resources/intune_apps_iosmobileappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ef6d8-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="ef6d8-104">Prerequisites</span></span>
<span data-ttu-id="ef6d8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="ef6d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ef6d8-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="ef6d8-107">Permission type</span></span>|<span data-ttu-id="ef6d8-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ef6d8-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef6d8-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ef6d8-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ef6d8-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef6d8-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ef6d8-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ef6d8-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef6d8-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="ef6d8-112">Not supported.</span></span>|
|<span data-ttu-id="ef6d8-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="ef6d8-113">Application</span></span>|<span data-ttu-id="ef6d8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ef6d8-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef6d8-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ef6d8-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ef6d8-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="ef6d8-116">Request headers</span></span>
|<span data-ttu-id="ef6d8-117">标头</span><span class="sxs-lookup"><span data-stu-id="ef6d8-117">Header</span></span>|<span data-ttu-id="ef6d8-118">值</span><span class="sxs-lookup"><span data-stu-id="ef6d8-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef6d8-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef6d8-119">Authorization</span></span>|<span data-ttu-id="ef6d8-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ef6d8-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef6d8-121">Accept</span><span class="sxs-lookup"><span data-stu-id="ef6d8-121">Accept</span></span>|<span data-ttu-id="ef6d8-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ef6d8-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef6d8-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="ef6d8-123">Request body</span></span>
<span data-ttu-id="ef6d8-124">在请求正文中，提供 iosMobileAppConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ef6d8-124">In the request body, supply a JSON representation for the windows10GeneralConfiguration object.</span></span>

<span data-ttu-id="ef6d8-125">下表显示创建 iosMobileAppConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ef6d8-125">The following table shows the properties that are required when you create the iosUpdateDeviceStatus.</span></span>

|<span data-ttu-id="ef6d8-126">属性</span><span class="sxs-lookup"><span data-stu-id="ef6d8-126">Property</span></span>|<span data-ttu-id="ef6d8-127">类型</span><span class="sxs-lookup"><span data-stu-id="ef6d8-127">Type</span></span>|<span data-ttu-id="ef6d8-128">说明</span><span class="sxs-lookup"><span data-stu-id="ef6d8-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef6d8-129">id</span><span class="sxs-lookup"><span data-stu-id="ef6d8-129">id</span></span>|<span data-ttu-id="ef6d8-130">String</span><span class="sxs-lookup"><span data-stu-id="ef6d8-130">String</span></span>|<span data-ttu-id="ef6d8-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ef6d8-131">Key of the entity.</span></span> <span data-ttu-id="ef6d8-132">继承自 [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef6d8-132">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="ef6d8-133">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="ef6d8-133">targetedMobileApps</span></span>|<span data-ttu-id="ef6d8-134">String 集合</span><span class="sxs-lookup"><span data-stu-id="ef6d8-134">String collection</span></span>|<span data-ttu-id="ef6d8-135">关联的应用。</span><span class="sxs-lookup"><span data-stu-id="ef6d8-135">the associated app.</span></span> <span data-ttu-id="ef6d8-136">继承自 [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef6d8-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="ef6d8-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ef6d8-137">createdDateTime</span></span>|<span data-ttu-id="ef6d8-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef6d8-138">DateTimeOffset</span></span>|<span data-ttu-id="ef6d8-139">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ef6d8-139">DateTime the object was created.</span></span> <span data-ttu-id="ef6d8-140">继承自 [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef6d8-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="ef6d8-141">description</span><span class="sxs-lookup"><span data-stu-id="ef6d8-141">description</span></span>|<span data-ttu-id="ef6d8-142">String</span><span class="sxs-lookup"><span data-stu-id="ef6d8-142">String</span></span>|<span data-ttu-id="ef6d8-143">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="ef6d8-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ef6d8-144">继承自 [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef6d8-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="ef6d8-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ef6d8-145">lastModifiedDateTime</span></span>|<span data-ttu-id="ef6d8-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef6d8-146">DateTimeOffset</span></span>|<span data-ttu-id="ef6d8-147">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ef6d8-147">DateTime the object was last modified.</span></span> <span data-ttu-id="ef6d8-148">继承自 [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef6d8-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="ef6d8-149">displayName</span><span class="sxs-lookup"><span data-stu-id="ef6d8-149">displayName</span></span>|<span data-ttu-id="ef6d8-150">String</span><span class="sxs-lookup"><span data-stu-id="ef6d8-150">String</span></span>|<span data-ttu-id="ef6d8-151">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="ef6d8-151">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ef6d8-152">继承自 [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef6d8-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="ef6d8-153">version</span><span class="sxs-lookup"><span data-stu-id="ef6d8-153">version</span></span>|<span data-ttu-id="ef6d8-154">Int32</span><span class="sxs-lookup"><span data-stu-id="ef6d8-154">Int32</span></span>|<span data-ttu-id="ef6d8-155">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="ef6d8-155">Version of the device configuration.</span></span> <span data-ttu-id="ef6d8-156">继承自 [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef6d8-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="ef6d8-157">encodedSettingXml</span><span class="sxs-lookup"><span data-stu-id="ef6d8-157">encodedSettingXml</span></span>|<span data-ttu-id="ef6d8-158">Binary</span><span class="sxs-lookup"><span data-stu-id="ef6d8-158">Binary</span></span>|<span data-ttu-id="ef6d8-159">mdm 应用配置 Base64 二进制。</span><span class="sxs-lookup"><span data-stu-id="ef6d8-159">mdm app configuration Base64 binary.</span></span>|
|<span data-ttu-id="ef6d8-160">settings</span><span class="sxs-lookup"><span data-stu-id="ef6d8-160">settings</span></span>|<span data-ttu-id="ef6d8-161">[appConfigurationSettingItem](../resources/intune_apps_appconfigurationsettingitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ef6d8-161">[appConfigurationSettingItem](../resources/intune_apps_appconfigurationsettingitem.md) collection</span></span>|<span data-ttu-id="ef6d8-162">应用配置设置项。</span><span class="sxs-lookup"><span data-stu-id="ef6d8-162">app configuration setting items.</span></span>|



## <a name="response"></a><span data-ttu-id="ef6d8-163">响应</span><span class="sxs-lookup"><span data-stu-id="ef6d8-163">Response</span></span>
<span data-ttu-id="ef6d8-164">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ef6d8-164">If successful, this method returns a `201 Created` response code and a [windowsPhone81CompliancePolicy](../resources/intune_apps_iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef6d8-165">示例</span><span class="sxs-lookup"><span data-stu-id="ef6d8-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="ef6d8-166">请求</span><span class="sxs-lookup"><span data-stu-id="ef6d8-166">Request</span></span>
<span data-ttu-id="ef6d8-167">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ef6d8-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations
Content-type: application/json
Content-length: 598

{
  "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
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

### <a name="response"></a><span data-ttu-id="ef6d8-168">响应</span><span class="sxs-lookup"><span data-stu-id="ef6d8-168">Response</span></span>
<span data-ttu-id="ef6d8-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ef6d8-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



