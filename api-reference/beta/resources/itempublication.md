---
title: itemPublication 资源类型
description: itemPublication 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 5cdc4a741205be696e584100d1ce6900052a951354481cc0dceffb7d1e19464b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54248285"
---
# <a name="itempublication-resource-type"></a>itemPublication 资源类型

命名空间：microsoft.graph

表示已与用户配置文件关联的出版物或 [文章](../resources/profile.md)。

继承自 [itemFacet](../resources/itemfacet.md)。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出出版物](../api/profile-list-publications.md)|[itemPublication](../resources/itempublication.md) 集合|从出版物导航属性获取 itemPublication 资源。|
|[创建 itemPublication](../api/profile-post-publications.md)|[itemPublication](../resources/itempublication.md)|创建新的 itemPublication 对象。|
|[获取 itemPublication](../api/itempublication-get.md)|[itemPublication](../resources/itempublication.md)|读取 [itemPublication 对象的属性和](../resources/itempublication.md) 关系。|
|[更新 itemPublication](../api/itempublication-update.md)|[itemPublication](../resources/itempublication.md)|更新 [itemPublication 对象](../resources/itempublication.md) 的属性。|
|[删除 itemPublication](../api/itempublication-delete.md)|无|删除 [itemPublication](../resources/itempublication.md) 对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|allowedAudiences|String|能够查看实体中包含的值的访问群体。 继承自 [itemFacet](../resources/itemfacet.md)。 可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。|
|createdBy|[identitySet](../resources/identityset.md)|提供创建实体的用户和/或应用程序的标识符。 继承自 [itemFacet](../resources/itemfacet.md)。|
|createdDateTime|DateTimeOffset|提供实体创建时的日期时间Offset。 继承自 [itemFacet](../resources/itemfacet.md)。|
|description    |String      |出版物的说明。                   |
|displayName    |String      |出版物的标题。                         |
|id|字符串|用于单独寻址实体的标识符。 继承自 [实体](../resources/entity.md)|
|inference|[inferenceData](../resources/inferencedata.md)|如果实体是由创建或修改应用程序推断出来的，则包含推断详细信息。 继承自 [itemFacet](../resources/itemfacet.md)。|
|lastModifiedBy|[identitySet](../resources/identityset.md)|提供上次修改实体的用户和/或应用程序的标识符。 继承自 [itemFacet](../resources/itemfacet.md)。|
|lastModifiedDateTime|DateTimeOffset|提供实体创建时的日期时间Offset。 继承自 [itemFacet](../resources/itemfacet.md)。|
|publishedDate  |日期        |出版物的发布日期。      |
|发布者      |String      |出版物或出版物的发布者。     |
|source|[personDataSource](../resources/persondatasource.md)|如果从另一个服务同步，则值源自何处。 继承自 [itemFacet](../resources/itemfacet.md)。|
|thumbnailUrl   |字符串      |引用出版物缩略图的 URL。   |
|WebUrl         |String      |引用出版物的 URL。                  |

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.itemPublication",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.itemPublication",
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
  "description": "String",
  "displayName": "String",
  "publishedDate": "Date",
  "publisher": "String",
  "thumbnailUrl": "String",
  "webUrl": "String"
}
```


