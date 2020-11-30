---
title: searchRequest 资源类型
description: 要发送到查询终结点的搜索请求。 它包含响应中的预期实体类型、基础源、分页参数、字段请求和实际搜索查询。
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: f673c551ce27c16fd4fddabc26e55cd234a9f19e
ms.sourcegitcommit: 5345c2f3265ede107fa0faaff7a3f1c2afee3810
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377970"
---
# <a name="searchrequest-resource-type"></a><span data-ttu-id="c776e-104">searchRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="c776e-104">searchRequest resource type</span></span>

<span data-ttu-id="c776e-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c776e-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c776e-106">JSON blob 中格式化的搜索请求。</span><span class="sxs-lookup"><span data-stu-id="c776e-106">A search request formatted in a JSON blob.</span></span> 

<span data-ttu-id="c776e-107">JSON blob 包含响应中预期的资源类型、基础源、分页参数、排序选项、请求的聚合和字段以及实际搜索查询。</span><span class="sxs-lookup"><span data-stu-id="c776e-107">The JSON blob contains the types of resources expected in the response, the underlying sources, paging parameters, sort options, requested aggregations and fields, and actual search query.</span></span> <span data-ttu-id="c776e-108">请参阅各种资源上的搜索请求的 [示例](#see-also) 。</span><span class="sxs-lookup"><span data-stu-id="c776e-108">See [examples](#see-also) of search requests on various resources.</span></span>

> [!NOTE]
> <span data-ttu-id="c776e-109">了解有关搜索实体类型的特定组合以及对搜索结果进行排序或聚合的 [已知限制](search-api-overview.md#known-limitations) 。</span><span class="sxs-lookup"><span data-stu-id="c776e-109">Be aware of [known limitations](search-api-overview.md#known-limitations) on searching specific combinations of entity types, and sorting or aggregating search results.</span></span>


## <a name="properties"></a><span data-ttu-id="c776e-110">属性</span><span class="sxs-lookup"><span data-stu-id="c776e-110">Properties</span></span>

| <span data-ttu-id="c776e-111">属性</span><span class="sxs-lookup"><span data-stu-id="c776e-111">Property</span></span>     | <span data-ttu-id="c776e-112">类型</span><span class="sxs-lookup"><span data-stu-id="c776e-112">Type</span></span>        | <span data-ttu-id="c776e-113">说明</span><span class="sxs-lookup"><span data-stu-id="c776e-113">Description</span></span> |
|:-------------|:------------|:------------|:------------|
|<span data-ttu-id="c776e-114">contentSources</span><span class="sxs-lookup"><span data-stu-id="c776e-114">contentSources</span></span>|<span data-ttu-id="c776e-115">String collection</span><span class="sxs-lookup"><span data-stu-id="c776e-115">String collection</span></span>|<span data-ttu-id="c776e-116">包含要设定的连接。</span><span class="sxs-lookup"><span data-stu-id="c776e-116">Contains the connection to be targeted.</span></span>|
|<span data-ttu-id="c776e-117">enableTopResults</span><span class="sxs-lookup"><span data-stu-id="c776e-117">enableTopResults</span></span>|<span data-ttu-id="c776e-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="c776e-118">Boolean</span></span>|<span data-ttu-id="c776e-119">这将触发邮件的混合排序：前3个邮件最相关。</span><span class="sxs-lookup"><span data-stu-id="c776e-119">This triggers hybrid sort for messages : the first 3 messages are the most relevant.</span></span> <span data-ttu-id="c776e-120">此属性仅适用于 entityType = `message` 。</span><span class="sxs-lookup"><span data-stu-id="c776e-120">This property is only applicable to entityType=`message`.</span></span> <span data-ttu-id="c776e-121">可选。</span><span class="sxs-lookup"><span data-stu-id="c776e-121">Optional.</span></span>|
|<span data-ttu-id="c776e-122">entityTypes</span><span class="sxs-lookup"><span data-stu-id="c776e-122">entityTypes</span></span>|<span data-ttu-id="c776e-123">entityType 集合</span><span class="sxs-lookup"><span data-stu-id="c776e-123">entityType collection</span></span>| <span data-ttu-id="c776e-124">响应中预期的一种或多种类型的资源。</span><span class="sxs-lookup"><span data-stu-id="c776e-124">One or more types of resources expected in the response.</span></span> <span data-ttu-id="c776e-125">可取值为：`list`、`site`、`listItem`、`message`、`event`、`drive` 或 `driveItem`。</span><span class="sxs-lookup"><span data-stu-id="c776e-125">Possible values are: `list`, `site`, `listItem`, `message`, `event`, `drive`, `driveItem`.</span></span> <span data-ttu-id="c776e-126">请参阅相同搜索请求中支持的两个或更多实体类型的组合的 [已知限制](search-api-overview.md#known-limitations) 。</span><span class="sxs-lookup"><span data-stu-id="c776e-126">See [known limitations](search-api-overview.md#known-limitations) for those combinations of two or more entity types that are supported in the same search request.</span></span> <span data-ttu-id="c776e-127">必填。</span><span class="sxs-lookup"><span data-stu-id="c776e-127">Required.</span></span>|
|<span data-ttu-id="c776e-128">fields</span><span class="sxs-lookup"><span data-stu-id="c776e-128">fields</span></span>|<span data-ttu-id="c776e-129">String collection</span><span class="sxs-lookup"><span data-stu-id="c776e-129">String collection</span></span> |<span data-ttu-id="c776e-130">包含要为 **entityTypes** 中指定的每个资源对象返回的字段，允许自定义默认情况下返回的字段，包括其他字段，如来自 SharePoint 和 OneDrive 的自定义托管属性。</span><span class="sxs-lookup"><span data-stu-id="c776e-130">Contains the fields to be returned for each resource object specified in **entityTypes**, allowing customization of the fields returned by default otherwise, including additional fields such as custom managed properties from SharePoint and OneDrive.</span></span> <span data-ttu-id="c776e-131">可选。</span><span class="sxs-lookup"><span data-stu-id="c776e-131">Optional.</span></span>|
|<span data-ttu-id="c776e-132">起始数量</span><span class="sxs-lookup"><span data-stu-id="c776e-132">from</span></span>|<span data-ttu-id="c776e-133">Int32</span><span class="sxs-lookup"><span data-stu-id="c776e-133">Int32</span></span>|<span data-ttu-id="c776e-134">指定搜索结果的偏移量。</span><span class="sxs-lookup"><span data-stu-id="c776e-134">Specifies the offset for the search results.</span></span> <span data-ttu-id="c776e-135">偏移量0返回的第一个结果。</span><span class="sxs-lookup"><span data-stu-id="c776e-135">Offset 0 returns the very first result.</span></span> <span data-ttu-id="c776e-136">可选。</span><span class="sxs-lookup"><span data-stu-id="c776e-136">Optional.</span></span>|
|<span data-ttu-id="c776e-137">查询</span><span class="sxs-lookup"><span data-stu-id="c776e-137">query</span></span>|[<span data-ttu-id="c776e-138">searchQuery</span><span class="sxs-lookup"><span data-stu-id="c776e-138">searchQuery</span></span>](searchquery.md)|<span data-ttu-id="c776e-139">包含查询词。</span><span class="sxs-lookup"><span data-stu-id="c776e-139">Contains the query terms.</span></span> <span data-ttu-id="c776e-140">必填。</span><span class="sxs-lookup"><span data-stu-id="c776e-140">Required.</span></span>|
|<span data-ttu-id="c776e-141">大小</span><span class="sxs-lookup"><span data-stu-id="c776e-141">size</span></span>|<span data-ttu-id="c776e-142">Int32</span><span class="sxs-lookup"><span data-stu-id="c776e-142">Int32</span></span>|<span data-ttu-id="c776e-143">要检索的页面的大小。</span><span class="sxs-lookup"><span data-stu-id="c776e-143">The size of the page to be retrieved.</span></span> <span data-ttu-id="c776e-144">可选。</span><span class="sxs-lookup"><span data-stu-id="c776e-144">Optional.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c776e-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c776e-145">JSON representation</span></span>

<span data-ttu-id="c776e-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c776e-146">The following is a JSON representation of the resource.</span></span>

```json
{
  "entityTypes": ["String"],
  "contentSources": ["String"],
  "query": {"@odata.type": "microsoft.graph.searchQuery"},
  "from": 1024,
  "size": 1024,
  "fields": ["String"],
  "enableTopResults": true  
}
```

## <a name="see-also"></a><span data-ttu-id="c776e-147">另请参阅</span><span class="sxs-lookup"><span data-stu-id="c776e-147">See also</span></span>
- <span data-ttu-id="c776e-148">搜索 [邮件消息](/graph/search-concept-messages)</span><span class="sxs-lookup"><span data-stu-id="c776e-148">Search [mail messages](/graph/search-concept-messages)</span></span>
- <span data-ttu-id="c776e-149">搜索 [日历事件](/graph/search-concept-events)</span><span class="sxs-lookup"><span data-stu-id="c776e-149">Search [calendar events](/graph/search-concept-events)</span></span>
- <span data-ttu-id="c776e-150">在 SharePoint 和 OneDrive 中搜索内容 ([文件、列表和网站](/graph/search-concept-files)) </span><span class="sxs-lookup"><span data-stu-id="c776e-150">Search content in SharePoint and OneDrive ([files, lists and sites](/graph/search-concept-files))</span></span>



<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


