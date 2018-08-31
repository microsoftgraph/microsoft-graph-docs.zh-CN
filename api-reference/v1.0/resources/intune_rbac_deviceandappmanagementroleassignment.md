# <a name="deviceandappmanagementroleassignment-resource-type"></a>deviceAndAppManagementRoleAssignment 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

角色分配资源。 角色分配将角色定义与成员和作用域绑定在一起。 每个角色可以具有一个或多个角色分配。 这适用于自定义和内置角色。

继承自 [roleAssignment](../resources/intune_rbac_roleassignment.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceAndAppManagementRoleAssignments](../api/intune_rbac_deviceandappmanagementroleassignment_list.md)|[deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) 集合|列出 [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) 对象的属性和关系。|
|[获取 deviceAndAppManagementRoleAssignment](../api/intune_rbac_deviceandappmanagementroleassignment_get.md)|[deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md)|读取 [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) 对象的属性和关系。|
|[创建 deviceAndAppManagementRoleAssignment](../api/intune_rbac_deviceandappmanagementroleassignment_create.md)|[deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md)|创建新的 [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) 对象。|
|[删除 deviceAndAppManagementRoleAssignment](../api/intune_rbac_deviceandappmanagementroleassignment_delete.md)|无|删除 [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md)。|
|[更新 deviceAndAppManagementRoleAssignment](../api/intune_rbac_deviceandappmanagementroleassignment_update.md)|[deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md)|更新 [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|ID|字符串|实体的键。 此为只读，且自动生成。 继承自 [roleAssignment](../resources/intune_rbac_roleassignment.md)|
|displayName|字符串|角色分配的显示或友好名称。 继承自 [roleAssignment](../resources/intune_rbac_roleassignment.md)|
|说明|字符串|角色分配的说明。 继承自 [roleAssignment](../resources/intune_rbac_roleassignment.md)|
|resourceScopes|String 集合|角色作用域成员安全组的 ID 列表。  这些是 Azure Active Directory 中的 ID。 继承自 [roleAssignment](../resources/intune_rbac_roleassignment.md)|
|成员|String 集合|角色成员安全组的 ID 列表。 这些是 Azure Active Directory 中的 ID。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|roleDefinition|[roleDefinition](../resources/intune_rbac_roledefinition.md)|此分配所属的角色定义。 继承自 [roleAssignment](../resources/intune_rbac_roleassignment.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.roleAssignment",
  "@odata.type": "microsoft.graph.deviceAndAppManagementRoleAssignment"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "resourceScopes": [
    "String"
  ],
  "members": [
    "String"
  ]
}
```



