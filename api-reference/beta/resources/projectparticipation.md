---
title: projectParticipation 资源类型
description: projectParticipation 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 1d349b33dc3325451e97d055c178082676b48de3
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156362"
---
# <a name="projectparticipation-resource-type"></a>projectParticipation 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关与用户关联的项目的详细信息。

继承自 [itemFacet](itemfacet.md)。

## <a name="methods"></a>方法

|方法|返回类型|说明|
|:---|:---|:---|
|[列出项目](../api/profile-list-projects.md)|[projectParticipation](../resources/projectparticipation.md) 集合|从项目导航属性获取 projectParticipation 资源。|
|[创建 projectParticipation](../api/profile-post-projects.md)|[projectParticipation](../resources/projectparticipation.md)|创建新的 projectParticipation 对象。|
|[获取 projectParticipation](../api/projectparticipation-get.md)|[projectParticipation](../resources/projectparticipation.md)|读取 [projectParticipation](../resources/projectparticipation.md) 对象的属性和关系。|
|[更新 projectParticipation](../api/projectparticipation-update.md)|[projectParticipation](../resources/projectparticipation.md)|更新 [projectParticipation 对象](../resources/projectparticipation.md) 的属性。|
|[删除 projectParticipation](../api/projectparticipation-delete.md)|无|删除 [projectParticipation](../resources/projectparticipation.md) 对象。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|allowedAudiences|String|能够查看实体中包含的值的访问群体。 继承自 [itemFacet](../resources/itemfacet.md)。 可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。|
|categories|String 集合|包含用户与项目计划关联的类别 (例如，数字转换、该项目) 。 |
|client|[companyDetail](../resources/companydetail.md)|包含有关项目用于的客户端的详细信息。 |
|collaborationTags|字符串集合|包含用户与兴趣相关联的体验方案标记。 集合中允许的值是： `askMeAbout` ， `ableToMentor` ， `wantsToLearn` 。 `wantsToImprove`|
|同事|[relatedPerson](../resources/relatedperson.md) 集合|列出同样参与项目的人。 |
|createdBy|[identitySet](../resources/identityset.md)|提供创建实体的用户和/或应用程序的标识符。 继承自 [itemFacet](../resources/itemfacet.md)。|
|createdDateTime|DateTimeOffset|提供实体创建时的日期时间Offset。 继承自 [itemFacet](../resources/itemfacet.md)。|
|detail|[positionDetail](../resources/positiondetail.md)|包含有关用户在项目上的角色的详细信息。|
|displayName|String|包含项目的友好名称。|
|id|String|用于单独寻址实体的标识符。 继承自 [实体](../resources/entity.md)|
|推断|[inferenceData](../resources/inferencedata.md)|包含通过创建或修改应用程序推断实体的推断详细信息。 继承自 [itemFacet](../resources/itemfacet.md)。|
|lastModifiedBy|[identitySet](../resources/identityset.md)|提供上次修改实体的用户和/或应用程序的标识符。 继承自 [itemFacet](../resources/itemfacet.md)。|
|lastModifiedDateTime|DateTimeOffset|提供实体创建时的日期时间Offset。 继承自 [itemFacet](../resources/itemfacet.md)。|
|source|[personDataSource](../resources/persondatasource.md)|如果从另一个服务同步，则值的来源。 继承自 [itemFacet](../resources/itemfacet.md)。|
|发起人|[relatedPerson](../resources/relatedperson.md) 集合|发起项目的一个或多个人员。    |
## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.projectParticipation"
}-->

```json
{
  "@odata.type": "#microsoft.graph.projectParticipation",
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
  "client": {
    "@odata.type": "microsoft.graph.companyDetail"
  },
  "displayName": "String",
  "detail": {
    "@odata.type": "microsoft.graph.positionDetail"
  },
  "colleagues": [
    {
      "@odata.type": "microsoft.graph.relatedPerson"
    }
  ],
  "sponsors": [
    {
      "@odata.type": "microsoft.graph.relatedPerson"
    }
  ],
  "collaborationTags": [
    "String"
  ]
}
```


