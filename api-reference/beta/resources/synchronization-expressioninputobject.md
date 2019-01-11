---
title: expressionInputObject 资源类型
description: '代表要用作输入的测试数据时[synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md)操作执行表达式求值。'
localization_priority: Normal
ms.openlocfilehash: acf0fa5125d863224de6df76d46109b9888f8ddf
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820109"
---
# <a name="expressioninputobject-resource-type"></a>expressionInputObject 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

代表要用作输入的测试数据时[synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md)操作执行表达式求值。

## <a name="properties"></a>属性
| 属性     | 类型   |Description|
|:---------------|:--------|:----------|
|definition|[objectDefinition](synchronization-objectdefinition.md)|测试对象的定义。|
|properties|[stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md)集合|测试对象的属性值。|

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
<!-- {
  "type": "#page.annotation",
  "description": "expressionInputObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
