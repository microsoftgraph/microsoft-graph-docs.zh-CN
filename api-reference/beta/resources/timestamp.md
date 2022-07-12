---
title: timeStamp 资源类型
description: 时间点的日期和时间信息。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
author: JeremyKelley
ms.openlocfilehash: fb82ddf1e69b8ea06cb425ed5199d1f6c5862b52
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2022
ms.locfileid: "66737103"
---
# <a name="timestamp-resource-type"></a>timeStamp 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

时间点的日期和时间信息。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|date|Date|时间戳的日期部分。|
|time|TimeOfDay|时间戳的时间部分。|
|timeZone|String|时间戳的时区部分，它是世界上 24 个纵向区域之一。|

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeStamp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


