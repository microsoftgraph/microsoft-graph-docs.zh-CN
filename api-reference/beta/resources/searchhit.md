---
title: searchHit 资源类型
description: SearchHit 实体的说明
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: c140a30d4e77840b1fd7c7ccceec16e0554cd855
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193608"
---
# <a name="searchhit-resource-type"></a><span data-ttu-id="d7965-103">searchHit 资源类型</span><span class="sxs-lookup"><span data-stu-id="d7965-103">searchHit resource type</span></span>

<span data-ttu-id="d7965-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7965-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [search-api-deprecation](../../includes/search-api-deprecation.md)]

<span data-ttu-id="d7965-105">代表搜索结果列表中的单个结果。</span><span class="sxs-lookup"><span data-stu-id="d7965-105">Represents a single result within the list of search results.</span></span>

## <a name="properties"></a><span data-ttu-id="d7965-106">属性</span><span class="sxs-lookup"><span data-stu-id="d7965-106">Properties</span></span>

| <span data-ttu-id="d7965-107">属性</span><span class="sxs-lookup"><span data-stu-id="d7965-107">Property</span></span>     | <span data-ttu-id="d7965-108">类型</span><span class="sxs-lookup"><span data-stu-id="d7965-108">Type</span></span>        | <span data-ttu-id="d7965-109">描述</span><span class="sxs-lookup"><span data-stu-id="d7965-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d7965-110">hitId</span><span class="sxs-lookup"><span data-stu-id="d7965-110">hitId</span></span>|<span data-ttu-id="d7965-111">字符串</span><span class="sxs-lookup"><span data-stu-id="d7965-111">String</span></span>|<span data-ttu-id="d7965-112">项的内部标识符。</span><span class="sxs-lookup"><span data-stu-id="d7965-112">The internal identifier for the item.</span></span>|
|<span data-ttu-id="d7965-113">排名</span><span class="sxs-lookup"><span data-stu-id="d7965-113">rank</span></span>|<span data-ttu-id="d7965-114">Int32</span><span class="sxs-lookup"><span data-stu-id="d7965-114">Int32</span></span>|<span data-ttu-id="d7965-115">结果的排名或顺序。</span><span class="sxs-lookup"><span data-stu-id="d7965-115">The rank or the order of the result.</span></span>|
|<span data-ttu-id="d7965-116">contentSource</span><span class="sxs-lookup"><span data-stu-id="d7965-116">contentSource</span></span>|<span data-ttu-id="d7965-117">字符串</span><span class="sxs-lookup"><span data-stu-id="d7965-117">String</span></span>|<span data-ttu-id="d7965-118">**ExternalItem**所属的内容源的名称。</span><span class="sxs-lookup"><span data-stu-id="d7965-118">The name of the content source which the **externalItem** is part of .</span></span>|
|<span data-ttu-id="d7965-119">摘要</span><span class="sxs-lookup"><span data-stu-id="d7965-119">summary</span></span>|<span data-ttu-id="d7965-120">字符串</span><span class="sxs-lookup"><span data-stu-id="d7965-120">String</span></span>|<span data-ttu-id="d7965-121">如果摘要可用，则为结果摘要。</span><span class="sxs-lookup"><span data-stu-id="d7965-121">A summary of the result, if a summary is available.</span></span>|
|<span data-ttu-id="d7965-122">resource</span><span class="sxs-lookup"><span data-stu-id="d7965-122">resource</span></span>|[<span data-ttu-id="d7965-123">实体</span><span class="sxs-lookup"><span data-stu-id="d7965-123">entity</span></span>](entity.md)|<span data-ttu-id="d7965-124">搜索结果的基本 Microsoft Graph 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d7965-124">The underlying Microsoft Graph representation of the search result.</span></span>|
|<span data-ttu-id="d7965-125">_id (已弃用) </span><span class="sxs-lookup"><span data-stu-id="d7965-125">_id (deprecated)</span></span>|<span data-ttu-id="d7965-126">字符串</span><span class="sxs-lookup"><span data-stu-id="d7965-126">String</span></span>| <span data-ttu-id="d7965-127">重命名为 **hitId**。</span><span class="sxs-lookup"><span data-stu-id="d7965-127">Renamed as **hitId**.</span></span> <span data-ttu-id="d7965-128">项的内部标识符。</span><span class="sxs-lookup"><span data-stu-id="d7965-128">The internal identifier for the item.</span></span>|
|<span data-ttu-id="d7965-129">_score (已弃用) </span><span class="sxs-lookup"><span data-stu-id="d7965-129">_score (deprecated)</span></span>|<span data-ttu-id="d7965-130">Int32</span><span class="sxs-lookup"><span data-stu-id="d7965-130">Int32</span></span>|<span data-ttu-id="d7965-131">重命名为 **rank**。</span><span class="sxs-lookup"><span data-stu-id="d7965-131">Renamed as **rank**.</span></span> <span data-ttu-id="d7965-132">结果的分数或顺序。</span><span class="sxs-lookup"><span data-stu-id="d7965-132">The score or the order of the result.</span></span>|
|<span data-ttu-id="d7965-133">_summary (已弃用) </span><span class="sxs-lookup"><span data-stu-id="d7965-133">_summary (deprecated)</span></span>|<span data-ttu-id="d7965-134">字符串</span><span class="sxs-lookup"><span data-stu-id="d7965-134">String</span></span>|<span data-ttu-id="d7965-135">重命名为 **摘要**。</span><span class="sxs-lookup"><span data-stu-id="d7965-135">Renamed as **summary**.</span></span> <span data-ttu-id="d7965-136"> (如果摘要可用) 的结果摘要。</span><span class="sxs-lookup"><span data-stu-id="d7965-136">A summary of the result (if summary is available).</span></span>|
|<span data-ttu-id="d7965-137">_sortField (已弃用) </span><span class="sxs-lookup"><span data-stu-id="d7965-137">_sortField (deprecated)</span></span>|<span data-ttu-id="d7965-138">字符串</span><span class="sxs-lookup"><span data-stu-id="d7965-138">String</span></span>|<span data-ttu-id="d7965-139">此属性已被删除。</span><span class="sxs-lookup"><span data-stu-id="d7965-139">This property has been removed.</span></span>|
|<span data-ttu-id="d7965-140">_source (已弃用) </span><span class="sxs-lookup"><span data-stu-id="d7965-140">_source (deprecated)</span></span>|[<span data-ttu-id="d7965-141">实体</span><span class="sxs-lookup"><span data-stu-id="d7965-141">entity</span></span>](entity.md)|<span data-ttu-id="d7965-142">重命名为 **资源**。</span><span class="sxs-lookup"><span data-stu-id="d7965-142">Renamed as **resource**.</span></span> <span data-ttu-id="d7965-143">搜索结果的基础图形表示形式。</span><span class="sxs-lookup"><span data-stu-id="d7965-143">The underlying Graph representation of the search result.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d7965-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d7965-144">JSON representation</span></span>

<span data-ttu-id="d7965-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d7965-145">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchHit",
  "baseType": null
}-->

```json
{
  "hitId": "String",
  "rank": 1,
  "summary": "String",
  "contentSource": "String",
  "resource": { "@odata.type": "microsoft.graph.entity" },
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

