# <a name="devicemanagement-resource-type"></a>deviceManagement 资源类型

> **注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

充当所有设备管理功能的容器的单例实体。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 deviceManagement](../api/intune_rbac_devicemanagement_get.md)|[deviceManagement](../resources/intune_rbac_devicemanagement.md)|读取 [deviceManagement](../resources/intune_rbac_devicemanagement.md) 对象的属性和关系。|
|[更新 deviceManagement](../api/intune_rbac_devicemanagement_update.md)|[deviceManagement](../resources/intune_rbac_devicemanagement.md)|更新 [deviceManagement](../resources/intune_rbac_devicemanagement.md) 对象的属性。|
|[getEffectivePermissions 函数](../api/intune_rbac_devicemanagement_geteffectivepermissions.md)|[rolePermission](../resources/intune_rbac_rolepermission.md) 集合|检索当前验证的用户的有效权限|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|尚未记录|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|roleDefinitions|[roleDefinition](../resources/intune_rbac_roledefinition.md) 集合|角色定义。|
|roleAssignments|[deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) 集合|角色分配。|
|resourceOperations|[resourceOperation](../resources/intune_rbac_resourceoperation.md) 集合|资源操作。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)"
}
```



