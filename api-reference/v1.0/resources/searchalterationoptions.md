---
title: searchAlterationOptions 资源类型
description: 提供用于拼写更正的搜索更改选项。
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 1692cf40700c9af40b4ecab77b32210291e60f78
ms.sourcegitcommit: b19b19bf192688f4c513492e8391e4d8dc104633
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2022
ms.locfileid: "62878676"
---
# <a name="searchalterationoptions-resource-type"></a>searchAlterationOptions 资源类型

命名空间：microsoft.graph

提供用于拼写更正的搜索更改选项。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|enableModification|布尔|指示是否启用拼写修改。 如果启用，如果原始查询没有拼写错误的结果，用户将获取更正的查询的搜索结果。 该 [响应](/graph/api/resources/searchresponse) 还将在 **queryAlterationResponse 属性中包括拼写修改** 信息。 可选。|
|enableSuggestion|布尔|指示是否启用拼写建议。 如果启用，用户将获取原始搜索查询的搜索结果，以及查询中拼写错误的响应的 **queryAlterationResponse** 属性中的拼写更正建议。[](/graph/api/resources/searchresponse) 可选。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchAlterationOptions",
  "baseType": null
}-->

```json
{
  "enableModification": "Boolean",
  "enableSuggestion": "Boolean"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchAlterationOptions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
