# <a name="devicecompliancepolicy-resource-type"></a>deviceCompliancePolicy 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

这是符合性策略的基类。 符合性策略特定于平台，每个平台的符合性策略相互独立，且继承自此处。 
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列举 deviceCompliancePolicies](../api/intune_deviceconfig_devicecompliancepolicy_list.md)|[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) 集合|列出 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) 对象的属性和关系。|
|[获取 deviceCompliancePolicy](../api/intune_deviceconfig_devicecompliancepolicy_get.md)|[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|读取 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) 对象的属性和关系。|
|[assign 操作](../api/intune_deviceconfig_devicecompliancepolicy_assign.md)|[deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) 集合|尚未记录|
|[scheduleActionsForRules 操作](../api/intune_deviceconfig_devicecompliancepolicy_scheduleactionsforrules.md)|无|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|ID|字符串|实体的键。|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。|
|说明|字符串|管理员提供的设备配置说明。|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。|
|displayName|字符串|管理员提供的设备配置名称。|
|版本|Int32|设备配置的版本。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|scheduledActionsForRule|[deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md) 集合|此规则的计划操作列表|
|deviceStatuses|[deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md) 集合|DeviceComplianceDeviceStatus 的列表。|
|userStatuses|[deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) 集合|DeviceComplianceUserStatus 的列表。|
|deviceStatusOverview|[deviceComplianceDeviceOverview](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md)|设备符合性设备状态概述|
|userStatusOverview|[deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md)|设备符合性用户状态概述|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) 集合|符合性设置状态设备摘要|
|赋值|[deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) 集合|此符合性策略的分配集合。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "abstract": true,
  "@odata.type": "microsoft.graph.deviceCompliancePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicy",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```



