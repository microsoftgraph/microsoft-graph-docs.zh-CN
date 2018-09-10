# <a name="resourceoperation-resource-type"></a>resourceOperation 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

这可以定义能够在 Intune 资源（或实体）上执行的操作或行为。  常用操作有读取、删除、更新或创建。  这些操作提供对基础 Intune 资源本身的基本管理。  某些情况下，Intune 资源可以采用资源使用的操作，以与其他资源合并采用。  例如，Assign 操作用于向 AAD 安全组分配 MobileApp 资源。  无法修改内置角色的资源操作。这会定义能够在 Intune 资源（或实体）上执行的操作或行为。  常用操作有获取、列出、删除、更新或创建。  这些操作提供对基础 Intune 资源本身的基本管理。  某些情况下，Intune 资源可以采用资源使用的操作，以与其他资源合并采用。  例如，“Assign”操作用于向 AAD 安全组分配 MobileApp 资源。  无法修改内置角色的资源操作。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列举 resourceOperations](../api/intune_rbac_resourceoperation_list.md)|[resourceOperation](../resources/intune_rbac_resourceoperation.md) 集合|列出 [resourceOperation](../resources/intune_rbac_resourceoperation.md) 对象的属性和关系。|
|[获取 resourceOperation](../api/intune_rbac_resourceoperation_get.md)|[resourceOperation](../resources/intune_rbac_resourceoperation.md)|读取 [resourceOperation](../resources/intune_rbac_resourceoperation.md) 对象的属性和关系。|
|[创建 resourceOperation](../api/intune_rbac_resourceoperation_create.md)|[resourceOperation](../resources/intune_rbac_resourceoperation.md)|创建新的 [resourceOperation](../resources/intune_rbac_resourceoperation.md) 对象。|
|[删除 resourceOperation](../api/intune_rbac_resourceoperation_delete.md)|无|删除 [resourceOperation](../resources/intune_rbac_resourceoperation.md)。|
|[更新 resourceOperation](../api/intune_rbac_resourceoperation_update.md)|[resourceOperation](../resources/intune_rbac_resourceoperation.md)|更新 [resourceOperation](../resources/intune_rbac_resourceoperation.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|ID|字符串|资源操作的键。 只读，且自动生成。|
|resourceName|字符串|执行此操作的资源的名称。|
|actionName|字符串|此操作将执行的操作类型。 actionName 应简明，并尽可能限制在几个字以内。|
|说明|字符串|资源操作的说明。 当在 Azure 门户中显示时，会在操作的鼠标悬停文本中使用说明。|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.resourceOperation"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceOperation",
  "id": "String (identifier)",
  "resourceName": "String",
  "actionName": "String",
  "description": "String"
}
```








