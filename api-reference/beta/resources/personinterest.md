---
title: personInterest 资源类型
description: personInterest 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: ef2675b8c604115fc5e04a7747dc4c110d567604
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939023"
---
# <a name="personinterest-resource-type"></a>personInterest 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[PersonInterest](personinterest.md)资源类型提供有关用户在各种服务中与其自身关联的兴趣的详细信息。

继承自[itemFacet](itemfacet.md)。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:---------------------------------------------------|:------------------------------------|:------------------------------------------------------------|
| [获取 personInterest](../api/personinterest-get.md) | [personInterest](personinterest.md) | 读取 personInterest 对象的属性和关系。 |
| [Update](../api/personinterest-update.md)          | [personInterest](personinterest.md) | 更新 personInterest 对象。                               |
| [删除](../api/personinterest-delete.md)          | 无                                | 删除 personInterest 对象。                               |

## <a name="properties"></a>属性

| 属性     | 类型             | 描述                                                                          |
|:-------------|:-----------------|:-------------------------------------------------------------------------------------|
|类别    |String collection | 包含用户与兴趣相关联的类别（例如： personal、recipies） |
|description   |字符串            | 包含对利息的说明。                                              |
|displayName   |String            | 包含利息的友好名称。                                           |
|webUrl        |String            | 包含有关感兴趣的网页或资源的链接。                         |

## <a name="relationships"></a>关系

无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。 

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personInterest",
  "baseType": ""
}-->

```json
{
  "categories": ["String"],
  "description": "String",
  "displayName": "String",
  "webUrl": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "personInterest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->