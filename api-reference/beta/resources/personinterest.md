---
title: personInterest 资源类型
description: personInterest 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 0b635ab19f4cda9985de05e317316579ad60f7b1
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161395"
---
# <a name="personinterest-resource-type"></a>personInterest 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

提供有关用户在各种服务中与自己相关联的兴趣的详细信息。

继承自 [itemFacet](itemfacet.md)。

## <a name="methods"></a>方法

| 方法                                                    | 返回类型                         | 说明                                                           |
|:----------------------------------------------------------|:------------------------------------|:----------------------------------------------------------------------|
|[列出兴趣](../api/profile-list-interests.md)|[personInterest](../resources/personinterest.md) 集合|从 interests 导航属性获取 personInterest 资源。|
|[创建 personInterest](../api/profile-post-interests.md)|[personInterest](../resources/personinterest.md)|创建新的 personInterest 对象。|
|[获取 personInterest](../api/personinterest-get.md)|[personInterest](../resources/personinterest.md)|读取 [personInterest 对象的属性和](../resources/personinterest.md) 关系。|
|[更新 personInterest](../api/personinterest-update.md)|[personInterest](../resources/personinterest.md)|更新 [personInterest 对象](../resources/personinterest.md) 的属性。|
|[删除 personInterest](../api/personinterest-delete.md)|无|删除 [personInterest](../resources/personinterest.md) 对象。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|allowedAudiences|String|能够查看实体中包含的值的访问群体。 继承自 [itemFacet](../resources/itemfacet.md)。 可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。|
|categories|String 集合|包含用户与感兴趣的类别 (例如，个人、) 。 |
|collaborationTags|字符串集合|包含用户与兴趣相关联的体验方案标记。 集合中允许的值是： `askMeAbout` ， `ableToMentor` ， `wantsToLearn` 。 `wantsToImprove`|
|createdBy|[identitySet](../resources/identityset.md)|提供创建实体的用户和/或应用程序的标识符。 继承自 [itemFacet](../resources/itemfacet.md)。|
|createdDateTime|DateTimeOffset|提供实体创建时的日期时间Offset。 继承自 [itemFacet](../resources/itemfacet.md)。|
|说明|String|包含对利息的说明。|
|displayName|String|包含兴趣的友好名称。  |
|id|String|用于单独寻址实体的标识符。 继承自 [实体](../resources/entity.md)|
|inference|[inferenceData](../resources/inferencedata.md)|包含通过创建或修改应用程序推断实体的推断详细信息。 继承自 [itemFacet](../resources/itemfacet.md)。|
|lastModifiedBy|[identitySet](../resources/identityset.md)|提供上次修改实体的用户和/或应用程序的标识符。 继承自 [itemFacet](../resources/itemfacet.md)。|
|lastModifiedDateTime|DateTimeOffset|提供实体创建时的日期时间Offset。 继承自 [itemFacet](../resources/itemfacet.md)。|
|source|[personDataSource](../resources/persondatasource.md)|如果从另一个服务同步，则值的来源。 继承自 [itemFacet](../resources/itemfacet.md)。|
|WebUrl|String|包含指向有关感兴趣的网页或资源的链接。 |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personInterest"
}-->

```json
{
  "@odata.type": "#microsoft.graph.personInterest",
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
  "categories": [
    "String"
  ],
  "description": "String",
  "displayName": "String",
  "webUrl": "String",
  "collaborationTags": [
    "String"
  ]
}
```


