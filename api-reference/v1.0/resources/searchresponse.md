---
title: searchResponse 资源类型
description: searchResponse 的说明
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: b7d5668a86204e95e3f0f5e024ec985f98027ac9
ms.sourcegitcommit: b19b19bf192688f4c513492e8391e4d8dc104633
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2022
ms.locfileid: "62878650"
---
# <a name="searchresponse-resource-type"></a>searchResponse 资源类型

命名空间：microsoft.graph

表示来自搜索查询的结果，以及用于查询的术语。 

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|hitsContainers|[searchHitsContainer](searchhitscontainer.md) 集合|搜索结果的集合。|
|resultTemplates|[resultTemplate](resulttemplate.md) 集合|**resultTemplateIds** 和关联值的字典，其中包括结果模板的名称和 JSON 架构。|
|searchTerms|String 集合|包含初始搜索查询中发送的搜索词。|
|queryAlterationResponse|[更改response](alterationresponse.md)|提供与更改响应中的拼写更正有关的信息。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchResponse",
  "baseType": null
}-->

```json
{
  "hitsContainers": [{"@odata.type": "microsoft.graph.searchHitsContainer"}],
  "queryAlterationResponse": {"@odata.type": "microsoft.graph.alterationResponse"},
  "resultTemplates": [{"@odata.type":"microsoft.graph.resultTemplateDictionary"}],
  "searchTerms": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchResponse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

