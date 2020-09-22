---
title: bucketAggregationRange 资源类型
description: 允许在聚合请求中指定一些手动范围。 这仅适用于非字符串精简程序：数值和日期。
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 77f89503a8f19bd8b057575643ebf89e6dbc43a8
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193868"
---
# <a name="bucketaggregationrange-resource-type"></a>bucketAggregationRange 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定用于聚合搜索结果的范围的下限和上限。 仅适用于日期或数值类型的精简程序。

## <a name="properties"></a>属性

| 属性     | 类型        | 描述 |
|:-------------|:------------|:------------|
|from|字符串| 定义从中计算聚合的下限。 它可以是数字值，也可以是使用格式的日期的字符串表示形式 `YYYY-MM-DDTHH:mm:ss.sssZ` 。 必需。|
|更改为|字符串| 定义要计算聚合的上限。 它可以是数字值，也可以是使用格式的日期的字符串表示形式 `YYYY-MM-DDTHH:mm:ss.sssZ` 。 此为必需属性。|

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
