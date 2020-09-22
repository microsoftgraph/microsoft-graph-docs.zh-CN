---
title: skillProficiency 资源类型
description: skillProficiency 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: d01c9fe6c4171c16d96e5b81eb8537ea0cbeb1a1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997674"
---
# <a name="skillproficiency-resource-type"></a>skillProficiency 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关与各种服务中的用户相关的技能的详细信息。

继承自 [itemFacet](itemfacet.md)。

## <a name="methods"></a>方法
 
|方法|返回类型|说明|
|:---|:---|:---|
|[列表技能](../api/profile-list-skills.md)|[skillProficiency](../resources/skillproficiency.md) 集合|从技能导航属性中获取 skillProficiency 资源。|
|[创建 skillProficiency ](../api/profile-post-skills.md)|[skillProficiency](../resources/skillproficiency.md)|创建新的 skillProficiency 对象。|
|[获取 skillProficiency](../api/skillproficiency-get.md)|[skillProficiency](../resources/skillproficiency.md)|读取 [skillProficiency](../resources/skillproficiency.md) 对象的属性和关系。|
|[更新 skillProficiency](../api/skillproficiency-update.md)|[skillProficiency](../resources/skillproficiency.md)|更新 [skillProficiency](../resources/skillproficiency.md) 对象的属性。|
|[删除 skillProficiency](../api/skillproficiency-delete.md)|无|删除一个 [skillProficiency](../resources/skillproficiency.md) 对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|allowedAudiences|String|能够查看实体中包含的值的访问群体。 继承自 [itemFacet](../resources/itemfacet.md)。 可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。|
|类别|String collection|包含用户与技能相关联的类别 (例如，个人、职业、爱好) 。 |
|collaborationTags|String collection|包含用户与兴趣相关的体验方案标记。 集合中允许的值为： `askMeAbout` 、 `ableToMentor` 、 `wantsToLearn` 、 `wantsToImprove` 。|
|createdBy|[identitySet](../resources/identityset.md)|提供创建实体的用户和/或应用程序的标识符。 继承自 [itemFacet](../resources/itemfacet.md)。|
|createdDateTime|DateTimeOffset|为创建实体时提供 dateTimeOffset。 继承自 [itemFacet](../resources/itemfacet.md)。|
|displayName|String|包含技能的友好名称。 |
|id|String|用于单独寻址实体的标识符。 继承自 [entity](../resources/entity.md)|
|推导|[inferenceData](../resources/inferencedata.md)|如果实体是由创建或修改应用程序推断的，则包含推理详细信息。 继承自 [itemFacet](../resources/itemfacet.md)。|
|lastModifiedBy|[identitySet](../resources/identityset.md)|提供上次修改实体的用户和/或应用程序的标识符。 继承自 [itemFacet](../resources/itemfacet.md)。|
|lastModifiedDateTime|DateTimeOffset|为创建实体时提供 dateTimeOffset。 继承自 [itemFacet](../resources/itemfacet.md)。|
|水平|skillProficiencyLevel|熟练掌握此技能的用户的详细信息。 可取值为：`elementary`、`limitedWorking`、`generalProfessional`、`advancedProfessional`、`expert`、`unknownFutureValue`。|
|source|[personDataSource](../resources/persondatasource.md)|值的来源，如果从另一个服务同步。 继承自 [itemFacet](../resources/itemfacet.md)。|
|webUrl|String|包含指向有关技能的信息源的链接。 |

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.skillProficiency",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.skillProficiency",
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
  "displayName": "String",
  "proficiency": "String",
  "webUrl": "String",
  "collaborationTags": [
    "String"
  ]
}
```

