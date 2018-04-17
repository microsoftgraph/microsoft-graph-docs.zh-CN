# <a name="devicemanagement-resource-type"></a>deviceManagement 资源类型

> **重要说明：**Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

充当所有设备管理功能的容器的单例实体。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 deviceManagement](../api/intune_troubleshooting_devicemanagement_get.md)|[deviceManagement](../resources/intune_troubleshooting_devicemanagement.md)|读取 [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) 对象的属性和关系。|
|[更新 deviceManagement](../api/intune_troubleshooting_devicemanagement_update.md)|[deviceManagement](../resources/intune_troubleshooting_devicemanagement.md)|更新 [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|尚未记录|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|troubleshootingEvents|[deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) 集合|租户的故障排除事件列表。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)"
}
```



