---
title: itemAddress 资源类型
description: itemAddress 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 7e11ab6a69e377144a53c298e1c8ad99d496557769be5d799dd0afa2beb38ea7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54167882"
---
# <a name="itemaddress-resource-type"></a>itemAddress 资源类型

命名空间：microsoft.graph

表示物理地址和找到该地址的位置的详细信息。

继承自 [itemFacet](../resources/itemfacet.md)。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出地址](../api/profile-list-addresses.md)|[itemAddress](../resources/itemaddress.md) 集合|从 addresses 导航属性获取 itemAddress 资源。|
|[创建 itemAddress](../api/profile-post-addresses.md)|[itemAddress](../resources/itemaddress.md)|创建新的 itemAddress 对象。|
|[获取 itemAddress](../api/itemaddress-get.md)|[itemAddress](../resources/itemaddress.md)|读取 [itemAddress 对象的属性和](../resources/itemaddress.md) 关系。|
|[更新 itemAddress](../api/itemaddress-update.md)|[itemAddress](../resources/itemaddress.md)|更新 [itemAddress 对象](../resources/itemaddress.md) 的属性。|
|[删除 itemAddress](../api/itemaddress-delete.md)|无|删除 [itemAddress](../resources/itemaddress.md) 对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|allowedAudiences|String|能够查看实体中包含的值的访问群体。 继承自 [itemFacet](../resources/itemfacet.md)。 可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。|
|createdBy|[identitySet](../resources/identityset.md)|提供创建实体的用户和/或应用程序的标识符。 继承自 [itemFacet](../resources/itemfacet.md)。|
|createdDateTime|DateTimeOffset|提供实体创建时的日期时间Offset。 继承自 [itemFacet](../resources/itemfacet.md)。|
|detail|[physicalAddress](../resources/physicaladdress.md)|有关地址本身的详细信息。|
|displayName|String|用户分配给此地址的友好名称。 |
|geoCoordinates|[geoCoordinates](../resources/geocoordinates.md)|地址的地理序号。|
|id|字符串|用于单独寻址实体的标识符。 继承自 [实体](../resources/entity.md)|
|inference|[inferenceData](../resources/inferencedata.md)|如果实体是由创建或修改应用程序推断出来的，则包含推断详细信息。 继承自 [itemFacet](../resources/itemfacet.md)。|
|lastModifiedBy|[identitySet](../resources/identityset.md)|提供上次修改实体的用户和/或应用程序的标识符。 继承自 [itemFacet](../resources/itemfacet.md)。|
|lastModifiedDateTime|DateTimeOffset|提供实体创建时的日期时间Offset。 继承自 [itemFacet](../resources/itemfacet.md)。|
|source|[personDataSource](../resources/persondatasource.md)|如果从另一个服务同步，则值源自何处。 继承自 [itemFacet](../resources/itemfacet.md)。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.itemAddress",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.itemAddress",
  "id": "String (identifier)",
  "allowedAudiences": "String",
  "inference": {
    "@odata.type": "microsoft.graph.inferenceData"
  },
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "source": {
    "@odata.type": "microsoft.graph.personDataSource"
  },
  "displayName": "String",
  "detail": {
    "@odata.type": "microsoft.graph.physicalAddress"
  },
  "geoCoordinates": {
    "@odata.type": "microsoft.graph.geoCoordinates"
  }
}
```


