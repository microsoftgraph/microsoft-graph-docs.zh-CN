---
title: mailTipsError 资源类型
description: 操作过程中发生的错误。
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: d9f5df716d62f2ae33e9a6c90d5803413b8c69b9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43461829"
---
# <a name="mailtipserror-resource-type"></a>mailTipsError 资源类型

命名空间：microsoft.graph

操作过程中发生的错误。

## <a name="properties"></a>属性
| 属性     | 类型   |描述|
|:-----|:-----|:-----|
| message | String | 错误消息。 |
| code | String | 错误代码。 |

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
