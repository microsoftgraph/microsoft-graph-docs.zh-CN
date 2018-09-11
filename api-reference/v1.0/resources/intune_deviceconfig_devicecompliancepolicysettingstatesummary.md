# <a name="devicecompliancepolicysettingstatesummary-resource-type"></a>deviceCompliancePolicySettingStateSummary 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

跨帐户的设备合规性策略设置状态摘要。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceCompliancePolicySettingStateSummaries](../api/intune_deviceconfig_devicecompliancepolicysettingstatesummary_list.md)|[deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) 集合|列出 [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) 对象的属性和关系。|
|[获取 deviceCompliancePolicySettingStateSummary](../api/intune_deviceconfig_devicecompliancepolicysettingstatesummary_get.md)|[deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md)|读取 [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) 对象的属性和关系。|
|[创建 deviceCompliancePolicySettingStateSummary](../api/intune_deviceconfig_devicecompliancepolicysettingstatesummary_create.md)|[deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md)|创建新的 [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) 对象。|
|[删除 deviceCompliancePolicySettingStateSummary](../api/intune_deviceconfig_devicecompliancepolicysettingstatesummary_delete.md)|无|删除 [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md)。|
|[更新 deviceCompliancePolicySettingStateSummary](../api/intune_deviceconfig_devicecompliancepolicysettingstatesummary_update.md)|[deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md)|更新 [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|ID|字符串|实体的键。|
|设置|字符串|设置类名和属性名。|
|settingName|字符串|设置的名称。|
|platformType|[policyPlatformType](../resources/intune_deviceconfig_policyplatformtype.md)|设置平台。 可取值为：`android`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`all`。|
|unknownDeviceCount|Int32|未知设备的数量|
|notApplicableDeviceCount|Int32|不适用设备的数量|
|compliantDeviceCount|Int32|兼容设备的数量|
|remediatedDeviceCount|Int32|已修复设备的数量|
|nonCompliantDeviceCount|Int32|不兼容设备的数量|
|errorDeviceCount|Int32|错误设备的数量|
|conflictDeviceCount|Int32|冲突设备的数量|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|deviceComplianceSettingStates|[deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) 集合|尚未记录|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicySettingStateSummary"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "id": "String (identifier)",
  "setting": "String",
  "settingName": "String",
  "platformType": "String",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024
}
```








