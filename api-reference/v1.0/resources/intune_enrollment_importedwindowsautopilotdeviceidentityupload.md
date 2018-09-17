# <a name="importedwindowsautopilotdeviceidentityupload-resource-type"></a>importedWindowsAutopilotDeviceIdentityUpload 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

使用上载导入 windows autopilot 设备。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List importedWindowsAutopilotDeviceIdentityUploads](../api/intune_enrollment_importedwindowsautopilotdeviceidentityupload_list.md)|[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) 集合|列出 [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) 对象的属性和关系。|
|[Get importedWindowsAutopilotDeviceIdentityUpload](../api/intune_enrollment_importedwindowsautopilotdeviceidentityupload_get.md)|[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md)|读取 [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) 对象的属性和关系。|
|[Create importedWindowsAutopilotDeviceIdentityUpload](../api/intune_enrollment_importedwindowsautopilotdeviceidentityupload_create.md)|[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md)|创建新的 [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) 对象。|
|[Delete importedWindowsAutopilotDeviceIdentityUpload](../api/intune_enrollment_importedwindowsautopilotdeviceidentityupload_delete.md)|无|删除 [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md)。|
|[Update importedWindowsAutopilotDeviceIdentityUpload](../api/intune_enrollment_importedwindowsautopilotdeviceidentityupload_update.md)|[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md)|更新 [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) 对象的属性。|
|[autopilotDeviceStream function](../api/intune_enrollment_importedwindowsautopilotdeviceidentityupload_autopilotdevicestream.md)|字符串|创建其中有 autopilot 设备流的上载请求。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|ID|字符串|对象的 GUID|
|createdDateTimeUtc|DateTimeOffset|创建实体时的日期时间。|
|status|[importedWindowsAutopilotDeviceIdentityUploadStatus](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityuploadstatus.md)|上载状态。 可取值为：`noUpload`、`pending`、`complete`、`error`。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|deviceIdentities|[importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md) 集合|作为此上载一部分的 Autopilot 设备集合。|

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








