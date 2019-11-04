---
title: projectParticipation 资源类型
description: projectParticipation 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 465a45a2ba8a607d0537e66b96207b3d60626517
ms.sourcegitcommit: dd94c3a0f7663699825b6dbc119cdcef494cd130
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2019
ms.locfileid: "37950470"
---
# <a name="projectparticipation-resource-type"></a>projectParticipation 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关与用户关联的项目的详细信息。

继承自[itemFacet](itemfacet.md)。

## <a name="methods"></a>方法

| 方法                                                         | 返回类型                                     | 说明                                                       |
|:---------------------------------------------------------------|:------------------------------------------------|:------------------------------------------------------------------|
| [获取 projectParticipation](../api/projectparticipation-get.md) | [projectParticipation](projectparticipation.md) | 读取**projectParticipation**对象的属性和关系。 |
| [更新 projectParticipation](../api/projectparticipation-update.md)                | [projectParticipation](projectparticipation.md) | 更新**projectParticipation**对象。                               |
| [删除 projectParticipation](../api/projectparticipation-delete.md)                | 无。                                            | 删除**projectParticipation**对象。                               |

## <a name="properties"></a>属性

| 属性     | 类型                                        | 描述                                                                                      |
|:-------------|:--------------------------------------------|:-------------------------------------------------------------------------------------------------|
|类别    | String collection                           | 包含用户与项目相关联的类别（例如，数字转换、石油远程测试机组）。 |
|客户端        |[companyDetail](companydetail.md)            | 包含有关项目所针对的客户端的详细信息。                              |
|征求    |[relatedPerson](relatedperson.md)集合 | 列出也在项目中工作的人员。                                                          |
|介绍        |[positionDetail](positiondetail.md)          | 包含有关用户在项目上的角色的详细信息。                                             |
|displayName   |String                                       |包含项目的友好名称。                                                         |
|人      |[relatedPerson](relatedperson.md)集合 | 发起项目的人员或人员。                                                         |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.projectParticipation",
  "baseType": ""
}-->

```json
{
  "categories": ["String"],
  "client": {"@odata.type": "microsoft.graph.companyDetail"},
  "colleagues": [{"@odata.type": "microsoft.graph.relatedPerson"}],
  "detail": {"@odata.type": "microsoft.graph.positionDetail"},
  "displayName": "String",
  "sponsors": [{"@odata.type": "microsoft.graph.relatedPerson"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "projectParticipation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
