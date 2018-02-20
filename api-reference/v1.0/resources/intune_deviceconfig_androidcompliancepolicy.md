# <a name="androidcompliancepolicy-resource-type"></a>androidCompliancePolicy 资源类型

> **注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

此类包含 Android 的合规性设置。

继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List androidCompliancePolicies](../api/intune_deviceconfig_androidcompliancepolicy_list.md)|[androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md) 集合|列出 [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md) 对象的属性和关系。|
|[Get androidCompliancePolicy](../api/intune_deviceconfig_androidcompliancepolicy_get.md)|[androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md)|读取 [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md) 对象的属性和关系。|
|[Create androidCompliancePolicy](../api/intune_deviceconfig_androidcompliancepolicy_create.md)|[androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md)|创建新的 [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md) 对象。|
|[Delete androidCompliancePolicy](../api/intune_deviceconfig_androidcompliancepolicy_delete.md)|无|删除 [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md)。|
|[Update androidCompliancePolicy](../api/intune_deviceconfig_androidcompliancepolicy_update.md)|[androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md)|更新 [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|description|String|管理员提供的设备配置的说明。 继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|displayName|String|管理员提供的设备配置的名称。 继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|version|Int32|设备配置的版本。 继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|passwordRequired|Boolean|需要密码才可解锁设备。|
|passwordMinimumLength|Int32|最短密码长度。 有效值为 4 至 16|
|passwordRequiredType|String|密码中的字符类型 可取值为：`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any`。|
|passwordMinutesOfInactivityBeforeLock|Int32|在需要密码之前不活动的分钟数。|
|passwordExpirationDays|Int32|密码过期前的天数。 有效值为 1 至 365|
|passwordPreviousPasswordBlockCount|Int32|要阻止的以前密码的数量。|
|securityPreventInstallAppsFromUnknownSources|Boolean|要求设备不允许安装来自未知源的应用。|
|securityDisableUsbDebugging|Boolean|在 Android 设备上禁用 USB 调试。|
|securityRequireVerifyApps|Boolean|要求启用 Android 验证应用功能。|
|deviceThreatProtectionEnabled|Boolean|要求设备已启用设备威胁防护。|
|deviceThreatProtectionRequiredSecurityLevel|String|要求移动威胁防护最低风险级别来报告不合规情况。 可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。|
|securityBlockJailbrokenDevices|Boolean|设备不得越狱或取得 root 权限。|
|osMinimumVersion|String|最低 Android 版本。|
|osMaximumVersion|String|最高 Android 版本。|
|minAndroidSecurityPatchLevel|String|最低 Android 安全修补程序级别。|
|storageRequireEncryption|Boolean|要求对 Android 设备加密。|
|securityRequireSafetyNetAttestationBasicIntegrity|Boolean|要求设备传递 SafetyNet 基本完整性检查。|
|securityRequireSafetyNetAttestationCertifiedDevice|Boolean|要求设备传递 SafetyNet 认证设备检查。|
|securityRequireGooglePlayServices|Boolean|要求在设备上安装并启用 Google Play Services。|
|securityRequireUpToDateSecurityProviders|Boolean|要求设备具有最新的安全提供程序。 设备将要求启用 Google Play Services 并保持最新状态。|
|securityRequireCompanyPortalAppIntegrity|Boolean|要求设备传递公司门户客户端应用运行时完整性检查。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|scheduledActionsForRule|[deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md) 集合|此规则的计划操作的列表 继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|deviceStatuses|[deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md) 集合|DeviceComplianceDeviceStatus 的列表。 继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|userStatuses|[deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) 集合|DeviceComplianceUserStatus 的列表。 继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|deviceStatusOverview|[deviceComplianceDeviceOverview](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md)|设备合规性设备状态概述 继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|userStatusOverview|[deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md)|设备合规性用户状态概述 继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) 集合|合规性设置状态设备摘要 继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|assignments|[deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) 集合|此合规性策略的分配集合。 继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidCompliancePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidCompliancePolicy",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024,
  "passwordRequired": true,
  "passwordMinimumLength": 1024,
  "passwordRequiredType": "String",
  "passwordMinutesOfInactivityBeforeLock": 1024,
  "passwordExpirationDays": 1024,
  "passwordPreviousPasswordBlockCount": 1024,
  "securityPreventInstallAppsFromUnknownSources": true,
  "securityDisableUsbDebugging": true,
  "securityRequireVerifyApps": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "String",
  "securityBlockJailbrokenDevices": true,
  "osMinimumVersion": "String",
  "osMaximumVersion": "String",
  "minAndroidSecurityPatchLevel": "String",
  "storageRequireEncryption": true,
  "securityRequireSafetyNetAttestationBasicIntegrity": true,
  "securityRequireSafetyNetAttestationCertifiedDevice": true,
  "securityRequireGooglePlayServices": true,
  "securityRequireUpToDateSecurityProviders": true,
  "securityRequireCompanyPortalAppIntegrity": true
}
```



