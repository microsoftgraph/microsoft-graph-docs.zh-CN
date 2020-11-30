---
title: searchHitsContainer 资源类型
description: 表示搜索结果的列表。
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: f32fa198624c04da6eadfc828b60350164cbdddc
ms.sourcegitcommit: 5345c2f3265ede107fa0faaff7a3f1c2afee3810
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378013"
---
# <a name="searchhitscontainer-resource-type"></a><span data-ttu-id="d15d4-103">searchHitsContainer 资源类型</span><span class="sxs-lookup"><span data-stu-id="d15d4-103">searchHitsContainer resource type</span></span>

<span data-ttu-id="d15d4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d15d4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d15d4-105">表示搜索结果的列表。</span><span class="sxs-lookup"><span data-stu-id="d15d4-105">Represent the list of search results.</span></span>

## <a name="properties"></a><span data-ttu-id="d15d4-106">属性</span><span class="sxs-lookup"><span data-stu-id="d15d4-106">Properties</span></span>

| <span data-ttu-id="d15d4-107">属性</span><span class="sxs-lookup"><span data-stu-id="d15d4-107">Property</span></span>     | <span data-ttu-id="d15d4-108">类型</span><span class="sxs-lookup"><span data-stu-id="d15d4-108">Type</span></span>        | <span data-ttu-id="d15d4-109">说明</span><span class="sxs-lookup"><span data-stu-id="d15d4-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d15d4-110">影响</span><span class="sxs-lookup"><span data-stu-id="d15d4-110">hits</span></span>|<span data-ttu-id="d15d4-111">[searchHit](searchhit.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d15d4-111">[searchHit](searchhit.md) collection</span></span>|<span data-ttu-id="d15d4-112">搜索结果的集合。</span><span class="sxs-lookup"><span data-stu-id="d15d4-112">A collection of the search results.</span></span>|
|<span data-ttu-id="d15d4-113">moreResultsAvailable</span><span class="sxs-lookup"><span data-stu-id="d15d4-113">moreResultsAvailable</span></span>|<span data-ttu-id="d15d4-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="d15d4-114">Boolean</span></span>|<span data-ttu-id="d15d4-115">如果有更多结果可用，则提供信息。</span><span class="sxs-lookup"><span data-stu-id="d15d4-115">Provides information if more results are available.</span></span> <span data-ttu-id="d15d4-116">根据此信息，您可以相应地调整 [searchRequest](searchrequest.md)的 " **from** " 和 " **size** " 属性。</span><span class="sxs-lookup"><span data-stu-id="d15d4-116">Based on this information, you can adjust the **from** and **size** properties of the [searchRequest](searchrequest.md) accordingly.</span></span>|
|<span data-ttu-id="d15d4-117">total</span><span class="sxs-lookup"><span data-stu-id="d15d4-117">total</span></span>|<span data-ttu-id="d15d4-118">Int32</span><span class="sxs-lookup"><span data-stu-id="d15d4-118">Int32</span></span>|<span data-ttu-id="d15d4-119">总结果数。</span><span class="sxs-lookup"><span data-stu-id="d15d4-119">The total number of results.</span></span> <span data-ttu-id="d15d4-120">注释这不是页面上的结果数，而是满足查询的总结果数。</span><span class="sxs-lookup"><span data-stu-id="d15d4-120">Note this is not the number of results on the page, but the total number of results satisfying the query.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="d15d4-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d15d4-121">JSON representation</span></span>

<span data-ttu-id="d15d4-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d15d4-122">The following is a JSON representation of the resource.</span></span>

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


