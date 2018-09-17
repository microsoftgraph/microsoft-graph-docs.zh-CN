# <a name="androidstoreapp-resource-type"></a>androidStoreApp 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

包含 Android 应用商店应用的属性和继承的属性。

继承自 [mobileApp](../resources/intune_apps_mobileapp.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 androidStoreApps](../api/intune_apps_androidstoreapp_list.md)|[androidStoreApp](../resources/intune_apps_androidstoreapp.md) 集合|列出 [androidStoreApp](../resources/intune_apps_androidstoreapp.md) 对象的属性和关系。|
|[获取 androidStoreApp](../api/intune_apps_androidstoreapp_get.md)|[androidStoreApp](../resources/intune_apps_androidstoreapp.md)|读取 [androidStoreApp](../resources/intune_apps_androidstoreapp.md) 对象的属性和关系。|
|[创建 androidStoreApp](../api/intune_apps_androidstoreapp_create.md)|[androidStoreApp](../resources/intune_apps_androidstoreapp.md)|创建新的 [androidStoreApp](../resources/intune_apps_androidstoreapp.md) 对象。|
|[删除 androidStoreApp](../api/intune_apps_androidstoreapp_delete.md)|无|删除 [androidStoreApp](../resources/intune_apps_androidstoreapp.md)。|
|[更新 androidStoreApp](../api/intune_apps_androidstoreapp_update.md)|[androidStoreApp](../resources/intune_apps_androidstoreapp.md)|更新 [androidStoreApp](../resources/intune_apps_androidstoreapp.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|ID|字符串|实体的键。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|displayName|字符串|管理员提供或导入的应用标题。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|说明|字符串|应用的说明。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|发布者|字符串|应用的发布者。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|largeIcon|[mimeContent](../resources/intune_shared_mimecontent.md)|要显示在应用详细信息中并用于图标上传的大图标。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|createdDateTime|DateTimeOffset|创建应用的日期和时间。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改应用的日期和时间。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|isFeatured|布尔|指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|privacyInformationUrl|字符串|隐私声明 Url。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|informationUrl|字符串|详细信息 Url。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|所有者|字符串|应用的所有者。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|开发者|字符串|应用的开发者。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|备注|字符串|应用的备注。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|publishingState|[mobileAppPublishingState](../resources/intune_apps_mobileapppublishingstate.md)|应用的发布状态。除非应用已发布，否则不能被分配。继承自 [mobileApp](../resources/intune_apps_mobileapp.md)。可能的值为：`notPublished`、`processing`、`published`。|
|packageId|字符串|包标识符。|
|appStoreUrl|字符串|Android 应用商店 URL。|
|minimumSupportedOperatingSystem|[androidMinimumOperatingSystem](../resources/intune_apps_androidminimumoperatingsystem.md)|最低适用操作系统的值。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|类别|[mobileAppCategory](../resources/intune_apps_mobileappcategory.md) 集合|此应用的类别列表。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|assignments|[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) 集合|此移动应用的组分配的列表。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.mobileApp",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidStoreApp"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.androidStoreApp",
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
  "publishingState": "String",
  "packageId": "String",
  "appStoreUrl": "String",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  }
}
```








