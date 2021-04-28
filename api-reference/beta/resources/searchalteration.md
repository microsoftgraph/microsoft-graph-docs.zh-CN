---
title: searchAlteration 资源类型
description: 提供用于拼写更正的搜索更改的详细信息。
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 5caab3a3fbd8f8487e6893c5f5f530cc8471bb80
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52068000"
---
# <a name="searchalteration-resource-type"></a>searchAlteration 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

提供用于拼写更正的搜索更改的详细信息。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|alteredQueryString|String| 使用拼写更正定义更改的查询字符串。|
|alteredHighlightedQueryString|String| 使用拼写更正定义更改的突出显示查询字符串。 更正的线段周围的批注 (\ue000， \ue001) |
|alteredQueryTokens|[alteredQueryToken](alteredquerytoken.md) 集合| 表示与原始查询有关更改的线段。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchAlteration",
  "baseType": null
}-->

```json
{
  "alteredQueryString": "String",
  "alteredHighlightedQueryString": "String",
  "alteredQueryTokens": [{"@odata.type": "microsoft.graph.alteredQueryToken"}]
}
```