# <a name="manageddevicemobileappconfiguration-resource-type"></a>managedDeviceMobileAppConfiguration 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

已注册设备移动应用配置的抽象类
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列举 managedDeviceMobileAppConfigurations](../api/intune_apps_manageddevicemobileappconfiguration_list.md)|[managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) 集合|列出 [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) 对象的属性和关系。|
|[获取 managedDeviceMobileAppConfiguration](../api/intune_apps_manageddevicemobileappconfiguration_get.md)|[managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)|读取 [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) 对象的属性和关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|ID|字符串|实体的键。|
|targetedMobileApps|String 集合|关联的应用。|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。|
|说明|字符串|管理员提供的设备配置说明。|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。|
|displayName|字符串|管理员提供的设备配置名称。|
|版本|Int32|设备配置的版本。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|赋值|[managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) 集合|应用配置的组分配列表。|
|deviceStatuses|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md) 集合|ManagedDeviceMobileAppConfigurationDeviceStatus 的列表。|
|userStatuses|[managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md) 集合|ManagedDeviceMobileAppConfigurationUserStatus 列表|
|deviceStatusSummary|[managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md)|应用配置设备状态摘要。|
|userStatusSummary|[managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md)|应用配置用户状态摘要。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!--{
  "blockType": "resource",
  "abstract": true,
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfiguration"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfiguration",
  "id": "String (identifier)",
  "targetedMobileApps": [
    "String"
  ],
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```



