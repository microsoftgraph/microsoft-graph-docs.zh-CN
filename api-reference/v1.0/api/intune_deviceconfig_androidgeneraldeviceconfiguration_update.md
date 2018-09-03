# <a name="update-androidgeneraldeviceconfiguration"></a>更新 androidGeneralDeviceConfiguration

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

更新 [androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md) 对象的属性。
## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。

|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementConfiguration.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|授权|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md) 对象的 JSON 表示形式。

下表显示创建 [androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md) 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|字符串|实体的键。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|描述|字符串|管理员提供的设备配置的说明。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|displayName|字符串|管理员提供的设备配置的名称。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|版本|Int32|设备配置的版本。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|appsBlockClipboardSharing|布尔|指示是否阻止剪贴板共享以在应用程序之间复制和粘贴。|
|appsBlockCopyPaste|布尔|指示是否阻止在应用程序内复制和粘贴。|
|appsBlockYouTube|布尔|指示是否阻止 YouTube 应用。|
|bluetoothBlocked|布尔|指示是否阻止蓝牙。|
|cameraBlocked|布尔|指示是否阻止照相机的使用。|
|cellularBlockDataRoaming|布尔|指示是否阻止数据漫游。|
|cellularBlockMessaging|布尔|指示是否阻止 SMS/MMS 消息。|
|cellularBlockVoiceRoaming|布尔|指示是否阻止语音漫游。|
|cellularBlockWiFiTethering|布尔|指示是否阻止同步 Wi-Fi 网络共享。|
|compliantAppsList|[appListItem](../resources/intune_deviceconfig_applistitem.md) 集合|符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。 该集合最多可包含 10000 个元素。|
|compliantAppListType|[appListType](../resources/intune_deviceconfig_applisttype.md)|位于 CompliantAppsList 中的列表类型。 可能的值为： `none` 、 `appsInListCompliant` 、 `appsNotInListCompliant` 。|
|diagnosticDataBlockSubmission|布尔|指示是否阻止诊断数据提交。|
|locationServicesBlocked|布尔|指示是否阻止位置服务。|
|googleAccountBlockAutoSync|布尔|指示是否阻止 Google 帐户自动同步。|
|googlePlayStoreBlocked|布尔|指示是否阻止 Google Play 商店。|
|kioskModeBlockSleepButton|布尔|指示在展台模式下是否阻止屏幕睡眠按钮。|
|kioskModeBlockVolumeButtons|布尔|指示在展台模式下是否阻止音量按钮。|
|kioskModeApps|[appListItem](../resources/intune_deviceconfig_applistitem.md) 集合|设备处于展台模式时将允许运行的应用列表。 该集合最多可包含 500 个元素。|
|nfcBlocked|布尔|指示是否阻止近场通信。|
|passwordBlockFingerprintUnlock|布尔|指示是否阻止指纹解锁。|
|passwordBlockTrustAgents|布尔|指示是否阻止 Smart Lock 和其他信任代理。|
|passwordExpirationDays|Int32|密码过期前的天数。 有效值为 1 至 365。|
|passwordMinimumLength|Int32|密码的最小长度。 有效值为 4 至 16|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|屏幕超时之前的不活动分钟数。|
|passwordPreviousPasswordBlockCount|Int32|要阻止的以前密码的数量。 有效值为 0 至 24|
|passwordSignInFailureCountBeforeFactoryReset|Int32|恢复出厂设置之前允许登录失败的次数。 有效值为 4 至 11|
|passwordRequiredType|[androidRequiredPasswordType](../resources/intune_deviceconfig_androidrequiredpasswordtype.md)|必需的密码类型。 可取值为： `deviceDefault` 、 `alphabetic` 、 `alphanumeric` 、 `alphanumericWithSymbols` 、 `lowSecurityBiometric` 、 `numeric` 、 `numericComplex` 、 `any` 。|
|passwordRequired|布尔|指示是否需要密码。|
|powerOffBlocked|布尔|指示是否阻止关闭设备。|
|factoryResetBlocked|布尔|指示是否阻止用户执行恢复出厂设置。|
|screenCaptureBlocked|布尔|指示是否阻止屏幕截图。|
|deviceSharingAllowed|布尔|指示是否允许设备共享模式。|
|storageBlockGoogleBackup|布尔|指示是否阻止 Google 备份。|
|storageBlockRemovableStorage|布尔|指示是否阻止可移动存储使用。|
|storageRequireDeviceEncryption|布尔|指示是否需要设备加密。|
|storageRequireRemovableStorageEncryption|布尔|指示是否需要可移动存储加密。|
|voiceAssistantBlocked|布尔|指示是否阻止使用语音助手。|
|voiceDialingBlocked|布尔|指示是否阻止语音拨号。|
|webBrowserBlockPopups|布尔|指示是否阻止 Web 浏览器内的弹出窗口。|
|webBrowserBlockAutofill|布尔|指示是否阻止 Web 浏览器的自动填充功能。|
|webBrowserBlockJavaScript|布尔|指示是否阻止 Web 浏览器内的 JavaScript。|
|webBrowserBlocked|布尔|指示是否阻止 Web 浏览器。|
|webBrowserCookieSettings|[webBrowserCookieSettings](../resources/intune_deviceconfig_webbrowsercookiesettings.md)|Web 浏览器内的 Cookie 设置。 可取值为： `browserDefault` 、 `blockAlways` 、 `allowCurrentWebSite` 、 `allowFromWebsitesVisited` 、 `allowAlways` 。|
|wiFiBlocked|布尔|指示是否阻止同步 Wi-Fi。|
|appsInstallAllowList|[appListItem](../resources/intune_deviceconfig_applistitem.md) 集合|可以在 KNOX 设备上安装的应用列表。 该集合最多可包含 500 个元素。|
|appsLaunchBlockList|[appListItem](../resources/intune_deviceconfig_applistitem.md) 集合|阻止在 KNOX 设备上启动的应用列表。 该集合最多可包含 500 个元素。|
|appsHideList|[appListItem](../resources/intune_deviceconfig_applistitem.md) 集合|要在 KNOX 设备上隐藏的应用列表。 该集合最多可包含 500 个元素。|
|securityRequireVerifyApps|布尔|要求启用 Android 验证应用功能。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md) 对象。

