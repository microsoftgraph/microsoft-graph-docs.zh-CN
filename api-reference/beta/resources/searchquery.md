---
title: searchQuery 资源类型
description: searchQuery
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 1d2d643fed135f97f1ccf2c6346d8fdd6e22f8b5
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193363"
---
# <a name="searchquery-resource-type"></a>searchQuery 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [search-api-deprecation](../../includes/search-api-deprecation.md)]

表示包含搜索词和可选筛选器的搜索查询。

## <a name="properties"></a>属性

| 属性     | 类型        | 描述 |
|:-------------|:------------|:------------|
|queryString|字符串|包含搜索词的搜索查询。 必需。|
|query_string (已弃用) |[searchQueryString](searchquerystring.md)|现在，它将替换为 **queryString** 属性。 包含搜索词的搜索查询。|


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchQuery",
  "baseType": null
}-->

```json
{
  "queryString": "String",
  "query_string": {"@odata.type": "microsoft.graph.searchQueryString"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchQuery resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

