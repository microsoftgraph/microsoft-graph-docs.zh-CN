---
title: macOSLobApp 资源类型
description: MacOS LOB 应用程序中包含的属性和继承的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f6a9f76cfe32261cb01d286ef0bc0f898d04943a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402844"
---
# <a name="macoslobapp-resource-type"></a>macOSLobApp 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

MacOS LOB 应用程序中包含的属性和继承的属性。


继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 macOSLobApps](../api/intune-apps-macoslobapp-list.md)|[macOSLobApp](../resources/intune-apps-macoslobapp.md)集合|列出属性和[macOSLobApp](../resources/intune-apps-macoslobapp.md)对象之间的关系。|
|[获取 macOSLobApp](../api/intune-apps-macoslobapp-get.md)|[macOSLobApp](../resources/intune-apps-macoslobapp.md)|读取属性和[macOSLobApp](../resources/intune-apps-macoslobapp.md)对象的关系。|
|[创建 macOSLobApp](../api/intune-apps-macoslobapp-create.md)|[macOSLobApp](../resources/intune-apps-macoslobapp.md)|创建新的[macOSLobApp](../resources/intune-apps-macoslobapp.md)对象。|
|[删除 macOSLobApp](../api/intune-apps-macoslobapp-delete.md)|无|删除[macOSLobApp](../resources/intune-apps-macoslobapp.md)。|
|[更新 macOSLobApp](../api/intune-apps-macoslobapp-update.md)|[macOSLobApp](../resources/intune-apps-macoslobapp.md)|更新[macOSLobApp](../resources/intune-apps-macoslobapp.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|displayName|String|管理员提供或导入的应用标题。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|description|String|应用的说明。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|publisher|String|应用的发布者。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|largeIcon|[mimeContent](../resources/intune-shared-mimecontent.md)|要显示在应用详细信息中并用于图标上传的大图标。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|createdDateTime|DateTimeOffset|创建应用的日期和时间。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改应用的日期和时间。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|isFeatured|Boolean|指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|privacyInformationUrl|String|隐私声明 Url。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|informationUrl|String|详细信息 Url。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|owner|String|应用的所有者。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|developer|String|应用的开发者。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|notes|String|应用的备注。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|uploadState|Int32|上载状态。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|应用的发布状态。 除非应用已发布，否则无法分配应用。 继承自[mobileApp](../resources/intune-apps-mobileapp.md)。 可取值为：`notPublished`、`processing`、`published`。|
|isAssigned|Boolean|值，指示是否将应用程序分配给至少一个组。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|roleScopeTagIds|String 集合|此移动应用程序的作用域标记 id 的列表。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|committedContentVersion|String|内部提交的内容版本。 继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)|
|fileName|String|主 Lob 应用程序文件的名称。 继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)|
|size|Int64|总大小，包括所有已上传文件。 继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)|
|bundleId|String|绑定 id。|
|minimumSupportedOperatingSystem|[macOSMinimumOperatingSystem](../resources/intune-apps-macosminimumoperatingsystem.md)|最低适用操作系统的值。|
|buildNumber|String|MacOS 行业务 (LoB) 应用程序的内部版本号。|
|versionNumber|String|MacOS 线 (LoB) 企业应用程序的版本号。|
|childApps|[macOSLobChildApp](../resources/intune-apps-macoslobchildapp.md)集合|此绑定程序包中应用程序列表|
|identityVersion|String|标识版本。|
|md5HashChunkSize|Int32|MD5 哈希块区大小|
|md5Hash|String 集合|MD5 哈希代码|
|ignoreVersionDetection|Boolean|控制应用的版本是否将用于检测安装在设备上的应用的布尔值。 将其设置为 true macOS 使用自我更新功能的业务线 (LoB) 应用程序。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|categories|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 集合|此应用的类别列表。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|assignments|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 集合|此移动应用的组分配的列表。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|移动应用安装摘要。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|deviceStatuses|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)集合|此移动应用程序的安装状态的列表。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|userStatuses|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)集合|此移动应用程序的安装状态的列表。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|contentVersions|[mobileAppContent](../resources/intune-apps-mobileappcontent.md) 集合|此应用的内容版本列表。 继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.macOSLobApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSLobApp",
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
  "uploadState": 1024,
  "publishingState": "String",
  "isAssigned": true,
  "roleScopeTagIds": [
    "String"
  ],
  "committedContentVersion": "String",
  "fileName": "String",
  "size": 1024,
  "bundleId": "String",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.macOSMinimumOperatingSystem",
    "v10_7": true,
    "v10_8": true,
    "v10_9": true,
    "v10_10": true,
    "v10_11": true,
    "v10_12": true,
    "v10_13": true
  },
  "buildNumber": "String",
  "versionNumber": "String",
  "childApps": [
    {
      "@odata.type": "microsoft.graph.macOSLobChildApp",
      "bundleId": "String",
      "buildNumber": "String",
      "versionNumber": "String"
    }
  ],
  "identityVersion": "String",
  "md5HashChunkSize": 1024,
  "md5Hash": [
    "String"
  ],
  "ignoreVersionDetection": true
}
```




