---
ms.author: yiwenwang
title: searchRequest 资源类型
description: 要发送到查询终结点的搜索请求。 它包含响应中预期的实体类型、基础源、分页参数、字段请求和实际搜索查询。
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 7deba4c4c59947505b0ed6eff61a0d9cae5d59ef
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440121"
---
# <a name="searchrequest-resource-type"></a><span data-ttu-id="89876-104">searchRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="89876-104">searchRequest resource type</span></span>

<span data-ttu-id="89876-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89876-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [search-api-deprecation](../../includes/search-api-deprecation.md)]

<span data-ttu-id="89876-106">JSON blob 中格式化的搜索请求。</span><span class="sxs-lookup"><span data-stu-id="89876-106">A search request formatted in a JSON blob.</span></span> 

<span data-ttu-id="89876-107">JSON blob 包含响应中预期的资源类型、基础源、分页参数、排序选项、请求的聚合和字段以及实际搜索查询。</span><span class="sxs-lookup"><span data-stu-id="89876-107">The JSON blob contains the types of resources expected in the response, the underlying sources, paging parameters, sort options, requested aggregations and fields, and actual search query.</span></span> <span data-ttu-id="89876-108">请参阅 [各种](#see-also) 资源上的搜索请求示例。</span><span class="sxs-lookup"><span data-stu-id="89876-108">See [examples](#see-also) of search requests on various resources.</span></span>

> [!NOTE]
> <span data-ttu-id="89876-109">请注意搜索 [实体](search-api-overview.md#known-limitations) 类型的特定组合以及排序或聚合搜索结果的已知限制。</span><span class="sxs-lookup"><span data-stu-id="89876-109">Be aware of [known limitations](search-api-overview.md#known-limitations) on searching specific combinations of entity types, and sorting or aggregating search results.</span></span>


## <a name="properties"></a><span data-ttu-id="89876-110">属性</span><span class="sxs-lookup"><span data-stu-id="89876-110">Properties</span></span>

| <span data-ttu-id="89876-111">属性</span><span class="sxs-lookup"><span data-stu-id="89876-111">Property</span></span>     | <span data-ttu-id="89876-112">类型</span><span class="sxs-lookup"><span data-stu-id="89876-112">Type</span></span>        | <span data-ttu-id="89876-113">说明</span><span class="sxs-lookup"><span data-stu-id="89876-113">Description</span></span> |
|:-------------|:------------|:------------|:------------|
|<span data-ttu-id="89876-114">聚合</span><span class="sxs-lookup"><span data-stu-id="89876-114">aggregations</span></span>|<span data-ttu-id="89876-115">[aggregationOption](aggregationOption.md) 集合</span><span class="sxs-lookup"><span data-stu-id="89876-115">[aggregationOption](aggregationOption.md) collection</span></span>|<span data-ttu-id="89876-116">指定与 (一起返回) 精简程序。</span><span class="sxs-lookup"><span data-stu-id="89876-116">Specifies aggregations (also known as refiners) to be returned alongside search results.</span></span> <span data-ttu-id="89876-117">可选。</span><span class="sxs-lookup"><span data-stu-id="89876-117">Optional.</span></span>|
|<span data-ttu-id="89876-118">aggregationFilters</span><span class="sxs-lookup"><span data-stu-id="89876-118">aggregationFilters</span></span>|<span data-ttu-id="89876-119">字符串集合</span><span class="sxs-lookup"><span data-stu-id="89876-119">String collection</span></span>|<span data-ttu-id="89876-120">包含一个或多个筛选器，用于获取聚合并筛选为字段特定值的搜索结果。</span><span class="sxs-lookup"><span data-stu-id="89876-120">Contains one or more filters to obtain search results aggregated and filtered to a specific value of a field.</span></span> <span data-ttu-id="89876-121">可选。</span><span class="sxs-lookup"><span data-stu-id="89876-121">Optional.</span></span><br><span data-ttu-id="89876-122">基于按同一字段聚合的先前搜索生成此筛选器。</span><span class="sxs-lookup"><span data-stu-id="89876-122">Build this filter based on a prior search that aggregates by the same field.</span></span> <span data-ttu-id="89876-123">从之前搜索的响应中，确定将结果筛选为字段特定值的 [searchBucket，](searchBucket.md) 在其 **aggregationFilterToken 属性中使用该** 字符串，并构建一个聚合筛选器字符串，格式为 **"{field}： \\ "{aggregationFilterToken} \\ ""**。</span><span class="sxs-lookup"><span data-stu-id="89876-123">From the response of the prior search, identify the [searchBucket](searchBucket.md) that filters results to the specific value of the field, use the string in its **aggregationFilterToken** property, and build an aggregation filter string in the format **"{field}:\\"{aggregationFilterToken}\\""**.</span></span> <br><span data-ttu-id="89876-124">如果需要为同一字段提供多个值，请使用 **其 aggregationFilterToken** 属性中的字符串，并生成一个聚合筛选器字符串，格式为 **"{field}：或 \\ ("{aggregationFilterToken1} \\ "， \\ "{aggregationFilterToken2} \\ ") "。**</span><span class="sxs-lookup"><span data-stu-id="89876-124">If multiple values for the same field need to be provided, use the strings in its **aggregationFilterToken** property and build an aggregation filter string in the format **"{field}:or(\\"{aggregationFilterToken1}\\",\\"{aggregationFilterToken2}\\")"**.</span></span> <br><span data-ttu-id="89876-125">例如，按文件类型搜索和聚合驱动器项在响应中返回文件类型的 **searchBucket。** `docx`</span><span class="sxs-lookup"><span data-stu-id="89876-125">For example, searching and aggregating drive items by file type returns a **searchBucket** for the file type `docx` in the response.</span></span> <span data-ttu-id="89876-126">在后续搜索查询中，可以方便地使用此 **searchBucket** 返回的 **aggregationFilterToken，** 筛选器向下匹配以驱动 `docx` 文件类型的项。</span><span class="sxs-lookup"><span data-stu-id="89876-126">You can conveniently use the **aggregationFilterToken** returned for this **searchBucket** in a subsequent search query and filter matches down to drive items of the `docx` file type.</span></span> <span data-ttu-id="89876-127">[示例 1](/graph/search-concept-aggregation#example-1-request-aggregations-by-string-fields) [和示例 2](/graph/search-concept-aggregation#example-2-apply-an-aggregation-filter-based-on-a-previous-request) 显示实际请求和响应。</span><span class="sxs-lookup"><span data-stu-id="89876-127">[Example 1](/graph/search-concept-aggregation#example-1-request-aggregations-by-string-fields) and [example 2](/graph/search-concept-aggregation#example-2-apply-an-aggregation-filter-based-on-a-previous-request) show the actual requests and responses.</span></span>|
|<span data-ttu-id="89876-128">contentSources</span><span class="sxs-lookup"><span data-stu-id="89876-128">contentSources</span></span>|<span data-ttu-id="89876-129">字符串集合</span><span class="sxs-lookup"><span data-stu-id="89876-129">String collection</span></span>|<span data-ttu-id="89876-130">包含要定向的连接。</span><span class="sxs-lookup"><span data-stu-id="89876-130">Contains the connection to be targeted.</span></span> <br><span data-ttu-id="89876-131">遵循以下格式：在连接器管理中定义 `/external/connections/connectionid` `connectionid` ConnectionId 的位置。</span><span class="sxs-lookup"><span data-stu-id="89876-131">Respects the following format : `/external/connections/connectionid` where `connectionid` is the ConnectionId defined in the Connectors Administration.</span></span> <br> <span data-ttu-id="89876-132">注意：contentSource 仅适用于 entityType= `externalItem` 。</span><span class="sxs-lookup"><span data-stu-id="89876-132">Note: contentSource is only applicable when entityType=`externalItem`.</span></span> <span data-ttu-id="89876-133">可选。</span><span class="sxs-lookup"><span data-stu-id="89876-133">Optional.</span></span>|
|<span data-ttu-id="89876-134">enableTopResults</span><span class="sxs-lookup"><span data-stu-id="89876-134">enableTopResults</span></span>|<span data-ttu-id="89876-135">布尔</span><span class="sxs-lookup"><span data-stu-id="89876-135">Boolean</span></span>|<span data-ttu-id="89876-136">这将触发邮件的混合排序：前 3 条消息最相关。</span><span class="sxs-lookup"><span data-stu-id="89876-136">This triggers hybrid sort for messages: the first 3 messages are the most relevant.</span></span> <span data-ttu-id="89876-137">此属性仅适用于 entityType= `message` 。</span><span class="sxs-lookup"><span data-stu-id="89876-137">This property is only applicable to entityType=`message`.</span></span> <span data-ttu-id="89876-138">可选。</span><span class="sxs-lookup"><span data-stu-id="89876-138">Optional.</span></span>|
|<span data-ttu-id="89876-139">entityTypes</span><span class="sxs-lookup"><span data-stu-id="89876-139">entityTypes</span></span>|<span data-ttu-id="89876-140">entityType 集合</span><span class="sxs-lookup"><span data-stu-id="89876-140">entityType collection</span></span>| <span data-ttu-id="89876-141">响应中预期的一种或多种资源类型。</span><span class="sxs-lookup"><span data-stu-id="89876-141">One or more types of resources expected in the response.</span></span> <span data-ttu-id="89876-142">可取值为：`list`、`site`、`listItem`、`message`、`event`、`drive`、`driveItem`、`externalItem`。</span><span class="sxs-lookup"><span data-stu-id="89876-142">Possible values are: `list`, `site`, `listItem`, `message`, `event`, `drive`, `driveItem`, `externalItem`.</span></span> <span data-ttu-id="89876-143">请参阅 [同一](search-api-overview.md#known-limitations) 搜索请求中支持的两个或多个实体类型的这些组合的已知限制。</span><span class="sxs-lookup"><span data-stu-id="89876-143">See [known limitations](search-api-overview.md#known-limitations) for those combinations of two or more entity types that are supported in the same search request.</span></span> <span data-ttu-id="89876-144">必需。</span><span class="sxs-lookup"><span data-stu-id="89876-144">Required.</span></span>|
|<span data-ttu-id="89876-145">fields</span><span class="sxs-lookup"><span data-stu-id="89876-145">fields</span></span>|<span data-ttu-id="89876-146">字符串集合</span><span class="sxs-lookup"><span data-stu-id="89876-146">String collection</span></span> |<span data-ttu-id="89876-147">包含为 **entityTypes** 中指定的每个资源对象返回的字段，从而允许自定义默认情况下返回的字段，包括其他字段（如 SharePoint 和 OneDrive 中的自定义托管属性）或 Microsoft Graph 连接器引入的内容中的 **externalItem** 中的自定义字段。</span><span class="sxs-lookup"><span data-stu-id="89876-147">Contains the fields to be returned for each resource object specified in **entityTypes**, allowing customization of the fields returned by default otherwise, including additional fields such as custom managed properties from SharePoint and OneDrive, or custom fields in **externalItem** from content that Microsoft Graph connectors bring in.</span></span> <br><span data-ttu-id="89876-148">fields 属性可以使用应用于 [属性的](https://docs.microsoft.com/microsoftsearch/configure-connector#step-5-assign-property-labels) 语义标签。</span><span class="sxs-lookup"><span data-stu-id="89876-148">The fields property can be using the [semantic labels](https://docs.microsoft.com/microsoftsearch/configure-connector#step-5-assign-property-labels) applied to properties.</span></span> <span data-ttu-id="89876-149">例如，如果属性标记为标题，可以使用以下语法进行检索：label_title。</span><span class="sxs-lookup"><span data-stu-id="89876-149">For example, if a property is label as title, you can retrieve it using the following syntax : label_title.</span></span><br><span data-ttu-id="89876-150">可选。</span><span class="sxs-lookup"><span data-stu-id="89876-150">Optional.</span></span>|
|<span data-ttu-id="89876-151">发件人</span><span class="sxs-lookup"><span data-stu-id="89876-151">from</span></span>|<span data-ttu-id="89876-152">Int32</span><span class="sxs-lookup"><span data-stu-id="89876-152">Int32</span></span>|<span data-ttu-id="89876-153">指定搜索结果的偏移量。</span><span class="sxs-lookup"><span data-stu-id="89876-153">Specifies the offset for the search results.</span></span> <span data-ttu-id="89876-154">偏移量 0 返回第一个结果。</span><span class="sxs-lookup"><span data-stu-id="89876-154">Offset 0 returns the very first result.</span></span> <span data-ttu-id="89876-155">可选。</span><span class="sxs-lookup"><span data-stu-id="89876-155">Optional.</span></span>|
|<span data-ttu-id="89876-156">查询</span><span class="sxs-lookup"><span data-stu-id="89876-156">query</span></span>|[<span data-ttu-id="89876-157">searchQuery</span><span class="sxs-lookup"><span data-stu-id="89876-157">searchQuery</span></span>](searchquery.md)|<span data-ttu-id="89876-158">包含查询词。</span><span class="sxs-lookup"><span data-stu-id="89876-158">Contains the query terms.</span></span> <span data-ttu-id="89876-159">必需。</span><span class="sxs-lookup"><span data-stu-id="89876-159">Required.</span></span>|
|<span data-ttu-id="89876-160">size</span><span class="sxs-lookup"><span data-stu-id="89876-160">size</span></span>|<span data-ttu-id="89876-161">Int32</span><span class="sxs-lookup"><span data-stu-id="89876-161">Int32</span></span>|<span data-ttu-id="89876-162">要检索的页面的大小。</span><span class="sxs-lookup"><span data-stu-id="89876-162">The size of the page to be retrieved.</span></span> <span data-ttu-id="89876-163">可选。</span><span class="sxs-lookup"><span data-stu-id="89876-163">Optional.</span></span>|
|<span data-ttu-id="89876-164">sortProperties</span><span class="sxs-lookup"><span data-stu-id="89876-164">sortProperties</span></span>|<span data-ttu-id="89876-165">[sortProperty](sortProperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="89876-165">[sortProperty](sortProperty.md) collection</span></span>|<span data-ttu-id="89876-166">包含排序结果的字段和方向的有序集合。</span><span class="sxs-lookup"><span data-stu-id="89876-166">Contains the ordered collection of fields and direction to sort results.</span></span> <span data-ttu-id="89876-167">集合中最多只能有 5 个排序属性。</span><span class="sxs-lookup"><span data-stu-id="89876-167">There can be at most 5 sort properties in the collection.</span></span> <span data-ttu-id="89876-168">可选。</span><span class="sxs-lookup"><span data-stu-id="89876-168">Optional.</span></span>|
|<span data-ttu-id="89876-169">stored_fields (已弃) </span><span class="sxs-lookup"><span data-stu-id="89876-169">stored_fields (deprecated)</span></span>|<span data-ttu-id="89876-170">字符串集合</span><span class="sxs-lookup"><span data-stu-id="89876-170">String collection</span></span> |<span data-ttu-id="89876-171">现在，这被 **fields 属性** 所取代。</span><span class="sxs-lookup"><span data-stu-id="89876-171">This is now replaced by the **fields** property.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="89876-172">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="89876-172">JSON representation</span></span>

<span data-ttu-id="89876-173">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="89876-173">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="89876-174">另请参阅</span><span class="sxs-lookup"><span data-stu-id="89876-174">See also</span></span>
- <span data-ttu-id="89876-175">搜索 [邮件](/graph/search-concept-messages)</span><span class="sxs-lookup"><span data-stu-id="89876-175">Search [mail messages](/graph/search-concept-messages)</span></span>
- <span data-ttu-id="89876-176">搜索 [日历事件](/graph/search-concept-events)</span><span class="sxs-lookup"><span data-stu-id="89876-176">Search [calendar events](/graph/search-concept-events)</span></span>
- <span data-ttu-id="89876-177">搜索 SharePoint 和 OneDrive ([文件、列表和网站) ](/graph/search-concept-files)</span><span class="sxs-lookup"><span data-stu-id="89876-177">Search content in SharePoint and OneDrive ([files, lists and sites](/graph/search-concept-files))</span></span>
- <span data-ttu-id="89876-178">搜索 [使用连接器导入的自定义) ](/graph/search-concept-custom-types) 数据</span><span class="sxs-lookup"><span data-stu-id="89876-178">Search [custom types imported using connectors)](/graph/search-concept-custom-types) data</span></span>
- <span data-ttu-id="89876-179">[对](/graph/search-concept-sort) 搜索结果进行排序</span><span class="sxs-lookup"><span data-stu-id="89876-179">[Sort](/graph/search-concept-sort) search results</span></span>
- <span data-ttu-id="89876-180">使用 [聚合](/graph/search-concept-aggregations) 优化搜索结果</span><span class="sxs-lookup"><span data-stu-id="89876-180">Use [aggregations](/graph/search-concept-aggregations) to refine search results</span></span>


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


