# <a name="termsandconditionsassignment-resource-type"></a>termsAndConditionsAssignment 资源类型

> **注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

termsAndConditionsAssignment 实体表示对给定组的给定条款和条件 (T & C) 策略的分配。 组中的用户需要接受这些条款，才能将设备注册到 Intune。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List termsAndConditionsAssignments](../api/intune_companyterms_termsandconditionsassignment_list.md)|[termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md) 集合|列出 [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md) 对象的属性和关系。|
|[Get termsAndConditionsAssignment](../api/intune_companyterms_termsandconditionsassignment_get.md)|[termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md)|读取 [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md) 对象的属性和关系。|
|[Create termsAndConditionsAssignment](../api/intune_companyterms_termsandconditionsassignment_create.md)|[termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md)|创建新的 [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md) 对象。|
|[Delete termsAndConditionsAssignment](../api/intune_companyterms_termsandconditionsassignment_delete.md)|无|删除 [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md).|
|[Update termsAndConditionsAssignment](../api/intune_companyterms_termsandconditionsassignment_update.md)|[termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md)|更新 [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的唯一标识符。|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune_companyterms_deviceandappmanagementassignmenttarget.md)|将 T&C 策略分配到的分配目标。|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditionsAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



