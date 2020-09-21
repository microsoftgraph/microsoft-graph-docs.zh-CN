---
title: itemPublication 资源类型
description: itemPublication 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 59b30c08e78db52af9e10c6aac2550dc02c11e62
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48084000"
---
# <a name="itempublication-resource-type"></a>itemPublication 资源类型

命名空间：microsoft.graph

表示已与用户的 [配置文件](../resources/profile.md)相关联的出版物或文章。

继承自 [itemFacet](../resources/itemfacet.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出出版物](../api/profile-list-publications.md)|[itemPublication](../resources/itempublication.md) 集合|从 "发布" 导航属性中获取 itemPublication 资源。|
|[创建 itemPublication](../api/profile-post-publications.md)|[itemPublication](../resources/itempublication.md)|创建新的 itemPublication 对象。|
|[获取 itemPublication](../api/itempublication-get.md)|[itemPublication](../resources/itempublication.md)|读取 [itemPublication](../resources/itempublication.md) 对象的属性和关系。|
|[更新 itemPublication](../api/itempublication-update.md)|[itemPublication](../resources/itempublication.md)|更新 [itemPublication](../resources/itempublication.md) 对象的属性。|
|[删除 itemPublication](../api/itempublication-delete.md)|无|删除一个 [itemPublication](../resources/itempublication.md) 对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|allowedAudiences|字符串|能够查看实体中包含的值的访问群体。 继承自 [itemFacet](../resources/itemfacet.md)。 可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。|
|createdBy|[identitySet](../resources/identityset.md)|提供创建实体的用户和/或应用程序的标识符。 继承自 [itemFacet](../resources/itemfacet.md)。|
|createdDateTime|DateTimeOffset|为创建实体时提供 dateTimeOffset。 继承自 [itemFacet](../resources/itemfacet.md)。|
|说明    |字符串      |出版物的说明。                   |
|displayName    |字符串      |出版物的标题。                         |
|id|字符串|用于单独寻址实体的标识符。 继承自 [entity](../resources/entity.md)|
|推导|[inferenceData](../resources/inferencedata.md)|如果实体是由创建或修改应用程序推断的，则包含推理详细信息。 继承自 [itemFacet](../resources/itemfacet.md)。|
|lastModifiedBy|[identitySet](../resources/identityset.md)|提供上次修改实体的用户和/或应用程序的标识符。 继承自 [itemFacet](../resources/itemfacet.md)。|
|lastModifiedDateTime|DateTimeOffset|为创建实体时提供 dateTimeOffset。 继承自 [itemFacet](../resources/itemfacet.md)。|
|publishedDate  |日期        |发布出版物的日期。      |
|发布者      |String      |出版物的出版物或发布者。     |
|source|[personDataSource](../resources/persondatasource.md)|值的来源，如果从另一个服务同步。 继承自 [itemFacet](../resources/itemfacet.md)。|
|thumbnailUrl   |字符串      |URL 引用出版物的缩略图。   |
|webUrl         |String      |引用发布的 URL。                  |

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


