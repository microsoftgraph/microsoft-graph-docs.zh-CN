---
title: searchResultSet 资源类型
description: searchResultSet 的说明
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 5d17791a618f1d587520f23524da9ce19241d3b1
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067864"
---
# <a name="searchresultset-resource-type"></a>searchResultSet 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示来自搜索查询的结果，以及用于查询的术语。 

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|hitsContainers|[searchHitsContainer](searchhitscontainer.md) 集合|搜索结果的集合。|
|searchTerms|字符串集合|包含初始搜索查询中发送的搜索词。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchResultSet",
  "baseType": null
}-->

```json
{
  "hitsContainers": [{"@odata.type": "microsoft.graph.searchHitsContainer"}],
  "searchTerms": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchResultSet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

