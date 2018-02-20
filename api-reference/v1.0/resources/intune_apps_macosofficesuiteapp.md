# <a name="macosofficesuiteapp-resource-type"></a>macOSOfficeSuiteApp 资源类型

> **注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

包含 MacOS Office 套件应用的属性和继承的属性。

继承自 [mobileApp](../resources/intune_apps_mobileapp.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List macOSOfficeSuiteApps](../api/intune_apps_macosofficesuiteapp_list.md)|[macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md) 集合|列出 [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md) 对象的属性和关系。|
|[Get macOSOfficeSuiteApp](../api/intune_apps_macosofficesuiteapp_get.md)|[macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md)|读取 [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md) 对象的属性和关系。|
|[Create macOSOfficeSuiteApp](../api/intune_apps_macosofficesuiteapp_create.md)|[macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md)|创建新的 [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md) 对象。|
|[Delete macOSOfficeSuiteApp](../api/intune_apps_macosofficesuiteapp_delete.md)|无|删除 [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md)。|
|[Update macOSOfficeSuiteApp](../api/intune_apps_macosofficesuiteapp_update.md)|[macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md)|更新 [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|displayName|String|管理员提供或导入的应用标题。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|description|String|应用的说明。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|publisher|String|应用的发布者。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|largeIcon|[mimeContent](../resources/intune_apps_mimecontent.md)|要显示在应用详细信息中并用于图标上传的大图标。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|createdDateTime|DateTimeOffset|创建应用的日期和时间。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改应用的日期和时间。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|isFeatured|Boolean|指示应用是否被管理员标记为特色的值 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|privacyInformationUrl|String|隐私声明 Url。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|informationUrl|String|详细信息 Url。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|owner|String|应用的所有者。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|developer|String|应用的开发者。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|notes|String|应用的备注。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|publishingState|String|应用的发布状态。 除非应用已发布，否则无法分配应用。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md) 可取值为：`notPublished`、`processing`、`published`。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|categories|[mobileAppCategory](../resources/intune_apps_mobileappcategory.md) 集合|此应用的类别列表。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|assignments|[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) 集合|此移动应用的组分配列表。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.macOSOfficeSuiteApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSOfficeSuiteApp",
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



