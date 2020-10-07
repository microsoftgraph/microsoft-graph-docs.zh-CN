---
title: searchBucket 资源类型
description: 在响应中提供特定聚合，即特定存储桶的值。
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: a6b26c01133f519b0308ffee430d85c9df6d868b
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/07/2020
ms.locfileid: "48373851"
---
# <a name="searchbucket-resource-type"></a>searchBucket 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示一个或多个搜索结果的容器，这些搜索结果共享聚合它们的实体字段的相同值。 

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|Key|String| 计算聚合所依据的字段的离散值。|
|count|Int32| 与在 **key** 属性中指定的相同值共享的近似搜索匹配数。 请注意，此数字不是精确的匹配数。|
|aggregationFilterToken|String| 包含编码的筛选器的令牌，以聚合搜索匹配项的特定 **键值** 。 若要使用筛选器，请将令牌作为**searchRequest**对象中的**aggregationFilter**属性的一部分进行传递，格式为 **"{field}： \\ " {aggregationFilterToken} \\ ""**。 请参阅[示例](/graph/search-concept-aggregation#example-2-apply-an-aggregation-filter-based-on-a-previous-request)。|

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
