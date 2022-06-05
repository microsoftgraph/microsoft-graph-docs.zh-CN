---
title: FilterDatetime 资源类型
description: 表示在筛选值时如何筛选日期。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: workbooks-and-charts
author: ruoyingl
ms.openlocfilehash: f57ab1fbd17d31568dfdc17d6f7cb4baa379bb06
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65899986"
---
# <a name="filterdatetime-resource-type"></a>FilterDatetime 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示在筛选值时如何筛选日期。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|date|string|用于筛选数据的采用 ISO8601 格式的日期。|
|specificity|string|用于保留数据的日期的具体程度。例如，如果日期是 2005-04-02 并将特殊性设置为“月”，则筛选操作将保留包含 2009 年 4 月日期的所有行。可能的值是：`Year`、`Monday`、`Day`、`Hour`、`Minute`、`Second`。|

## <a name="relationships"></a>关系
无


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterDateTime"
}-->

```json
{
  "date": "string",
  "specificity": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "FilterDatetime resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


