---
title: integerRange 资源类型
description: 表示由两个 Int64 边界描述的非独占整数范围。
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: e370d7b0fcf67c76fcb43cba7c9382521e8ada78
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900133"
---
# <a name="integerrange-resource-type"></a>integerRange 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示由两个 Int64 边界描述的非独占整数范围。

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|start|Int64|整数范围的非独占下限。|
|end|Int64|整数范围的非独占上限。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.integerRange"
}-->

```json
{
    "start": 12345,
    "end": 12345
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "integerRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

