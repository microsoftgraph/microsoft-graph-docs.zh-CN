# <a name="managedandroidstoreapp-resource-type"></a>managedAndroidStoreApp 资源类型

> **注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

包含可以使用 Intune 应用保护策略管理的 Android 应用商店应用的属性和继承的属性。

继承自 [managedApp](../resources/intune_apps_managedapp.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List managedAndroidStoreApps](../api/intune_apps_managedandroidstoreapp_list.md)|[managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md) 集合|列出 [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md) 对象的属性和关系。|
|[Get managedAndroidStoreApp](../api/intune_apps_managedandroidstoreapp_get.md)|[managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md)|读取 [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md) 对象的属性和关系。|
|[Create managedAndroidStoreApp](../api/intune_apps_managedandroidstoreapp_create.md)|[managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md)|创建新的 [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md) 对象。|
|[Delete managedAndroidStoreApp](../api/intune_apps_managedandroidstoreapp_delete.md)|无|删除 [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md)。|
|[Update managedAndroidStoreApp](../api/intune_apps_managedandroidstoreapp_update.md)|[managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md)|更新 [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|displayName|String|管理员提供或导入的应用标题。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|description|String|应用的说明。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|publisher|String|应用的发布者。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|largeIcon|[mimeContent](../resources/intune_apps_mimecontent.md)|要显示在应用详细信息中或用于图标上传的大图标。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|createdDateTime|DateTimeOffset|创建应用的日期和时间。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改应用的日期和时间。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|isFeatured|Boolean|指示应用是否被管理员标记为特色的值 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|privacyInformationUrl|String|隐私声明 Url。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|informationUrl|String|详细信息 Url。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|owner|String|应用的所有者。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|developer|String|应用的开发者。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|notes|String|应用的备注。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|publishingState|String|应用的发布状态。 除非应用已发布，否则无法分配应用。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md) 可取值为：`notPublished`、`processing`、`published`。|
|appAvailability|String|应用程序的可用性。 继承自 [managedApp](../resources/intune_apps_managedapp.md) 可取值为：`global`、`lineOfBusiness`。|
|version|String|应用程序的版本。 继承自 [managedApp](../resources/intune_apps_managedapp.md)|
|packageId|String|该应用的包 ID。|
|appStoreUrl|String|Android AppStoreUrl。|
|minimumSupportedOperatingSystem|[androidMinimumOperatingSystem](../resources/intune_apps_androidminimumoperatingsystem.md)|最低受支持操作系统的值。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|categories|[mobileAppCategory](../resources/intune_apps_mobileappcategory.md) 集合|此应用的类别列表。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|assignments|[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) 集合|此移动应用的组分配的列表。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAndroidStoreApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
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
  "appAvailability": "String",
  "version": "String",
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



