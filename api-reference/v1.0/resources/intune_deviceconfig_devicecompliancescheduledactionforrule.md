# <a name="devicecompliancescheduledactionforrule-resource-type"></a>deviceComplianceScheduledActionForRule 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

计划的规则操作
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceComplianceScheduledActionForRules](../api/intune_deviceconfig_devicecompliancescheduledactionforrule_list.md)|[deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md) 集合|列出 [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md) 对象的属性和关系。|
|[获取 deviceComplianceScheduledActionForRule](../api/intune_deviceconfig_devicecompliancescheduledactionforrule_get.md)|[deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md)|读取 [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md) 对象的属性和关系。|
|[创建 deviceComplianceScheduledActionForRule](../api/intune_deviceconfig_devicecompliancescheduledactionforrule_create.md)|[deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md)|创建新的 [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md) 对象。|
|[删除 deviceComplianceScheduledActionForRule](../api/intune_deviceconfig_devicecompliancescheduledactionforrule_delete.md)|无|删除 [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md)。|
|[更新 deviceComplianceScheduledActionForRule](../api/intune_deviceconfig_devicecompliancescheduledactionforrule_update.md)|[deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md)|更新 [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|ID|字符串|实体的键。|
|ruleName|String|此计划操作适用的规则名称。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|scheduledActionConfigurations|[deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) 集合|此合规性策略的计划操作配置列表。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceScheduledActionForRule"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "id": "String (identifier)",
  "ruleName": "String"
}
```








