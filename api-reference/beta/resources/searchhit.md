---
title: searchHit 资源类型
description: 在此处提供说明
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 722641b42a403565afcf7baa9de42af2b36a9dec
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520926"
---
# <a name="searchhit-resource-type"></a><span data-ttu-id="0aec9-103">searchHit 资源类型</span><span class="sxs-lookup"><span data-stu-id="0aec9-103">searchHit resource type</span></span>

<span data-ttu-id="0aec9-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="0aec9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0aec9-105">表示搜索结果列表中的单个结果。</span><span class="sxs-lookup"><span data-stu-id="0aec9-105">Represent a single result within the list of search results.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="0aec9-106">属性</span><span class="sxs-lookup"><span data-stu-id="0aec9-106">Properties</span></span>

| <span data-ttu-id="0aec9-107">属性</span><span class="sxs-lookup"><span data-stu-id="0aec9-107">Property</span></span>     | <span data-ttu-id="0aec9-108">类型</span><span class="sxs-lookup"><span data-stu-id="0aec9-108">Type</span></span>        | <span data-ttu-id="0aec9-109">说明</span><span class="sxs-lookup"><span data-stu-id="0aec9-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0aec9-110">_id</span><span class="sxs-lookup"><span data-stu-id="0aec9-110">_id</span></span>|<span data-ttu-id="0aec9-111">String</span><span class="sxs-lookup"><span data-stu-id="0aec9-111">String</span></span>|<span data-ttu-id="0aec9-112">项的内部标识符。</span><span class="sxs-lookup"><span data-stu-id="0aec9-112">The internal identifier for the item.</span></span>|
|<span data-ttu-id="0aec9-113">_score</span><span class="sxs-lookup"><span data-stu-id="0aec9-113">_score</span></span>|<span data-ttu-id="0aec9-114">Int32</span><span class="sxs-lookup"><span data-stu-id="0aec9-114">Int32</span></span>|<span data-ttu-id="0aec9-115">结果的分数或顺序。</span><span class="sxs-lookup"><span data-stu-id="0aec9-115">The score or the order of the result.</span></span>|
|<span data-ttu-id="0aec9-116">_sortField</span><span class="sxs-lookup"><span data-stu-id="0aec9-116">_sortField</span></span>|<span data-ttu-id="0aec9-117">String</span><span class="sxs-lookup"><span data-stu-id="0aec9-117">String</span></span>|<span data-ttu-id="0aec9-118">使用的排序顺序。</span><span class="sxs-lookup"><span data-stu-id="0aec9-118">The sort order used.</span></span> <span data-ttu-id="0aec9-119">它可以是 DateTime 或相关性。</span><span class="sxs-lookup"><span data-stu-id="0aec9-119">It can be DateTime or Relevance.</span></span>|
|<span data-ttu-id="0aec9-120">_summary</span><span class="sxs-lookup"><span data-stu-id="0aec9-120">_summary</span></span>|<span data-ttu-id="0aec9-121">String</span><span class="sxs-lookup"><span data-stu-id="0aec9-121">String</span></span>|<span data-ttu-id="0aec9-122">结果的摘要（如果摘要可用）。</span><span class="sxs-lookup"><span data-stu-id="0aec9-122">A summary of the result (if summary is available).</span></span>|
|<span data-ttu-id="0aec9-123">_source</span><span class="sxs-lookup"><span data-stu-id="0aec9-123">_source</span></span>|[<span data-ttu-id="0aec9-124">实体</span><span class="sxs-lookup"><span data-stu-id="0aec9-124">entity</span></span>](entity.md)|<span data-ttu-id="0aec9-125">搜索结果的基础图形表示形式。</span><span class="sxs-lookup"><span data-stu-id="0aec9-125">The underlying Graph representation of the search result.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0aec9-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0aec9-126">JSON representation</span></span>

<span data-ttu-id="0aec9-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0aec9-127">The following is a JSON representation of the resource.</span></span>

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