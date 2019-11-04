---
title: searchQuery 资源类型
description: searchQuery
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 3cb46a41b0c46fe5f70d94a64a91489c9c2e7d43
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936585"
---
# <a name="searchquery-resource-type"></a>searchQuery 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示包含搜索词和可选筛选器的搜索查询。

## <a name="properties"></a>属性

| 属性     | 类型        | 描述 |
|:-------------|:------------|:------------|
|query_string|[searchQueryString](searchquerystring.md)|包含搜索词的搜索查询。|

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