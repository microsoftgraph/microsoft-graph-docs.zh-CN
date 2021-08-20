---
title: personAnnotation 资源类型
description: personAnnotation 资源类型
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 49e7945b1ba07d7daedbd197b826148921f2f0227dd71b5780413a3b67b6c6be
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54197847"
---
# <a name="personannotation-resource-type"></a>personAnnotation 资源类型

命名空间：microsoft.graph

在注释中提供用户在各种服务中与自己关联并与其他人员共享的信息。

继承自 [itemFacet](../resources/itemfacet.md)。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出注释](../api/profile-list-notes.md)|[personAnnotation](../resources/personannotation.md) 集合|从 notes 导航属性获取 personAnnotation 资源。|
|[创建 personAnnotation](../api/profile-post-notes.md)|[personAnnotation](../resources/personannotation.md)|创建新的 personAnnotation 对象。|
|[获取 personAnnotation](../api/personannotation-get.md)|[personAnnotation](../resources/personannotation.md)|读取 [personAnnotation 对象的属性和](../resources/personannotation.md) 关系。|
|[更新 personAnnotation](../api/personannotation-update.md)|[personAnnotation](../resources/personannotation.md)|更新 [personAnnotation 对象](../resources/personannotation.md) 的属性。|
|[删除 personAnnotation](../api/personannotation-delete.md)|无|删除 [personAnnotation](../resources/personannotation.md) 对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|allowedAudiences|String|能够查看实体中包含的值的访问群体。 继承自 [itemFacet](../resources/itemfacet.md)。 可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。|
|createdBy|[identitySet](../resources/identityset.md)|提供创建实体的用户和/或应用程序的标识符。 继承自 [itemFacet](../resources/itemfacet.md)。|
|createdDateTime|DateTimeOffset|提供实体创建时的日期时间Offset。 继承自 [itemFacet](../resources/itemfacet.md)。|
|detail|[itemBody](../resources/itembody.md)|包含注释本身的详细信息。|
|displayName|String|包含便笺的友好名称。|
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
  "@odata.type": "microsoft.graph.personAnnotation",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.personAnnotation",
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
  "detail": {
    "@odata.type": "microsoft.graph.itemBody"
  },
  "displayName": "String"
}
```


