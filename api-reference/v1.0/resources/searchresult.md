---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SearchResult
ms.openlocfilehash: 33ce07c947d858f05844dd9dc2589379131c9dbb
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="searchresult-resource-type"></a>SearchResult 资源类型

**SearchResult** 资源指示项是搜索查询的响应。

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

有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。

<!-- {
  "type": "#page.annotation",
  "description": "The search result facet indicates an item is from a search.",
  "keywords": "search result facet",
  "section": "documentation",
  "tocPath": "Facets/SearchResult"
} -->
