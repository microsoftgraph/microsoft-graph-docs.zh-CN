---
title: searchHitsContainer 资源类型
description: 表示搜索结果列表。
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 42abefb12b0ae1953caf9ecbfa04cd2bc29b69d8c9d8ca2a0797497efb8d6271
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54134957"
---
# <a name="searchhitscontainer-resource-type"></a>searchHitsContainer 资源类型

命名空间：microsoft.graph

表示搜索结果列表。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|hits|[searchHit](searchhit.md) 集合|搜索结果的集合。|
|moreResultsAvailable|Boolean|如果提供了更多结果，则提供相关信息。 根据此信息，您可以相应地调整 [searchRequest](searchrequest.md)的 **from** 和 **size** 属性。|
|total|Int32|结果总数。 请注意，这不是页面上的结果数，而是满足查询的结果总数。|


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
  "total": 1024
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


