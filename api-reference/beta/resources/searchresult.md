---
author: JeremyKelley
description: SearchResult 资源指示项是搜索查询的响应。
ms.date: 09/10/2017
title: Searchresult.xml
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: cc819d8b81138ef279735d1daead9839d7f3b93f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520883"
---
# <a name="searchresult-resource-type"></a>SearchResult 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**SearchResult** 资源指示项是搜索查询的响应。

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

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

<!--
{
  "type": "#page.annotation",
  "description": "The search result facet indicates an item is from a search.",
  "keywords": "search result facet",
  "section": "documentation",
  "tocPath": "Facets/SearchResult",
  "suppressions": []
}
-->
