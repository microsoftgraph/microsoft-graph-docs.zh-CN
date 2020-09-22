---
title: bucketAggregationDefinition 资源类型
description: 提供有关如何在结果中生成 agregations 的详细信息
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 1f9fdadefc43b99b8772217db9a9b101357a1c9c
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193869"
---
# <a name="bucketaggregationdefinition-resource-type"></a>bucketAggregationDefinition 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定聚合搜索结果的详细信息。

## <a name="properties"></a>属性

| 属性     | 类型        | 描述 |
|:-------------|:------------|:------------|
|sortBy|bucketAggregationSortProperty| 可能的值是 `count` 按聚合中的匹配项数进行排序，基于聚合中的键对 `keyAsString` alphabeticaly 进行排序，以 `keyAsNumber` 实现基于聚合中键的数值排序。 必需。
|isDescending|Boolean|`True` 指定排序次序为降序。 默认值为 `false` ，排序次序为升序。 可选。|
|prefixFilter|字符串|用于定义匹配条件的筛选器。 该密钥应以指定的前缀开头，以在响应中返回。 可选。|
|minimumCount|Int32|应在存储桶中返回的聚合中应存在的最小项目数。 可选。|
|ranges|[bucketAggregationRange](bucketaggregationrange.md) 集合|指定用于计算聚合的手动范围。 这仅对日期或数值类型的非字符串精简程序有效。 可选。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bucketAggregationDefinition",
  "baseType": null
}-->

```json
{
  "sortBy": "String",
  "isDescending": true,
  "prefixFilter": "String",
  "minimumCount": 1024,
  "ranges": [{"@odata.type": "microsoft.graph.bucketAggregationRange"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sortProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->