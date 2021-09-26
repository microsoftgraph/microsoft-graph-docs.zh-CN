---
title: bucketAggregationDefinition 资源类型
description: 提供在结果中如何生成注册的详细信息
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 57bda80518e176e353f8521929c4ec695363ddf9
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59766339"
---
# <a name="bucketaggregationdefinition-resource-type"></a>bucketAggregationDefinition 资源类型

命名空间：microsoft.graph

提供有关如何在结果中生成 agregations 的详细信息。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|isDescending|Boolean|`True` 将排序顺序指定为降序。 默认值为 `false` ，按升序排序。 可选。|
|minimumCount|Int32|聚合中应存在于存储桶中返回的最小项目数。 可选。|
|prefixFilter|String|用于定义匹配条件的筛选器。 键应从响应中返回的指定前缀开始。 可选。|
|ranges|[bucketAggregationRange](bucketaggregationrange.md) 集合|指定计算聚合的手动范围。 这仅适用于日期或数值类型的非字符串精简条件。 可选。|
|sortBy|bucketAggregationSortProperty| 可能的值为按聚合中的匹配数进行排序，根据聚合中的键按字母顺序排序，根据聚合中的键进行数字 `count` `keyAsString` `keyAsNumber` 排序。 此为必需属性。

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