---
author: JeremyKelley
title: searchResult 资源类型
ms.localizationpriority: medium
description: searchResult 资源指示的不是项是对搜索查询的响应。
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: 376e0a709f7607215aac1b1509434549bd437db3
ms.sourcegitcommit: 423e698a580c3b902f2816b0216ab9d5b91e6d20
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2022
ms.locfileid: "66034794"
---
# <a name="searchresult-resource-type"></a>searchResult 资源类型

命名空间：microsoft.graph

**searchResult** 资源指示的不是项是对搜索查询的响应。

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "onClickTelemtryUrl" ],
  "@odata.type": "microsoft.graph.searchResult"
}-->

```json
{
  "onClickTelemetryUrl": "url"
}
```

## <a name="properties"></a>属性

| 属性            | 类型   | 说明
|:--------------------|:-------|:----------------------------------------------
| onClickTelemetryUrl | String | 可用于记录遥测信息的回调 URL。如果用户与此项交互以改善结果的质量，应用程序应在此 URL 中发出 GET。

## <a name="remarks"></a>注解 

有关 DriveItem 上的分面的详细信息，请参阅 [driveItem](driveitem.md)。

<!-- {
  "type": "#page.annotation",
  "description": "The search result facet indicates an item is from a search.",
  "keywords": "search result facet",
  "section": "documentation",
  "tocPath": "Facets/SearchResult"
} -->

