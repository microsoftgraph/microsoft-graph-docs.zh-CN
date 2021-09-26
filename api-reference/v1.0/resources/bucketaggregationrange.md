---
title: bucketAggregationRange 资源类型
description: 指定聚合搜索结果的范围下限和上限。 仅适用于日期或数值类型的精简条件
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 8199abddd8e098e40f101459d197adaa41f33ff0
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59777194"
---
# <a name="bucketaggregationrange-resource-type"></a>bucketAggregationRange 资源类型

命名空间：microsoft.graph

指定聚合搜索结果的范围下限和上限。 仅适用于日期或数字类型的精简条件。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|from|String| 定义用于计算聚合的下限。 这可以是数字值，或者是使用格式的日期的字符串 `YYYY-MM-DDTHH:mm:ss.sssZ` 表示形式。 必需。|
|更改为|String| 定义要计算聚合的上限。 这可以是数字值，或者是使用格式的日期的字符串 `YYYY-MM-DDTHH:mm:ss.sssZ` 表示形式。 此为必需属性。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bucketAggregationRange",
  "baseType": null
}-->

```json
{
  "from": "String",
  "to": "String"
}
```
