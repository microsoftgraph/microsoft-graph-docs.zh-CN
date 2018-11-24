# <a name="importedwindowsautopilotdeviceidentityupload-resource-type"></a>importedWindowsAutopilotDeviceIdentityUpload 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

导入 windows 自动执行某些操作设备使用上载。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 importedWindowsAutopilotDeviceIdentityUploads](../api/intune_enrollment_importedwindowsautopilotdeviceidentityupload_list.md)|[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md)集合|列出属性和[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md)对象之间的关系。|
|[获取 importedWindowsAutopilotDeviceIdentityUpload](../api/intune_enrollment_importedwindowsautopilotdeviceidentityupload_get.md)|[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md)|读取属性和[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md)对象的关系。|
|[创建 importedWindowsAutopilotDeviceIdentityUpload](../api/intune_enrollment_importedwindowsautopilotdeviceidentityupload_create.md)|[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md)|创建新的[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md)对象。|
|[删除 importedWindowsAutopilotDeviceIdentityUpload](../api/intune_enrollment_importedwindowsautopilotdeviceidentityupload_delete.md)|无|删除[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md)。|
|[更新 importedWindowsAutopilotDeviceIdentityUpload](../api/intune_enrollment_importedwindowsautopilotdeviceidentityupload_update.md)|[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md)|更新[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md)对象的属性。|
|[autopilotDeviceStream 函数](../api/intune_enrollment_importedwindowsautopilotdeviceidentityupload_autopilotdevicestream.md)|字符串|创建自动执行某些操作设备流上载请求。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|对象的 GUID|
|createdDateTimeUtc|DateTimeOffset|创建实体时的日期时间。|
|状态|[importedWindowsAutopilotDeviceIdentityUploadStatus](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityuploadstatus.md)|上载状态。 可取值为：`noUpload`、`pending`、`complete`、`error`。|

## <a name="relationships"></a>Relationships
|关系|类型|说明|
|:---|:---|:---|
|deviceIdentities|[importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md) 集合|作为此上载的一部分自动执行某些操作的所有设备的集合。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "id": "String (identifier)",
  "createdDateTimeUtc": "String (timestamp)",
  "status": "String"
}
```



