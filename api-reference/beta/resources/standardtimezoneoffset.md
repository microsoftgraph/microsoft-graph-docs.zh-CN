---
title: standardTimeZoneOffset 资源类型
description: 指定时区何时从夏令时切换到标准时间。
localization_priority: Normal
ms.openlocfilehash: cc3de9a0977caf6c222291fdff2b4e0f96a9d9e5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514479"
---
# <a name="standardtimezoneoffset-resource-type"></a>standardTimeZoneOffset 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
| dayOfWeek | string | 表示从夏令时切换为标准时间时一周的具体某日。 |
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
<!--
{
  "type": "#page.annotation",
  "description": "standardTimeZoneOffset resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/standardtimezoneoffset.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
