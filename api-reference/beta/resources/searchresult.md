---
author: JeremyKelley
description: SearchResult 资源指示项是搜索查询的响应。
ms.date: 09/10/2017
title: Searchresult.xml
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: fa2d8b59c2046efb1ff0e995af429f85c8deeba3
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703924"
---
# <a name="searchresult-resource-type"></a><span data-ttu-id="97ee4-103">SearchResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="97ee4-103">SearchResult resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97ee4-104">**SearchResult** 资源指示项是搜索查询的响应。</span><span class="sxs-lookup"><span data-stu-id="97ee4-104">The **SearchResult** resource indicates than an item is the response to a search query.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="json-representation"></a><span data-ttu-id="97ee4-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="97ee4-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="97ee4-106">属性</span><span class="sxs-lookup"><span data-stu-id="97ee4-106">Properties</span></span>

| <span data-ttu-id="97ee4-107">属性</span><span class="sxs-lookup"><span data-stu-id="97ee4-107">Property</span></span>            | <span data-ttu-id="97ee4-108">类型</span><span class="sxs-lookup"><span data-stu-id="97ee4-108">Type</span></span>   | <span data-ttu-id="97ee4-109">说明</span><span class="sxs-lookup"><span data-stu-id="97ee4-109">Description</span></span>
|:--------------------|:-------|:----------------------------------------------
| <span data-ttu-id="97ee4-110">onClickTelemetryUrl</span><span class="sxs-lookup"><span data-stu-id="97ee4-110">onClickTelemetryUrl</span></span> | <span data-ttu-id="97ee4-111">String</span><span class="sxs-lookup"><span data-stu-id="97ee4-111">String</span></span> | <span data-ttu-id="97ee4-p101">可用于记录遥测信息的回调 URL。如果用户与此项交互以改善结果的质量，应用程序应在此 URL 中发出 GET。</span><span class="sxs-lookup"><span data-stu-id="97ee4-p101">A callback URL that can be used to record telemetry information. The application should issue a GET on this URL if the user interacts with this item to improve the quality of results.</span></span>

## <a name="remarks"></a><span data-ttu-id="97ee4-114">注解</span><span class="sxs-lookup"><span data-stu-id="97ee4-114">Remarks</span></span>

<span data-ttu-id="97ee4-115">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="97ee4-115">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

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
