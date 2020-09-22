---
title: searchHit 资源类型
description: SearchHit 实体的说明
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: c140a30d4e77840b1fd7c7ccceec16e0554cd855
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193608"
---
# <a name="searchhit-resource-type"></a>searchHit 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [search-api-deprecation](../../includes/search-api-deprecation.md)]

代表搜索结果列表中的单个结果。

## <a name="properties"></a>属性

| 属性     | 类型        | 描述 |
|:-------------|:------------|:------------|
|hitId|字符串|项的内部标识符。|
|排名|Int32|结果的排名或顺序。|
|contentSource|字符串|**ExternalItem**所属的内容源的名称。|
|摘要|字符串|如果摘要可用，则为结果摘要。|
|resource|[实体](entity.md)|搜索结果的基本 Microsoft Graph 表示形式。|
|_id (已弃用) |字符串| 重命名为 **hitId**。 项的内部标识符。|
|_score (已弃用) |Int32|重命名为 **rank**。 结果的分数或顺序。|
|_summary (已弃用) |字符串|重命名为 **摘要**。  (如果摘要可用) 的结果摘要。|
|_sortField (已弃用) |字符串|此属性已被删除。|
|_source (已弃用) |[实体](entity.md)|重命名为 **资源**。 搜索结果的基础图形表示形式。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchHit",
  "baseType": null
}-->

```json
{
  "hitId": "String",
  "rank": 1,
  "summary": "String",
  "contentSource": "String",
  "resource": { "@odata.type": "microsoft.graph.entity" },
  "_id": "String",
  "_score": 1024,
  "_sortField": "String",
  "_summary": "String",
  "_source": { "@odata.type": "microsoft.graph.entity" }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchHit resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

