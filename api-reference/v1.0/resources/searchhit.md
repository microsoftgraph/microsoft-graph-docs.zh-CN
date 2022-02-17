---
title: searchHit 资源类型
description: searchHit 实体的说明
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 487fbee4e501b6d4154b1ed08102730fd278730c
ms.sourcegitcommit: b19b19bf192688f4c513492e8391e4d8dc104633
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2022
ms.locfileid: "62878825"
---
# <a name="searchhit-resource-type"></a>searchHit 资源类型

命名空间：microsoft.graph

表示搜索结果列表中的单个结果。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|contentSource|String|**externalItem** 是 的内容源的名称。|
|hitId|String|项的内部标识符。|
|排名|Int32|结果的排名或顺序。|
|resultTemplateId|String|用于呈现搜索结果的结果模板的 ID。 此 ID 必须映射到 [searchResponse](searchresponse.md) 中也包含的 **resultTemplates** 字典中的显示布局。|
|resource|[实体](entity.md)|基础 Microsoft Graph搜索结果的表示形式。|
|摘要|String|结果摘要（如果摘要可用）。|

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
  "contentSource": "String",
  "hitId": "String",
  "rank": "Int32",
  "resultTemplateId": "String",
  "resource": { "@odata.type": "microsoft.graph.entity" },
  "summary": "String"
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

