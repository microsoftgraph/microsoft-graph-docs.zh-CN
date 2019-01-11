---
title: mailTipsError 资源类型
description: 操作过程中发生的错误。
localization_priority: Normal
ms.openlocfilehash: a4916bc34d7c76dc6c6592ee03e64b20a6485190
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892091"
---
# <a name="mailtipserror-resource-type"></a>mailTipsError 资源类型

操作过程中发生的错误。

## <a name="properties"></a>属性
| 属性     | 类型   |Description|
|:-----|:-----|:-----|
| message | 字符串 | 错误消息。 |
| code | 字符串 | 错误代码。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mailTipsError"
}-->

```json
{
  "message": "string",
  "code": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailTipsError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
