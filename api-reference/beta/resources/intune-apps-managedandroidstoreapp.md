---
title: managedAndroidStoreApp 资源类型
description: 包含可以使用 Intune 应用保护策略管理的 Android 应用商店应用的属性和继承的属性。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c82a50ca98d826430b95f336958b1d3570d50e34
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59057605"
---
# <a name="managedandroidstoreapp-resource-type"></a>managedAndroidStoreApp 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含可以使用 Intune 应用保护策略管理的 Android 应用商店应用的属性和继承的属性。


继承自 [managedApp](../resources/intune-apps-managedapp.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List managedAndroidStoreApps](../api/intune-apps-managedandroidstoreapp-list.md)|[managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) 集合|列出 [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) 对象的属性和关系。|
|[Get managedAndroidStoreApp](../api/intune-apps-managedandroidstoreapp-get.md)|[managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md)|读取 [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) 对象的属性和关系。|
|[Create managedAndroidStoreApp](../api/intune-apps-managedandroidstoreapp-create.md)|[managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md)|创建新的 [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) 对象。|
|[Delete managedAndroidStoreApp](../api/intune-apps-managedandroidstoreapp-delete.md)|无|删除 [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md)。|
|[Update managedAndroidStoreApp](../api/intune-apps-managedandroidstoreapp-update.md)|[managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md)|更新 [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [mobileApp](../resources/intune-shared-mobileapp.md)|
|displayName|String|管理员提供或导入的应用标题。 继承自 [mobileApp](../resources/intune-shared-mobileapp.md)|
|说明|String|应用的说明。 继承自 [mobileApp](../resources/intune-shared-mobileapp.md)|
|publisher|String|应用的发布者。 继承自 [mobileApp](../resources/intune-shared-mobileapp.md)|
|largeIcon|[mimeContent](../resources/intune-shared-mimecontent.md)|要显示在应用详细信息中并用于图标上传的大图标。 继承自 [mobileApp](../resources/intune-shared-mobileapp.md)|
|createdDateTime|DateTimeOffset|创建应用的日期和时间。 继承自 [mobileApp](../resources/intune-shared-mobileapp.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改应用的日期和时间。 继承自 [mobileApp](../resources/intune-shared-mobileapp.md)|
|isFeatured|Boolean|指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)|
|privacyInformationUrl|String|隐私声明 URL。 继承自 [mobileApp](../resources/intune-shared-mobileapp.md)|
|informationUrl|String|详细信息 URL。 继承自 [mobileApp](../resources/intune-shared-mobileapp.md)|
|owner|String|应用的所有者。 继承自 [mobileApp](../resources/intune-shared-mobileapp.md)|
|developer|String|应用的开发者。 继承自 [mobileApp](../resources/intune-shared-mobileapp.md)|
|notes|String|应用的备注。 继承自 [mobileApp](../resources/intune-shared-mobileapp.md)|
|uploadState|Int32|上载状态。 可能的值是：0 - `Not Ready` 、1 - `Ready` 、2 - `Processing` 。 继承自 [mobileApp](../resources/intune-shared-mobileapp.md)|
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|应用的发布状态。 除非应用已发布，否则无法分配应用。 继承自 [mobileApp](../resources/intune-shared-mobileapp.md)。 可取值为：`notPublished`、`processing`、`published`。|
|isAssigned|Boolean|指示是否将应用分配给至少一个组的值。 继承自 [mobileApp](../resources/intune-shared-mobileapp.md)|
|roleScopeTagIds|字符串集合|此移动应用的范围标记 ID 列表。 继承自 [mobileApp](../resources/intune-shared-mobileapp.md)|
|dependentAppCount|Int32|子应用具有的依赖项总数。 继承自 [mobileApp](../resources/intune-shared-mobileapp.md)|
|supersedingAppCount|Int32|此应用直接或间接取代的应用总数。 继承自 [mobileApp](../resources/intune-shared-mobileapp.md)|
|supersededAppCount|Int32|此应用直接或间接被取代的应用总数。 继承自 [mobileApp](../resources/intune-shared-mobileapp.md)|
|appAvailability|[managedAppAvailability](../resources/intune-apps-managedappavailability.md)|应用程序的可用性。 继承自 [managedApp](../resources/intune-apps-managedapp.md)。 可取值为：`global`、`lineOfBusiness`。|
|version|String|应用程序的版本。 继承自 [managedApp](../resources/intune-apps-managedapp.md)|
|packageId|String|应用的包 ID。|
|appStoreUrl|String|Android AppStoreUrl。|
|minimumSupportedOperatingSystem|[androidMinimumOperatingSystem](../resources/intune-apps-androidminimumoperatingsystem.md)|最低受支持操作系统的值。|

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
  "uploadState": 1024,
  "publishingState": "String",
  "isAssigned": true,
  "roleScopeTagIds": [
    "String"
  ],
  "dependentAppCount": 1024,
  "supersedingAppCount": 1024,
  "supersededAppCount": 1024,
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
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true
  }
}
```



