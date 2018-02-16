# <a name="enrollmentconfigurationassignment-resource-type"></a>enrollmentConfigurationAssignment 资源类型

> **注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

尚未记录
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 enrollmentConfigurationAssignments](../api/intune_onboarding_enrollmentconfigurationassignment_list.md)|[enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md) 集合|列出 [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md) 对象的属性和关系。|
|[获取 enrollmentConfigurationAssignment](../api/intune_onboarding_enrollmentconfigurationassignment_get.md)|[enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md)|读取 [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md) 对象的属性和关系。|
|[创建 enrollmentConfigurationAssignment](../api/intune_onboarding_enrollmentconfigurationassignment_create.md)|[enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md)|创建新的 [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md) 对象。|
|[删除 enrollmentConfigurationAssignment](../api/intune_onboarding_enrollmentconfigurationassignment_delete.md)|无|删除 [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md)。|
|[更新 enrollmentConfigurationAssignment](../api/intune_onboarding_enrollmentconfigurationassignment_update.md)|[enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md)|更新 [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|尚未记录|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune_onboarding_deviceandappmanagementassignmenttarget.md)|尚未记录|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.enrollmentConfigurationAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



