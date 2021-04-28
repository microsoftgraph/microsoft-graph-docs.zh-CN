---
title: searchResponse 资源类型
description: searchResponse 的说明
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 5778d82c0c4718b9f34c686a613270eebfcc56e1
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067087"
---
# <a name="searchresponse-resource-type"></a>searchResponse 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示来自搜索查询的响应。 

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|queryAlterationResponse|[更改response](alterationResponse.md)|提供用于拼写更正的查询更改响应的详细信息。|
|值|[searchResultSet](searchResultSet.md) 集合|表示来自搜索查询的结果，以及用于查询的术语。|

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
  "queryAlterationResponse": {"@odata.type": "microsoft.graph.alterationResponse"},
  "value": [{"@odata.type": "microsoft.graph.searchResultSet"}]
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

