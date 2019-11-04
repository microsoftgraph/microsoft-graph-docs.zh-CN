---
title: searchHit 资源类型
description: 在此处提供说明
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 2ce5671933589f6066698df3e082390207474b49
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939864"
---
# <a name="searchhit-resource-type"></a><span data-ttu-id="03e6e-103">searchHit 资源类型</span><span class="sxs-lookup"><span data-stu-id="03e6e-103">searchHit resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03e6e-104">表示搜索结果列表中的单个结果。</span><span class="sxs-lookup"><span data-stu-id="03e6e-104">Represent a single result within the list of search results.</span></span>

## <a name="properties"></a><span data-ttu-id="03e6e-105">属性</span><span class="sxs-lookup"><span data-stu-id="03e6e-105">Properties</span></span>

| <span data-ttu-id="03e6e-106">属性</span><span class="sxs-lookup"><span data-stu-id="03e6e-106">Property</span></span>     | <span data-ttu-id="03e6e-107">类型</span><span class="sxs-lookup"><span data-stu-id="03e6e-107">Type</span></span>        | <span data-ttu-id="03e6e-108">描述</span><span class="sxs-lookup"><span data-stu-id="03e6e-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="03e6e-109">_id</span><span class="sxs-lookup"><span data-stu-id="03e6e-109">_id</span></span>|<span data-ttu-id="03e6e-110">字符串</span><span class="sxs-lookup"><span data-stu-id="03e6e-110">String</span></span>|<span data-ttu-id="03e6e-111">项的内部标识符。</span><span class="sxs-lookup"><span data-stu-id="03e6e-111">The internal identifier for the item.</span></span>|
|<span data-ttu-id="03e6e-112">_score</span><span class="sxs-lookup"><span data-stu-id="03e6e-112">_score</span></span>|<span data-ttu-id="03e6e-113">Int32</span><span class="sxs-lookup"><span data-stu-id="03e6e-113">Int32</span></span>|<span data-ttu-id="03e6e-114">结果的分数或顺序。</span><span class="sxs-lookup"><span data-stu-id="03e6e-114">The score or the order of the result.</span></span>|
|<span data-ttu-id="03e6e-115">_sortField</span><span class="sxs-lookup"><span data-stu-id="03e6e-115">_sortField</span></span>|<span data-ttu-id="03e6e-116">字符串</span><span class="sxs-lookup"><span data-stu-id="03e6e-116">String</span></span>|<span data-ttu-id="03e6e-117">使用的排序顺序。</span><span class="sxs-lookup"><span data-stu-id="03e6e-117">The sort order used.</span></span> <span data-ttu-id="03e6e-118">它可以是 DateTime 或相关性。</span><span class="sxs-lookup"><span data-stu-id="03e6e-118">It can be DateTime or Relevance.</span></span>|
|<span data-ttu-id="03e6e-119">_summary</span><span class="sxs-lookup"><span data-stu-id="03e6e-119">_summary</span></span>|<span data-ttu-id="03e6e-120">字符串</span><span class="sxs-lookup"><span data-stu-id="03e6e-120">String</span></span>|<span data-ttu-id="03e6e-121">结果的摘要（如果摘要可用）。</span><span class="sxs-lookup"><span data-stu-id="03e6e-121">A summary of the result (if summary is available).</span></span>|
|<span data-ttu-id="03e6e-122">_source</span><span class="sxs-lookup"><span data-stu-id="03e6e-122">_source</span></span>|[<span data-ttu-id="03e6e-123">实体</span><span class="sxs-lookup"><span data-stu-id="03e6e-123">entity</span></span>](entity.md)|<span data-ttu-id="03e6e-124">搜索结果的基础图形表示形式。</span><span class="sxs-lookup"><span data-stu-id="03e6e-124">The underlying Graph representation of the search result.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="03e6e-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="03e6e-125">JSON representation</span></span>

<span data-ttu-id="03e6e-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="03e6e-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchHit",
  "baseType": null
}-->

```json
{
  "_id": "String",
  "_score": 1024,
  "_sortField": "String",
  "_summary": "String",
  "_source": { "@odata.type": "microsoft.graph.entity" }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchHit resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->