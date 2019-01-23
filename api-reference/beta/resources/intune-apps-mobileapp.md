---
title: mobileApp 资源类型
description: 包含 Intune 移动应用基属性的抽象类。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0e1e68ede0e4beef689d753aca9af8292812d64c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408332"
---
# <a name="mobileapp-resource-type"></a>mobileApp 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含 Intune 移动应用基属性的抽象类。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List mobileApps](../api/intune-apps-mobileapp-list.md)|[mobileApp](../resources/intune-apps-mobileapp.md) 集合|列出 [mobileApp](../resources/intune-apps-mobileapp.md) 对象的属性和关系。|
|[Get mobileApp](../api/intune-apps-mobileapp-get.md)|[mobileApp](../resources/intune-apps-mobileapp.md)|读取 [mobileApp](../resources/intune-apps-mobileapp.md) 对象的属性和关系。|
|[assign 操作](../api/intune-apps-mobileapp-assign.md)|无|尚未记录|
|[getMobileAppCount 函数](../api/intune-apps-mobileapp-getmobileappcount.md)|Int64|尚未记录|
|[getTopMobileApps 函数](../api/intune-apps-mobileapp-gettopmobileapps.md)|[mobileApp](../resources/intune-apps-mobileapp.md) 集合|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|displayName|String|管理员提供或导入的应用标题。|
|description|String|应用的说明。|
|publisher|String|应用的发布者。|
|largeIcon|[mimeContent](../resources/intune-shared-mimecontent.md)|要显示在应用详细信息中并用于图标上传的大图标。|
|createdDateTime|DateTimeOffset|创建应用的日期和时间。|
|lastModifiedDateTime|DateTimeOffset|上次修改应用的日期和时间。|
|isFeatured|Boolean|指示应用是否被管理员标记为特色的值。|
|privacyInformationUrl|String|隐私声明 Url。|
|informationUrl|String|详细信息 Url。|
|owner|String|应用的所有者。|
|developer|String|应用的开发者。|
|notes|String|应用的备注。|
|uploadState|Int32|上载状态。|
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|应用的发布状态。 除非应用已发布，否则无法分配应用。 可取值为：`notPublished`、`processing`、`published`。|
|isAssigned|Boolean|值，指示是否将应用程序分配给至少一个组。|
|roleScopeTagIds|String 集合|此移动应用程序的作用域标记 id 的列表。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|categories|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 集合|此应用的类别列表。|
|assignments|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 集合|此移动应用的组分配的列表。|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|移动应用安装摘要。|
|deviceStatuses|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)集合|此移动应用程序的安装状态的列表。|
|userStatuses|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)集合|此移动应用程序的安装状态的列表。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileApp",
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
  ]
}
```




