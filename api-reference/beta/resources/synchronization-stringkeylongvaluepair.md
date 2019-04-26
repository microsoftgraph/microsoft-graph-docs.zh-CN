---
title: stringKeyLongValuePair 资源类型
description: 表示键值对, 其中键是字符串, 值为 Int64。
localization_priority: Normal
ms.openlocfilehash: 48ca44c70e02be153aaeb5ee1171cd8c60e0fa2d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342748"
---
# <a name="stringkeylongvaluepair-resource-type"></a>stringKeyLongValuePair 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示键值对, 其中键是字符串, 值为 Int64。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|Key|String|键。|
|值|Int64|值。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyLongValuePair"
}-->

```json
{
  "key": "String",
  "value": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "stringKeyLongValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
