---
title: stringKeyLongValuePair 资源类型
description: 表示其中的密钥是一个字符串，并且值为 Int64 的键 / 值对。
localization_priority: Normal
ms.openlocfilehash: 21d081dcb488c406bc0971f6b1aeadacfcc8c208
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812234"
---
# <a name="stringkeylongvaluepair-resource-type"></a>stringKeyLongValuePair 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

表示其中的密钥是一个字符串，并且值为 Int64 的键 / 值对。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|Key|字符串|键。|
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
<!-- {
  "type": "#page.annotation",
  "description": "stringKeyLongValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
