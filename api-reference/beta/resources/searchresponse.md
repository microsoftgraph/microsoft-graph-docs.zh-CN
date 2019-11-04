---
title: searchResponse 资源类型
description: 在此处提供说明
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 7e68eae7c31486646c4b3d135881fd04fa8c7222
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938756"
---
# <a name="searchresponse-resource-type"></a>searchResponse 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

SearchResponse 包含搜索查询中的结果。

## <a name="properties"></a>属性

| 属性     | 类型        | 描述 |
|:-------------|:------------|:------------|
|hitsContainers|[searchHitsContainer](searchhitscontainer.md)集合|搜索结果的集合。|
|searchTerms|String collection|包含在初始搜索查询中发送的搜索词。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchResponse",
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
  "description": "searchResponse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->