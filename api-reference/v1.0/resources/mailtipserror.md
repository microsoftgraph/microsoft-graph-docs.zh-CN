---
title: mailTipsError 资源类型
description: 操作过程中发生的错误。
ms.openlocfilehash: 8604207844ade4e0c10981f30d03b33eacf4a0a2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009187"
---
# <a name="mailtipserror-resource-type"></a>mailTipsError 资源类型

操作过程中发生的错误。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
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