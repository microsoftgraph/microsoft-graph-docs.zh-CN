---
title: searchHit 资源类型
description: searchHit 实体的说明
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: e64d4d3a2d7599df3ce6674abab352ab474ae18f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59137544"
---
# <a name="searchhit-resource-type"></a>searchHit 资源类型

命名空间：microsoft.graph

表示搜索结果列表中的单个结果。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|hitId|String|项的内部标识符。|
|排名|Int32|结果的排名或顺序。|
|contentSource|String|**externalItem** 是 的内容源的名称。|
|摘要|String|结果摘要（如果摘要可用）。|
|resource|[实体](entity.md)|基础 Microsoft Graph搜索结果的表示形式。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchHit",
  "baseType": null
}-->

```json
{
  "hitId": "String",
  "rank": 1,
  "summary": "String",
  "contentSource": "String",
  "resource": { "@odata.type": "microsoft.graph.entity" }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchHit resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

