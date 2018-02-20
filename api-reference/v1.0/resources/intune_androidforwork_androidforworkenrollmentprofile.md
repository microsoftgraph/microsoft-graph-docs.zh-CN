# <a name="androidforworkenrollmentprofile-resource-type"></a>androidForWorkEnrollmentProfile 资源类型

> **注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

注册配置文件，用于使用 Google 的云管理注册 COSU 设备。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List androidForWorkEnrollmentProfiles](../api/intune_androidforwork_androidforworkenrollmentprofile_list.md)|[androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) 集合|列出 [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) 对象的属性和关系。|
|[Get androidForWorkEnrollmentProfile](../api/intune_androidforwork_androidforworkenrollmentprofile_get.md)|[androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md)|读取 [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) 对象的属性和关系。|
|[Create androidForWorkEnrollmentProfile](../api/intune_androidforwork_androidforworkenrollmentprofile_create.md)|[androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md)|创建新的 [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) 对象。|
|[Delete androidForWorkEnrollmentProfile](../api/intune_androidforwork_androidforworkenrollmentprofile_delete.md)|无|删除 [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md)。|
|[Update androidForWorkEnrollmentProfile](../api/intune_androidforwork_androidforworkenrollmentprofile_update.md)|[androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md)|更新 [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) 对象的属性。|
|[revokeToken 操作](../api/intune_androidforwork_androidforworkenrollmentprofile_revoketoken.md)|无|尚未记录|
|[createToken 操作](../api/intune_androidforwork_androidforworkenrollmentprofile_createtoken.md)|无|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|accountId|String|注册配置文件隶属的租户 GUID。|
|id|String|注册配置文件的唯一 GUID。|
|name|String|（已弃用）注册配置文件的显示名称。|
|displayName|String|注册配置文件的显示名称。|
|description|String|注册配置文件的说明。|
|createdDateTime|DateTimeOffset|注册配置文件的创建日期/时间。|
|modifiedDateTime|DateTimeOffset|（已弃用）上次修改注册配置文件的日期/时间。|
|lastModifiedDateTime|DateTimeOffset|上次修改注册配置文件的日期/时间。|
|tokenValue|String|为此注册配置文件最新创建的令牌的值。|
|tokenExpirationDateTime|DateTimeOffset|最新创建的令牌的到期日期/时间。|
|totalEnrollmentCount|Int32|（已弃用）已使用此注册配置文件进行注册的 Android 设备总数。|
|enrolledDeviceCount|Int32|已使用此注册配置文件进行注册的 Android 设备总数。|
|qrCode|String|（已弃用）用于生成此令牌的 QR 码的字符串。|
|qrCodeContent|String|用于生成此令牌的 QR 码的字符串。|
|qrCodeImage|[mimeContent](../resources/intune_androidforwork_mimecontent.md)|用于生成此令牌的 QR 码的字符串。|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidForWorkEnrollmentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkEnrollmentProfile",
  "accountId": "String",
  "id": "String (identifier)",
  "name": "String",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "tokenValue": "String",
  "tokenExpirationDateTime": "String (timestamp)",
  "totalEnrollmentCount": 1024,
  "enrolledDeviceCount": 1024,
  "qrCode": "String",
  "qrCodeContent": "String",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  }
}
```



