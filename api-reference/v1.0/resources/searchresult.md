---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: searchresult.xml
localization_priority: Normal
ms.openlocfilehash: ee6825860f5c1ed82c368b53eb3510175e7d3a11
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481228"
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
