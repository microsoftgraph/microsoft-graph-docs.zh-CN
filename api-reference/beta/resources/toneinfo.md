---
title: toneInfo 资源类型
description: 单个 DTMF 事件。
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: b9be7e0e69be8d127df92f717ab462021f9684b7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817106"
---
# <a name="toneinfo-resource-type"></a>toneInfo 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

单个 DTMF 事件。

## <a name="properties"></a>属性

| 属性       | 类型    | Description|
|:---------------|:--------|:----------|
| sequenceId | Int64 | 用于排序 DTMF 事件增量标识符。 |
| 音 | 字符串 | 可能的值为： `tone0`， `tone1`， `tone2`， `tone3`， `tone4`， `tone5`， `tone6`， `tone7`， `tone8`， `tone9`， `star`， `pound`， `a`， `b`， `c`， `d`， `flash`。 |

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
<!-- {
  "type": "#page.annotation",
  "description": "toneInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
