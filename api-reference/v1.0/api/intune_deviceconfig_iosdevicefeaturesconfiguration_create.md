# <a name="create-iosdevicefeaturesconfiguration"></a><span data-ttu-id="f26fc-101">创建 iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="f26fc-101">Create iosDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="f26fc-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f26fc-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f26fc-103">创建新的 [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f26fc-103">Create a new [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f26fc-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="f26fc-104">Prerequisites</span></span>
<span data-ttu-id="f26fc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="f26fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f26fc-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="f26fc-107">Permission type</span></span>|<span data-ttu-id="f26fc-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f26fc-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f26fc-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f26fc-109">Delegated (work or school account)</span></span>|<span data-ttu-id="f26fc-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f26fc-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f26fc-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f26fc-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f26fc-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="f26fc-112">Not supported.</span></span>|
|<span data-ttu-id="f26fc-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="f26fc-113">Application</span></span>|<span data-ttu-id="f26fc-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f26fc-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f26fc-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f26fc-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f26fc-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="f26fc-116">Request headers</span></span>
|<span data-ttu-id="f26fc-117">标头</span><span class="sxs-lookup"><span data-stu-id="f26fc-117">Header</span></span>|<span data-ttu-id="f26fc-118">值</span><span class="sxs-lookup"><span data-stu-id="f26fc-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f26fc-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="f26fc-119">Authorization</span></span>|<span data-ttu-id="f26fc-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f26fc-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f26fc-121">Accept</span><span class="sxs-lookup"><span data-stu-id="f26fc-121">Accept</span></span>|<span data-ttu-id="f26fc-122">application/json</span><span class="sxs-lookup"><span data-stu-id="f26fc-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f26fc-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="f26fc-123">Request body</span></span>
<span data-ttu-id="f26fc-124">在请求正文中，提供 iosDeviceFeaturesConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f26fc-124">In the request body, supply a JSON representation for the iosDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="f26fc-125">下表显示创建 iosDeviceFeaturesConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f26fc-125">The following table shows the properties that are required when you create the iosDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="f26fc-126">属性</span><span class="sxs-lookup"><span data-stu-id="f26fc-126">Property</span></span>|<span data-ttu-id="f26fc-127">类型</span><span class="sxs-lookup"><span data-stu-id="f26fc-127">Type</span></span>|<span data-ttu-id="f26fc-128">说明</span><span class="sxs-lookup"><span data-stu-id="f26fc-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f26fc-129">id</span><span class="sxs-lookup"><span data-stu-id="f26fc-129">id</span></span>|<span data-ttu-id="f26fc-130">String</span><span class="sxs-lookup"><span data-stu-id="f26fc-130">String</span></span>|<span data-ttu-id="f26fc-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f26fc-131">Key of the entity.</span></span> <span data-ttu-id="f26fc-132">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f26fc-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f26fc-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f26fc-133">lastModifiedDateTime</span></span>|<span data-ttu-id="f26fc-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f26fc-134">DateTimeOffset</span></span>|<span data-ttu-id="f26fc-135">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f26fc-135">DateTime the object was last modified.</span></span> <span data-ttu-id="f26fc-136">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f26fc-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f26fc-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f26fc-137">createdDateTime</span></span>|<span data-ttu-id="f26fc-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f26fc-138">DateTimeOffset</span></span>|<span data-ttu-id="f26fc-139">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f26fc-139">DateTime the object was created.</span></span> <span data-ttu-id="f26fc-140">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f26fc-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f26fc-141">description</span><span class="sxs-lookup"><span data-stu-id="f26fc-141">description</span></span>|<span data-ttu-id="f26fc-142">String</span><span class="sxs-lookup"><span data-stu-id="f26fc-142">String</span></span>|<span data-ttu-id="f26fc-143">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="f26fc-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f26fc-144">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f26fc-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f26fc-145">displayName</span><span class="sxs-lookup"><span data-stu-id="f26fc-145">displayName</span></span>|<span data-ttu-id="f26fc-146">String</span><span class="sxs-lookup"><span data-stu-id="f26fc-146">String</span></span>|<span data-ttu-id="f26fc-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="f26fc-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f26fc-148">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f26fc-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f26fc-149">version</span><span class="sxs-lookup"><span data-stu-id="f26fc-149">version</span></span>|<span data-ttu-id="f26fc-150">Int32</span><span class="sxs-lookup"><span data-stu-id="f26fc-150">Int32</span></span>|<span data-ttu-id="f26fc-151">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="f26fc-151">Version of the device configuration.</span></span> <span data-ttu-id="f26fc-152">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f26fc-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f26fc-153">assetTagTemplate</span><span class="sxs-lookup"><span data-stu-id="f26fc-153">assetTagTemplate</span></span>|<span data-ttu-id="f26fc-154">String</span><span class="sxs-lookup"><span data-stu-id="f26fc-154">String</span></span>|<span data-ttu-id="f26fc-155">设备的资产标签信息，显示在登录窗口和锁定屏幕上。</span><span class="sxs-lookup"><span data-stu-id="f26fc-155">Asset tag information for the device, displayed on the login window and lock screen.</span></span>|
|<span data-ttu-id="f26fc-156">lockScreenFootnote</span><span class="sxs-lookup"><span data-stu-id="f26fc-156">lockScreenFootnote</span></span>|<span data-ttu-id="f26fc-157">String</span><span class="sxs-lookup"><span data-stu-id="f26fc-157">String</span></span>|<span data-ttu-id="f26fc-158">显示在登录窗口和锁定屏幕上的脚注。</span><span class="sxs-lookup"><span data-stu-id="f26fc-158">A footnote displayed on the login window and lock screen.</span></span> <span data-ttu-id="f26fc-159">在 iOS 9.3.1 及更高版本中可用。</span><span class="sxs-lookup"><span data-stu-id="f26fc-159">Available in iOS 9.3.1 and later.</span></span>|
|<span data-ttu-id="f26fc-160">homeScreenDockIcons</span><span class="sxs-lookup"><span data-stu-id="f26fc-160">homeScreenDockIcons</span></span>|<span data-ttu-id="f26fc-161">[iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f26fc-161">[iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="f26fc-162">主屏幕 Dock 上显示的应用和文件夹的列表。</span><span class="sxs-lookup"><span data-stu-id="f26fc-162">A list of app and folders to appear on the Home Screen Dock.</span></span> <span data-ttu-id="f26fc-163">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="f26fc-163">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="f26fc-164">homeScreenPages</span><span class="sxs-lookup"><span data-stu-id="f26fc-164">homeScreenPages</span></span>|<span data-ttu-id="f26fc-165">[iosHomeScreenPage](../resources/intune_deviceconfig_ioshomescreenpage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f26fc-165">[iosHomeScreenPage](../resources/intune_deviceconfig_ioshomescreenpage.md) collection</span></span>|<span data-ttu-id="f26fc-166">主屏幕上的页面的列表。</span><span class="sxs-lookup"><span data-stu-id="f26fc-166">A list of pages on the Home Screen.</span></span> <span data-ttu-id="f26fc-167">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="f26fc-167">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="f26fc-168">notificationSettings</span><span class="sxs-lookup"><span data-stu-id="f26fc-168">notificationSettings</span></span>|<span data-ttu-id="f26fc-169">[iosNotificationSettings](../resources/intune_deviceconfig_iosnotificationsettings.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f26fc-169">[iosNotificationSettings](../resources/intune_deviceconfig_iosnotificationsettings.md) collection</span></span>|<span data-ttu-id="f26fc-170">每个捆绑 ID 的通知设置。仅适用于监督模式下的设备（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="f26fc-170">Notification settings for each bundle id. Applicable to devices in supervised mode only (iOS 9.3 and later).</span></span> <span data-ttu-id="f26fc-171">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="f26fc-171">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="f26fc-172">响应</span><span class="sxs-lookup"><span data-stu-id="f26fc-172">Response</span></span>
<span data-ttu-id="f26fc-173">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f26fc-173">If successful, this method returns a `201 Created` response code and a [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f26fc-174">示例</span><span class="sxs-lookup"><span data-stu-id="f26fc-174">Example</span></span>
### <a name="request"></a><span data-ttu-id="f26fc-175">请求</span><span class="sxs-lookup"><span data-stu-id="f26fc-175">Request</span></span>
<span data-ttu-id="f26fc-176">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f26fc-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1988

{
  "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "assetTagTemplate": "Asset Tag Template value",
  "lockScreenFootnote": "Lock Screen Footnote value",
  "homeScreenDockIcons": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolder",
      "displayName": "Display Name value",
      "pages": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
          "displayName": "Display Name value",
          "apps": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenApp",
              "displayName": "Display Name value",
              "bundleID": "Bundle ID value"
            }
          ]
        }
      ]
    }
  ],
  "homeScreenPages": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenPage",
      "displayName": "Display Name value",
      "icons": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolder",
          "displayName": "Display Name value",
          "pages": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
              "displayName": "Display Name value",
              "apps": [
                {
                  "@odata.type": "microsoft.graph.iosHomeScreenApp",
                  "displayName": "Display Name value",
                  "bundleID": "Bundle ID value"
                }
              ]
            }
          ]
        }
      ]
    }
  ],
  "notificationSettings": [
    {
      "@odata.type": "microsoft.graph.iosNotificationSettings",
      "bundleID": "Bundle ID value",
      "appName": "App Name value",
      "publisher": "Publisher value",
      "enabled": true,
      "showInNotificationCenter": true,
      "showOnLockScreen": true,
      "alertType": "banner",
      "badgesEnabled": true,
      "soundsEnabled": true
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="f26fc-177">响应</span><span class="sxs-lookup"><span data-stu-id="f26fc-177">Response</span></span>
<span data-ttu-id="f26fc-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f26fc-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2160

{
  "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
  "id": "651e0ab3-0ab3-651e-b30a-1e65b30a1e65",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "assetTagTemplate": "Asset Tag Template value",
  "lockScreenFootnote": "Lock Screen Footnote value",
  "homeScreenDockIcons": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolder",
      "displayName": "Display Name value",
      "pages": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
          "displayName": "Display Name value",
          "apps": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenApp",
              "displayName": "Display Name value",
              "bundleID": "Bundle ID value"
            }
          ]
        }
      ]
    }
  ],
  "homeScreenPages": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenPage",
      "displayName": "Display Name value",
      "icons": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolder",
          "displayName": "Display Name value",
          "pages": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
              "displayName": "Display Name value",
              "apps": [
                {
                  "@odata.type": "microsoft.graph.iosHomeScreenApp",
                  "displayName": "Display Name value",
                  "bundleID": "Bundle ID value"
                }
              ]
            }
          ]
        }
      ]
    }
  ],
  "notificationSettings": [
    {
      "@odata.type": "microsoft.graph.iosNotificationSettings",
      "bundleID": "Bundle ID value",
      "appName": "App Name value",
      "publisher": "Publisher value",
      "enabled": true,
      "showInNotificationCenter": true,
      "showOnLockScreen": true,
      "alertType": "banner",
      "badgesEnabled": true,
      "soundsEnabled": true
    }
  ]
}
```



