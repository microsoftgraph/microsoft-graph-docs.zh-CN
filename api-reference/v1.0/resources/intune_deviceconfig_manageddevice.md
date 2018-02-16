# <a name="manageddevice-resource-type"></a>managedDevice 资源类型

> **注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

通过 Intune 托管或预注册的设备
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 managedDevices](../api/intune_deviceconfig_manageddevice_list.md)|[managedDevice](../resources/intune_deviceconfig_manageddevice.md) 集合|列出 [managedDevice](../resources/intune_deviceconfig_manageddevice.md) 对象的属性和关系。|
|[获取 managedDevice](../api/intune_deviceconfig_manageddevice_get.md)|[managedDevice](../resources/intune_deviceconfig_manageddevice.md)|读取 [managedDevice](../resources/intune_deviceconfig_manageddevice.md) 对象的属性和关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|尚未记录|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|deviceConfigurationStates|[deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md) 集合|此设备的设备配置状态。|
|deviceCompliancePolicyStates|[deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md) 集合|此设备的设备合规性策略状态。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDevice",
  "id": "String (identifier)"
}
```



