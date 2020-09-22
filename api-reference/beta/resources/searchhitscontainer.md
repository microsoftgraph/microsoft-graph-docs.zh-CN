---
title: searchHitsContainer 资源类型
description: 表示搜索结果的列表。
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: a2d120722179cb0fd771a84f867948a7fbfffdd4
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48192782"
---
# <a name="searchhitscontainer-resource-type"></a>searchHitsContainer 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示搜索结果的列表。

## <a name="properties"></a>属性

| 属性     | 类型        | 描述 |
|:-------------|:------------|:------------|
|影响|[searchHit](searchhit.md) 集合|搜索结果的集合。|
|moreResultsAvailable|Boolean|如果有更多结果可用，则提供信息。 根据此信息，您可以相应地调整[searchRequest](searchrequest.md)的 " **from** " 和 " **size** " 属性。|
|total|Int32|总结果数。 注释这不是页面上的结果数，而是满足查询的总结果数。|
|aggregations|[searchAggregation](searchaggregation.md) 集合|包含根据请求中指定的提供的 [aggregationOption](aggregationoption.md) 计算出的聚合集合。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchHitsContainer",
  "baseType": null
}-->


```json
{
  "hits": [{"@odata.type": "microsoft.graph.searchHit"}],
  "moreResultsAvailable": true,
  "total": 1024,
  "aggregations": [{"@odata.type": "microsoft.graph.searchAggregation"}]
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchHitsContainer resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


