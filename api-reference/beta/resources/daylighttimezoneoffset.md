---
title: daylightTimeZoneOffset 资源类型
description: 指定时区何时从标准时间切换到夏令时。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: calendar
author: abheek-das
ms.openlocfilehash: 06d816085d13a6e921ebbdd98a9a18d72ecf289f
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65898061"
---
# <a name="daylighttimezoneoffset-resource-type"></a>daylightTimeZoneOffset 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定时区何时从标准时间切换到夏令时。

例如，如果为一个时区指定了以下属性：

- **bias** 为 300
- **daylightBias** 为 -100
- **dayOccurrence** 为 4
- **dayOfWeek** 为“sunday”
- **month** 为 5
- **time** 为 02:00:00 _ **year** 为 0，意味着夏令时的时长比 UTC 早 +300-100=200 分钟。 从夏令时到标准时间的时区切换出现在每年五月第四个星期日的早上 2 点。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
| daylightBias | Edm.Int32 | 夏时制与协调世界时 (UTC) 的时间偏移量。 此值以分钟为单位。  |
| dayOccurrence | Edm.Int32 | 表示从标准时间到夏令时的切换在一周的具体某天出现的次数。 |
| dayOfWeek | string | 表示从标准时间到夏令时的切换出现时一周的具体某日。 |
| month | Edm.Int32 | 表示从标准时间到夏令时的切换出现时一年的具体月份。 |
| time | Edm.TimeOfDay | 表示从标准时间到夏令时的切换出现时某日的具体时间。 |
| year | Edm.Int32 | 表示从标准时间到夏令时的变更出现时的年度频率。 例如，值为 0 意味着每年。|


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.daylightTimeZoneOffset"
}-->

```json
{
  "daylightBias": "Int32",
  "dayOccurrence": "Int32",
  "dayOfWeek": "string",
  "month": "Int32",
  "time": "TimeOfDay",
  "year": "Int32"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "daylightTimeZoneOffset resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


