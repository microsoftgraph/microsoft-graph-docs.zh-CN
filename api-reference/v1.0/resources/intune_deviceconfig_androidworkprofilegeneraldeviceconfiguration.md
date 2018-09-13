# <a name="androidworkprofilegeneraldeviceconfiguration-resource-type"></a>androidWorkProfileGeneralDeviceConfiguration 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

Android 工作配置文件常规设备配置。

继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List androidWorkProfileGeneralDeviceConfigurations](../api/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration_list.md)|[androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md) 集合|列出 [androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md) 对象的属性和关系。|
|[Get androidWorkProfileGeneralDeviceConfiguration](../api/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration_get.md)|[androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md)|读取 [androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md) 对象的属性和关系。|
|[Create androidWorkProfileGeneralDeviceConfiguration](../api/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration_create.md)|[androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md)|创建新的 [androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md) 对象。|
|[Delete androidWorkProfileGeneralDeviceConfiguration](../api/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration_delete.md)|无|删除 [androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md)。|
|[Update androidWorkProfileGeneralDeviceConfiguration](../api/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration_update.md)|[androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md)|更新 [androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|ID|字符串|实体的键。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|说明|字符串|管理员提供的设备配置的说明。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|displayName|字符串|管理员提供的设备配置的名称。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|version|Int32|设备配置的版本。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|passwordBlockFingerprintUnlock|布尔|指示是否阻止指纹解锁。|
|passwordBlockTrustAgents|布尔|指示是否阻止 Smart Lock 和其他信任代理。|
|passwordExpirationDays|Int32|密码过期前的天数。 有效值为 1 至 365。|
|passwordMinimumLength|Int32|密码的最小长度。 有效值为 4 至 16|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|屏幕超时之前的不活动分钟数。|
|passwordPreviousPasswordBlockCount|Int32|要阻止的以前密码的数量。 有效值为 0 至 24|
|passwordSignInFailureCountBeforeFactoryReset|Int32|恢复出厂设置之前允许登录失败的次数。 有效值为 4 至 11|
|passwordRequiredType|[androidWorkProfileRequiredPasswordType](../resources/intune_deviceconfig_androidworkprofilerequiredpasswordtype.md)|必需的密码类型。 可取值为：`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols`。|
|workProfileDataSharingType|[androidWorkProfileCrossProfileDataSharingType](../resources/intune_deviceconfig_androidworkprofilecrossprofiledatasharingtype.md)|允许共享的数据的类型。 可取值为：`deviceDefault`、`preventAny`、`allowPersonalToWork`、`noRestrictions`。|
|workProfileBlockNotificationsWhileDeviceLocked|布尔值|指示在设备锁定时是否阻止通知。|
|workProfileBlockAddingAccounts|布尔值|阻止用户在工作配置文件中添加/删除帐户。|
|workProfileBluetoothEnableContactSharing|布尔值|允许蓝牙设备访问企业联系人。|
|workProfileBlockScreenCapture|布尔值|阻止工作配置文件中的屏幕截图。|
|workProfileBlockCrossProfileCallerId|布尔值|阻止在个人资料中显示工作配置文件来电显示。|
|workProfileBlockCamera|布尔值|阻止工作配置文件摄像头。|
|workProfileBlockCrossProfileContactsSearch|布尔值|阻止工作配置文件联系人在个人资料中的可用性。|
|workProfileBlockCrossProfileCopyPaste|布尔值|布尔值，指示是否启用了禁止交叉配置文件复制/粘贴的设置。|
|workProfileDefaultAppPermissionPolicy|[androidWorkProfileDefaultAppPermissionPolicyType](../resources/intune_deviceconfig_androidworkprofiledefaultapppermissionpolicytype.md)|必需的密码类型。 可取值为：`deviceDefault`、`prompt`、`autoGrant`、`autoDeny`。|
|workProfilePasswordBlockFingerprintUnlock|布尔值|指示是否阻止工作配置文件的指纹解锁。|
|workProfilePasswordBlockTrustAgents|布尔值|指示是否阻止工作配置文件的 Smart Lock 和其他信任代理。|
|workProfilePasswordExpirationDays|Int32|工作配置文件密码过期前的天数。 有效值为 1 至 365|
|workProfilePasswordMinimumLength|Int32|工作配置文件密码最小长度。 有效值为 4 至 16|
|workProfilePasswordMinNumericCharacters|Int32|工作配置文件密码中所需的最小数字字符数。 有效值为 1 至 10|
|workProfilePasswordMinNonLetterCharacters|Int32|工作配置文件密码必须包含的最小非字母数。 有效值为 1 至 10|
|workProfilePasswordMinLetterCharacters|Int32|工作配置文件密码必须包含的最小字母数。 有效值为 1 至 10|
|workProfilePasswordMinLowerCaseCharacters|Int32|工作配置文件密码中必须包含的最小小写字符数。 有效值为 1 至 10|
|workProfilePasswordMinUpperCaseCharacters|Int32|工作配置文件密码中必须包含的最小大写字符数。 有效值为 1 至 10|
|workProfilePasswordMinSymbolCharacters|Int32|工作配置文件密码中必须包含的最小符号数。 有效值为 1 至 10|
|workProfilePasswordMinutesOfInactivityBeforeScreenTimeout|Int32|屏幕超时之前的不活动分钟数。|
|workProfilePasswordPreviousPasswordBlockCount|Int32|要阻止的以前工作配置文件密码的数量。 有效值为 0 至 24|
|workProfilePasswordSignInFailureCountBeforeFactoryReset|Int32|删除工作配置文件并删除所有公司数据之前允许的登录失败次数。 有效值为 4 至 11|
|workProfilePasswordRequiredType|[androidWorkProfileRequiredPasswordType](../resources/intune_deviceconfig_androidworkprofilerequiredpasswordtype.md)|所需的工作配置文件密码的类型。 可取值为：`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols`。|
|workProfileRequirePassword|布尔值|工作配置文件是否需要密码|
|securityRequireVerifyApps|布尔|要求启用 Android 验证应用功能。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|assignments|[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) 集合|设备配置文件的分配列表。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) 集合|按设备的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) 集合|用户的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) 集合|设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.deviceConfiguration",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidWorkProfileGeneralDeviceConfiguration"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordSignInFailureCountBeforeFactoryReset": 1024,
  "passwordRequiredType": "String",
  "workProfileDataSharingType": "String",
  "workProfileBlockNotificationsWhileDeviceLocked": true,
  "workProfileBlockAddingAccounts": true,
  "workProfileBluetoothEnableContactSharing": true,
  "workProfileBlockScreenCapture": true,
  "workProfileBlockCrossProfileCallerId": true,
  "workProfileBlockCamera": true,
  "workProfileBlockCrossProfileContactsSearch": true,
  "workProfileBlockCrossProfileCopyPaste": true,
  "workProfileDefaultAppPermissionPolicy": "String",
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockTrustAgents": true,
  "workProfilePasswordExpirationDays": 1024,
  "workProfilePasswordMinimumLength": 1024,
  "workProfilePasswordMinNumericCharacters": 1024,
  "workProfilePasswordMinNonLetterCharacters": 1024,
  "workProfilePasswordMinLetterCharacters": 1024,
  "workProfilePasswordMinLowerCaseCharacters": 1024,
  "workProfilePasswordMinUpperCaseCharacters": 1024,
  "workProfilePasswordMinSymbolCharacters": 1024,
  "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "workProfilePasswordPreviousPasswordBlockCount": 1024,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 1024,
  "workProfilePasswordRequiredType": "String",
  "workProfileRequirePassword": true,
  "securityRequireVerifyApps": true
}
```








