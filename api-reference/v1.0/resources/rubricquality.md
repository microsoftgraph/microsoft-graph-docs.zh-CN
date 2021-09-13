---
title: rubricQuality 资源类型
description: 标准的质量。
ms.localizationpriority: medium
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: f75b873d37acfa23b7c60a9cd435948b73c0eb7a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59117765"
---
# <a name="rubricquality-resource-type"></a>rubricQuality 资源类型

命名空间：microsoft.graph

标准的质量。 

有关标准质量、级别和条件之间的关系的说明，请参阅[educationRubric。](educationrubric.md) 

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|条件|[rubricCriterion](rubriccriterion.md) 集合|此标准质量标准的集合。|
|说明|[itemBody](itembody.md)|此标准质量的说明。|
|displayName|String|此标准质量的名称。|
|qualityId|String|此资源的 ID。|
|weight|单一|如果存在，则此质量的数字权重。  权重必须最多增加 100。|

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

