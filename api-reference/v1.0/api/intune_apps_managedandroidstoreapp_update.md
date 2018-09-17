# <a name="update-managedandroidstoreapp"></a>更新 managedAndroidStoreApp

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

更新 [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md) 对象的属性。
## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。

|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementApps.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|授权|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md) 对象的 JSON 表示形式。

下表显示了创建 [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md) 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|ID|字符串|实体的键。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|displayName|字符串|管理员提供或导入的应用标题。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|描述|字符串|应用的说明。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|发布服务器|字符串|应用的发布者。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|largeIcon|[mimeContent](../resources/intune_shared_mimecontent.md)|要显示在应用详细信息中并用于图标上传的大图标。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|createdDateTime|DateTimeOffset|创建应用的日期和时间。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改应用的日期和时间。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|isFeatured|布尔|指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|privacyInformationUrl|字符串|隐私声明 Url。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|informationUrl|字符串|详细信息 Url。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|所有者|字符串|应用的所有者。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|开发者|字符串|应用的开发者。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|备注|字符串|应用的备注。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|publishingState|[mobileAppPublishingState](../resources/intune_apps_mobileapppublishingstate.md)|应用程序的发布状态。除非应用程序已发布，否则无法分配应用。继承自 [mobileApp](../resources/intune_apps_mobileapp.md)。可能的值为：`notPublished`、`processing`、`published`。|
|appAvailability|[managedAppAvailability](../resources/intune_apps_managedappavailability.md)|应用程序的可用性。继承自 [managedApp](../resources/intune_apps_managedapp.md)。可能的值为：`global`、`lineOfBusiness`。|
|version|字符串|应用程序的版本。 继承自 [managedApp](../resources/intune_apps_managedapp.md)|
|packageId|字符串|应用的包 ID。|
|appStoreUrl|字符串|Android AppStoreUrl。|
|minimumSupportedOperatingSystem|[androidMinimumOperatingSystem](../resources/intune_apps_androidminimumoperatingsystem.md)|最低受支持操作系统的值。|



## <a name="response"></a>响应
如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md) 对象。

## <a name="example"></a>示例
### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1019

{
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "packageId": "Package Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  }
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1188

{
  "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
  "id": "89e7e991-e991-89e7-91e9-e78991e9e789",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "packageId": "Package Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  }
}
```








