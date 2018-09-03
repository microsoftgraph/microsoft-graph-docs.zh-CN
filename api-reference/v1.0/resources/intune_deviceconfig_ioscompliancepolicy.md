# <a name="ioscompliancepolicy-resource-type"></a>iosCompliancePolicy 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

此类包含 iOS 的合规性设置。

继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列举 iosCompliancePolicies](../api/intune_deviceconfig_ioscompliancepolicy_list.md)|[iosCompliancePolicy](../resources/intune_deviceconfig_ioscompliancepolicy.md) 集合|列出 [iosCompliancePolicy](../resources/intune_deviceconfig_ioscompliancepolicy.md) 对象的属性和关系。|
|[获取 iosCompliancePolicy](../api/intune_deviceconfig_ioscompliancepolicy_get.md)|[iosCompliancePolicy](../resources/intune_deviceconfig_ioscompliancepolicy.md)|读取 [iosCompliancePolicy](../resources/intune_deviceconfig_ioscompliancepolicy.md) 对象的属性和关系。|
|[创建 iosCompliancePolicy](../api/intune_deviceconfig_ioscompliancepolicy_create.md)|[iosCompliancePolicy](../resources/intune_deviceconfig_ioscompliancepolicy.md)|创建新的 [iosCompliancePolicy](../resources/intune_deviceconfig_ioscompliancepolicy.md) 对象。|
|[删除 iosCompliancePolicy](../api/intune_deviceconfig_ioscompliancepolicy_delete.md)|无|删除 [iosCompliancePolicy](../resources/intune_deviceconfig_ioscompliancepolicy.md)。|
|[更新 iosCompliancePolicy](../api/intune_deviceconfig_ioscompliancepolicy_update.md)|[iosCompliancePolicy](../resources/intune_deviceconfig_ioscompliancepolicy.md)|更新 [iosCompliancePolicy](../resources/intune_deviceconfig_ioscompliancepolicy.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|ID|字符串|实体的键。 继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|说明|字符串|管理员提供的设备配置的说明。 继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|displayName|字符串|管理员提供的设备配置的名称。 继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|版本|Int32|设备配置的版本。 继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|passcodeBlockSimple|布尔值|指示是否阻止简单密码。|
|passcodeExpirationDays|Int32|密码过期前的天数。 有效值为 1 至 65535|
|passcodeMinimumLength|Int32|密码的最小长度。 有效值为 4 至 14|
|passcodeMinutesOfInactivityBeforeLock|Int32|在需要密码之前不活动的分钟数。|
|passcodePreviousPasscodeBlockCount|Int32|要阻止的以前密码的数量。 有效值为 1 至 24|
|passcodeMinimumCharacterSetCount|Int32|密码中必需的字符集数。|
|passcodeRequiredType|[requiredPasswordType](../resources/intune_deviceconfig_requiredpasswordtype.md)|必需的密码类型。 可取值为： `deviceDefault`, `alphanumeric`, `numeric`.|
|passcodeRequired|布尔值|指示是否需要密码。|
|osMinimumVersion|字符串|最低 IOS 版本。|
|osMaximumVersion|字符串|最高 IOS 版本。|
|securityBlockJailbrokenDevices|布尔值|设备不得越狱或取得 root 权限。|
|deviceThreatProtectionEnabled|布尔值|要求设备已启用设备威胁防护。|
|deviceThreatProtectionRequiredSecurityLevel|[deviceThreatProtectionLevel](../resources/intune_deviceconfig_devicethreatprotectionlevel.md)|要求按移动威胁防护最低风险级别来报告不符合情况。 可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。|
|managedEmailProfileRequired|布尔值|指示是否需要托管电子邮件配置文件。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|scheduledActionsForRule|[deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md) 集合|此规则的计划操作的列表 继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|deviceStatuses|[deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md) 集合|DeviceComplianceDeviceStatus 的列表。 继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|userStatuses|[deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) 集合|DeviceComplianceUserStatus 的列表。 继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|deviceStatusOverview|[deviceComplianceDeviceOverview](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md)|设备合规性设备状态概述 继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|userStatusOverview|[deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md)|设备合规性用户状态概述 继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) 集合|合规性设置状态设备摘要 继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|赋值|[deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) 集合|此合规性策略的作业集合。 继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.deviceCompliancePolicy",
  "@odata.type": "microsoft.graph.iosCompliancePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosCompliancePolicy",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 1024,
  "passcodeMinimumLength": 1024,
  "passcodeMinutesOfInactivityBeforeLock": 1024,
  "passcodePreviousPasscodeBlockCount": 1024,
  "passcodeMinimumCharacterSetCount": 1024,
  "passcodeRequiredType": "String",
  "passcodeRequired": true,
  "osMinimumVersion": "String",
  "osMaximumVersion": "String",
  "securityBlockJailbrokenDevices": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "String",
  "managedEmailProfileRequired": true
}
```



