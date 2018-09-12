# <a name="devicecompliancesettingstate-resource-type"></a>deviceComplianceSettingState 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

给定设备的设备符合性设置状态。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceComplianceSettingStates](../api/intune_deviceconfig_devicecompliancesettingstate_list.md)|[deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) 集合|列出 [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) 对象的属性和关系。|
|[获取 deviceComplianceSettingState](../api/intune_deviceconfig_devicecompliancesettingstate_get.md)|[deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md)|读取 [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) 对象的属性和关系。|
|[创建 deviceComplianceSettingState](../api/intune_deviceconfig_devicecompliancesettingstate_create.md)|[deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md)|创建新的 [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) 对象。|
|[删除 deviceComplianceSettingState](../api/intune_deviceconfig_devicecompliancesettingstate_delete.md)|无|删除 [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md)。|
|[更新 deviceComplianceSettingState](../api/intune_deviceconfig_devicecompliancesettingstate_update.md)|[deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md)|更新 [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|ID|字符串|实体的键|
|setting|字符串|设置类名和属性名。|
|settingName|字符串|报告的设置名称|
|deviceId|字符串|报告的设备 ID|
|deviceName|字符串|报告的设备名称|
|userId|字符串|报告的用户 ID|
|userEmail|字符串|报告的用户电子邮件地址|
|userName|字符串|报告的用户名|
|userPrincipalName|字符串|报告的用户主体名称|
|deviceModel|字符串|报告的设备模型|
|state|[complianceStatus](../resources/intune_shared_compliancestatus.md)|设置的合规性状态。可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|设备合规性宽限期的到期日期/时间|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceSettingState"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
  "id": "String (identifier)",
  "setting": "String",
  "settingName": "String",
  "deviceId": "String",
  "deviceName": "String",
  "userId": "String",
  "userEmail": "String",
  "userName": "String",
  "userPrincipalName": "String",
  "deviceModel": "String",
  "state": "String",
  "complianceGracePeriodExpirationDateTime": "String (timestamp)"
}
```








