---
title: expressionEvaluationDetails 资源类型
description: 表示表达式详细信息、结果和属性详细信息。
ms.localizationpriority: medium
author: psaffaie
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: d588719e8d6bcf32ff337beec8815b6fe329ee0b
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2022
ms.locfileid: "64587033"
---
# <a name="expressionevaluationdetails-resource-type"></a>expressionEvaluationDetails 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示表达式详细信息、结果和属性详细信息。

## <a name="properties"></a>属性

| 属性                    | 类型                                        | 说明                                                      |
| :-------------------------- | :------------------------------------------ | :--------------------------------------------------------------- |
| 表达式                  | String                                      | 表示已求值表达式。                  |
| expressionEvaluationDetails | expressionEvaluationDetails 集合      | 表示表达式的计算的详细信息。      |
| expressionResult            | Boolean                                     | 表示当前表达式的结果的值。    |
| propertyToEvaluate          | [propertyToEvaluate](propertytoevaluate.md) | 定义属性的名称和该属性的值。 |

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
  "expressionEvaluationDetails": [
    { "@odata.type": "microsoft.graph.expressionEvaluationDetails" }
  ],
  "expressionResult": true,
  "propertyToEvaluate": { "@odata.type": "microsoft.graph.propertyToEvaluate" }
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
