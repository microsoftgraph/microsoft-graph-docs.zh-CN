---
title: managedAndroidLobApp 资源类型
description: 包含托管 Android 业务线应用的属性和继承的属性。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 89557903ce134f3fb3e612e77c49b8da2b13e81e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59113684"
---
# <a name="managedandroidlobapp-resource-type"></a>managedAndroidLobApp 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含托管 Android 业务线应用的属性和继承的属性。


继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List managedAndroidLobApps](../api/intune-apps-managedandroidlobapp-list.md)|[managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) 集合|列出 [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) 对象的属性和关系。|
|[Get managedAndroidLobApp](../api/intune-apps-managedandroidlobapp-get.md)|[managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md)|读取 [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) 对象的属性和关系。|
|[Create managedAndroidLobApp](../api/intune-apps-managedandroidlobapp-create.md)|[managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md)|创建新的 [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) 对象。|
|[Delete managedAndroidLobApp](../api/intune-apps-managedandroidlobapp-delete.md)|无|删除 [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md)。|
|[Update managedAndroidLobApp](../api/intune-apps-managedandroidlobapp-update.md)|[managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md)|更新 [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
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
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|应用的发布状态。 除非应用已发布，否则无法分配应用。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)。 可取值为：`notPublished`、`processing`、`published`。|
|appAvailability|[managedAppAvailability](../resources/intune-apps-managedappavailability.md)|应用程序的可用性。 继承自 [managedApp](../resources/intune-apps-managedapp.md)。 可取值为：`global`、`lineOfBusiness`。|
|version|String|应用程序的版本。 继承自 [managedApp](../resources/intune-apps-managedapp.md)|
|committedContentVersion|String|内部提交的内容版本。 继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)|
|fileName|String|主 Lob 应用程序文件的名称。 继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)|
|size|Int64|总大小，包括所有已上传文件。 继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)|
|packageId|String|包标识符。|
|minimumSupportedOperatingSystem|[androidMinimumOperatingSystem](../resources/intune-apps-androidminimumoperatingsystem.md)|最低适用操作系统的值。|
|versionName|String|托管 Android 业务线 (LoB) 应用的版本名称。|
|versionCode|String|托管 Android 业务线 (LoB) 应用的版本代码。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|categories|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 集合|此应用的类别列表。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|assignments|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 集合|此移动应用的组分配的列表。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|contentVersions|[mobileAppContent](../resources/intune-apps-mobileappcontent.md) 集合|此应用的内容版本列表。 继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAndroidLobApp"
}
-->
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
    "v5_1": true,
    "v10_0": true,
    "v11_0": true
  },
  "versionName": "String",
  "versionCode": "String"
}
```