## <a name="example"></a>示例
### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 3025

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "appsBlockClipboardSharing": true,
  "appsBlockCopyPaste": true,
  "appsBlockYouTube": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockMessaging": true,
  "cellularBlockVoiceRoaming": true,
  "cellularBlockWiFiTethering": true,
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
  "diagnosticDataBlockSubmission": true,
  "locationServicesBlocked": true,
  "googleAccountBlockAutoSync": true,
  "googlePlayStoreBlocked": true,
  "kioskModeBlockSleepButton": true,
  "kioskModeBlockVolumeButtons": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "nfcBlocked": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphabetic",
  "passwordRequired": true,
  "powerOffBlocked": true,
  "factoryResetBlocked": true,
  "screenCaptureBlocked": true,
  "deviceSharingAllowed": true,
  "storageBlockGoogleBackup": true,
  "storageBlockRemovableStorage": true,
  "storageRequireDeviceEncryption": true,
  "storageRequireRemovableStorageEncryption": true,
  "voiceAssistantBlocked": true,
  "voiceDialingBlocked": true,
  "webBrowserBlockPopups": true,
  "webBrowserBlockAutofill": true,
  "webBrowserBlockJavaScript": true,
  "webBrowserBlocked": true,
  "webBrowserCookieSettings": "blockAlways",
  "wiFiBlocked": true,
  "appsInstallAllowList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsLaunchBlockList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsHideList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "securityRequireVerifyApps": true
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3205

{
  "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
  "id": "9e00d534-d534-9e00-34d5-009e34d5009e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "appsBlockClipboardSharing": true,
  "appsBlockCopyPaste": true,
  "appsBlockYouTube": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockMessaging": true,
  "cellularBlockVoiceRoaming": true,
  "cellularBlockWiFiTethering": true,
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
  "diagnosticDataBlockSubmission": true,
  "locationServicesBlocked": true,
  "googleAccountBlockAutoSync": true,
  "googlePlayStoreBlocked": true,
  "kioskModeBlockSleepButton": true,
  "kioskModeBlockVolumeButtons": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "nfcBlocked": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphabetic",
  "passwordRequired": true,
  "powerOffBlocked": true,
  "factoryResetBlocked": true,
  "screenCaptureBlocked": true,
  "deviceSharingAllowed": true,
  "storageBlockGoogleBackup": true,
  "storageBlockRemovableStorage": true,
  "storageRequireDeviceEncryption": true,
  "storageRequireRemovableStorageEncryption": true,
  "voiceAssistantBlocked": true,
  "voiceDialingBlocked": true,
  "webBrowserBlockPopups": true,
  "webBrowserBlockAutofill": true,
  "webBrowserBlockJavaScript": true,
  "webBrowserBlocked": true,
  "webBrowserCookieSettings": "blockAlways",
  "wiFiBlocked": true,
  "appsInstallAllowList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsLaunchBlockList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsHideList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "securityRequireVerifyApps": true
}
```



