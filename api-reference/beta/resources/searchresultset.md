---
title: searchResultSet 资源类型
description: searchResultSet 的说明
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: ee5ac6d892b6562ca5c1053b474135f1dd745ba5
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210204"
---
# <a name="searchresultset-resource-type"></a>searchResultSet 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示来自搜索查询的结果，以及用于查询的术语。 

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|hitsContainers|[searchHitsContainer](searchhitscontainer.md) 集合|搜索结果的集合。|
|searchTerms|String collection|包含初始搜索查询中发送的搜索词。|
|resultTemplates|[resultTemplate](resultTemplate.md) 集合|resultTemplateIds 和关联值的字典，其中包括结果模板的名称和 JSON 架构。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchResultSet",
  "baseType": null
}-->

```json
{
  "hitsContainers": [{"@odata.type": "microsoft.graph.searchHitsContainer"}],
  "searchTerms": ["String"],
  "resultTemplates": [{"@odata.type":"microsoft.graph.resultTemplateDictionary"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchResultSet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

