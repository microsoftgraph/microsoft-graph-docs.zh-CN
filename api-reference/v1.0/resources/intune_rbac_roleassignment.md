# <a name="roleassignment-resource-type"></a>roleAssignment 资源类型

> **注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

角色分配资源。 角色分配将角色定义与成员和作用域绑定在一起。 每个角色可以具有一个或多个角色分配。 这适用于自定义和内置角色。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List roleAssignments](../api/intune_rbac_roleassignment_list.md)|[roleAssignment](../resources/intune_rbac_roleassignment.md) 集合|列出 [roleAssignment](../resources/intune_rbac_roleassignment.md) 对象的属性和关系。|
|[Get roleAssignment](../api/intune_rbac_roleassignment_get.md)|[roleAssignment](../resources/intune_rbac_roleassignment.md)|读取 [roleAssignment](../resources/intune_rbac_roleassignment.md) 对象的属性和关系。|
|[Create roleAssignment](../api/intune_rbac_roleassignment_create.md)|[roleAssignment](../resources/intune_rbac_roleassignment.md)|创建新的 [roleAssignment](../resources/intune_rbac_roleassignment.md) 对象。|
|[Delete roleAssignment](../api/intune_rbac_roleassignment_delete.md)|无|删除 [roleAssignment](../resources/intune_rbac_roleassignment.md)。|
|[Update roleAssignment](../api/intune_rbac_roleassignment_update.md)|[roleAssignment](../resources/intune_rbac_roleassignment.md)|更新 [roleAssignment](../resources/intune_rbac_roleassignment.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 此为只读，且自动生成。|
|displayName|String|角色分配的显示或友好名称。|
|description|String|角色分配的说明。|
|resourceScopes|String 集合|角色作用域成员安全组的 ID 列表。  这些是 Azure Active Directory 中的 ID。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|roleDefinition|[roleDefinition](../resources/intune_rbac_roledefinition.md)|此分配所属的角色定义。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "resourceScopes": [
    "String"
  ]
}
```



