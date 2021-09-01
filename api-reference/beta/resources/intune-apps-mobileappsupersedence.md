---
title: mobileAppSupersedence 资源类型
description: 描述两个移动应用程序之间的取代关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e56e8c23c852028cec007b29de7f7b7931a47c2d
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58806262"
---
# <a name="mobileappsupersedence-resource-type"></a>mobileAppSupersedence 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

描述两个移动应用程序之间的取代关系。


继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 mobileAppSupersedences](../api/intune-apps-mobileappsupersedence-list.md)|[mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) 集合|列出 [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) 对象的属性和关系。|
|[获取 mobileAppSupersedence](../api/intune-apps-mobileappsupersedence-get.md)|[mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md)|读取 [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) 对象的属性和关系。|
|[创建 mobileAppSupersedence](../api/intune-apps-mobileappsupersedence-create.md)|[mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md)|创建新的 [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) 对象。|
|[删除 mobileAppSupersedence](../api/intune-apps-mobileappsupersedence-delete.md)|无|删除 [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md)。|
|[更新 mobileAppSupersedence](../api/intune-apps-mobileappsupersedence-update.md)|[mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md)|更新 [mobileAppSupersedence 对象](../resources/intune-apps-mobileappsupersedence.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|关系实体 ID。继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetId|String|目标移动应用的应用 ID。继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetDisplayName|字符串|目标移动应用显示名称。 继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetDisplayVersion|字符串|目标移动应用的显示版本。 继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetPublisher|String|目标移动应用的发布者。 继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetType|[mobileAppRelationshipType](../resources/intune-apps-mobileapprelationshiptype.md)|关系类型，指示目标是父对象还是子级。 继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)。 可取值为：`child`、`parent`。|
|supersedenceType|[mobileAppSupersedenceType](../resources/intune-apps-mobileappsupersedencetype.md)|父应用和子应用之间的取代关系类型。 可取值为：`update`、`replace`。|
|supersededAppCount|Int32|被子应用直接或间接取代的应用总数。|
|supersedingAppCount|Int32|直接或间接取代父应用的应用总数。|

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
  "targetDisplayVersion": "String",
  "targetPublisher": "String",
  "targetType": "String",
  "supersedenceType": "String",
  "supersededAppCount": 1024,
  "supersedingAppCount": 1024
}
```



