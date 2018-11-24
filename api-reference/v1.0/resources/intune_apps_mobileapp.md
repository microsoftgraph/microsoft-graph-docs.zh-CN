# <a name="mobileapp-resource-type"></a>mobileApp 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

包含 Intune 移动应用基属性的抽象类。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List mobileApps](../api/intune_apps_mobileapp_list.md)|[mobileApp](../resources/intune_apps_mobileapp.md) 集合|列出 [mobileApp](../resources/intune_apps_mobileapp.md) 对象的属性和关系。|
|[Get mobileApp](../api/intune_apps_mobileapp_get.md)|[mobileApp](../resources/intune_apps_mobileapp.md)|读取 [mobileApp](../resources/intune_apps_mobileapp.md) 对象的属性和关系。|
|[assign 操作](../api/intune_apps_mobileapp_assign.md)|无|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|displayName|String|管理员提供或导入的应用标题。|
|description|String|应用的说明。|
|publisher|String|应用的发布者。|
|largeIcon|[mimeContent](../resources/intune_shared_mimecontent.md)|要显示在应用详细信息中并用于图标上传的大图标。|
|createdDateTime|DateTimeOffset|创建应用的日期和时间。|
|lastModifiedDateTime|DateTimeOffset|上次修改应用的日期和时间。|
|isFeatured|Boolean|指示应用是否被管理员标记为特色的值。|
|privacyInformationUrl|String|隐私声明 Url。|
|informationUrl|String|详细信息 Url。|
|owner|String|应用的所有者。|
|developer|String|应用的开发者。|
|notes|String|应用的备注。|
|publishingState|[mobileAppPublishingState](../resources/intune_apps_mobileapppublishingstate.md)|应用的发布状态。 除非应用已发布，否则无法分配应用。 可取值为：`notPublished`、`processing`、`published`。|

## <a name="relationships"></a>Relationships
|关系|类型|说明|
|:---|:---|:---|
|categories|[mobileAppCategory](../resources/intune_apps_mobileappcategory.md) 集合|此应用的类别列表。|
|assignments|[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) 集合|此移动应用的组分配列表。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileApp",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "isFeatured": true,
  "privacyInformationUrl": "String",
  "informationUrl": "String",
  "owner": "String",
  "developer": "String",
  "notes": "String",
  "publishingState": "String"
}
```



