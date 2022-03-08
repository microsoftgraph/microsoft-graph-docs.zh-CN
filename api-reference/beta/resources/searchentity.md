---
title: searchEntity 资源类型
description: 表示 API 终结点的顶级Microsoft 搜索对象。
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 39f5213e9be29f9fd87332513c3d0b090e3d3e1f
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335183"
---
# <a name="searchentity-resource-type"></a>searchEntity 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 API 终结点的顶级Microsoft 搜索对象。

它用作查询操作和搜索应答[](../api/search-query.md)关系（如首字母[缩写](../resources/search-acronym.md)词、书签和 [qnas）的定位点](../resources/search-qna.md)。 [](../resources/search-bookmark.md) 

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[查询](../api/search-query.md) |[searchResponse](searchresponse.md) 集合 | 运行指定的搜索查询。   |

## <a name="properties"></a>属性
无。

## <a name="relationships"></a>关系
| 关系 | 类型 |说明|
|:---------------|:--------|:----------|
| 首字母缩略词 | [microsoft.graph.search.acronym](../resources/search-acronym.md) 集合 | 用于定义Microsoft 搜索常见首字母缩略词的结果中的管理答案。  |
| bookmarks | [microsoft.graph.search.bookmark](../resources/search-bookmark.md) 集合 | 管理答案Microsoft 搜索组织中常见搜索查询的结果。 |
| qnas | [microsoft.graph.search.qna](../resources/search-qna.md) 集合 | 管理答案Microsoft 搜索结果，为组织的特定搜索关键字提供答案。 |


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


## <a name="see-also"></a>另请参阅

[查询](../api/search-query.md)


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "A top level object representing the Microsoft Search API endpoint.",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


