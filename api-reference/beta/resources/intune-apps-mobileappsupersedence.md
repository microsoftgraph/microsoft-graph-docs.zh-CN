---
title: mobileAppSupersedence 资源类型
description: 介绍两个移动应用之间的取代关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 46a19d4032a661bc1f17161d2fdadde774558bcb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973966"
---
# <a name="mobileappsupersedence-resource-type"></a>mobileAppSupersedence 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

介绍两个移动应用之间的取代关系。


继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 mobileAppSupersedences](../api/intune-apps-mobileappsupersedence-list.md)|[mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) 集合|列出 [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) 对象的属性和关系。|
|[获取 mobileAppSupersedence](../api/intune-apps-mobileappsupersedence-get.md)|[mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md)|读取 [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) 对象的属性和关系。|
|[创建 mobileAppSupersedence](../api/intune-apps-mobileappsupersedence-create.md)|[mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md)|创建新的 [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) 对象。|
|[删除 mobileAppSupersedence](../api/intune-apps-mobileappsupersedence-delete.md)|无|删除 [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md)。|
|[更新 mobileAppSupersedence](../api/intune-apps-mobileappsupersedence-update.md)|[mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md)|更新 [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|关系实体 id。继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetId|String|目标移动应用程序的应用程序 id。继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetDisplayName|String|目标移动应用程序的显示名称。 继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetType|[mobileAppRelationshipType](../resources/intune-apps-mobileapprelationshiptype.md)|表示目标是父项还是子项的关系的类型。 继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)。 可取值为：`child`、`parent`。|
|supersedenceType|[mobileAppSupersedenceType](../resources/intune-apps-mobileappsupersedencetype.md)|父应用和子应用之间的取代关系类型。 可取值为：`update`、`replace`。|
|supersededAppCount|Int32|由子应用直接或间接取代的应用程序总数。|
|supersedingAppCount|Int32|直接或间接取代父应用程序的应用程序总数量。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppSupersedence"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppSupersedence",
  "id": "String (identifier)",
  "targetId": "String",
  "targetDisplayName": "String",
  "targetType": "String",
  "supersedenceType": "String",
  "supersededAppCount": 1024,
  "supersedingAppCount": 1024
}
```






