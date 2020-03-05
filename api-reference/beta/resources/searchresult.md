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
# <a name="searchresult-resource-type"></a><span data-ttu-id="39c4c-103">SearchResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="39c4c-103">SearchResult resource type</span></span>

<span data-ttu-id="39c4c-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="39c4c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39c4c-105">**SearchResult** 资源指示项是搜索查询的响应。</span><span class="sxs-lookup"><span data-stu-id="39c4c-105">The **SearchResult** resource indicates than an item is the response to a search query.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="json-representation"></a><span data-ttu-id="39c4c-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="39c4c-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="39c4c-107">属性</span><span class="sxs-lookup"><span data-stu-id="39c4c-107">Properties</span></span>

| <span data-ttu-id="39c4c-108">属性</span><span class="sxs-lookup"><span data-stu-id="39c4c-108">Property</span></span>            | <span data-ttu-id="39c4c-109">类型</span><span class="sxs-lookup"><span data-stu-id="39c4c-109">Type</span></span>   | <span data-ttu-id="39c4c-110">说明</span><span class="sxs-lookup"><span data-stu-id="39c4c-110">Description</span></span>
|:--------------------|:-------|:----------------------------------------------
| <span data-ttu-id="39c4c-111">onClickTelemetryUrl</span><span class="sxs-lookup"><span data-stu-id="39c4c-111">onClickTelemetryUrl</span></span> | <span data-ttu-id="39c4c-112">String</span><span class="sxs-lookup"><span data-stu-id="39c4c-112">String</span></span> | <span data-ttu-id="39c4c-p101">可用于记录遥测信息的回调 URL。如果用户与此项交互以改善结果的质量，应用程序应在此 URL 中发出 GET。</span><span class="sxs-lookup"><span data-stu-id="39c4c-p101">A callback URL that can be used to record telemetry information. The application should issue a GET on this URL if the user interacts with this item to improve the quality of results.</span></span>

## <a name="remarks"></a><span data-ttu-id="39c4c-115">注解</span><span class="sxs-lookup"><span data-stu-id="39c4c-115">Remarks</span></span>

<span data-ttu-id="39c4c-116">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="39c4c-116">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

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
