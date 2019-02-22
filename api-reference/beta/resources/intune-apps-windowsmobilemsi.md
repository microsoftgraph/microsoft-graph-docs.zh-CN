---
title: windowsMobileMSI 资源类型
description: 包含 Windows Mobile MSI 业务线应用的属性和继承的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4072af262862a6c95b6677e2969dde2241ef1bf2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144448"
---
# <a name="windowsmobilemsi-resource-type"></a>windowsMobileMSI 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

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
|id|字串符号|实体的键。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|displayName|字符串|管理员提供或导入的应用标题。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|description|字符串|应用的说明。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|publisher|字符串|应用的发布者。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|largeIcon|[mimeContent](../resources/intune-shared-mimecontent.md)|要显示在应用详细信息中并用于图标上传的大图标。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|createdDateTime|DateTimeOffset|创建应用的日期和时间。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改应用的日期和时间。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|isFeatured|Boolean|指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|privacyInformationUrl|字符串|隐私声明 Url。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|informationUrl|字符串|详细信息 Url。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|owner|String|应用的所有者。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|developer|String|应用的开发者。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|notes|String|应用的备注。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|uploadState|Int32|上载状态。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|应用的发布状态。 除非应用已发布，否则无法分配应用。 继承自[mobileApp](../resources/intune-apps-mobileapp.md)。 可取值为：`notPublished`、`processing`、`published`。|
|isAssigned|Boolean|指示是否至少向一个组分配了应用程序的值。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|roleScopeTagIds|String collection|此移动应用的作用域标记 id 列表。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|committedContentVersion|字符串|内部提交的内容版本。 继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)|
|fileName|字符串|主 Lob 应用程序文件的名称。 继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)|
|size|Int64|总大小，包括所有已上传文件。 继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)|
|commandLine|字符串|命令行。|
|productCode|字符串|产品代码。|
|productVersion|字符串|Windows Mobile MSI 业务线 (LoB) 应用的产品版本。|
|ignoreVersionDetection|Boolean|控制应用的版本是否将用于检测安装在设备上的应用的布尔值。 对于使用自更新功能的 Windows Mobile MSI 业务线 (LoB) 应用，将此值设置为 true。|
|identityVersion|String|标识版本。|
|useDeviceContext|布尔值|指示是否在设备上下文中安装双模式 MSI。 如果为 true, 则将为所有用户安装应用程序。 如果为 false, 将按用户安装应用程序。 如果为 null, 服务将使用 MSI 包的默认安装上下文。 在双模式 MSI 的情况下, 此默认值将为每个用户。  不能为非双重模式的应用程序进行设置。  在首次创建应用程序后, 不能更改。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|categories|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 集合|此应用的类别列表。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|assignments|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 集合|此移动应用的组分配的列表。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|移动应用安装摘要。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|deviceStatuses|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)集合|此移动应用程序的安装状态列表。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|userStatuses|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)集合|此移动应用程序的安装状态列表。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
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




