---
title: workPosition 资源类型
description: workPosition 资源类型
ms.localizationpriority: medium
author: kevinbellinger
ms.prod: people-and-workplace-intelligence
doc_type: resourcePageType
ms.openlocfilehash: e26e9d5a4d48cb2b1186b1ea69e4b462a8ef93a4
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2022
ms.locfileid: "66730579"
---
# <a name="workposition-resource-type"></a>workPosition 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关与用户 [配置文件](profile.md)关联的工作位置的详细信息。

此资源类型继承自 [itemFacet](itemfacet.md)。


## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出位置](../api/profile-list-positions.md)|[workPosition](../resources/workposition.md) 集合|从位置导航属性获取 workPosition 资源。|
|[创建 workPosition](../api/profile-post-positions.md)|[workPosition](../resources/workposition.md)|创建新的 workPosition 对象。|
|[获取 workPosition](../api/workposition-get.md)|[workPosition](../resources/workposition.md)|读取 [workPosition](../resources/workposition.md) 对象的属性和关系。|
|[更新 workPosition](../api/workposition-update.md)|[workPosition](../resources/workposition.md)|更新 [workPosition](../resources/workposition.md) 对象的属性。|
|[删除 workPosition](../api/workposition-delete.md)|None|删除 [workPosition](../resources/workposition.md) 对象。|


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|allowedAudiences|String|能够查看实体中包含的值的受众。 继承自 [itemFacet](../resources/itemfacet.md)。 可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。|
|类别|String collection|用户与此位置关联的类别。|
|同事|[relatedPerson](../resources/relatedperson.md) 集合|与此位置相关联的同事。|
|createdBy|[identitySet](../resources/identityset.md)|提供创建实体的用户和/或应用程序的标识符。 继承自 [itemFacet](../resources/itemfacet.md)。|
|createdDateTime|DateTimeOffset|提供创建实体时的 dateTimeOffset。 继承自 [itemFacet](../resources/itemfacet.md)。|
|详细|[positionDetail](../resources/positiondetail.md)|包含有关位置的详细信息。 |
|id|String|用于单独寻址实体的标识符。 继承自 [实体](../resources/entity.md)|
|推理|[inferenceData](../resources/inferencedata.md)|如果实体是由创建或修改应用程序推断的，则包含推理详细信息。 继承自 [itemFacet](../resources/itemfacet.md)。|
|isCurrent|Boolean|表示位置是否为当前位置。|
|lastModifiedBy|[identitySet](../resources/identityset.md)|提供上次修改实体的用户和/或应用程序的标识符。 继承自 [itemFacet](../resources/itemfacet.md)。|
|lastModifiedDateTime|DateTimeOffset|提供创建实体时的 dateTimeOffset。 继承自 [itemFacet](../resources/itemfacet.md)。|
|manager|[relatedPerson](../resources/relatedperson.md)|包含此位置中用户的经理的详细信息。|
|source|[personDataSource](../resources/persondatasource.md)|如果从另一个服务同步，则值源自何处。 继承自 [itemFacet](../resources/itemfacet.md)。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workPosition",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workPosition",
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
  "detail": {
    "@odata.type": "microsoft.graph.positionDetail"
  },
  "manager": {
    "@odata.type": "microsoft.graph.relatedPerson"
  },
  "colleagues": [
    {
      "@odata.type": "microsoft.graph.relatedPerson"
    }
  ],
  "isCurrent": "Boolean"
}
```

