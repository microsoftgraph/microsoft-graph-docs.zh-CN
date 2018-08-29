# <a name="mobileappassignment-resource-type"></a>mobileAppAssignment 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

包含用于移动应用的组分配的属性的类。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 mobileAppAssignments](../api/intune_apps_mobileappassignment_list.md)|[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) 集合|列出 [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) 对象的属性和关系。|
|[获取 mobileAppAssignment](../api/intune_apps_mobileappassignment_get.md)|[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)|读取 [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) 对象的属性和关系。|
|[创建 mobileAppAssignment](../api/intune_apps_mobileappassignment_create.md)|[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)|创建新的 [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) 对象。|
|[删除 mobileAppAssignment](../api/intune_apps_mobileappassignment_delete.md)|无|删除 [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)|
|[更新 mobileAppAssignment](../api/intune_apps_mobileappassignment_update.md)|[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)|更新 [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|实体的键。|
|intent|[installIntent](../resources/intune_shared_installintent.md)|由管理员定义的安装用途。可能的值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|由管理员定义的目标组分配。|
|settings|[mobileAppAssignmentSettings](../resources/intune_apps_mobileappassignmentsettings.md)|由管理员定义的目标分配的设置。|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.mobileAppAssignment"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "id": "String (identifier)",
  "intent": "String",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  }
}
```



