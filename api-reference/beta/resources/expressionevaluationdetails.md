---
title: expressionEvaluationDetails 资源类型
description: 表示表达式详细信息、结果和属性详细信息。
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: a2e2b2620f30234c23753ef743f14e55e29f6f91
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52679896"
---
# <a name="expressionevaluationdetails-resource-type"></a>expressionEvaluationDetails 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示表达式详细信息、结果和属性详细信息。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
| 表达式 | String | 表示已求值表达式。 |
| expressionEvaluationDetails | expressionEvaluationDetails 集合 | 表示表达式的计算的详细信息。 |
| expressionResult | Boolean | 表示当前表达式的结果的值。 |
| propertyToEvaluate | [propertyToEvaluate](propertytoevaluate.md) | 定义属性的名称和该属性的值。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.expressionEvaluationDetails",
  "baseType": null
}-->

```json
{
  "expression": "String",
  "expressionEvaluationDetails": [{"@odata.type": "microsoft.graph.expressionEvaluationDetails"}],
  "expressionResult": true,
  "propertyToEvaluate": {"@odata.type": "microsoft.graph.propertyToEvaluate"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "expressionEvaluationDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


