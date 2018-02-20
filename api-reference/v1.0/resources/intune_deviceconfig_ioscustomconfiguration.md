# <a name="ioscustomconfiguration-resource-type"></a>iosCustomConfiguration 资源类型

> **注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

本主题提供由 iosCustomConfiguration 资源公开的已声明方法、属性和关系的说明。

继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List iosCustomConfigurations](../api/intune_deviceconfig_ioscustomconfiguration_list.md)|[iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md) 集合|列出 [iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md) 对象的属性和关系。|
|[Get iosCustomConfiguration](../api/intune_deviceconfig_ioscustomconfiguration_get.md)|[iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md)|读取 [iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md) 对象的属性和关系。|
|[Create iosCustomConfiguration](../api/intune_deviceconfig_ioscustomconfiguration_create.md)|[iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md)|创建新的 [iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md) 对象。|
|[Delete iosCustomConfiguration](../api/intune_deviceconfig_ioscustomconfiguration_delete.md)|无|删除 [iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md)。|
|[Update iosCustomConfiguration](../api/intune_deviceconfig_ioscustomconfiguration_update.md)|[iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md)|更新 [iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|description|String|管理员提供的设备配置的说明。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|displayName|String|管理员提供的设备配置的名称。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|version|Int32|设备配置的版本。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|payloadName|String|向用户显示的名称。|
|payloadFileName|String|有效负载文件名 (*.mobileconfig | *.xml)。|
|payload|Binary|有效负载。 （UTF8 编码的字节数组）|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|assignments|[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) 集合|设备配置文件的分配列表。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) 集合|按设备的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) 集合|按用户的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) 集合|设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosCustomConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosCustomConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "payloadName": "String",
  "payloadFileName": "String",
  "payload": "binary"
}
```



