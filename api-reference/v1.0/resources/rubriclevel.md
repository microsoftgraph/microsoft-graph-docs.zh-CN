---
title: rubricLevel 资源类型
description: 标准级别。
ms.localizationpriority: medium
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 5db0dac5bf68047f0ebc9dd38554d002a678dca6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59113530"
---
# <a name="rubriclevel-resource-type"></a>rubricLevel 资源类型

命名空间：microsoft.graph

标准级别。 

有关标准质量、级别和条件之间的关系的说明，请参阅[educationRubric。](educationrubric.md) 

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|说明|[itemBody](itembody.md)|此标准级别的说明。|
|displayName|String|此标准级别的名称。|
|一个|[educationAssignmentGradeType](educationassignmentgradetype.md)|如果这是无点数的分值，则其为 Null; [educationAssignmentPointsGradeType（](educationassignmentpointsgradetype.md) 如果为分数）。|
|levelId|String|此资源的 ID。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rubricLevel",
  "baseType": null
}-->

```json
{
  "description": {"@odata.type": "microsoft.graph.itemBody"},
  "displayName": "String",
  "grading": {"@odata.type": "microsoft.graph.educationAssignmentGradeType"},
  "levelId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rubricLevel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

