---
title: searchHit 资源类型
description: searchHit 实体的说明
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 7c546483eea81e7d89a3a87ba5b8c0eb0ff48783
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210330"
---
# <a name="searchhit-resource-type"></a>searchHit 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [search-api-deprecation](../../includes/search-api-deprecation.md)]

表示搜索结果列表中的单个结果。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|hitId|String|项的内部标识符。|
|排名|Int32|结果的排名或顺序。|
|contentSource|String|**externalItem** 是 的内容源的名称。|
|摘要|String|结果摘要（如果摘要可用）。|
|resultTemplateId|String|用于呈现搜索结果的结果模板的 ID。 此 ID 必须映射到 **resultTemplates** 字典（也包含在 [searchresponse](searchresponse.md) 中）中的显示布局。|
|resource|[实体](entity.md)|基础 Microsoft Graph搜索结果的表示形式。|
|_id (弃用) |String| 重命名为 **hitId**。 项的内部标识符。|
|_score (弃用) |Int32|重命名为 **排名**。 结果的分数或顺序。|
|_summary (弃用) |String|重命名为 **摘要**。 如果摘要可用， (结果摘要) 。|
|_sortField (弃用) |String|此属性已删除。|
|_source (弃用) |[实体](entity.md)|重命名为 **资源**。 基础Graph搜索结果的表示形式。|

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
  "resultTemplateId": "String",
  "contentSource": "String",
  "resource": { "@odata.type": "microsoft.graph.entity" },
  "_id": "String",
  "_score": 1024,
  "_sortField": "String",
  "_summary": "String",
  "_source": { "@odata.type": "microsoft.graph.entity" }
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

