# <a name="sharedpcconfiguration-resource-type"></a>sharedPCConfiguration 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

本主题提供由 sharedPCConfiguration 资源公开的已声明方法、属性和关系的说明。

继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列举 sharedPCConfigurations](../api/intune_deviceconfig_sharedpcconfiguration_list.md)|[sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md) 集合|列出 [sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md) 对象的属性和关系。|
|[获取 sharedPCConfiguration](../api/intune_deviceconfig_sharedpcconfiguration_get.md)|[sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md)|读取 [sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md) 对象的属性和关系。|
|[创建 sharedPCConfiguration](../api/intune_deviceconfig_sharedpcconfiguration_create.md)|[sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md)|创建新的 [sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md) 对象。|
|[删除 sharedPCConfiguration](../api/intune_deviceconfig_sharedpcconfiguration_delete.md)|无|删除 [sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md)。|
|[更新 sharedPCConfiguration](../api/intune_deviceconfig_sharedpcconfiguration_update.md)|[sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md)|更新 [sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|ID|字符串|实体的键。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|说明|字符串|管理员提供的设备配置的说明。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|displayName|字符串|管理员提供的设备配置的名称。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|版本|Int32|设备配置的版本。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|accountManagerPolicy|[sharedPCAccountManagerPolicy](../resources/intune_deviceconfig_sharedpcaccountmanagerpolicy.md)|指定在共享电脑上管理帐户的方式。 仅当 disableAccountManager 为 false 时适用。|
|allowedAccounts|[sharedPCAllowedAccountType](../resources/intune_deviceconfig_sharedpcallowedaccounttype.md)|表明哪种类型的账号允许在共享计算机上使用。可取值为`guest`、`domain`。|
|allowLocalStorage|布尔值|指定在共享电脑上是否允许本地存储。|
|disableAccountManager|布尔值|禁用共享电脑模式的帐户管理器。|
|disableEduPolicies|布尔值|指定是否应禁用默认的共享电脑教育环境策略。 对于 Windows 10 RS2 及更高版本，将应用此策略而不将 Enabled 设置为 true。|
|disablePowerPolicies|布尔值|指定是否应禁用默认的共享电脑电源策略。|
|disableSignInOnResume|布尔值|禁用每当设备从睡眠模式唤醒时需要登录的要求。|
|已启用|布尔值|启用共享的电脑模式并应用共享的电脑策略。|
|idleTimeBeforeSleepInSeconds|Int32|指定电脑进入睡眠状态之前设备必须保持空闲状态的时间（以秒为单位）。 将此值设置为 0 可防止发生睡眠超时。|
|kioskAppDisplayName|字符串|指定启动由 SetKioskAppUserModelId 指定的应用的登录屏幕上显示的帐户的显示文本。 仅在设置 KioskAppUserModelId 后适用。|
|kioskAppUserModelId|字符串|指定要与分配的访问权限结合使用的应用的应用程序用户模型 ID。|
|maintenanceStartTime|TimeOfDay|指定维护小时的每日开始时间。|

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
  "baseType": "microsoft.graph.deviceConfiguration",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.sharedPCConfiguration"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.sharedPCConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "accountManagerPolicy": {
    "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy",
    "accountDeletionPolicy": "String",
    "cacheAccountsAboveDiskFreePercentage": 1024,
    "inactiveThresholdDays": 1024,
    "removeAccountsBelowDiskFreePercentage": 1024
  },
  "allowedAccounts": "String",
  "allowLocalStorage": true,
  "disableAccountManager": true,
  "disableEduPolicies": true,
  "disablePowerPolicies": true,
  "disableSignInOnResume": true,
  "enabled": true,
  "idleTimeBeforeSleepInSeconds": 1024,
  "kioskAppDisplayName": "String",
  "kioskAppUserModelId": "String",
  "maintenanceStartTime": "String (time of day)"
}
```








