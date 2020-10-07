---
title: searchRequest 资源类型
description: 要发送到查询终结点的搜索请求。 它包含响应中的预期实体类型、基础源、分页参数、字段请求和实际搜索查询。
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 04bdca98f4676454a72e503e8bfe747bbda306cc
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/07/2020
ms.locfileid: "48372691"
---
# <a name="searchrequest-resource-type"></a><span data-ttu-id="1a9f3-104">searchRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="1a9f3-104">searchRequest resource type</span></span>

<span data-ttu-id="1a9f3-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a9f3-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [search-api-deprecation](../../includes/search-api-deprecation.md)]

<span data-ttu-id="1a9f3-106">JSON blob 中格式化的搜索请求。</span><span class="sxs-lookup"><span data-stu-id="1a9f3-106">A search request formatted in a JSON blob.</span></span> 

<span data-ttu-id="1a9f3-107">JSON blob 包含响应中预期的资源类型、基础源、分页参数、排序选项、请求的聚合和字段以及实际搜索查询。</span><span class="sxs-lookup"><span data-stu-id="1a9f3-107">The JSON blob contains the types of resources expected in the response, the underlying sources, paging parameters, sort options, requested aggregations and fields, and actual search query.</span></span> <span data-ttu-id="1a9f3-108">请参阅各种资源上的搜索请求的 [示例](#see-also) 。</span><span class="sxs-lookup"><span data-stu-id="1a9f3-108">See [examples](#see-also) of search requests on various resources.</span></span>

> [!NOTE]
> <span data-ttu-id="1a9f3-109">了解有关搜索实体类型的特定组合以及对搜索结果进行排序或聚合的 [已知限制](search-api-overview.md#known-limitations) 。</span><span class="sxs-lookup"><span data-stu-id="1a9f3-109">Be aware of [known limitations](search-api-overview.md#known-limitations) on searching specific combinations of entity types, and sorting or aggregating search results.</span></span>


## <a name="properties"></a><span data-ttu-id="1a9f3-110">属性</span><span class="sxs-lookup"><span data-stu-id="1a9f3-110">Properties</span></span>

| <span data-ttu-id="1a9f3-111">属性</span><span class="sxs-lookup"><span data-stu-id="1a9f3-111">Property</span></span>     | <span data-ttu-id="1a9f3-112">类型</span><span class="sxs-lookup"><span data-stu-id="1a9f3-112">Type</span></span>        | <span data-ttu-id="1a9f3-113">说明</span><span class="sxs-lookup"><span data-stu-id="1a9f3-113">Description</span></span> |
|:-------------|:------------|:------------|:------------|
|<span data-ttu-id="1a9f3-114">聚合</span><span class="sxs-lookup"><span data-stu-id="1a9f3-114">aggregations</span></span>|<span data-ttu-id="1a9f3-115">[aggregationOption](aggregationOption.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1a9f3-115">[aggregationOption](aggregationOption.md) collection</span></span>|<span data-ttu-id="1a9f3-116">指定 (也称为精简条件) 与搜索结果一起返回的聚合。</span><span class="sxs-lookup"><span data-stu-id="1a9f3-116">Specifies aggregations (also known as refiners) to be returned alongside search results.</span></span> <span data-ttu-id="1a9f3-117">可选。</span><span class="sxs-lookup"><span data-stu-id="1a9f3-117">Optional.</span></span>|
|<span data-ttu-id="1a9f3-118">aggregationFilters</span><span class="sxs-lookup"><span data-stu-id="1a9f3-118">aggregationFilters</span></span>|<span data-ttu-id="1a9f3-119">字符串集合</span><span class="sxs-lookup"><span data-stu-id="1a9f3-119">String collection</span></span>|<span data-ttu-id="1a9f3-120">包含一个或多个筛选器，以获取聚合并筛选为字段的特定值的搜索结果。</span><span class="sxs-lookup"><span data-stu-id="1a9f3-120">Contains one or more filters to obtain search results aggregated and filtered to a specific value of a field.</span></span> <span data-ttu-id="1a9f3-121">可选。</span><span class="sxs-lookup"><span data-stu-id="1a9f3-121">Optional.</span></span><br><span data-ttu-id="1a9f3-122">基于按相同字段聚合的先前搜索生成此筛选器。</span><span class="sxs-lookup"><span data-stu-id="1a9f3-122">Build this filter based on a prior search that aggregates by the same field.</span></span> <span data-ttu-id="1a9f3-123">从以前的搜索的响应中，确定将结果筛选为字段的特定值的 [searchBucket](searchBucket.md) ，使用其 **aggregationFilterToken** 属性中的字符串，并以 **"{field}： \\ {aggregationFilterToken} \\ "** 格式生成聚合筛选器字符串。</span><span class="sxs-lookup"><span data-stu-id="1a9f3-123">From the response of the prior search, identify the [searchBucket](searchBucket.md) that filters results to the specific value of the field, use the string in its **aggregationFilterToken** property, and build an aggregation filter string in the format **"{field}:\\"{aggregationFilterToken}\\""**.</span></span> <br><span data-ttu-id="1a9f3-124">例如，按文件类型搜索和聚合 drive 项目为响应中**searchBucket**的文件类型返回 searchBucket `docx` 。</span><span class="sxs-lookup"><span data-stu-id="1a9f3-124">For example, searching and aggregating drive items by file type returns a **searchBucket** for the file type `docx` in the response.</span></span> <span data-ttu-id="1a9f3-125">您可以在随后的搜索查询中方便地使用为此**searchBucket**返回的**aggregationFilterToken** ，并筛选出与驱动文件类型的项目相匹配的项目 `docx` 。</span><span class="sxs-lookup"><span data-stu-id="1a9f3-125">You can conveniently use the **aggregationFilterToken** returned for this **searchBucket** in a subsequent search query and filter matches down to drive items of the `docx` file type.</span></span> <span data-ttu-id="1a9f3-126">[示例 1](/graph/search-concept-aggregation#example-1-request-aggregations-by-string-fields) 和 [示例 2](/graph/search-concept-aggregation#example-2-apply-an-aggregation-filter-based-on-a-previous-request) 显示实际的请求和响应。</span><span class="sxs-lookup"><span data-stu-id="1a9f3-126">[Example 1](/graph/search-concept-aggregation#example-1-request-aggregations-by-string-fields) and [example 2](/graph/search-concept-aggregation#example-2-apply-an-aggregation-filter-based-on-a-previous-request) show the actual requests and responses.</span></span>|
|<span data-ttu-id="1a9f3-127">contentSources</span><span class="sxs-lookup"><span data-stu-id="1a9f3-127">contentSources</span></span>|<span data-ttu-id="1a9f3-128">字符串集合</span><span class="sxs-lookup"><span data-stu-id="1a9f3-128">String collection</span></span>|<span data-ttu-id="1a9f3-129">包含要设定的连接。</span><span class="sxs-lookup"><span data-stu-id="1a9f3-129">Contains the connection to be targeted.</span></span> <br><span data-ttu-id="1a9f3-130">遵循以下格式： `/external/connections/connectionid` 其中 `connectionid` 是连接器管理中定义的 ConnectionId。</span><span class="sxs-lookup"><span data-stu-id="1a9f3-130">Respects the following format : `/external/connections/connectionid` where `connectionid` is the ConnectionId defined in the Connectors Administration.</span></span> <br> <span data-ttu-id="1a9f3-131">注意：仅当 entityType = 时，contentSource 才适用 `externalItem` 。</span><span class="sxs-lookup"><span data-stu-id="1a9f3-131">Note : contentSource is only applicable when entityType=`externalItem`.</span></span> <span data-ttu-id="1a9f3-132">可选。</span><span class="sxs-lookup"><span data-stu-id="1a9f3-132">Optional.</span></span>|
|<span data-ttu-id="1a9f3-133">enableTopResults</span><span class="sxs-lookup"><span data-stu-id="1a9f3-133">enableTopResults</span></span>|<span data-ttu-id="1a9f3-134">布尔值</span><span class="sxs-lookup"><span data-stu-id="1a9f3-134">Boolean</span></span>|<span data-ttu-id="1a9f3-135">这将触发邮件的混合排序：前3个邮件最相关。</span><span class="sxs-lookup"><span data-stu-id="1a9f3-135">This triggers hybrid sort for messages : the first 3 messages are the most relevant.</span></span> <span data-ttu-id="1a9f3-136">此属性仅适用于 entityType = `message` 。</span><span class="sxs-lookup"><span data-stu-id="1a9f3-136">This property is only applicable to entityType=`message`.</span></span> <span data-ttu-id="1a9f3-137">可选。</span><span class="sxs-lookup"><span data-stu-id="1a9f3-137">Optional.</span></span>|
|<span data-ttu-id="1a9f3-138">entityTypes</span><span class="sxs-lookup"><span data-stu-id="1a9f3-138">entityTypes</span></span>|<span data-ttu-id="1a9f3-139">entityType 集合</span><span class="sxs-lookup"><span data-stu-id="1a9f3-139">entityType collection</span></span>| <span data-ttu-id="1a9f3-140">响应中预期的一种或多种类型的资源。</span><span class="sxs-lookup"><span data-stu-id="1a9f3-140">One or more types of resources expected in the response.</span></span> <span data-ttu-id="1a9f3-141">可取值为：`list`、`site`、`listItem`、`message`、`event`、`drive`、`driveItem`、`externalItem`。</span><span class="sxs-lookup"><span data-stu-id="1a9f3-141">Possible values are: `list`, `site`, `listItem`, `message`, `event`, `drive`, `driveItem`, `externalItem`.</span></span> <span data-ttu-id="1a9f3-142">请参阅相同搜索请求中支持的两个或更多实体类型的组合的 [已知限制](search-api-overview.md#known-limitations) 。</span><span class="sxs-lookup"><span data-stu-id="1a9f3-142">See [known limitations](search-api-overview.md#known-limitations) for those combinations of two or more entity types that are supported in the same search request.</span></span> <span data-ttu-id="1a9f3-143">必需。</span><span class="sxs-lookup"><span data-stu-id="1a9f3-143">Required.</span></span>|
|<span data-ttu-id="1a9f3-144">fields</span><span class="sxs-lookup"><span data-stu-id="1a9f3-144">fields</span></span>|<span data-ttu-id="1a9f3-145">字符串集合</span><span class="sxs-lookup"><span data-stu-id="1a9f3-145">String collection</span></span> |<span data-ttu-id="1a9f3-146">包含要为 **entityTypes**中指定的每个资源对象返回的字段，允许自定义默认情况下返回的字段（包括其他字段，如来自 SharePoint 和 OneDrive 的自定义托管属性）或 **externalItem** 中从内容引入 x 连接器的自定义字段。</span><span class="sxs-lookup"><span data-stu-id="1a9f3-146">Contains the fields to be returned for each resource object specified in **entityTypes**, allowing customization of the fields returned by default otherwise, including additional fields such as custom managed properties from SharePoint and OneDrive, or custom fields in **externalItem** from content ingested by Graph connectors.</span></span> <span data-ttu-id="1a9f3-147">可选。</span><span class="sxs-lookup"><span data-stu-id="1a9f3-147">Optional.</span></span>|
|<span data-ttu-id="1a9f3-148">起始数量</span><span class="sxs-lookup"><span data-stu-id="1a9f3-148">from</span></span>|<span data-ttu-id="1a9f3-149">Int32</span><span class="sxs-lookup"><span data-stu-id="1a9f3-149">Int32</span></span>|<span data-ttu-id="1a9f3-150">指定搜索结果的偏移量。</span><span class="sxs-lookup"><span data-stu-id="1a9f3-150">Specifies the offset for the search results.</span></span> <span data-ttu-id="1a9f3-151">偏移量0返回的第一个结果。</span><span class="sxs-lookup"><span data-stu-id="1a9f3-151">Offset 0 returns the very first result.</span></span> <span data-ttu-id="1a9f3-152">可选。</span><span class="sxs-lookup"><span data-stu-id="1a9f3-152">Optional.</span></span>|
|<span data-ttu-id="1a9f3-153">查询</span><span class="sxs-lookup"><span data-stu-id="1a9f3-153">query</span></span>|[<span data-ttu-id="1a9f3-154">searchQuery</span><span class="sxs-lookup"><span data-stu-id="1a9f3-154">searchQuery</span></span>](searchquery.md)|<span data-ttu-id="1a9f3-155">包含查询词。</span><span class="sxs-lookup"><span data-stu-id="1a9f3-155">Contains the query terms.</span></span> <span data-ttu-id="1a9f3-156">必需。</span><span class="sxs-lookup"><span data-stu-id="1a9f3-156">Required.</span></span>|
|<span data-ttu-id="1a9f3-157">大小</span><span class="sxs-lookup"><span data-stu-id="1a9f3-157">size</span></span>|<span data-ttu-id="1a9f3-158">Int32</span><span class="sxs-lookup"><span data-stu-id="1a9f3-158">Int32</span></span>|<span data-ttu-id="1a9f3-159">要检索的页面的大小。</span><span class="sxs-lookup"><span data-stu-id="1a9f3-159">The size of the page to be retrieved.</span></span> <span data-ttu-id="1a9f3-160">可选。</span><span class="sxs-lookup"><span data-stu-id="1a9f3-160">Optional.</span></span>|
|<span data-ttu-id="1a9f3-161">sortProperties</span><span class="sxs-lookup"><span data-stu-id="1a9f3-161">sortProperties</span></span>|<span data-ttu-id="1a9f3-162">[sortProperty](sortProperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1a9f3-162">[sortProperty](sortProperty.md) collection</span></span>|<span data-ttu-id="1a9f3-163">包含用于对结果进行排序的字段和方向的已排序集合。</span><span class="sxs-lookup"><span data-stu-id="1a9f3-163">Contains the ordered collection of fields and direction to sort results.</span></span> <span data-ttu-id="1a9f3-164">集合中最多可以有5个排序属性。</span><span class="sxs-lookup"><span data-stu-id="1a9f3-164">There can be at most 5 sort properties in the collection.</span></span> <span data-ttu-id="1a9f3-165">可选。</span><span class="sxs-lookup"><span data-stu-id="1a9f3-165">Optional.</span></span>|
|<span data-ttu-id="1a9f3-166">stored_fields (已弃用) </span><span class="sxs-lookup"><span data-stu-id="1a9f3-166">stored_fields (deprecated)</span></span>|<span data-ttu-id="1a9f3-167">字符串集合</span><span class="sxs-lookup"><span data-stu-id="1a9f3-167">String collection</span></span> |<span data-ttu-id="1a9f3-168">现在，此属性将替换为 **fields** 属性。</span><span class="sxs-lookup"><span data-stu-id="1a9f3-168">This is now replaced by the **fields** property.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="1a9f3-169">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1a9f3-169">JSON representation</span></span>

<span data-ttu-id="1a9f3-170">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1a9f3-170">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchRequest",
  "baseType": null
}-->

```json
{
  "entityTypes": ["String"],
  "contentSources": ["String"],
  "query": {"@odata.type": "microsoft.graph.searchQuery"},
  "from": 1024,
  "size": 1024,
  "fields": ["String"],
  "sortProperties": [{"@odata.type": "microsoft.graph.sortProperty"}],
  "aggregations": [{"@odata.type": "microsoft.graph.aggregationOption"}],
  "aggregationFilters": ["String"],
  "enableTopResults": true  
}
```

## <a name="see-also"></a><span data-ttu-id="1a9f3-171">另请参阅</span><span class="sxs-lookup"><span data-stu-id="1a9f3-171">See also</span></span>
- <span data-ttu-id="1a9f3-172">搜索 [邮件消息](/graph/search-concept-messages)</span><span class="sxs-lookup"><span data-stu-id="1a9f3-172">Search [mail messages](/graph/search-concept-messages)</span></span>
- <span data-ttu-id="1a9f3-173">搜索 [日历事件](/graph/search-concept-events)</span><span class="sxs-lookup"><span data-stu-id="1a9f3-173">Search [calendar events](/graph/search-concept-events)</span></span>
- <span data-ttu-id="1a9f3-174">在 SharePoint 和 OneDrive 中搜索内容 ([文件、列表和网站](/graph/search-concept-files)) </span><span class="sxs-lookup"><span data-stu-id="1a9f3-174">Search content in SharePoint and OneDrive ([files, lists and sites](/graph/search-concept-files))</span></span>
- <span data-ttu-id="1a9f3-175">搜索 [自定义类型 (Graph 连接器) ](/graph/search-concept-custom-types) 数据</span><span class="sxs-lookup"><span data-stu-id="1a9f3-175">Search [custom types (Graph Connectors)](/graph/search-concept-custom-types) data</span></span>
- <span data-ttu-id="1a9f3-176">[对搜索结果进行排序](/graph/search-concept-sort)</span><span class="sxs-lookup"><span data-stu-id="1a9f3-176">[Sort](/graph/search-concept-sort) search results</span></span>
- <span data-ttu-id="1a9f3-177">使用 [聚合](/graph/search-concept-aggregations) 优化搜索结果</span><span class="sxs-lookup"><span data-stu-id="1a9f3-177">Use [aggregations](/graph/search-concept-aggregations) to refine search results</span></span>


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


