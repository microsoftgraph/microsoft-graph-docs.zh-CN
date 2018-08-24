# <a name="importedwindowsautopilotdeviceidentity-resource-type"></a>importedWindowsAutopilotDeviceIdentity 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

导入 Windows AutoPilot 的设备。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 importedWindowsAutopilotDeviceIdentities](../api/intune_enrollment_importedwindowsautopilotdeviceidentity_list.md)|[importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md) 集合|列表属性和[importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md)对象关系。|
|[获取 importedWindowsAutopilotDeviceIdentity](../api/intune_enrollment_importedwindowsautopilotdeviceidentity_get.md)|[importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md)|阅读属性和关系[importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md)对象。|
|[Create importedWindowsAutopilotDeviceIdentity](../api/intune_enrollment_importedwindowsautopilotdeviceidentity_create.md)|[importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md)|创建新[importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md)对象。|
|[删除 importedWindowsAutopilotDeviceIdentity](../api/intune_enrollment_importedwindowsautopilotdeviceidentity_delete.md)|无|删除[importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md)。|
|[更新 importedWindowsAutopilotDeviceIdentity](../api/intune_enrollment_importedwindowsautopilotdeviceidentity_update.md)|[importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md)|更新 [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|对象的 GUID|
|orderIdentifier|字符串|Windows autopilot 设备订单 Id。|
|serialNumber|字符串|Windows autopilot 设备序列号。|
|productKey|字符串|Windows autopilot 设备产品密钥。|
|hardwareIdentifier|二进制|Windows autopilot 设备硬件 Blob。|
|状态|[importedWindowsAutopilotDeviceIdentityState](../resources/intune_enrollment_importedwindowsautopilotdeviceidentitystate.md)|导入设备的当前状态。|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
  "id": "String (identifier)",
  "orderIdentifier": "String",
  "serialNumber": "String",
  "productKey": "String",
  "hardwareIdentifier": "binary",
  "state": {
    "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
    "deviceImportStatus": "String",
    "deviceRegistrationId": "String",
    "deviceErrorCode": 1024,
    "deviceErrorName": "String"
  }
}
```



