# <a name="updatewindowsdeviceaccountactionparameter-resource-type"></a>updateWindowsDeviceAccountActionParameter 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

尚未记录
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|deviceAccount|[windowsDeviceAccount](../resources/intune_devices_windowsdeviceaccount.md)|尚未记录|
|passwordRotationEnabled|布尔值|尚未记录|
|calendarSyncEnabled|布尔值|尚未记录|
|deviceAccountEmail|String|尚未记录|
|exchangeServer|String|尚未记录|
|sessionInitiationProtocalAddress|String|尚未记录|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.updateWindowsDeviceAccountActionParameter"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.updateWindowsDeviceAccountActionParameter",
  "deviceAccount": {
    "@odata.type": "microsoft.graph.windowsDeviceAccount",
    "password": "String"
  },
  "passwordRotationEnabled": true,
  "calendarSyncEnabled": true,
  "deviceAccountEmail": "String",
  "exchangeServer": "String",
  "sessionInitiationProtocalAddress": "String"
}
```








