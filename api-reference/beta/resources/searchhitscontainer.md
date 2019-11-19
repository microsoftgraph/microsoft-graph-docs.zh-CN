---
title: searchHitsContainer 资源类型
description: 在此处提供说明
localization_priority: Normal
author: nmoreau
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 0bb960156a6c8f3a407dbd0691cdbed32e03693d
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703910"
---
# <a name="searchhitscontainer-resource-type"></a><span data-ttu-id="0a821-103">searchHitsContainer 资源类型</span><span class="sxs-lookup"><span data-stu-id="0a821-103">searchHitsContainer resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a821-104">表示搜索结果的列表。</span><span class="sxs-lookup"><span data-stu-id="0a821-104">Represent the list of search results.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="0a821-105">属性</span><span class="sxs-lookup"><span data-stu-id="0a821-105">Properties</span></span>

| <span data-ttu-id="0a821-106">属性</span><span class="sxs-lookup"><span data-stu-id="0a821-106">Property</span></span>     | <span data-ttu-id="0a821-107">类型</span><span class="sxs-lookup"><span data-stu-id="0a821-107">Type</span></span>        | <span data-ttu-id="0a821-108">说明</span><span class="sxs-lookup"><span data-stu-id="0a821-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0a821-109">影响</span><span class="sxs-lookup"><span data-stu-id="0a821-109">hits</span></span>|<span data-ttu-id="0a821-110">[searchHit](searchhit.md)集合</span><span class="sxs-lookup"><span data-stu-id="0a821-110">[searchHit](searchhit.md) collection</span></span>|<span data-ttu-id="0a821-111">Encasulate 搜索结果。</span><span class="sxs-lookup"><span data-stu-id="0a821-111">Encasulate the Search results.</span></span>|
|<span data-ttu-id="0a821-112">moreResultsAvailable</span><span class="sxs-lookup"><span data-stu-id="0a821-112">moreResultsAvailable</span></span>|<span data-ttu-id="0a821-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="0a821-113">Boolean</span></span>|<span data-ttu-id="0a821-114">如果有更多结果可用，则提供信息。</span><span class="sxs-lookup"><span data-stu-id="0a821-114">Provides information if more results are available.</span></span> <span data-ttu-id="0a821-115">在这种情况下，您可以增加 "from" 和 "to" 偏移量。</span><span class="sxs-lookup"><span data-stu-id="0a821-115">In that case you can increase the "from" and "to" offset.</span></span>|
|<span data-ttu-id="0a821-116">total</span><span class="sxs-lookup"><span data-stu-id="0a821-116">total</span></span>|<span data-ttu-id="0a821-117">Int32</span><span class="sxs-lookup"><span data-stu-id="0a821-117">Int32</span></span>|<span data-ttu-id="0a821-118">总结果数。</span><span class="sxs-lookup"><span data-stu-id="0a821-118">The total number of results.</span></span> <span data-ttu-id="0a821-119">注释这不是页面结果中的数值，而是满足查询的结果总数。</span><span class="sxs-lookup"><span data-stu-id="0a821-119">Note this is not the number on results in the page, but the total number of results satisfying the query.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0a821-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0a821-120">JSON representation</span></span>

<span data-ttu-id="0a821-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0a821-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchHitsContainer",
  "baseType": null
}-->

```json
{
  "hits": [{"@odata.type": "microsoft.graph.searchHit"}],
  "moreResultsAvailable": true,
  "total": 1024
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchHitsContainer resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->