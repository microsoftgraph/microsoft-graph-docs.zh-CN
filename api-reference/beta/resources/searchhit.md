---
title: searchHit 资源类型
description: searchHit 实体的说明
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 7c546483eea81e7d89a3a87ba5b8c0eb0ff48783
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210330"
---
# <a name="searchhit-resource-type"></a><span data-ttu-id="4d063-103">searchHit 资源类型</span><span class="sxs-lookup"><span data-stu-id="4d063-103">searchHit resource type</span></span>

<span data-ttu-id="4d063-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4d063-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [search-api-deprecation](../../includes/search-api-deprecation.md)]

<span data-ttu-id="4d063-105">表示搜索结果列表中的单个结果。</span><span class="sxs-lookup"><span data-stu-id="4d063-105">Represents a single result within the list of search results.</span></span>

## <a name="properties"></a><span data-ttu-id="4d063-106">属性</span><span class="sxs-lookup"><span data-stu-id="4d063-106">Properties</span></span>

| <span data-ttu-id="4d063-107">属性</span><span class="sxs-lookup"><span data-stu-id="4d063-107">Property</span></span>     | <span data-ttu-id="4d063-108">类型</span><span class="sxs-lookup"><span data-stu-id="4d063-108">Type</span></span>        | <span data-ttu-id="4d063-109">说明</span><span class="sxs-lookup"><span data-stu-id="4d063-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4d063-110">hitId</span><span class="sxs-lookup"><span data-stu-id="4d063-110">hitId</span></span>|<span data-ttu-id="4d063-111">String</span><span class="sxs-lookup"><span data-stu-id="4d063-111">String</span></span>|<span data-ttu-id="4d063-112">项的内部标识符。</span><span class="sxs-lookup"><span data-stu-id="4d063-112">The internal identifier for the item.</span></span>|
|<span data-ttu-id="4d063-113">排名</span><span class="sxs-lookup"><span data-stu-id="4d063-113">rank</span></span>|<span data-ttu-id="4d063-114">Int32</span><span class="sxs-lookup"><span data-stu-id="4d063-114">Int32</span></span>|<span data-ttu-id="4d063-115">结果的排名或顺序。</span><span class="sxs-lookup"><span data-stu-id="4d063-115">The rank or the order of the result.</span></span>|
|<span data-ttu-id="4d063-116">contentSource</span><span class="sxs-lookup"><span data-stu-id="4d063-116">contentSource</span></span>|<span data-ttu-id="4d063-117">String</span><span class="sxs-lookup"><span data-stu-id="4d063-117">String</span></span>|<span data-ttu-id="4d063-118">**externalItem** 是 的内容源的名称。</span><span class="sxs-lookup"><span data-stu-id="4d063-118">The name of the content source which the **externalItem** is part of .</span></span>|
|<span data-ttu-id="4d063-119">摘要</span><span class="sxs-lookup"><span data-stu-id="4d063-119">summary</span></span>|<span data-ttu-id="4d063-120">String</span><span class="sxs-lookup"><span data-stu-id="4d063-120">String</span></span>|<span data-ttu-id="4d063-121">结果摘要（如果摘要可用）。</span><span class="sxs-lookup"><span data-stu-id="4d063-121">A summary of the result, if a summary is available.</span></span>|
|<span data-ttu-id="4d063-122">resultTemplateId</span><span class="sxs-lookup"><span data-stu-id="4d063-122">resultTemplateId</span></span>|<span data-ttu-id="4d063-123">String</span><span class="sxs-lookup"><span data-stu-id="4d063-123">String</span></span>|<span data-ttu-id="4d063-124">用于呈现搜索结果的结果模板的 ID。</span><span class="sxs-lookup"><span data-stu-id="4d063-124">ID of the result template for rendering the search result.</span></span> <span data-ttu-id="4d063-125">此 ID 必须映射到 **resultTemplates** 字典（也包含在 [searchresponse](searchresponse.md) 中）中的显示布局。</span><span class="sxs-lookup"><span data-stu-id="4d063-125">This ID must map to a display layout in the **resultTemplates** dictionary, included in the [searchresponse](searchresponse.md) as well.</span></span>|
|<span data-ttu-id="4d063-126">resource</span><span class="sxs-lookup"><span data-stu-id="4d063-126">resource</span></span>|[<span data-ttu-id="4d063-127">实体</span><span class="sxs-lookup"><span data-stu-id="4d063-127">entity</span></span>](entity.md)|<span data-ttu-id="4d063-128">基础 Microsoft Graph搜索结果的表示形式。</span><span class="sxs-lookup"><span data-stu-id="4d063-128">The underlying Microsoft Graph representation of the search result.</span></span>|
|<span data-ttu-id="4d063-129">_id (弃用) </span><span class="sxs-lookup"><span data-stu-id="4d063-129">_id (deprecated)</span></span>|<span data-ttu-id="4d063-130">String</span><span class="sxs-lookup"><span data-stu-id="4d063-130">String</span></span>| <span data-ttu-id="4d063-131">重命名为 **hitId**。</span><span class="sxs-lookup"><span data-stu-id="4d063-131">Renamed as **hitId**.</span></span> <span data-ttu-id="4d063-132">项的内部标识符。</span><span class="sxs-lookup"><span data-stu-id="4d063-132">The internal identifier for the item.</span></span>|
|<span data-ttu-id="4d063-133">_score (弃用) </span><span class="sxs-lookup"><span data-stu-id="4d063-133">_score (deprecated)</span></span>|<span data-ttu-id="4d063-134">Int32</span><span class="sxs-lookup"><span data-stu-id="4d063-134">Int32</span></span>|<span data-ttu-id="4d063-135">重命名为 **排名**。</span><span class="sxs-lookup"><span data-stu-id="4d063-135">Renamed as **rank**.</span></span> <span data-ttu-id="4d063-136">结果的分数或顺序。</span><span class="sxs-lookup"><span data-stu-id="4d063-136">The score or the order of the result.</span></span>|
|<span data-ttu-id="4d063-137">_summary (弃用) </span><span class="sxs-lookup"><span data-stu-id="4d063-137">_summary (deprecated)</span></span>|<span data-ttu-id="4d063-138">String</span><span class="sxs-lookup"><span data-stu-id="4d063-138">String</span></span>|<span data-ttu-id="4d063-139">重命名为 **摘要**。</span><span class="sxs-lookup"><span data-stu-id="4d063-139">Renamed as **summary**.</span></span> <span data-ttu-id="4d063-140">如果摘要可用， (结果摘要) 。</span><span class="sxs-lookup"><span data-stu-id="4d063-140">A summary of the result (if summary is available).</span></span>|
|<span data-ttu-id="4d063-141">_sortField (弃用) </span><span class="sxs-lookup"><span data-stu-id="4d063-141">_sortField (deprecated)</span></span>|<span data-ttu-id="4d063-142">String</span><span class="sxs-lookup"><span data-stu-id="4d063-142">String</span></span>|<span data-ttu-id="4d063-143">此属性已删除。</span><span class="sxs-lookup"><span data-stu-id="4d063-143">This property has been removed.</span></span>|
|<span data-ttu-id="4d063-144">_source (弃用) </span><span class="sxs-lookup"><span data-stu-id="4d063-144">_source (deprecated)</span></span>|[<span data-ttu-id="4d063-145">实体</span><span class="sxs-lookup"><span data-stu-id="4d063-145">entity</span></span>](entity.md)|<span data-ttu-id="4d063-146">重命名为 **资源**。</span><span class="sxs-lookup"><span data-stu-id="4d063-146">Renamed as **resource**.</span></span> <span data-ttu-id="4d063-147">基础Graph搜索结果的表示形式。</span><span class="sxs-lookup"><span data-stu-id="4d063-147">The underlying Graph representation of the search result.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4d063-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4d063-148">JSON representation</span></span>

<span data-ttu-id="4d063-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4d063-149">The following is a JSON representation of the resource.</span></span>

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
  "resultTemplateId": "String",
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

