---
title: mobileApp 资源类型
description: 包含 Intune 移动应用基属性的抽象类。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: dbccfb27073c15e6a5fbf78842cc894aadea2c1c
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66441116"
---
# <a name="mobileapp-resource-type"></a>mobileApp 资源类型

命名空间：microsoft.graph

> **重要：** /beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产用途。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含 Intune 移动应用基属性的抽象类。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List mobileApps](../api/intune-shared-mobileapp-list.md)|[mobileApp](../resources/intune-shared-mobileapp.md) 集合|列出 [mobileApp](../resources/intune-shared-mobileapp.md) 对象的属性和关系。|
|[Get mobileApp](../api/intune-shared-mobileapp-get.md)|[mobileApp](../resources/intune-shared-mobileapp.md)|读取 [mobileApp](../resources/intune-shared-mobileapp.md) 对象的属性和关系。|
|**应用**|
|[分配操作](../api/intune-shared-mobileapp-assign.md)|无|尚未记录|
|[getMobileAppCount 函数](../api/intune-shared-mobileapp-getmobileappcount.md)|Int64|尚未记录|
|[getTopMobileApps 函数](../api/intune-shared-mobileapp-gettopmobileapps.md)|[mobileApp](../resources/intune-shared-mobileapp.md) 集合|尚未记录|
|[updateRelationships 操作](../api/intune-shared-mobileapp-updaterelationships.md)|无|尚未记录|
|[getRelatedAppStates 函数](../api/intune-shared-mobileapp-getrelatedappstates.md)|[mobileAppRelationshipState](../resources/intune-apps-mobileapprelationshipstate.md) 集合|尚未记录|
|**策略集**|
|[hasPayloadLinks 操作](../api/intune-shared-mobileapp-haspayloadlinks.md)|[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) 集合|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|displayName|String|管理员提供或导入的应用标题。|
|说明|String|应用的说明。|
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
|uploadState|Int32|上传状态。|
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|应用的发布状态。 除非应用已发布，否则无法分配应用。 可取值为：`notPublished`、`processing`、`published`。|
|isAssigned|Boolean|指示是否将应用分配给至少一个组的值。|
|roleScopeTagIds|字符串集合|此移动应用的范围标记 ID 列表。|
|dependentAppCount|Int32|子应用的依赖项总数。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|**应用**|
|categories|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 集合|此应用的类别列表。|
|assignments|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 集合|此移动应用的组分配的列表。|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|移动应用安装摘要。|
|deviceStatuses|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) 集合|此移动应用的安装状态列表。|
|userStatuses|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) 集合|此移动应用的安装状态列表。|
|关系|[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) 集合|此移动应用的关系列表。|

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
  ],
  "dependentAppCount": 1024
}
```



