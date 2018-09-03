# <a name="locatedeviceactionresult-resource-type"></a>locateDeviceActionResult 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

查找设备操作结果

继承自 [deviceActionResult](../resources/intune_devices_deviceactionresult.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|actionName|字符串|操作名称 继承自 [deviceActionResult](../resources/intune_devices_deviceactionresult.md)|
|actionState|[actionState](../resources/intune_devices_actionstate.md)|从 deviceActionResult 继承的操作状态。[ ](../resources/intune_devices_deviceactionresult.md) 可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。|
|startDateTime|DateTimeOffset|启动操作的时间 继承自 [deviceActionResult](../resources/intune_devices_deviceactionresult.md)|
|lastUpdatedDateTime|DateTimeOffset|操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune_devices_deviceactionresult.md)|
|deviceLocation|[deviceGeoLocation](../resources/intune_devices_devicegeolocation.md)|设备位置|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.deviceActionResult",
  "@odata.type": "microsoft.graph.locateDeviceActionResult"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.locateDeviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "deviceLocation": {"@odata.type": "microsoft.graph.deviceGeoLocation"}
}
```



