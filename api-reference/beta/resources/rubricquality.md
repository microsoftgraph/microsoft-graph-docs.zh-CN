---
title: rubricQuality 资源类型
description: Rubric 的质量
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 6f900056db140719ff5bc7902a6a7a9531cebe9b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521003"
---
# <a name="rubricquality-resource-type"></a>rubricQuality 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Rubric 的质量。 有关 rubric*质量*、*级别*和*条件*之间的关系的说明，请参阅[educationRubric](educationrubric.md) 。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|条件|[rubricCriterion](rubriccriterion.md)集合|此 rubric 质量的条件集合。|
|说明|[itemBody](itembody.md)|此 rubric 质量的说明。|
|displayName|String|此 rubric 质量的名称。|
|qualityId|String|此资源的 ID。|
|weight|单精度|如果有，则为此质量的数字权重。  权重必须添加到100。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rubricQuality",
  "baseType": null
}-->

```json
{
  "criteria": [{"@odata.type": "microsoft.graph.rubricCriterion"}],
  "description": {"@odata.type": "microsoft.graph.itemBody"},
  "displayName": "String",
  "qualityId": "String",
  "weight": "Double"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rubricQuality resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->