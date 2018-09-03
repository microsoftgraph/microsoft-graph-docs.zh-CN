# <a name="windows81generalconfiguration-resource-type"></a>windows81GeneralConfiguration 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

本主题提供由 windows81GeneralConfiguration 资源公开的已声明方法、属性和关系的说明。

继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列举 windows81GeneralConfigurations](../api/intune_deviceconfig_windows81generalconfiguration_list.md)|[windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md) 集合|列出 [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md) 对象的属性和关系。|
|[获取 windows81GeneralConfiguration](../api/intune_deviceconfig_windows81generalconfiguration_get.md)|[windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md)|读取 [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md) 对象的属性和关系。|
|[创建 windows81GeneralConfiguration](../api/intune_deviceconfig_windows81generalconfiguration_create.md)|[windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md)|创建新的 [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md) 对象。|
|[删除 windows81GeneralConfiguration](../api/intune_deviceconfig_windows81generalconfiguration_delete.md)|无|删除 [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md)。|
|[更新 windows81GeneralConfiguration](../api/intune_deviceconfig_windows81generalconfiguration_update.md)|[windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md)|更新 [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|windows81GeneralConfiguration|字符串|实体的键。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|说明|字符串|管理员提供的设备配置的说明。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|displayName|字符串|管理员提供的设备配置的名称。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|版本|Int32|设备配置的版本。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|accountsBlockAddingNonMicrosoftAccountEmail|布尔值|指示是否阻止用户将电子邮件帐户添加到未与 Microsoft 帐户关联的设备。|
|applyOnlyToWindows81|布尔值|指示此策略是否仅适用于 Windows 8.1 的值。 此属性是只读的。|
|browserBlockAutofill|布尔值|指示是否阻止自动填充。|
|browserBlockAutomaticDetectionOfIntranetSites|布尔值|指示是否阻止自动检测 Intranet 站点。|
|browserBlockEnterpriseModeAccess|布尔值|指示是否阻止企业模式访问。|
|browserBlockJavaScript|布尔值|指示是否阻止用户使用 JavaScript。|
|browserBlockPlugins|布尔值|指示是否阻止插件。|
|browserBlockPopups|布尔值|指示是否阻止弹出窗口。|
|browserBlockSendingDoNotTrackHeader|布尔值|指示是否阻止用户发送 Do Not Track 标头。|
|browserBlockSingleWordEntryOnIntranetSites|布尔值|指示是否阻止在 Intranet 站点上使用单字条目。|
|browserRequireSmartScreen|布尔值|指示是否要求用户使用智能屏幕筛选器。|
|browserEnterpriseModeSiteListLocation|字符串|企业模式网站列表位置。 可能是本地文件、本地网络或 http 位置。|
|browserInternetSecurityLevel|[internetSiteSecurityLevel](../resources/intune_deviceconfig_internetsitesecuritylevel.md)|Internet 安全级别。 可取值为：`userDefined`、`medium`、`mediumHigh`、`high`。|
|browserIntranetSecurityLevel|[siteSecurityLevel](../resources/intune_deviceconfig_sitesecuritylevel.md)|Intranet 安全级别。 可取值为：`userDefined`、`low`、`mediumLow`、`medium`、`mediumHigh`、`high`。|
|browserLoggingReportLocation|字符串|日志记录报表位置。|
|browserRequireHighSecurityForRestrictedSites|布尔值|指示是否要求受限站点具有高安全性。|
|browserRequireFirewall|布尔值|指示是否需要防火墙。|
|browserRequireFraudWarning|布尔值|指示是否需要诈骗警告。|
|browserTrustedSitesSecurityLevel|[siteSecurityLevel](../resources/intune_deviceconfig_sitesecuritylevel.md)|受信任的站点安全级别。 可取值为：`userDefined`、`low`、`mediumLow`、`medium`、`mediumHigh`、`high`。|
|cellularBlockDataRoaming|布尔值|指示是否阻止数据漫游。|
|diagnosticsBlockDataSubmission|布尔值|指示是否阻止诊断数据提交。|
|passwordBlockPicturePasswordAndPin|布尔值|指示是否阻止用户使用图片密码和 PIN。|
|passwordExpirationDays|Int32|密码过期天数。|
|passwordMinimumLength|Int32|密码最短长度。|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|屏幕超时之前的不活动分钟数。|
|passwordMinimumCharacterSetCount|Int32|密码中必需的字符集数。|
|passwordPreviousPasswordBlockCount|Int32|防止重复使用的先前密码的数量。 有效值为 0 至 24|
|passwordRequiredType|[requiredPasswordType](../resources/intune_deviceconfig_requiredpasswordtype.md)|必需的密码类型。 可能的取值为：`deviceDefault`、`alphanumeric`、`numeric`。|
|passwordSignInFailureCountBeforeFactoryReset|Int32|恢复出厂设置之前登录失败的次数。|
|storageRequireDeviceEncryption|布尔值|指示是否要求对移动设备加密。|
|updatesRequireAutomaticUpdates|布尔值|指示是否需要自动更新。|
|userAccountControlSettings|[windowsUserAccountControlSettings](../resources/intune_deviceconfig_windowsuseraccountcontrolsettings.md)|用户帐户控制设置。 可取值为：`userDefined`、`alwaysNotify`、`notifyOnAppChanges`、`notifyOnAppChangesWithoutDimming`、`neverNotify`。|
|workFoldersUrl|字符串|工作文件夹 url。|

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
  "@odata.type": "microsoft.graph.windows81GeneralConfiguration",
  "@odata.annotations": [
    {
      "property": "applyOnlyToWindows81",
      "capabilities": {
        "computed": true,
        "permissions": "Read"
      }
    }
  ]
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "applyOnlyToWindows81": true,
  "browserBlockAutofill": true,
  "browserBlockAutomaticDetectionOfIntranetSites": true,
  "browserBlockEnterpriseModeAccess": true,
  "browserBlockJavaScript": true,
  "browserBlockPlugins": true,
  "browserBlockPopups": true,
  "browserBlockSendingDoNotTrackHeader": true,
  "browserBlockSingleWordEntryOnIntranetSites": true,
  "browserRequireSmartScreen": true,
  "browserEnterpriseModeSiteListLocation": "String",
  "browserInternetSecurityLevel": "String",
  "browserIntranetSecurityLevel": "String",
  "browserLoggingReportLocation": "String",
  "browserRequireHighSecurityForRestrictedSites": true,
  "browserRequireFirewall": true,
  "browserRequireFraudWarning": true,
  "browserTrustedSitesSecurityLevel": "String",
  "cellularBlockDataRoaming": true,
  "diagnosticsBlockDataSubmission": true,
  "passwordBlockPicturePasswordAndPin": true,
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passwordMinimumCharacterSetCount": 1024,
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordRequiredType": "String",
  "passwordSignInFailureCountBeforeFactoryReset": 1024,
  "storageRequireDeviceEncryption": true,
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "String",
  "workFoldersUrl": "String"
}
```



