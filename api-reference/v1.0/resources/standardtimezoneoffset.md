---
title: standardTimeZoneOffset 资源类型
description: 指定时区何时从夏令时切换到标准时间。
localization_priority: Normal
author: abheek-das
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 2e5675a4b63a4842b8470f0631a1819e5dd63570a9a2252448b52abb883b8de4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54180458"
---
# <a name="standardtimezoneoffset-resource-type"></a>standardTimeZoneOffset 资源类型

命名空间：microsoft.graph

指定时区何时从夏令时切换到标准时间。

例如，如果为一个时区指定了以下属性：

- **dayOccurrence** 为 3
- **dayOfWeek** 为“Sunday”
- **month** 为 10
- **time** 为 02:00:00 _ **year** 为 0，这意味着从夏令时切换到标准时间出现在每年十月第三个星期日的早上 2 点。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
| dayOccurrence | Edm.Int32 | 表示从夏令时到标准时间的切换在一周的具体某天出现的次数。 |
| dayOfWeek | dayOfWeek | 表示从夏令时切换为标准时间时一周的具体某日。 |
| month | Edm.Int32 | 表示从夏令时到标准时间的切换出现时一年的具体月份。 |
| time | Edm.TimeOfDay | 表示从夏令时到标准时间的切换出现时某日的具体时间。 |
| year | Edm.Int32 | 表示从夏令时到标准时间的变更出现时的年度频率。 例如，值为 0 意味着每年。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.standardTimeZoneOffset"
}-->

```json
{
  "dayOccurrence": "Int32",
  "dayOfWeek": "string",
  "month": "Int32",
  "time": "TimeOfDay",
  "year": "Int32"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "standardTimeZoneOffset resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

