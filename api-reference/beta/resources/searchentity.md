---
title: searchEntity 资源类型
description: 一个顶级对象，表示 Microsoft 搜索 API 终结点。
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: cb6d5bdd5288a3f6098f33d3432a0e4f0d7ac8bd
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193862"
---
# <a name="searchentity-resource-type"></a>searchEntity 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

一个顶级对象，表示 Microsoft 搜索 API 终结点。 它不像 Graph 中的任何其他资源一样工作，而是用作 [查询](../api/search-query.md) 操作的定位。 

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[查询](../api/search-query.md) |[searchResponse](searchresponse.md) 集合 | 运行请求正文中指定的查询。  |

## <a name="properties"></a>属性
无。

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.searchEntity",
  "baseType": "microsoft.graph.entity"
}
-->
``` json
{
  
}
```


## <a name="next-steps"></a>后续步骤

探索 [查询](../api/search-query.md) 操作。


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "A top level object representing the Microsoft Search API endpoint.",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


