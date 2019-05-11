---
title: microsoftStoreForBusinessApp 资源类型
description: 适用于企业的 Microsoft Store 应用。 此类不支持创建、删除或更新。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8870982c1322f5ee2c14dc399020f34e2fcc0924
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950044"
---
# <a name="microsoftstoreforbusinessapp-resource-type"></a>microsoftStoreForBusinessApp 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

适用于企业的 Microsoft Store 应用。 此类不支持创建、删除或更新。


继承自 [mobileApp](../resources/intune-apps-mobileapp.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List microsoftStoreForBusinessApps](../api/intune-apps-microsoftstoreforbusinessapp-list.md)|[microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) 集合|列出 [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) 对象的属性和关系。|
|[Get microsoftStoreForBusinessApp](../api/intune-apps-microsoftstoreforbusinessapp-get.md)|[microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md)|读取 [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) 对象的属性和关系。|
|[Create microsoftStoreForBusinessApp](../api/intune-apps-microsoftstoreforbusinessapp-create.md)|[microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md)|创建新的 [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) 对象。|
|[Delete microsoftStoreForBusinessApp](../api/intune-apps-microsoftstoreforbusinessapp-delete.md)|无|删除 [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md)。|
|[Update microsoftStoreForBusinessApp](../api/intune-apps-microsoftstoreforbusinessapp-update.md)|[microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md)|更新 [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|实体的键。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|displayName|String|管理员提供或导入的应用标题。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|说明|String|应用的说明。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|publisher|String|应用的发布者。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|largeIcon|[mimeContent](../resources/intune-shared-mimecontent.md)|要显示在应用详细信息中并用于图标上传的大图标。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|createdDateTime|DateTimeOffset|创建应用的日期和时间。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改应用的日期和时间。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|isFeatured|Boolean|指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|privacyInformationUrl|String|隐私声明 URL。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|informationUrl|String|详细信息 URL。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|owner|String|应用的所有者。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|developer|String|应用的开发者。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|notes|String|应用的备注。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|uploadState|Int32|上载状态。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|应用的发布状态。 除非应用已发布，否则无法分配应用。 继承自[mobileApp](../resources/intune-apps-mobileapp.md)。 可取值为：`notPublished`、`processing`、`published`。|
|isAssigned|Boolean|指示是否至少向一个组分配了应用程序的值。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|roleScopeTagIds|String collection|此移动应用的作用域标记 id 列表。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|dependentAppCount|Int32|子应用程序的依赖项总数。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|usedLicenseCount|Int32|使用中的适用于企业的 Microsoft Store 许可证数。|
|totalLicenseCount|Int32|适用于企业的 Microsoft Store 许可证总数。|
|productKey|String|应用产品密钥|
|licenseType|[microsoftStoreForBusinessLicenseType](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|应用程序许可证类型。 可取值为：`offline`、`online`。|
|packageIdentityName|String|应用包标识符|
|licensingType|[vppLicensingType](../resources/intune-apps-vpplicensingtype.md)|受支持的许可证类型。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|categories|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 集合|此应用的类别列表。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|assignments|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 集合|此移动应用的组分配的列表。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|移动应用安装摘要。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|deviceStatuses|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)集合|此移动应用程序的安装状态列表。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|userStatuses|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)集合|此移动应用程序的安装状态列表。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|相互|[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)集合|此移动应用的关系列表。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|containedApps|[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)集合|充当包的 mobileApp 中包含的应用程序的集合。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftStoreForBusinessApp"
}
-->
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
  "uploadState": 1024,
  "publishingState": "String",
  "isAssigned": true,
  "roleScopeTagIds": [
    "String"
  ],
  "dependentAppCount": 1024,
  "usedLicenseCount": 1024,
  "totalLicenseCount": 1024,
  "productKey": "String",
  "licenseType": "String",
  "packageIdentityName": "String",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  }
}
```




