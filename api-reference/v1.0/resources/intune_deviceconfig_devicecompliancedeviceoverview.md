# <a name="devicecompliancedeviceoverview-resource-type"></a>deviceComplianceDeviceOverview 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

尚未记录
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 deviceComplianceDeviceOverview](../api/intune_deviceconfig_devicecompliancedeviceoverview_get.md)|[deviceComplianceDeviceOverview](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md)|读取 [deviceComplianceDeviceOverview](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md) 对象的属性和关系。|
|[更新 deviceComplianceDeviceOverview](../api/intune_deviceconfig_devicecompliancedeviceoverview_update.md)|[deviceComplianceDeviceOverview](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md)|更新 [deviceComplianceDeviceOverview](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|ID|字符串|实体的键。|
|pendingCount|Int32|挂起设备的数量|
|notApplicableCount|Int32|不适用设备的数量|
|successCount|Int32|成功设备的数量|
|errorCount|Int32|错误设备的数量|
|failedCount|Int32|失败设备的数量|
|lastUpdateDateTime|DateTimeOffset|上次更新时间|
|configurationVersion|Int32|用于此概述的策略版本|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.deviceComplianceDeviceOverview"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceOverview",
  "id": "String (identifier)",
  "pendingCount": 1024,
  "notApplicableCount": 1024,
  "successCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "lastUpdateDateTime": "String (timestamp)",
  "configurationVersion": 1024
}
```



