---
title: searchHitsContainer 资源类型
description: 在此处提供说明
localization_priority: Normal
author: nmoreau
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 0bb960156a6c8f3a407dbd0691cdbed32e03693d
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703910"
---
# <a name="searchhitscontainer-resource-type"></a>searchHitsContainer 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示搜索结果的列表。

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|影响|[searchHit](searchhit.md)集合|Encasulate 搜索结果。|
|moreResultsAvailable|Boolean|如果有更多结果可用，则提供信息。 在这种情况下，您可以增加 "from" 和 "to" 偏移量。|
|total|Int32|总结果数。 注释这不是页面结果中的数值，而是满足查询的结果总数。|

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