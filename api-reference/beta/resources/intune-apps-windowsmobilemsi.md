---
title: windowsMobileMSI 资源类型
description: 包含 Windows Mobile MSI 业务线应用的属性和继承的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c26a47fddba04e55e2391a710f9cd5bd82a0e836
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2022
ms.locfileid: "66667137"
---
# <a name="windowsmobilemsi-resource-type"></a>windowsMobileMSI 资源类型

命名空间：microsoft.graph

> **重要：** /beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产用途。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含 Windows Mobile MSI 业务线应用的属性和继承的属性。


继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List windowsMobileMSIs](../api/intune-apps-windowsmobilemsi-list.md)|[windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) 集合|列出 [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) 对象的属性和关系。|
|[Get windowsMobileMSI](../api/intune-apps-windowsmobilemsi-get.md)|[windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md)|读取 [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) 对象的属性和关系。|
|[Create windowsMobileMSI](../api/intune-apps-windowsmobilemsi-create.md)|[windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md)|创建新的 [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) 对象。|
|[Delete windowsMobileMSI](../api/intune-apps-windowsmobilemsi-delete.md)|无|删除 [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md)。|
|[Update windowsMobileMSI](../api/intune-apps-windowsmobilemsi-update.md)|[windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md)|更新 [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|displayName|字符串|管理员提供或导入的应用标题。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|说明|String|应用的说明。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
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
|committedContentVersion|String|内部提交的内容版本。 继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)|
|fileName|String|主 Lob 应用程序文件的名称。 继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)|
|size|Int64|总大小，包括所有已上传文件。 继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)|
|commandLine|String|命令行。|
|productCode|String|产品代码。|
|productVersion|String|Windows Mobile MSI 业务线 (LoB) 应用的产品版本。|
|ignoreVersionDetection|Boolean|控制应用的版本是否将用于检测安装在设备上的应用的布尔值。 对于使用自更新功能的 Windows Mobile MSI 业务线 (LoB) 应用，将此值设置为 true。|
|identityVersion|String|标识版本。|
|useDeviceContext|布尔值|指示是否在设备上下文中安装双模式 MSI。 如果为 true，则将为所有用户安装应用。 如果为 false，则将按用户安装应用。 如果为 null，则服务将使用 MSI 包的默认安装上下文。 如果使用双模式 MSI，则此默认值为每用户。  无法为非双模式应用设置。  在初始创建应用程序后无法更改。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|categories|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 集合|此应用的类别列表。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|assignments|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 集合|此移动应用的组分配的列表。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|移动应用安装摘要。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|deviceStatuses|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) 集合|此移动应用的安装状态列表。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|userStatuses|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) 集合|此移动应用的安装状态列表。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|关系|[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) 集合|此应用的直接关系集。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|contentVersions|[mobileAppContent](../resources/intune-apps-mobileappcontent.md) 集合|此应用的内容版本列表。 继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsMobileMSI"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
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
  "committedContentVersion": "String",
  "fileName": "String",
  "size": 1024,
  "commandLine": "String",
  "productCode": "String",
  "productVersion": "String",
  "ignoreVersionDetection": true,
  "identityVersion": "String",
  "useDeviceContext": true
}
```




