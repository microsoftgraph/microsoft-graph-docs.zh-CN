---
title: windowsUniversalAppX 资源类型
description: 包含 Windows Universal AppX 业务线应用的属性和继承的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f325561eccb26daea409568447adf067f38b28bd22b7cb1a27685ae9a47a44e6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54243481"
---
# <a name="windowsuniversalappx-resource-type"></a>windowsUniversalAppX 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含 Windows Universal AppX 业务线应用的属性和继承的属性。


继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List windowsUniversalAppXs](../api/intune-apps-windowsuniversalappx-list.md)|[windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) 集合|列出 [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) 对象的属性和关系。|
|[Get windowsUniversalAppX](../api/intune-apps-windowsuniversalappx-get.md)|[windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md)|读取 [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) 对象的属性和关系。|
|[Create windowsUniversalAppX](../api/intune-apps-windowsuniversalappx-create.md)|[windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md)|创建新的 [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) 对象。|
|[Delete windowsUniversalAppX](../api/intune-apps-windowsuniversalappx-delete.md)|无|删除 [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md)。|
|[Update windowsUniversalAppX](../api/intune-apps-windowsuniversalappx-update.md)|[windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md)|更新 [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) 对象的属性。|

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
|所有者|String|应用的所有者。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|developer|String|应用的开发者。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|notes|String|应用的备注。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|应用的发布状态。 除非应用已发布，否则无法分配应用。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)。 可取值为：`notPublished`、`processing`、`published`。|
|committedContentVersion|String|内部提交的内容版本。 继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)|
|fileName|String|主 Lob 应用程序文件的名称。 继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)|
|size|Int64|总大小，包括所有已上传文件。 继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)|
|applicableArchitectures|[windowsArchitecture](../resources/intune-apps-windowsarchitecture.md)|可运行此应用的 Windows 体系结构。 可取值为：`none`、`x86`、`x64`、`arm`、`neutral`。|
|applicableDeviceTypes|[windowsDeviceType](../resources/intune-apps-windowsdevicetype.md)|可运行此应用的 Windows 设备类型。 可取值为：`none`、`desktop`、`mobile`、`holographic`、`team`。|
|identityName|String|标识名称。|
|identityPublisherHash|String|标识发布者哈希。|
|identityResourceIdentifier|String|标识资源标识符。|
|isBundle|Boolean|应用是否为捆绑包。|
|minimumSupportedOperatingSystem|[windowsMinimumOperatingSystem](../resources/intune-apps-windowsminimumoperatingsystem.md)|最低适用操作系统的值。|
|identityVersion|String|标识版本。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|categories|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 集合|此应用的类别列表。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|assignments|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 集合|此移动应用的组分配的列表。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|contentVersions|[mobileAppContent](../resources/intune-apps-mobileappcontent.md) 集合|此应用的内容版本列表。 继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUniversalAppX"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
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
  "committedContentVersion": "String",
  "fileName": "String",
  "size": 1024,
  "applicableArchitectures": "String",
  "applicableDeviceTypes": "String",
  "identityName": "String",
  "identityPublisherHash": "String",
  "identityResourceIdentifier": "String",
  "isBundle": true,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true
  },
  "identityVersion": "String"
}
```




