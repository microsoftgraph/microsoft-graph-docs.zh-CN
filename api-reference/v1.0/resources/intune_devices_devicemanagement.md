# <a name="devicemanagement-resource-type"></a>deviceManagement 资源类型

> **注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

充当所有设备管理功能的容器的单例实体。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 deviceManagement](../api/intune_devices_devicemanagement_get.md)|[deviceManagement](../resources/intune_devices_devicemanagement.md)|读取 [deviceManagement](../resources/intune_devices_devicemanagement.md) 对象的属性和关系。|
|[更新 deviceManagement](../api/intune_devices_devicemanagement_update.md)|[deviceManagement](../resources/intune_devices_devicemanagement.md)|更新 [deviceManagement](../resources/intune_devices_devicemanagement.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|设备唯一标识符。|
|subscriptionState|String|租户移动设备管理订阅状态。 可取值为：`pending`、`active`、`warning`、`disabled`、`deleted`、`blocked`、`lockedOut`。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|applePushNotificationCertificate|[applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md)|Apple 推送通知证书。|
|managedDeviceOverview|[managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md)|设备概述|
|detectedApps|[detectedApp](../resources/intune_devices_detectedapp.md) 集合|检测到与设备关联的应用的列表。|
|managedDevices|[managedDevice](../resources/intune_devices_manageddevice.md) 集合|托管设备列表。|

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
  "id": "String (identifier)",
  "subscriptionState": "String"
}
```



