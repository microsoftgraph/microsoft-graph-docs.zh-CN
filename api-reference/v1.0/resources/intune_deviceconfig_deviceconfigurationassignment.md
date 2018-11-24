# <a name="deviceconfigurationassignment-resource-type"></a>deviceConfigurationAssignment 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

设备配置分配实体将 AAD 组分配到特定设备配置。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceConfigurationAssignments](../api/intune_deviceconfig_deviceconfigurationassignment_list.md)|[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) 集合|列出 [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) 对象的属性和关系。|
|[获取 deviceConfigurationAssignment](../api/intune_deviceconfig_deviceconfigurationassignment_get.md)|[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)|读取 [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) 对象的属性和关系。|
|[创建 deviceConfigurationAssignment](../api/intune_deviceconfig_deviceconfigurationassignment_create.md)|[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)|创建新的 [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) 对象。|
|[删除 deviceConfigurationAssignment](../api/intune_deviceconfig_deviceconfigurationassignment_delete.md)|无|删除 [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)。|
|[更新 deviceConfigurationAssignment](../api/intune_deviceconfig_deviceconfigurationassignment_update.md)|[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)|更新 [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|分配的键。|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|设备配置的分配目标。|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



