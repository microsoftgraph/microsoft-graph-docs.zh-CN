# <a name="windowsuniversalappx-resource-type"></a>windowsUniversalAppX 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

包含 Windows Universal AppX 业务线应用的属性和继承的属性。

继承自 [mobileLobApp](../resources/intune_apps_mobilelobapp.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 windowsUniversalAppXs](../api/intune_apps_windowsuniversalappx_list.md)|[windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) 集合|列出 [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) 对象的属性和关系。|
|[获取 windowsUniversalAppX](../api/intune_apps_windowsuniversalappx_get.md)|[windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md)|读取 [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) 对象的属性和关系。|
|[创建 windowsUniversalAppX](../api/intune_apps_windowsuniversalappx_create.md)|[windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md)|创建新的 [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) 对象。|
|[删除 windowsUniversalAppX](../api/intune_apps_windowsuniversalappx_delete.md)|无|删除 [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md)。|
|[更新 windowsUniversalAppX](../api/intune_apps_windowsuniversalappx_update.md)|[windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md)|更新 [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|ID|字符串|实体的键。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
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
|publishingState|[mobileAppPublishingState](../resources/intune_apps_mobileapppublishingstate.md)|应用程序的发布状态。除非应用程序发布，否则无法分配应用程序。继承自 [mobileApp](../resources/intune_apps_mobileapp.md)。可能的值为：`notPublished`、`processing`、`published`。|
|committedContentVersion|字符串|内部提交的内容版本。 继承自 [mobileLobApp](../resources/intune_apps_mobilelobapp.md)|
|fileName|字符串|主 Lob 应用程序文件的名称。 继承自 [mobileLobApp](../resources/intune_apps_mobilelobapp.md)|
|size|Int64|总大小，包括所有已上传文件。 继承自 [mobileLobApp](../resources/intune_apps_mobilelobapp.md)|
|applicableArchitectures|[windowsArchitecture](../resources/intune_apps_windowsarchitecture.md)|此应用程序可以运行的 Windows 体系结构。可能的值为：`none`，`x86`，`x64`，`arm`，`neutral`。|
|applicableDeviceTypes|[windowsDeviceType](../resources/intune_apps_windowsdevicetype.md)|此应用程序可以运行的 Windows 设备类型。可能的值为：`none`，`desktop`，`mobile`，`holographic`，`team`。|
|identityName|字符串|标识名称。|
|identityPublisherHash|字符串|标识发布者哈希。|
|identityResourceIdentifier|字符串|标识资源标识符。|
|isBundle|布尔|应用是否为捆绑包。|
|minimumSupportedOperatingSystem|[windowsMinimumOperatingSystem](../resources/intune_apps_windowsminimumoperatingsystem.md)|最低适用操作系统的值。|
|identityVersion|字符串|标识版本。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|categories|[mobileAppCategory](../resources/intune_apps_mobileappcategory.md) 集合|此应用的类别列表。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|assignments|[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) 集合|此移动应用的组分配的列表。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|contentVersions|[mobileAppContent](../resources/intune_apps_mobileappcontent.md) 集合|此应用的内容版本列表。 继承自 [mobileLobApp](../resources/intune_apps_mobilelobapp.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.mobileLobApp",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUniversalAppX"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
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
  "committedContentVersion": "String",
  "fileName": "String",
  "size": 1024,
  "applicableArchitectures": "String",
  "applicableDeviceTypes": "String",
  "identityName": "String",
  "identityPublisherHash": "String",
  "identityResourceIdentifier": "String",
  "isBundle": true,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true
  },
  "identityVersion": "String"
}
```








