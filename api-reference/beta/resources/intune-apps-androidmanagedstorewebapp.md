---
title: androidManagedStoreWebApp 资源类型
description: 包含配置为通过托管 Android 应用商店分发的 Web 应用的属性和继承属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 75729e972cd08b9c61d9992e7c46dfe2d99200e5
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2022
ms.locfileid: "66669362"
---
# <a name="androidmanagedstorewebapp-resource-type"></a>androidManagedStoreWebApp 资源类型

命名空间：microsoft.graph

> **重要：** /beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产用途。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含配置为通过托管 Android 应用商店分发的 Web 应用的属性和继承属性。


继承自 [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 androidManagedStoreWebApps](../api/intune-apps-androidmanagedstorewebapp-list.md)|[androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) 集合|列出 [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) 对象的属性和关系。|
|[获取 androidManagedStoreWebApp](../api/intune-apps-androidmanagedstorewebapp-get.md)|[androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md)|读取 [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) 对象的属性和关系。|
|[创建 androidManagedStoreWebApp](../api/intune-apps-androidmanagedstorewebapp-create.md)|[androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md)|创建新的 [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) 对象。|
|[删除 androidManagedStoreWebApp](../api/intune-apps-androidmanagedstorewebapp-delete.md)|None|删除 [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md)。|
|[更新 androidManagedStoreWebApp](../api/intune-apps-androidmanagedstorewebapp-update.md)|[androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md)|更新 [androidManagedStoreWebApp 对象的](../resources/intune-apps-androidmanagedstorewebapp.md) 属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|displayName|字符串|管理员提供或导入的应用标题。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|说明|字符串|应用的说明。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|publisher|String|应用的发布者。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|largeIcon|[mimeContent](../resources/intune-shared-mimecontent.md)|要显示在应用详细信息中并用于图标上传的大图标。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|createdDateTime|DateTimeOffset|创建应用的日期和时间。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改应用的日期和时间。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|isFeatured|Boolean|指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|privacyInformationUrl|String|隐私声明 URL。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|informationUrl|String|详细信息 URL。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|所有者|String|应用的所有者。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|developer|String|应用的开发者。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|notes|String|应用的备注。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|uploadState|Int32|上传状态。 可能的值为： 0 - `Not Ready`， 1 - `Ready`， 2 - . `Processing` 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|应用的发布状态。 除非应用已发布，否则无法分配应用。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)。 可取值为：`notPublished`、`processing`、`published`。|
|isAssigned|Boolean|指示是否将应用分配给至少一个组的值。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|roleScopeTagIds|字符串集合|此移动应用的范围标记 ID 列表。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|dependentAppCount|Int32|子应用的依赖项总数。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|supersedingAppCount|Int32|此应用直接或间接取代的应用总数。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|supersededAppCount|Int32|此应用被直接或间接取代的应用总数。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|packageId|String|包标识符。 继承自 [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)|
|appIdentifier|String|标识名称。 继承自 [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)|
|usedLicenseCount|Int32|使用中的 VPP 许可证数量。 继承自 [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)|
|totalLicenseCount|Int32|VPP 许可证的总数。 继承自 [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)|
|appStoreUrl|String|Play for Work Store 应用 URL。 继承自 [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)|
|isPrivate|布尔|指示应用是否仅适用于给定企业的用户。 继承自 [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)|
|isSystemApp|布尔|指示应用是否为预安装的系统应用。 继承自 [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)|
|appTracks|[androidManagedStoreAppTrack](../resources/intune-apps-androidmanagedstoreapptrack.md) 集合|此企业可见的轨道。 继承自 [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)|
|supportsOemConfig|布尔|此应用是否支持 OEMConfig 策略。 继承自 [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|categories|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 集合|此应用的类别列表。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|assignments|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 集合|此移动应用的组分配的列表。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|移动应用安装摘要。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|deviceStatuses|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) 集合|此移动应用的安装状态列表。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|userStatuses|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) 集合|此移动应用的安装状态列表。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|关系|[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) 集合|此应用的直接关系集。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidManagedStoreWebApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreWebApp",
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
  "dependentAppCount": 1024,
  "supersedingAppCount": 1024,
  "supersededAppCount": 1024,
  "packageId": "String",
  "appIdentifier": "String",
  "usedLicenseCount": 1024,
  "totalLicenseCount": 1024,
  "appStoreUrl": "String",
  "isPrivate": true,
  "isSystemApp": true,
  "appTracks": [
    {
      "@odata.type": "microsoft.graph.androidManagedStoreAppTrack",
      "trackId": "String",
      "trackAlias": "String"
    }
  ],
  "supportsOemConfig": true
}
```




