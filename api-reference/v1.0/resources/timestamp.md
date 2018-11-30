---
title: 时间戳资源类型
description: 日期和时间点时间信息。
ms.openlocfilehash: 4f392e880bb165841fd8a9a31b6ed00bf2ba36fb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008356"
---
# <a name="timestamp-resource-type"></a>时间戳资源类型

日期和时间点时间信息。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeStamp"
}-->

```json
{
  "date": "String (timestamp)",
  "time": "String (timestamp)",
  "timeZone": "string"
}

```
## <a name="properties"></a>属性
| 属性       | 类型    |说明|
|:---------------|:--------|:----------|
|date|Date|时间戳日期部分。|
|time|TimeOfDay|时间戳时间部分中。|
|timeZone|字符串|时间戳，这是一个世界上 24 纵向方面 timezone 部分。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeStamp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->