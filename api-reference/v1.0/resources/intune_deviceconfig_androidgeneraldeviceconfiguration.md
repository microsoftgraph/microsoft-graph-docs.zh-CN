# <a name="androidgeneraldeviceconfiguration-resource-type"></a>androidGeneralDeviceConfiguration 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

本主题提供由 androidGeneralDeviceConfiguration 资源公开的已声明方法、属性和关系的说明。

继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列举 androidGeneralDeviceConfigurations](../api/intune_deviceconfig_androidgeneraldeviceconfiguration_list.md)|[androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md) 集合|列出 [androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md) 对象的属性和关系。|
|[获取 androidGeneralDeviceConfiguration](../api/intune_deviceconfig_androidgeneraldeviceconfiguration_get.md)|[androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md)|读取 [androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md) 对象的属性和关系。|
|[创建 androidGeneralDeviceConfiguration](../api/intune_deviceconfig_androidgeneraldeviceconfiguration_create.md)|[androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md)|创建新的 [androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md) 对象。|
|[删除 androidGeneralDeviceConfiguration](../api/intune_deviceconfig_androidgeneraldeviceconfiguration_delete.md)|无|删除 [androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md)。|
|[更新 androidGeneralDeviceConfiguration](../api/intune_deviceconfig_androidgeneraldeviceconfiguration_update.md)|[androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md)|更新 [androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|ID|字符串|实体的键。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|说明|ID|管理员提供的设备配置的说明。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|displayName|ID|管理员提供的设备配置的名称。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|版本|Int32|设备配置的版本。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|appsBlockClipboardSharing|布尔值|指示是否阻止剪贴板共享以在应用程序之间复制和粘贴。|
|appsBlockCopyPaste|布尔值|指示是否阻止在应用程序内复制和粘贴。|
|appsBlockYouTube|布尔值|指示是否阻止 YouTube 应用。|
|bluetoothBlocked|布尔值|指示是否阻止蓝牙。|
|cameraBlocked|布尔值|指示是否阻止照相机的使用。|
|cellularBlockDataRoaming|布尔值|指示是否阻止数据漫游。|
|cellularBlockMessaging|布尔值|指示是否阻止 SMS/MMS 消息。|
|cellularBlockVoiceRoaming|布尔值|指示是否阻止语音漫游。|
|cellularBlockWiFiTethering|布尔值|指示是否阻止同步 Wi-Fi 网络共享。|
|compliantAppsList|[appListItem](../resources/intune_deviceconfig_applistitem.md) 集合|符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。 该集合最多可包含 10000 个元素。|
|compliantAppListType|[appListType](../resources/intune_deviceconfig_applisttype.md)|CompliantAppsList 中的列表类型。 可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。|
|diagnosticDataBlockSubmission|布尔值|指示是否阻止诊断数据提交。|
|locationServicesBlocked|布尔值|指示是否阻止位置服务。|
|googleAccountBlockAutoSync|布尔值|指示是否阻止 Google 帐户自动同步。|
|googlePlayStoreBlocked|布尔值|指示是否阻止 Google Play 商店。|
|kioskModeBlockSleepButton|布尔值|指示在展台模式下是否阻止屏幕睡眠按钮。|
|kioskModeBlockVolumeButtons|布尔值|指示在展台模式下是否阻止音量按钮。|
|kioskModeApps|[appListItem](../resources/intune_deviceconfig_applistitem.md) 集合|设备处于展台模式时将允许运行的应用列表。 该集合最多可包含 500 个元素。|
|nfcBlocked|布尔值|指示是否阻止近场通信。|
|passwordBlockFingerprintUnlock|布尔值|指示是否阻止指纹解锁。|
|passwordBlockTrustAgents|布尔值|指示是否阻止 Smart Lock 和其他信任代理。|
|passwordExpirationDays|Int32|密码过期前的天数。 有效值为 1 至 365。|
|passwordMinimumLength|Int32|密码的最小长度。 有效值为 4 至 16|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|屏幕超时之前的不活动分钟数。|
|passwordPreviousPasswordBlockCount|Int32|要阻止的以前密码的数量。 有效值为 0 至 24|
|passwordSignInFailureCountBeforeFactoryReset|Int32|恢复出厂设置之前允许登录失败的次数。 有效值为 4 至 11|
|passwordRequiredType|[androidRequiredPasswordType](../resources/intune_deviceconfig_androidrequiredpasswordtype.md)|必需的密码类型。 可取值为：`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any`。|
|passwordRequired|布尔值|指示是否需要密码。|
|powerOffBlocked|布尔值|指示是否阻止关闭设备。|
|factoryResetBlocked|布尔值|指示是否阻止用户执行恢复出厂设置。|
|screenCaptureBlocked|布尔值|指示是否阻止屏幕截图。|
|deviceSharingAllowed|布尔值|指示是否允许设备共享模式。|
|storageBlockGoogleBackup|布尔值|指示是否阻止 Google 备份。|
|storageBlockRemovableStorage|布尔值|指示是否阻止可移动存储使用。|
|storageRequireDeviceEncryption|布尔值|指示是否需要设备加密。|
|storageRequireRemovableStorageEncryption|布尔值|指示是否需要可移动存储加密。|
|voiceAssistantBlocked|布尔值|指示是否阻止使用语音助手。|
|voiceDialingBlocked|布尔值|指示是否阻止语音拨号。|
|webBrowserBlockPopups|布尔值|指示是否阻止 Web 浏览器内的弹出窗口。|
|webBrowserBlockAutofill|布尔值|指示是否阻止 Web 浏览器的自动填充功能。|
|webBrowserBlockJavaScript|布尔值|指示是否阻止 Web 浏览器内的 JavaScript。|
|webBrowserBlocked|布尔值|指示是否阻止 Web 浏览器。|
|webBrowserCookieSettings|[webBrowserCookieSettings](../resources/intune_deviceconfig_webbrowsercookiesettings.md)|Web 浏览器内的 Cookie 设置。 可取值为：`browserDefault`、`blockAlways`、`allowCurrentWebSite`、`allowFromWebsitesVisited`、`allowAlways`。|
|wiFiBlocked|布尔值|指示是否阻止同步 Wi-Fi。|
|appsInstallAllowList|[appListItem](../resources/intune_deviceconfig_applistitem.md) 集合|可以在 KNOX 设备上安装的应用列表。 该集合最多可包含 500 个元素。|
|appsLaunchBlockList|[appListItem](../resources/intune_deviceconfig_applistitem.md) 集合|阻止在 KNOX 设备上启动的应用列表。 该集合最多可包含 500 个元素。|
|appsHideList|[appListItem](../resources/intune_deviceconfig_applistitem.md) 集合|要在 KNOX 设备上隐藏的应用列表。 该集合最多可包含 500 个元素。|
|securityRequireVerifyApps|布尔值|要求启用 Android 验证应用功能。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|赋值|[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) 集合|设备配置文件的分配列表。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) 集合|按设备的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) 集合|按用户的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) 集合|设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.deviceConfiguration",
  "@odata.type": "microsoft.graph.androidGeneralDeviceConfiguration"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
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
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "compliantAppListType": "String",
  "diagnosticDataBlockSubmission": true,
  "locationServicesBlocked": true,
  "googleAccountBlockAutoSync": true,
  "googlePlayStoreBlocked": true,
  "kioskModeBlockSleepButton": true,
  "kioskModeBlockVolumeButtons": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "nfcBlocked": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordSignInFailureCountBeforeFactoryReset": 1024,
  "passwordRequiredType": "String",
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
  "webBrowserCookieSettings": "String",
  "wiFiBlocked": true,
  "appsInstallAllowList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "appsLaunchBlockList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "appsHideList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "securityRequireVerifyApps": true
}
```



