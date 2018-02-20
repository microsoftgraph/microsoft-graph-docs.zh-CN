# <a name="iosvppebookassignment-resource-type"></a>iosVppEBookAssignment 资源类型

> **注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

包含用于为组分配 iOS VPP 电子书的属性。

继承自 [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List iosVppEBookAssignments](../api/intune_books_iosvppebookassignment_list.md)|[iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md) 集合|列出 [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md) 对象的属性和关系。|
|[Get iosVppEBookAssignment](../api/intune_books_iosvppebookassignment_get.md)|[iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md)|读取 [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md) 对象的属性和关系。|
|[Create iosVppEBookAssignment](../api/intune_books_iosvppebookassignment_create.md)|[iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md)|创建新的 [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md) 对象。|
|[Delete iosVppEBookAssignment](../api/intune_books_iosvppebookassignment_delete.md)|无|删除 [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md)。|
|[Update iosVppEBookAssignment](../api/intune_books_iosvppebookassignment_update.md)|[iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md)|更新 [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune_books_deviceandappmanagementassignmenttarget.md)|电子书的分配目标。 继承自 [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)|
|installIntent|String|电子书的安装意向。 继承自 [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) 可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosVppEBookAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppEBookAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "String"
}
```



