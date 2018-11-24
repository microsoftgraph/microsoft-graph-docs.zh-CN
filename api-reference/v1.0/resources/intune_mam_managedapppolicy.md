# <a name="managedapppolicy-resource-type"></a>managedAppPolicy 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

ManagedAppPolicy 资源表示特定于平台的策略的基类型。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List managedAppPolicies](../api/intune_mam_managedapppolicy_list.md)|[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) 集合|列出 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md) 对象的属性和关系。|
|[Get managedAppPolicy](../api/intune_mam_managedapppolicy_get.md)|[managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|读取 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md) 对象的属性和关系。|
|[targetApps 操作](../api/intune_mam_managedapppolicy_targetapps.md)|无|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|策略显示名称。|
|description|String|策略的说明。|
|createdDateTime|DateTimeOffset|创建策略的日期和时间。|
|lastModifiedDateTime|DateTimeOffset|上次修改策略的时间。|
|id|String|实体的键。|
|version|String|实体的版本。|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppPolicy",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "version": "String"
}
```



