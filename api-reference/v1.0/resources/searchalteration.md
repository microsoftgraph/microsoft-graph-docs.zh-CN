---
title: searchAlteration 资源类型
description: 提供有关用于拼写更正的搜索更改的详细信息。
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 9c89193a3d57f8dcb701e57e98160ee69b8a8a91
ms.sourcegitcommit: b19b19bf192688f4c513492e8391e4d8dc104633
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2022
ms.locfileid: "62878680"
---
# <a name="searchalteration-resource-type"></a>searchAlteration 资源类型

命名空间：microsoft.graph

提供有关用于拼写更正的搜索更改的详细信息。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|alteredHighlightedQueryString|String| 使用拼写更正定义更改的突出显示查询字符串。 更正的线段周围的注释是： `\ue000, \ue001`。|
|alteredQueryString|字符串| 使用拼写更正定义更改的查询字符串。|
|alteredQueryTokens|[alteredQueryToken](alteredquerytoken.md) 集合| 表示与原始用户查询相关的已更改的段。|

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
  "alteredHighlightedQueryString": "String",
  "alteredQueryString": "String",
  "alteredQueryTokens": [{"@odata.type": "microsoft.graph.alteredQueryToken"}]
}
```
