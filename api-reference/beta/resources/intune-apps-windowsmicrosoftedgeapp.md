---
title: windowsMicrosoftEdgeApp 资源类型
description: 包含 Windows 上 Microsoft Edge 应用的属性和继承属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fe513f5c01a8f7d4f31435490caa9385ed2c80ce
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2022
ms.locfileid: "66668046"
---
# <a name="windowsmicrosoftedgeapp-resource-type"></a>windowsMicrosoftEdgeApp 资源类型

命名空间：microsoft.graph

> **重要：** /beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产用途。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含 Windows 上 Microsoft Edge 应用的属性和继承属性。


继承自 [mobileApp](../resources/intune-apps-mobileapp.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 windowsMicrosoftEdgeApps](../api/intune-apps-windowsmicrosoftedgeapp-list.md)|[windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md) 集合|列出 [windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md) 对象的属性和关系。|
|[获取 windowsMicrosoftEdgeApp](../api/intune-apps-windowsmicrosoftedgeapp-get.md)|[windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md)|读取 [windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md) 对象的属性和关系。|
|[创建 windowsMicrosoftEdgeApp](../api/intune-apps-windowsmicrosoftedgeapp-create.md)|[windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md)|创建新的 [windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md) 对象。|
|[删除 windowsMicrosoftEdgeApp](../api/intune-apps-windowsmicrosoftedgeapp-delete.md)|None|删除 [windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md)。|
|[更新 windowsMicrosoftEdgeApp](../api/intune-apps-windowsmicrosoftedgeapp-update.md)|[windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md)|更新 [windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md) 对象的属性。|

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
|频道|[microsoftEdgeChannel](../resources/intune-apps-microsoftedgechannel.md)|要在目标设备上安装的通道。 可取值为：`dev`、`beta`、`stable`。|
|displayLanguageLocale|String|当 Edge 应用向用户显示文本时要使用的语言区域设置。|

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
  "@odata.type": "microsoft.graph.windowsMicrosoftEdgeApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsMicrosoftEdgeApp",
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
  "channel": "String",
  "displayLanguageLocale": "String"
}
```




