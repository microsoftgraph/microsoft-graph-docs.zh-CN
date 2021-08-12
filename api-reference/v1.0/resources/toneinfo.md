---
title: toneInfo 资源类型
description: 单个 DTMF 事件。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: eba7ef5b7251712da0c91ecc9f006bbf3e1c5e80eaa86c1ea53942e815c9df4b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54124001"
---
# <a name="toneinfo-resource-type"></a>toneInfo 资源类型

命名空间：microsoft.graph

单个 DTMF 事件。

## <a name="properties"></a>属性

| 属性       | 类型    | 说明|
|:---------------|:--------|:----------|
| sequenceId | Int64 | 用于对 DTMF 事件排序的增量标识符。 |
| tone | tone | 可能的值是 `tone0` `tone1` `tone2` ：、、、、、、、、、 `tone3` `tone4` `tone5` `tone6` `tone7` `tone8` `tone9` `star` `pound` `a` `b` `c` `d` `flash` 。 |

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

