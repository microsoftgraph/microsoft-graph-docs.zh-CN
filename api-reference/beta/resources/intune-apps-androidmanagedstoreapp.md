---
title: androidManagedStoreApp 资源类型
description: 包含 Android 托管应用商店应用的属性和继承的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bc47e549e8c4915d09d5fd2b9609f29b92bf6130
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58803817"
---
# <a name="androidmanagedstoreapp-resource-type"></a>androidManagedStoreApp 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含 Android 托管应用商店应用的属性和继承的属性。


继承自 [mobileApp](../resources/intune-shared-mobileapp.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 androidManagedStoreApps](../api/intune-apps-androidmanagedstoreapp-list.md)|[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) 集合|列出 [androidManagedStoreApp 对象的属性和](../resources/intune-apps-androidmanagedstoreapp.md) 关系。|
|[获取 androidManagedStoreApp](../api/intune-apps-androidmanagedstoreapp-get.md)|[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)|读取 [androidManagedStoreApp 对象的属性和](../resources/intune-apps-androidmanagedstoreapp.md) 关系。|
|[创建 androidManagedStoreApp](../api/intune-apps-androidmanagedstoreapp-create.md)|[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)|创建新的 [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) 对象。|
|[删除 androidManagedStoreApp](../api/intune-apps-androidmanagedstoreapp-delete.md)|无|删除 [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)。|
|[更新 androidManagedStoreApp](../api/intune-apps-androidmanagedstoreapp-update.md)|[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)|更新 [androidManagedStoreApp 对象](../resources/intune-apps-androidmanagedstoreapp.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [mobileApp](../resources/intune-shared-mobileapp.md)|
|displayName|String|管理员提供或导入的应用标题。 继承自 [mobileApp](../resources/intune-shared-mobileapp.md)|
|description|String|应用的说明。 继承自 [mobileApp](../resources/intune-shared-mobileapp.md)|
|publisher|String|应用的发布者。 继承自 [mobileApp](../resources/intune-shared-mobileapp.md)|
|largeIcon|[mimeContent](../resources/intune-shared-mimecontent.md)|要显示在应用详细信息中并用于图标上传的大图标。 继承自 [mobileApp](../resources/intune-shared-mobileapp.md)|
|createdDateTime|DateTimeOffset|创建应用的日期和时间。 继承自 [mobileApp](../resources/intune-shared-mobileapp.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改应用的日期和时间。 继承自 [mobileApp](../resources/intune-shared-mobileapp.md)|
|isFeatured|Boolean|指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)|
|privacyInformationUrl|String|隐私声明 URL。 继承自 [mobileApp](../resources/intune-shared-mobileapp.md)|
|informationUrl|String|详细信息 URL。 继承自 [mobileApp](../resources/intune-shared-mobileapp.md)|
|Owner|String|应用的所有者。 继承自 [mobileApp](../resources/intune-shared-mobileapp.md)|
|developer|String|应用的开发者。 继承自 [mobileApp](../resources/intune-shared-mobileapp.md)|
|notes|String|应用的备注。 继承自 [mobileApp](../resources/intune-shared-mobileapp.md)|
|uploadState|Int32|上载状态。 可能的值是：0 - `Not Ready` 、1 - `Ready` 、2 - `Processing` 。 继承自 [mobileApp](../resources/intune-shared-mobileapp.md)|
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|应用的发布状态。 除非应用已发布，否则无法分配应用。 继承自 [mobileApp](../resources/intune-shared-mobileapp.md)。 可取值为：`notPublished`、`processing`、`published`。|
|isAssigned|Boolean|指示是否将应用分配给至少一个组的值。 继承自 [mobileApp](../resources/intune-shared-mobileapp.md)|
|roleScopeTagIds|字符串集合|此移动应用的范围标记 ID 列表。 继承自 [mobileApp](../resources/intune-shared-mobileapp.md)|
|dependentAppCount|Int32|子应用具有的依赖项总数。 继承自 [mobileApp](../resources/intune-shared-mobileapp.md)|
|supersedingAppCount|Int32|此应用直接或间接取代的应用总数。 继承自 [mobileApp](../resources/intune-shared-mobileapp.md)|
|supersededAppCount|Int32|此应用直接或间接被取代的应用总数。 继承自 [mobileApp](../resources/intune-shared-mobileapp.md)|
|packageId|String|包标识符。|
|appIdentifier|String|标识名称。|
|usedLicenseCount|Int32|使用中的 VPP 许可证数量。|
|totalLicenseCount|Int32|VPP 许可证的总数。|
|appStoreUrl|String|"播放工作商店"应用 URL。|
|isPrivate|Boolean|指示应用是否仅适用于给定企业的用户。|
|isSystemApp|Boolean|指示应用是否是预安装的系统应用。|
|appTracks|[androidManagedStoreAppTrack](../resources/intune-apps-androidmanagedstoreapptrack.md) 集合|此企业可见的轨。|
|supportsOemConfig|Boolean|此应用是否支持 OEMConfig 策略。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|categories|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 集合|此应用的类别列表。 继承自 [mobileApp](../resources/intune-shared-mobileapp.md)|
|assignments|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 集合|此移动应用的组分配的列表。 继承自 [mobileApp](../resources/intune-shared-mobileapp.md)|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|移动应用安装摘要。 继承自 [mobileApp](../resources/intune-shared-mobileapp.md)|
|deviceStatuses|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) 集合|此移动应用的安装状态列表。 继承自 [mobileApp](../resources/intune-shared-mobileapp.md)|
|userStatuses|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) 集合|此移动应用的安装状态列表。 继承自 [mobileApp](../resources/intune-shared-mobileapp.md)|
|relationships|[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) 集合|此应用的直接关系集。 继承自 [mobileApp](../resources/intune-shared-mobileapp.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidManagedStoreApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreApp",
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



