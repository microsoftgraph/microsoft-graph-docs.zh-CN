---
title: mobileAppRelationship 资源类型
description: 介绍了如何将子移动应用程序与其父移动应用程序之间的关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 80cf0fd5897d0ff3d1b3b3adc5343ad4c059442e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43462580"
---
# <a name="mobileapprelationship-resource-type"></a>mobileAppRelationship 资源类型

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

介绍了如何将子移动应用程序与其父移动应用程序之间的关系。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 mobileAppRelationships](../api/intune-apps-mobileapprelationship-list.md)|[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)集合|列出[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)对象的属性和关系。|
|[获取 mobileAppRelationship](../api/intune-apps-mobileapprelationship-get.md)|[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|读取[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)对象的属性和关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|关系实体 id。|
|targetId|String|目标子移动应用程序的应用程序 id。|
|targetDisplayName|String|目标子移动应用程序的显示名称。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppRelationship"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppRelationship",
  "id": "String (identifier)",
  "targetId": "String",
  "targetDisplayName": "String"
}
```



