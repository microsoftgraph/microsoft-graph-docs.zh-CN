---
title: searchQueryString 资源类型
description: searchQueryString
localization_priority: Normal
author: nmoreau
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 93142dcc672c5fee18a5f98d0988352e6c02cbd0
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37935264"
---
# <a name="searchquerystring-resource-type"></a>searchQueryString 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

查询的搜索词。

## <a name="properties"></a>属性

| 属性     | 类型        | 描述 |
|:-------------|:------------|:------------|
|查询|字符串|包含请求的实际搜索词。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchQueryString",
  "baseType": null
}-->

```json
{
  "query": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchQueryString resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->