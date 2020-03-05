---
title: rubricLevel 资源类型
description: Rubric 的级别
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 24af9e9be6dc9b63934a02193958e0267dde8dea
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521010"
---
# <a name="rubriclevel-resource-type"></a>rubricLevel 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Rubric 的级别。 有关 rubric*质量*、*级别*和*条件*之间的关系的说明，请参阅[educationRubric](educationrubric.md) 。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|说明|[itemBody](itembody.md)|此 rubric 级别的说明。|
|displayName|String|此 rubric 级别的名称。|
|评分|[educationAssignmentGradeType](educationassignmentgradetype.md)|如果这是一个无点的 rubric，则为 Null;[educationAssignmentPointsGradeType](educationassignmentpointsgradetype.md)如果是点 rubric。|
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