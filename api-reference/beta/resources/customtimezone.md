---
title: customTimeZone 资源类型
description: 表示从标准时间到夏令时的切换不标准（反之亦然）的时区。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: calendar
author: abheek-das
ms.openlocfilehash: 9c7b240a010a5fb729cd12770648634decadf284
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900182"
---
# <a name="customtimezone-resource-type"></a>customTimeZone 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示从标准时间到夏令时的切换不标准（反之亦然）的时区。


## <a name="properties"></a>属性
| 属性 | 类型   |说明|
|:---------------|:--------|:----------|
| bias | Edm.Int32 | 时区与协调世界时 (UTC) 的时间偏移量。 此值以分钟为单位。 早于 UTC 的时区为正偏移；晚于 UTC 的时区为负偏移。|
| daylightOffset | [daylightTimeZoneOffset](daylighttimezoneoffset.md) | 指定时区何时从标准时间切换到夏令时。 |
| name | string | 自定义时区的名称。 |
| standardOffset | [standardTimeZoneOffset](standardtimezoneoffset.md) | 指定时区何时从夏令时切换到标准时间。 |


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.customTimeZone"
}-->

```json
{
  "bias": "Int32",
  "daylightOffset": {"@odata.type": "microsoft.graph.daylightTimeZoneOffset"},
  "name": "string",
  "standardOffset": {"@odata.type": "microsoft.graph.standardTimeZoneOffset"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "customTimeZone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


