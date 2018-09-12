# <a name="managedebookassignment-resource-type"></a>managedEBookAssignment 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

包含用于为组分配电子书的属性。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 managedEBookAssignments](../api/intune_books_managedebookassignment_list.md)|[managedEBookAssignment](../resources/intune_books_managedebookassignment.md) 集合|列出 [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) 对象的属性和关系。|
|[获取 managedEBookAssignment](../api/intune_books_managedebookassignment_get.md)|[managedEBookAssignment](../resources/intune_books_managedebookassignment.md)|读取 [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) 对象的属性和关系。|
|[创建 managedEBookAssignment](../api/intune_books_managedebookassignment_create.md)|[managedEBookAssignment](../resources/intune_books_managedebookassignment.md)|创建新的 [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) 对象。|
|[删除 managedEBookAssignment](../api/intune_books_managedebookassignment_delete.md)|无|删除 [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)|
|[更新 managedEBookAssignment](../api/intune_books_managedebookassignment_update.md)|[managedEBookAssignment](../resources/intune_books_managedebookassignment.md)|更新 [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|ID|字符串|实体的键。|
|目标|[deviceAndAppManagementAssignmentTarget](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|电子图书的分配目标。|
|installIntent|[installIntent](../resources/intune_shared_installintent.md)|电子图书的安装意图。可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedEBookAssignment"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedEBookAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "String"
}
```








