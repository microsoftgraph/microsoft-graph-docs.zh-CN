---
title: searchBucket 资源类型
description: 在响应中提供特定聚合，即特定存储桶的值。
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 3fe375ca2e9695a237b60e30cdd9e98a9e545d35
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193858"
---
# <a name="searchbucket-resource-type"></a>searchBucket 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示一个或多个搜索结果的容器，这些搜索结果共享聚合它们的实体字段的相同值。 



## <a name="properties"></a>属性

| 属性     | 类型        | 描述 |
|:-------------|:------------|:------------|
|Key|字符串| 计算聚合所依据的字段的离散值。|
|count|Int32| 与 **key** 属性中指定的值相同的搜索匹配项的数量。 |
|aggregationFilterToken|字符串| 包含编码的筛选器的令牌，以聚合搜索匹配项的特定 **键值** 。 若要使用筛选器，请将令牌作为**searchRequest**对象中的**aggregationFilter**属性的一部分进行传递，格式为 **"{field}： \\ " {aggregationFilterToken} \\ ""**。 请参阅[示例](/graph/search-concept-aggregation#example-2-apply-an-aggregation-filter-based-on-a-previous-request)。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchBucket",
  "baseType": null
}-->

```json
{
  "key": "String",
  "count": "10",  
  "aggregationFilterToken": "String"
}
```
