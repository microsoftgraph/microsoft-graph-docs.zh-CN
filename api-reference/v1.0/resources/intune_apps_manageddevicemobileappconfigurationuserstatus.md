# <a name="manageddevicemobileappconfigurationuserstatus-resource-type"></a>managedDeviceMobileAppConfigurationUserStatus 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

包含某个用户的 MDM 移动应用配置状态的属性、继承属性和操作。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 managedDeviceMobileAppConfigurationUserStatuses](../api/intune_apps_manageddevicemobileappconfigurationuserstatus_list.md)|[managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md) 集合|列出 [managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md) 对象的属性和关系。|
|[获取 managedDeviceMobileAppConfigurationUserStatus](../api/intune_apps_manageddevicemobileappconfigurationuserstatus_get.md)|[managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md)|读取 [managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md) 对象的属性和关系。|
|[创建 managedDeviceMobileAppConfigurationUserStatus](../api/intune_apps_manageddevicemobileappconfigurationuserstatus_create.md)|[managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md)|创建新的 [managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md) 对象。|
|[删除 managedDeviceMobileAppConfigurationUserStatus](../api/intune_apps_manageddevicemobileappconfigurationuserstatus_delete.md)|无|删除 [managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md)。|
|[更新 managedDeviceMobileAppConfigurationUserStatus](../api/intune_apps_manageddevicemobileappconfigurationuserstatus_update.md)|[managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md)|更新 [managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|实体的键。|
|userDisplayName|字符串|DevicePolicyStatus 的用户名。|
|devicesCount|Int32|该用户的设备计数。|
|status|[complianceStatus](../resources/intune_shared_compliancestatus.md)|策略报告的合规性状态。 可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`。|
|lastReportedDateTime|DateTimeOffset|策略报告的上次修改日期时间。|
|userPrincipalName|字符串|UserPrincipalName。|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationUserStatus"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserStatus",
  "id": "String (identifier)",
  "userDisplayName": "String",
  "devicesCount": 1024,
  "status": "String",
  "lastReportedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```



