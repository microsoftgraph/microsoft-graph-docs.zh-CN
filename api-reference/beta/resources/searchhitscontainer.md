---
title: searchHitsContainer 资源类型
description: 表示搜索结果的列表。
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: a2d120722179cb0fd771a84f867948a7fbfffdd4
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48192782"
---
# <a name="searchhitscontainer-resource-type"></a><span data-ttu-id="8daec-103">searchHitsContainer 资源类型</span><span class="sxs-lookup"><span data-stu-id="8daec-103">searchHitsContainer resource type</span></span>

<span data-ttu-id="8daec-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8daec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8daec-105">表示搜索结果的列表。</span><span class="sxs-lookup"><span data-stu-id="8daec-105">Represent the list of search results.</span></span>

## <a name="properties"></a><span data-ttu-id="8daec-106">属性</span><span class="sxs-lookup"><span data-stu-id="8daec-106">Properties</span></span>

| <span data-ttu-id="8daec-107">属性</span><span class="sxs-lookup"><span data-stu-id="8daec-107">Property</span></span>     | <span data-ttu-id="8daec-108">类型</span><span class="sxs-lookup"><span data-stu-id="8daec-108">Type</span></span>        | <span data-ttu-id="8daec-109">描述</span><span class="sxs-lookup"><span data-stu-id="8daec-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8daec-110">影响</span><span class="sxs-lookup"><span data-stu-id="8daec-110">hits</span></span>|<span data-ttu-id="8daec-111">[searchHit](searchhit.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8daec-111">[searchHit](searchhit.md) collection</span></span>|<span data-ttu-id="8daec-112">搜索结果的集合。</span><span class="sxs-lookup"><span data-stu-id="8daec-112">A collection of the search results.</span></span>|
|<span data-ttu-id="8daec-113">moreResultsAvailable</span><span class="sxs-lookup"><span data-stu-id="8daec-113">moreResultsAvailable</span></span>|<span data-ttu-id="8daec-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="8daec-114">Boolean</span></span>|<span data-ttu-id="8daec-115">如果有更多结果可用，则提供信息。</span><span class="sxs-lookup"><span data-stu-id="8daec-115">Provides information if more results are available.</span></span> <span data-ttu-id="8daec-116">根据此信息，您可以相应地调整[searchRequest](searchrequest.md)的 " **from** " 和 " **size** " 属性。</span><span class="sxs-lookup"><span data-stu-id="8daec-116">Based on this information, you can adjust the **from** and **size** properties of the [searchRequest](searchrequest.md) accordingly.</span></span>|
|<span data-ttu-id="8daec-117">total</span><span class="sxs-lookup"><span data-stu-id="8daec-117">total</span></span>|<span data-ttu-id="8daec-118">Int32</span><span class="sxs-lookup"><span data-stu-id="8daec-118">Int32</span></span>|<span data-ttu-id="8daec-119">总结果数。</span><span class="sxs-lookup"><span data-stu-id="8daec-119">The total number of results.</span></span> <span data-ttu-id="8daec-120">注释这不是页面上的结果数，而是满足查询的总结果数。</span><span class="sxs-lookup"><span data-stu-id="8daec-120">Note this is not the number of results on the page, but the total number of results satisfying the query.</span></span>|
|<span data-ttu-id="8daec-121">aggregations</span><span class="sxs-lookup"><span data-stu-id="8daec-121">aggregations</span></span>|<span data-ttu-id="8daec-122">[searchAggregation](searchaggregation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8daec-122">[searchAggregation](searchaggregation.md) collection</span></span>|<span data-ttu-id="8daec-123">包含根据请求中指定的提供的 [aggregationOption](aggregationoption.md) 计算出的聚合集合。</span><span class="sxs-lookup"><span data-stu-id="8daec-123">Contains the collection of aggregations computed based on the provided [aggregationOption](aggregationoption.md) specified in the request.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8daec-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8daec-124">JSON representation</span></span>

<span data-ttu-id="8daec-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8daec-125">The following is a JSON representation of the resource.</span></span>

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
  "total": 1024,
  "aggregations": [{"@odata.type": "microsoft.graph.searchAggregation"}]
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


