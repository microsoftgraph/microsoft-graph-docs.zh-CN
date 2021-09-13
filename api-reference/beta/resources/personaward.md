---
title: personAward 资源类型
description: personAward 资源类型
ms.localizationpriority: medium
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 3e1ec26b6df9ccc83f47eb26fc502c3756564629
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59020166"
---
# <a name="personaward-resource-type"></a>personAward 资源类型

命名空间：microsoft.graph

表示已与用户配置文件关联的 [奖励](../resources/profile.md)。

继承自 [itemFacet](../resources/itemfacet.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出奖励](../api/profile-list-awards.md)|[personAward](../resources/personaward.md) 集合|从导航属性获取 personAward 资源。|
|[创建 personAward](../api/profile-post-awards.md)|[personAward](../resources/personaward.md)|创建新的 personAward 对象。|
|[获取 personAward](../api/personaward-get.md)|[personAward](../resources/personaward.md)|读取 [personAward](../resources/personaward.md) 对象的属性和关系。|
|[更新 personAward](../api/personaward-update.md)|[personAward](../resources/personaward.md)|更新 [personAward 对象](../resources/personaward.md) 的属性。|
|[删除 personAward](../api/personaward-delete.md)|无|删除 [personAward](../resources/personaward.md) 对象。|

## <a name="properties"></a>属性
|属性|类型|描述|
|:---|:---|:---|
|allowedAudiences|String|能够查看实体中包含的值的访问群体。 继承自 [itemFacet](../resources/itemfacet.md)。 可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。|
|createdBy|[identitySet](../resources/identityset.md)|提供创建实体的用户和/或应用程序的标识符。 继承自 [itemFacet](../resources/itemfacet.md)。|
|createdDateTime|DateTimeOffset|提供实体创建时的日期时间Offset。 继承自 [itemFacet](../resources/itemfacet.md)。|
|说明|String|奖励或奖励的奖励。 |
|displayName|String|奖励或奖励的名称。 |
|id|String|用于单独寻址实体的标识符。 继承自 [实体](../resources/entity.md)|
|inference|[inferenceData](../resources/inferencedata.md)|如果实体是由创建或修改应用程序推断出来的，则包含推断详细信息。 继承自 [itemFacet](../resources/itemfacet.md)。|
|issuedDate|日期|授予奖励或奖励的日期。 |
|issuingAuthority|String|授予该奖励或奖励的颁发机构。  |
|lastModifiedBy|[identitySet](../resources/identityset.md)|提供上次修改实体的用户和/或应用程序的标识符。 继承自 [itemFacet](../resources/itemfacet.md)。|
|lastModifiedDateTime|DateTimeOffset|提供实体创建时的日期时间Offset。 继承自 [itemFacet](../resources/itemfacet.md)。|
|source|[personDataSource](../resources/persondatasource.md)|如果从另一个服务同步，则值源自何处。 继承自 [itemFacet](../resources/itemfacet.md)。|
|thumbnailUrl|String|引用奖励或奖励缩略图的 URL。  |
|WebUrl|String|引用奖励或奖励的 URL。 |

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.personAward",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.personAward",
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
  "issuedDate": "Date",
  "issuingAuthority": "String",
  "thumbnailUrl": "String",
  "webUrl": "String"
}
```


