# <a name="windowsdefenderscanactionresult-resource-type"></a>windowsDefenderScanActionResult 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

Windows Defender 最后扫描结果

继承自 [deviceActionResult](../resources/intune_devices_deviceactionresult.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|actionName|字符串|操作名称 继承自 [deviceActionResult](../resources/intune_devices_deviceactionresult.md)|
|actionState|[actionState](../resources/intune_devices_actionstate.md)|从 [ deviceActionResult ](../resources/intune_devices_deviceactionresult.md) 继承操作的状态。 可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。|
|startDateTime|DateTimeOffset|启动操作的时间 继承自 [deviceActionResult](../resources/intune_devices_deviceactionresult.md)|
|lastUpdatedDateTime|DateTimeOffset|操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune_devices_deviceactionresult.md)|
|scanType|字符串|扫描类型（完全扫描或快速扫描）|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsDefenderScanActionResult"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDefenderScanActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "scanType": "String"
}
```








