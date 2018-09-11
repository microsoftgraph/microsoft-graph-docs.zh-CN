# <a name="managedandroidlobapp-resource-type"></a>managedAndroidLobApp 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

包含托管 Android 业务线应用的属性和继承的属性。

继承自 [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 managedAndroidLobApps](../api/intune_apps_managedandroidlobapp_list.md)|[managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md) 集合|列出 [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md) 对象的属性和关系。|
|[获取 managedAndroidLobApp](../api/intune_apps_managedandroidlobapp_get.md)|[managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md)|读取 [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md) 对象的属性和关系。|
|[创建 managedAndroidLobApp](../api/intune_apps_managedandroidlobapp_create.md)|[managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md)|创建新的 [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md) 对象。|
|[删除 managedAndroidLobApp](../api/intune_apps_managedandroidlobapp_delete.md)|无|删除 [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md)。|
|[更新 managedAndroidLobApp](../api/intune_apps_managedandroidlobapp_update.md)|[managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md)|更新 [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|ID|字符串|实体的键。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|displayName|字符串|管理员提供或导入的应用标题。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|描述|字符串|应用的说明。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|发布服务器|字符串|应用的发布者。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|largeIcon|[mimeContent](../resources/intune_shared_mimecontent.md)|要显示在应用详细信息中并用于图标上传的大图标。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|createdDateTime|DateTimeOffset|创建应用的日期和时间。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改应用的日期和时间。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|isFeatured|布尔|指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|privacyInformationUrl|字符串|隐私声明 Url。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|informationUrl|字符串|详细信息 Url。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|所有者|字符串|应用的所有者。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|开发者|字符串|应用的开发者。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|备注|字符串|应用的备注。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|publishingState|[mobileAppPublishingState](../resources/intune_apps_mobileapppublishingstate.md)|应用的发布时间。除非应用已发布，否则不能被分配。继承自 [mobileApp](../resources/intune_apps_mobileapp.md)。可取值为：`notPublished`、`processing`、`published`。|
|appAvailability|[managedAppAvailability](../resources/intune_apps_managedappavailability.md)|应用程序的可用性。继承自 [managedApp](../resources/intune_apps_managedapp.md)。可取值为：`global`、`lineOfBusiness`。|
|version|字符串|应用程序的版本。 继承自 [managedApp](../resources/intune_apps_managedapp.md)|
|committedContentVersion|字符串|内部提交的内容版本。 继承自 [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)|
|fileName|字符串|主 Lob 应用程序文件的名称。 继承自 [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)|
|大小|Int64|总大小，包括所有已上传文件。 继承自 [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)|
|packageId|字符串|包标识符。|
|minimumSupportedOperatingSystem|[androidMinimumOperatingSystem](../resources/intune_apps_androidminimumoperatingsystem.md)|最低适用操作系统的值。|
|versionName|字符串|托管 Android 业务线 (LoB) 应用的版本名称。|
|versionCode|字符串|托管 Android 业务线 (LoB) 应用的版本代码。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|分类|[mobileAppCategory](../resources/intune_apps_mobileappcategory.md) 集合|此应用的类别列表。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|工作分配|[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) 集合|此移动应用的组分配的列表。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|contentVersions|[mobileAppContent](../resources/intune_apps_mobileappcontent.md) 集合|此应用的内容版本列表。 继承自 [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.managedMobileLobApp",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAndroidLobApp"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
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
  "committedContentVersion": "String",
  "fileName": "String",
  "size": 1024,
  "packageId": "String",
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
  },
  "versionName": "String",
  "versionCode": "String"
}
```








