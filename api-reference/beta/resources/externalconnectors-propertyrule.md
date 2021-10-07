---
title: propertyRule 资源类型
description: 定义显示 displayTemplate 的条件集
author: emzho
ms.localizationpriority: normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 7f1e021e4bc735ff7f5efd322e0a5a8080e5816b
ms.sourcegitcommit: 2a9b82dae63d8a998711679a379ae1fa89df80e0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/06/2021
ms.locfileid: "60214917"
---
# <a name="propertyrule-resource-type"></a>propertyRule 资源类型

命名空间：microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

定义显示 [displayTemplate](../resources/externalconnectors-displaytemplate.md)的条件集。 规则使用格式： (架构中的) + (操作) + () 。 例如 **，propertyRule** 可以指定"itemTitle""contains""contoso"。 因此，除非 itemTitle 包含值"contoso"，否则 **displayTemplate** 将不会显示。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|operation|字符串|指定在计算单个 **propertyRule** 期间要执行的操作，其中 和 集合中的字符串是 `property` `values` 各自的操作数。 可取值为：`null`、`equals`、`notEquals`、`contains`、`notContains`、`lessThan`、`greaterThan`、`startsWith`、`unknownFutureValue`。 必需。|
|property|字符串|[externalItem 架构中的](../resources/externalconnectors-externalitem.md)属性。 必需。|
|值|String collection|具有一个或多个字符串的集合。 指定的字符串 () 指定的操作与指定的属性匹配。 必需。|
|valuesJoinedBy|binaryOperator|用于计算多个 **propertyRules 的联接运算符**。 例如， `and` 如果指定了 ，则所有 **propertyRules** 都必须为 true，propertyRule 才为 true。  可取值为：`or`、`and`。 必填。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.externalConnectors.propertyRule"
}
-->
``` json
{
  "property": "String",
  "operation": "String",
  "valuesJoinedBy": "String",
  "values": [
    "String"
  ]
}
```

