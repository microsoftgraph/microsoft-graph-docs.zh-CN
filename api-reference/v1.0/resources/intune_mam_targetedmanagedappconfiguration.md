# <a name="targetedmanagedappconfiguration-resource-type"></a>targetedManagedAppConfiguration 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

用于将一组自定义设置按原样提供给目标安全组中的所有用户的配置

继承自 [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 targetedManagedAppConfigurations](../api/intune_mam_targetedmanagedappconfiguration_list.md)|[targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md) 集合|列出 [targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md) 对象的属性和关系。|
|[获取 targetedManagedAppConfiguration](../api/intune_mam_targetedmanagedappconfiguration_get.md)|[targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md)|读取 [targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md) 对象的属性和关系。|
|[创建 targetedManagedAppConfiguration](../api/intune_mam_targetedmanagedappconfiguration_create.md)|[targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md)|创建新的 [targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md) 对象。|
|[删除 targetedManagedAppConfiguration](../api/intune_mam_targetedmanagedappconfiguration_delete.md)|无|删除 [targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md)。|
|[更新 targetedManagedAppConfiguration](../api/intune_mam_targetedmanagedappconfiguration_update.md)|[targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md)|更新 [targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md) 对象的属性。|
|[assign 操作](../api/intune_mam_targetedmanagedappconfiguration_assign.md)|无|尚未记录|
|[targetApps 操作](../api/intune_mam_targetedmanagedappconfiguration_targetapps.md)|无|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|字符串|策略显示名称。 继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|
|description|字符串|策略的说明。 继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|
|createdDateTime|DateTimeOffset|创建策略的日期和时间。 继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改策略的时间。 继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|
|id|字符串|实体的键。 继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|
|版本|字符串|实体的版本。 继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|
|customSettings|[keyValuePair](../resources/intune_mam_keyvaluepair.md) 集合|要发送到配置范围确定的用户应用的一组字符串键和字符串值对，不由此服务更改。继承自 [ managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md)|
|deployedAppCount|Int32|当前策略部署到的应用的计数。|
|isAssigned|布尔|指示策略是否部署到任何包含组。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|apps|[managedMobileApp](../resources/intune_mam_managedmobileapp.md) 集合|策略部署到的应用的列表。|
|deploymentSummary|[managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md)|配置的部署摘要的导航属性。|
|作业|[targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md) 集合|策略部署到的包含组和排除组列表的导航属性。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.managedAppConfiguration",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.targetedManagedAppConfiguration"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "version": "String",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "deployedAppCount": 1024,
  "isAssigned": true
}
```








