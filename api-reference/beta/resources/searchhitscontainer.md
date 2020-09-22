---
title: searchHitsContainer 资源类型
description: 在此处提供说明
localization_priority: Normal
author: nmoreau
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d314fcdd2a62be5aea05bed3b2a9e1881f95c3d0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985785"
---
# <a name="searchhitscontainer-resource-type"></a><span data-ttu-id="534fd-103">searchHitsContainer 资源类型</span><span class="sxs-lookup"><span data-stu-id="534fd-103">searchHitsContainer resource type</span></span>

<span data-ttu-id="534fd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="534fd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="534fd-105">表示搜索结果的列表。</span><span class="sxs-lookup"><span data-stu-id="534fd-105">Represent the list of search results.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="534fd-106">属性</span><span class="sxs-lookup"><span data-stu-id="534fd-106">Properties</span></span>

| <span data-ttu-id="534fd-107">属性</span><span class="sxs-lookup"><span data-stu-id="534fd-107">Property</span></span>     | <span data-ttu-id="534fd-108">类型</span><span class="sxs-lookup"><span data-stu-id="534fd-108">Type</span></span>        | <span data-ttu-id="534fd-109">说明</span><span class="sxs-lookup"><span data-stu-id="534fd-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="534fd-110">影响</span><span class="sxs-lookup"><span data-stu-id="534fd-110">hits</span></span>|<span data-ttu-id="534fd-111">[searchHit](searchhit.md) 集合</span><span class="sxs-lookup"><span data-stu-id="534fd-111">[searchHit](searchhit.md) collection</span></span>|<span data-ttu-id="534fd-112">Encasulate 搜索结果。</span><span class="sxs-lookup"><span data-stu-id="534fd-112">Encasulate the Search results.</span></span>|
|<span data-ttu-id="534fd-113">moreResultsAvailable</span><span class="sxs-lookup"><span data-stu-id="534fd-113">moreResultsAvailable</span></span>|<span data-ttu-id="534fd-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="534fd-114">Boolean</span></span>|<span data-ttu-id="534fd-115">如果有更多结果可用，则提供信息。</span><span class="sxs-lookup"><span data-stu-id="534fd-115">Provides information if more results are available.</span></span> <span data-ttu-id="534fd-116">在这种情况下，您可以增加 "from" 和 "to" 偏移量。</span><span class="sxs-lookup"><span data-stu-id="534fd-116">In that case you can increase the "from" and "to" offset.</span></span>|
|<span data-ttu-id="534fd-117">total</span><span class="sxs-lookup"><span data-stu-id="534fd-117">total</span></span>|<span data-ttu-id="534fd-118">Int32</span><span class="sxs-lookup"><span data-stu-id="534fd-118">Int32</span></span>|<span data-ttu-id="534fd-119">总结果数。</span><span class="sxs-lookup"><span data-stu-id="534fd-119">The total number of results.</span></span> <span data-ttu-id="534fd-120">注释这不是页面结果中的数值，而是满足查询的结果总数。</span><span class="sxs-lookup"><span data-stu-id="534fd-120">Note this is not the number on results in the page, but the total number of results satisfying the query.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="534fd-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="534fd-121">JSON representation</span></span>

<span data-ttu-id="534fd-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="534fd-122">The following is a JSON representation of the resource.</span></span>

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

