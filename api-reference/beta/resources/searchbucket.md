---
title: searchBucket 资源类型
description: 表示一个或多个搜索结果的容器，它们共享聚合它们的实体字段的相同值
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: e9323bac249216cc1355e3944f4437d738da89b1
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59764589"
---
# <a name="searchbucket-resource-type"></a>searchBucket 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示一个或多个搜索结果的容器，这些搜索结果与聚合它们的实体字段具有相同的值。 

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|aggregationFilterToken|String| 包含编码筛选器的令牌，用于按特定键值聚合 **搜索** 匹配项。 若要使用该筛选器，请以 **"{field}："{aggregationFilterToken} \\ \\ ""** 格式将令牌作为 **searchRequest** 对象 **中 aggregationFilter** 属性的一部分传递。 请参阅[示例](/graph/search-concept-aggregation#example-2-apply-an-aggregation-filter-based-on-a-previous-request)。|
|count|Int32| 共享 key 属性中指定的相同值的近似搜索 **匹配项** 数。 请注意，此数目不是匹配项的确切数量。|
|注册表项|String| 计算聚合的字段的离散值。|

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
