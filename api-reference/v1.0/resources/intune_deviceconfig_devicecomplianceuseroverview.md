# <a name="devicecomplianceuseroverview-resource-type"></a>deviceComplianceUserOverview 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

尚未记录
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 deviceComplianceUserOverview](../api/intune_deviceconfig_devicecomplianceuseroverview_get.md)|[deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md)|读取 [deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md) 对象的属性和关系。|
|[更新 deviceComplianceUserOverview](../api/intune_deviceconfig_devicecomplianceuseroverview_update.md)|[deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md)|更新 [deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|pendingCount|Int32|待定用户的数量|
|notApplicableCount|Int32|不适用的用户数|
|successCount|Int32|成功的用户数量|
|errorCount|Int32|错误用户的数量|
|failedCount|Int32|失败用户的数量|
|lastUpdateDateTime|DateTimeOffset|上次更新时间|
|configurationVersion|Int32|用于此概述的策略版本|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceUserOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceUserOverview",
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



