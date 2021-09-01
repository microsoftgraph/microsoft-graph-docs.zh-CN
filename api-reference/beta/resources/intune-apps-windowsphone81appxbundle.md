---
title: windowsPhone81AppXBundle 资源类型
description: 包含 8.1 AppX 捆绑Windows Phone应用的属性和继承的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 985fed8214f31651b3daa592adee7ec5945a129c
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58783972"
---
# <a name="windowsphone81appxbundle-resource-type"></a>windowsPhone81AppXBundle 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含 8.1 AppX 捆绑Windows Phone应用的属性和继承的属性。


继承自 [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 windowsPhone81AppXBundles](../api/intune-apps-windowsphone81appxbundle-list.md)|[windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) 集合|列出 [windowsPhone81AppXBundle 对象的属性和](../resources/intune-apps-windowsphone81appxbundle.md) 关系。|
|[获取 windowsPhone81AppXBundle](../api/intune-apps-windowsphone81appxbundle-get.md)|[windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md)|读取 [windowsPhone81AppXBundle 对象的属性和](../resources/intune-apps-windowsphone81appxbundle.md) 关系。|
|[创建 windowsPhone81AppXBundle](../api/intune-apps-windowsphone81appxbundle-create.md)|[windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md)|创建新的 [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) 对象。|
|[删除 windowsPhone81AppXBundle](../api/intune-apps-windowsphone81appxbundle-delete.md)|无|删除 [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md)。|
|[更新 windowsPhone81AppXBundle](../api/intune-apps-windowsphone81appxbundle-update.md)|[windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md)|更新 [windowsPhone81AppXBundle 对象](../resources/intune-apps-windowsphone81appxbundle.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [mobileApp](../resources/intune-shared-mobileapp.md)|
|displayName|字符串|管理员提供或导入的应用标题。 继承自 [mobileApp](../resources/intune-shared-mobileapp.md)|
|description|字符串|应用的说明。 继承自 [mobileApp](../resources/intune-shared-mobileapp.md)|
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
|committedContentVersion|String|内部提交的内容版本。 继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)|
|fileName|String|主 Lob 应用程序文件的名称。 继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)|
|size|Int64|总大小，包括所有已上传文件。 继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)|
|applicableArchitectures|[windowsArchitecture](../resources/intune-apps-windowsarchitecture.md)|可运行此应用的 Windows 体系结构。 继承自 [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)。 可取值为：`none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。|
|identityName|String|标识名称。 继承自 [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)|
|identityPublisherHash|String|标识发布者哈希。 继承自 [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)|
|identityResourceIdentifier|String|标识资源标识符。 继承自 [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)|
|minimumSupportedOperatingSystem|[windowsMinimumOperatingSystem](../resources/intune-apps-windowsminimumoperatingsystem.md)|最低适用操作系统的值。 继承自 [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)|
|phoneProductIdentifier|字符串|产品电话标识符。 继承自 [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)|
|phonePublisherId|String|The 电话 Publisher Id. Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)|
|identityVersion|String|标识版本。 继承自 [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)|
|appXPackageInformationList|[windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md) 集合|AppX 程序包信息的列表。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|categories|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 集合|此应用的类别列表。 继承自 [mobileApp](../resources/intune-shared-mobileapp.md)|
|assignments|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 集合|此移动应用的组分配的列表。 继承自 [mobileApp](../resources/intune-shared-mobileapp.md)|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|移动应用安装摘要。 继承自 [mobileApp](../resources/intune-shared-mobileapp.md)|
|deviceStatuses|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) 集合|此移动应用的安装状态列表。 继承自 [mobileApp](../resources/intune-shared-mobileapp.md)|
|userStatuses|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) 集合|此移动应用的安装状态列表。 继承自 [mobileApp](../resources/intune-shared-mobileapp.md)|
|relationships|[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) 集合|此应用的直接关系集。 继承自 [mobileApp](../resources/intune-shared-mobileapp.md)|
|contentVersions|[mobileAppContent](../resources/intune-apps-mobileappcontent.md) 集合|此应用的内容版本列表。 继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsPhone81AppXBundle"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsPhone81AppXBundle",
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
  "applicableArchitectures": "String",
  "identityName": "String",
  "identityPublisherHash": "String",
  "identityResourceIdentifier": "String",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true,
    "v10_1909": true,
    "v10_2004": true,
    "v10_2H20": true,
    "v10_21H1": true
  },
  "phoneProductIdentifier": "String",
  "phonePublisherId": "String",
  "identityVersion": "String",
  "appXPackageInformationList": [
    {
      "@odata.type": "microsoft.graph.windowsPackageInformation",
      "applicableArchitecture": "String",
      "displayName": "String",
      "identityName": "String",
      "identityPublisher": "String",
      "identityResourceIdentifier": "String",
      "identityVersion": "String",
      "minimumSupportedOperatingSystem": {
        "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
        "v8_0": true,
        "v8_1": true,
        "v10_0": true,
        "v10_1607": true,
        "v10_1703": true,
        "v10_1709": true,
        "v10_1803": true,
        "v10_1809": true,
        "v10_1903": true,
        "v10_1909": true,
        "v10_2004": true,
        "v10_2H20": true,
        "v10_21H1": true
      }
    }
  ]
}
```



