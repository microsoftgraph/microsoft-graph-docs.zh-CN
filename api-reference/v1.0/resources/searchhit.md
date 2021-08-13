---
title: searchHit 资源类型
description: searchHit 实体的说明
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 3cc9d069e91dd8c8d51ba6b010c2c3ccc9dad01ac01695d6782e99bffea973e3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54138327"
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

