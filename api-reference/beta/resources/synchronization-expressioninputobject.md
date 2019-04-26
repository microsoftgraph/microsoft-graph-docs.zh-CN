---
title: expressionInputObject 资源类型
description: '表示当[synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md)操作执行表达式评估时用作输入测试数据的对象。'
localization_priority: Normal
ms.openlocfilehash: 90d394639de7050eaed3b696dd8526e144cac03d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345573"
---
# <a name="expressioninputobject-resource-type"></a>expressionInputObject 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示在[parseExpression](../api/synchronization-synchronizationschema-parseexpression.md)操作执行表达式评估时用作输入测试数据的对象。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|定义|[objectDefinition](synchronization-objectdefinition.md)|test 对象的定义。|
|properties|[stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md)集合|test 对象的属性值。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.expressionInputObject"
}-->

```json
{
  "definition": {"@odata.type": "microsoft.graph.objectDefinition"},
  "properties": [{"@odata.type": "microsoft.graph.stringKeyObjectValuePair"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "expressionInputObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
