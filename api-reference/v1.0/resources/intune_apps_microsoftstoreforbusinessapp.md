# <a name="microsoftstoreforbusinessapp-resource-type"></a>microsoftStoreForBusinessApp 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

适用于企业的 Microsoft Store 应用。 此类不支持创建、删除或更新。

继承自 [mobileApp](../resources/intune_apps_mobileapp.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 microsoftStoreForBusinessApps](../api/intune_apps_microsoftstoreforbusinessapp_list.md)|[microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md) 集合|列出 [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md) 对象的属性和关系。|
|[获取 microsoftStoreForBusinessApp](../api/intune_apps_microsoftstoreforbusinessapp_get.md)|[microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md)|读取 [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md) 对象的属性和关系。|
|[创建 microsoftStoreForBusinessApp](../api/intune_apps_microsoftstoreforbusinessapp_create.md)|[microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md)|创建新的 [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md) 对象。|
|[删除 microsoftStoreForBusinessApp](../api/intune_apps_microsoftstoreforbusinessapp_delete.md)|无|删除 [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md)。|
|[更新 microsoftStoreForBusinessApp](../api/intune_apps_microsoftstoreforbusinessapp_update.md)|[microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md)|更新 [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|实体的键。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|displayName|字符串|管理员提供或导入的应用标题。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|description|字符串|应用的说明。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|publisher|字符串|应用的发布者。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|largeIcon|[mimeContent](../resources/intune_shared_mimecontent.md)|要显示在应用详细信息中并用于图标上传的大图标。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|createdDateTime|DateTimeOffset|创建应用的日期和时间。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改应用的日期和时间。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|isFeatured|布尔|指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|privacyInformationUrl|字符串|隐私声明 Url。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|informationUrl|字符串|详细信息 Url。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|owner|字符串|应用的所有者。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|developer|字符串|应用的开发者。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|notes|字符串|应用的备注。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|publishingState|[mobileAppPublishingState](../resources/intune_apps_mobileapppublishingstate.md)|应用的发布状态。 除非应用已发布，否则无法分配应用。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)。 可取值为：`notPublished`、`processing`、`published`。|
|usedLicenseCount|Int32|使用中的适用于企业的 Microsoft Store 许可证数。|
|totalLicenseCount|Int32|适用于企业的 Microsoft Store 许可证总数。|
|productKey|字符串|应用产品密钥|
|licenseType|[microsoftStoreForBusinessLicenseType](../resources/intune_apps_microsoftstoreforbusinesslicensetype.md)|应用许可证类型。 可取值为：`offline`、`online`。|
|packageIdentityName|字符串|应用包标识符|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|categories|[mobileAppCategory](../resources/intune_apps_mobileappcategory.md) 集合|此应用的类别列表。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|assignments|[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) 集合|此移动应用的组分配的列表。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.mobileApp",
  "@odata.type": "microsoft.graph.microsoftStoreForBusinessApp"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
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
  "usedLicenseCount": 1024,
  "totalLicenseCount": 1024,
  "productKey": "String",
  "licenseType": "String",
  "packageIdentityName": "String"
}
```



