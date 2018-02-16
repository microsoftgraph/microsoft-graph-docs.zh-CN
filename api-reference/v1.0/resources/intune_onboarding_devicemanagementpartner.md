# <a name="devicemanagementpartner-resource-type"></a>deviceManagementPartner 资源类型

> **注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

表示与设备管理合作伙伴的连接的实体。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceManagementPartners](../api/intune_onboarding_devicemanagementpartner_list.md)|[deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) 集合|列出 [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) 对象的属性和关系。|
|[获取 deviceManagementPartner](../api/intune_onboarding_devicemanagementpartner_get.md)|[deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md)|读取 [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) 对象的属性和关系。|
|[创建 deviceManagementPartner](../api/intune_onboarding_devicemanagementpartner_create.md)|[deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md)|创建新的 [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) 对象。|
|[删除 deviceManagementPartner](../api/intune_onboarding_devicemanagementpartner_delete.md)|无|删除 [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md)。|
|[更新 deviceManagementPartner](../api/intune_onboarding_devicemanagementpartner_update.md)|[deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md)|更新 [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|尚未记录|
|lastHeartbeatDateTime|DateTimeOffset|管理员启用“连接到设备管理合作伙伴”选项后上次检测信号的时间戳|
|partnerState|String|此租户的合作伙伴状态 可取值为：`unknown`、`unavailable`、`enabled`、`terminated`、`rejected``unresponsive`。|
|partnerAppType|String|合作伙伴应用类型 可取值为：`unknown`、`singleTenantApp`、`multiTenantApp`。|
|singleTenantAppId|String|合作伙伴单个租户应用 ID|
|displayName|String|合作伙伴显示名称|
|isConfigured|Boolean|是否配置了设备管理合作伙伴|
|whenPartnerDevicesWillBeRemovedDateTime|DateTimeOffset|要删除 PartnerDevices 时的日期/时间（UTC 时间）|
|whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime|DateTimeOffset|PartnerDevices 将被标记为“不符合”时的日期/时间（UTC 时间）|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementPartner"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "id": "String (identifier)",
  "lastHeartbeatDateTime": "String (timestamp)",
  "partnerState": "String",
  "partnerAppType": "String",
  "singleTenantAppId": "String",
  "displayName": "String",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemovedDateTime": "String (timestamp)",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "String (timestamp)"
}
```



