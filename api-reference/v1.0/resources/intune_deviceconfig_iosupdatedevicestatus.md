# <a name="iosupdatedevicestatus-resource-type"></a>iosUpdateDeviceStatus 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

尚未记录
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 iosUpdateDeviceStatuses](../api/intune_deviceconfig_iosupdatedevicestatus_list.md)|[iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) 集合|列出 [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) 对象的属性和关系。|
|[获取 iosUpdateDeviceStatus](../api/intune_deviceconfig_iosupdatedevicestatus_get.md)|[iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md)|读取 [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) 对象的属性和关系。|
|[创建 iosUpdateDeviceStatus](../api/intune_deviceconfig_iosupdatedevicestatus_create.md)|[iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md)|创建新的 [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) 对象。|
|[删除 iosUpdateDeviceStatus](../api/intune_deviceconfig_iosupdatedevicestatus_delete.md)|无|删除 [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md)。|
|[更新 iosUpdateDeviceStatus](../api/intune_deviceconfig_iosupdatedevicestatus_update.md)|[iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md)|更新 [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|ID|字符串|实体的键。|
|installStatus|[iosUpdatesInstallStatus](../resources/intune_deviceconfig_iosupdatesinstallstatus.md)|策略报告安装状态。 可能的值为： `success` ， `available` ， `idle` ， `unknown` ， `downloading` ， `downloadFailed` ， `downloadRequiresComputer` ， `downloadInsufficientSpace` ， `downloadInsufficientPower` ， `downloadInsufficientNetwork` ， `installing` ， `installInsufficientSpace` ， `installInsufficientPower` ， `installPhoneCallInProgress` ， `installFailed` ， `notSupportedOperation` ， `sharedDeviceUserLoggedInError` 。|
|osVersion|字符串|报告的设备版本。|
|deviceId|字符串|报告的设备 ID。|
|userId|字符串|报告的用户 ID。|
|deviceDisplayName|字符串|DevicePolicyStatus 的设备名。|
|userName|字符串|报告的用户名|
|deviceModel|字符串|报告的设备模型|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|设备符合性宽限期的到期日期/时间|
|状态|[complianceStatus](../resources/intune_shared_compliancestatus.md)|策略报告的合规性状态。 可能的值为： `unknown` 、 `notApplicable` 、 `compliant` 、 `remediated` 、 `nonCompliant` 、 `error` 、 `conflict` 、 `notAssigned` 。|
|lastReportedDateTime|DateTimeOffset|策略报告的上次修改日期时间。|
|userPrincipalName|字符串|UserPrincipalName。|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosUpdateDeviceStatus"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.iosUpdateDeviceStatus",
  "id": "String (identifier)",
  "installStatus": "String",
  "osVersion": "String",
  "deviceId": "String",
  "userId": "String",
  "deviceDisplayName": "String",
  "userName": "String",
  "deviceModel": "String",
  "complianceGracePeriodExpirationDateTime": "String (timestamp)",
  "status": "String",
  "lastReportedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```








