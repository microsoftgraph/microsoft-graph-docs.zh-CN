# <a name="deviceinstallstate-resource-type"></a>deviceInstallState 资源类型

> **注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

包含某个设备的安装状态的属性。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceInstallStates](../api/intune_books_deviceinstallstate_list.md)|[deviceInstallState](../resources/intune_books_deviceinstallstate.md) 集合|列出 [deviceInstallState](../resources/intune_books_deviceinstallstate.md) 对象的属性和关系。|
|[获取 deviceInstallState](../api/intune_books_deviceinstallstate_get.md)|[deviceInstallState](../resources/intune_books_deviceinstallstate.md)|读取 [deviceInstallState](../resources/intune_books_deviceinstallstate.md) 对象的属性和关系。|
|[创建 deviceInstallState](../api/intune_books_deviceinstallstate_create.md)|[deviceInstallState](../resources/intune_books_deviceinstallstate.md)|创建新的 [deviceInstallState](../resources/intune_books_deviceinstallstate.md) 对象。|
|[删除 deviceInstallState](../api/intune_books_deviceinstallstate_delete.md)|无|删除 [deviceInstallState](../resources/intune_books_deviceinstallstate.md)。|
|[更新 deviceInstallState](../api/intune_books_deviceinstallstate_update.md)|[deviceInstallState](../resources/intune_books_deviceinstallstate.md)|更新 [deviceInstallState](../resources/intune_books_deviceinstallstate.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|deviceName|String|设备名称。|
|deviceId|String|设备 ID。|
|lastSyncDateTime|DateTimeOffset|上次同步日期和时间。|
|installState|String|电子书的安装状态。 可取值为：`notApplicable`、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`unknown`。|
|errorCode|String|安装失败的错误代码。|
|osVersion|String|操作系统版本。|
|osDescription|String|操作系统说明。|
|userName|String|设备用户名。|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceInstallState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceInstallState",
  "id": "String (identifier)",
  "deviceName": "String",
  "deviceId": "String",
  "lastSyncDateTime": "String (timestamp)",
  "installState": "String",
  "errorCode": "String",
  "osVersion": "String",
  "osDescription": "String",
  "userName": "String"
}
```



