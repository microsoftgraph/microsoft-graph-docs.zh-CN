---
title: searchAggregation 资源类型
description: 提供搜索响应中的搜索聚合的详细信息。
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 480a6f70a2815a174697ff22fc217057053e1f4b
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193860"
---
# <a name="searchaggregation-resource-type"></a>searchAggregation 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

提供搜索响应中的搜索聚合的详细信息。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|displayName|字符串| 聚合的友好名称。 输入中提供了此值。|
|字段|字符串| 定义在哪一字段上计算聚合。|
|buckets|[searchBucket](searchbucket.md) 集合| 定义计算出的聚合的实际存储桶。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchAggregation",
  "baseType": null
}-->

```json
{
  "displayName": "String",
  "field": "String",  
  "buckets": [{"@odata.type": "microsoft.graph.searchBucket"}]
}
```