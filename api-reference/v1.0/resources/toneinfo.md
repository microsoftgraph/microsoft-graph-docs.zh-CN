---
title: toneInfo 资源类型
description: 单个 DTMF 事件。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 82b67b18be4c0c9ba63b86c2ddc5e0f670b20c26
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446798"
---
# <a name="toneinfo-resource-type"></a>toneInfo 资源类型

命名空间： microsoft. graph

单个 DTMF 事件。

## <a name="properties"></a>属性

| 属性       | 类型    | 说明|
|:---------------|:--------|:----------|
| sequenceId | Int64 | 用于对 DTMF 事件进行排序的增量标识符。 |
| 按键 | String | 可能的值为`tone0`： `tone1`、 `tone2`、 `tone3` `tone4` `tone5` `tone6` `tone7` `tone8`、 `tone9`、、、、、 `star`、、`pound` |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.toneInfo"
}-->
```json
{
  "sequenceId": 1024,
  "tone": "tone0 | tone1 | tone2 | tone3 | tone4 | tone5 | tone6 | tone7 | tone8 | tone9 | star | pound | a | b | c | d | flash"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "toneInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
