---
title: aggregationOption 资源类型
description: 指定应在搜索结果旁边返回哪些聚合
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: c7cf67209fe7b043dcbf391322d3cc65db2a9b3a
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59766017"
---
# <a name="aggregationoption-resource-type"></a>aggregationOption 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定应在搜索结果旁边返回哪些聚合。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------| 
|bucketDefinition|[bucketAggregationDefinition](bucketaggregationdefinition.md)|指定计算聚合的条件。 可选。|
|字段|String|在当前实体类型中存在字段时计算字段的聚合。 必需。|
|大小|Int32|要返回 [的 searchBucket](searchBucket.md) 资源的数量。 当搜索请求中手动提供范围时，不需要这样做。 可选。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.aggregationOption",
  "baseType": null
}-->

```json
{
  "field": "String",
  "size": 1024,
  "bucketDefinition": {"@odata.type": "microsoft.graph.bucketAggregationDefinition"}
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