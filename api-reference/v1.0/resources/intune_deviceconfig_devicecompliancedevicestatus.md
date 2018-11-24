# <a name="devicecompliancedevicestatus-resource-type"></a>deviceComplianceDeviceStatus 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

尚未记录
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceComplianceDeviceStatuses](../api/intune_deviceconfig_devicecompliancedevicestatus_list.md)|[deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md) 集合|列出 [deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md) 对象的属性和关系。|
|[获取 deviceComplianceDeviceStatus](../api/intune_deviceconfig_devicecompliancedevicestatus_get.md)|[deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md)|读取 [deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md) 对象的属性和关系。|
|[创建 deviceComplianceDeviceStatus](../api/intune_deviceconfig_devicecompliancedevicestatus_create.md)|[deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md)|创建新的 [deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md) 对象。|
|[删除 deviceComplianceDeviceStatus](../api/intune_deviceconfig_devicecompliancedevicestatus_delete.md)|无|删除 [deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md)。|
|[更新 deviceComplianceDeviceStatus](../api/intune_deviceconfig_devicecompliancedevicestatus_update.md)|[deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md)|更新 [deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|deviceDisplayName|String|DevicePolicyStatus 的设备名。|
|userName|String|报告的用户名|
|deviceModel|String|报告的设备模型|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|设备合规性宽限期的到期日期/时间|
|状态|[complianceStatus](../resources/intune_shared_compliancestatus.md)|策略报告的符合性状态。 可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。|
|lastReportedDateTime|DateTimeOffset|策略报告的上次修改日期时间。|
|userPrincipalName|String|UserPrincipalName。|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceDeviceStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
  "id": "String (identifier)",
  "deviceDisplayName": "String",
  "userName": "String",
  "deviceModel": "String",
  "complianceGracePeriodExpirationDateTime": "String (timestamp)",
  "status": "String",
  "lastReportedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```



