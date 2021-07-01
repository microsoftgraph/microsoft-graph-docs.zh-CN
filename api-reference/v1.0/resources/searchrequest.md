---
title: searchRequest 资源类型
description: 要发送到查询终结点的搜索请求。 它包含响应中预期的实体类型、基础源、分页参数、字段请求和实际搜索查询。
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 4a797126a1dc6bc5fbecc9aad050711b499945ff
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207985"
---
# <a name="searchrequest-resource-type"></a><span data-ttu-id="2e16c-104">searchRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="2e16c-104">searchRequest resource type</span></span>

<span data-ttu-id="2e16c-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e16c-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2e16c-106">JSON blob 中格式化的搜索请求。</span><span class="sxs-lookup"><span data-stu-id="2e16c-106">A search request formatted in a JSON blob.</span></span> 

<span data-ttu-id="2e16c-107">JSON blob 包含响应中预期的资源类型、基础源、分页参数、排序选项、请求的聚合和字段以及实际搜索查询。</span><span class="sxs-lookup"><span data-stu-id="2e16c-107">The JSON blob contains the types of resources expected in the response, the underlying sources, paging parameters, sort options, requested aggregations and fields, and actual search query.</span></span> <span data-ttu-id="2e16c-108">请参阅 [各种](#see-also) 资源上的搜索请求示例。</span><span class="sxs-lookup"><span data-stu-id="2e16c-108">See [examples](#see-also) of search requests on various resources.</span></span>

> [!NOTE]
> <span data-ttu-id="2e16c-109">请注意搜索 [实体](search-api-overview.md#known-limitations) 类型的特定组合以及排序或聚合搜索结果的已知限制。</span><span class="sxs-lookup"><span data-stu-id="2e16c-109">Be aware of [known limitations](search-api-overview.md#known-limitations) on searching specific combinations of entity types, and sorting or aggregating search results.</span></span>


## <a name="properties"></a><span data-ttu-id="2e16c-110">属性</span><span class="sxs-lookup"><span data-stu-id="2e16c-110">Properties</span></span>

| <span data-ttu-id="2e16c-111">属性</span><span class="sxs-lookup"><span data-stu-id="2e16c-111">Property</span></span>     | <span data-ttu-id="2e16c-112">类型</span><span class="sxs-lookup"><span data-stu-id="2e16c-112">Type</span></span>        | <span data-ttu-id="2e16c-113">说明</span><span class="sxs-lookup"><span data-stu-id="2e16c-113">Description</span></span> |             |
|:-------------|:------------|:------------|:------------|
|<span data-ttu-id="2e16c-114">contentSources</span><span class="sxs-lookup"><span data-stu-id="2e16c-114">contentSources</span></span>|<span data-ttu-id="2e16c-115">String collection</span><span class="sxs-lookup"><span data-stu-id="2e16c-115">String collection</span></span>|<span data-ttu-id="2e16c-116">包含要定向的连接。</span><span class="sxs-lookup"><span data-stu-id="2e16c-116">Contains the connection to be targeted.</span></span>|
|<span data-ttu-id="2e16c-117">enableTopResults</span><span class="sxs-lookup"><span data-stu-id="2e16c-117">enableTopResults</span></span>|<span data-ttu-id="2e16c-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="2e16c-118">Boolean</span></span>|<span data-ttu-id="2e16c-119">这将触发邮件的混合排序：前 3 个邮件最相关。</span><span class="sxs-lookup"><span data-stu-id="2e16c-119">This triggers hybrid sort for messages : the first 3 messages are the most relevant.</span></span> <span data-ttu-id="2e16c-120">此属性仅适用于 entityType= `message` 。</span><span class="sxs-lookup"><span data-stu-id="2e16c-120">This property is only applicable to entityType=`message`.</span></span> <span data-ttu-id="2e16c-121">可选。</span><span class="sxs-lookup"><span data-stu-id="2e16c-121">Optional.</span></span>|
|<span data-ttu-id="2e16c-122">entityTypes</span><span class="sxs-lookup"><span data-stu-id="2e16c-122">entityTypes</span></span>|<span data-ttu-id="2e16c-123">entityType 集合</span><span class="sxs-lookup"><span data-stu-id="2e16c-123">entityType collection</span></span>| <span data-ttu-id="2e16c-124">响应中预期的一种或多种资源类型。</span><span class="sxs-lookup"><span data-stu-id="2e16c-124">One or more types of resources expected in the response.</span></span> <span data-ttu-id="2e16c-125">可取值为：`list`、`site`、`listItem`、`message`、`event`、`drive`、`driveItem`、`externalItem`。</span><span class="sxs-lookup"><span data-stu-id="2e16c-125">Possible values are: `list`, `site`, `listItem`, `message`, `event`, `drive`, `driveItem`, `externalItem`.</span></span> <span data-ttu-id="2e16c-126">有关 [同一](search-api-overview.md#known-limitations) 搜索请求中支持的两个或多个实体类型的组合，请参阅已知限制。</span><span class="sxs-lookup"><span data-stu-id="2e16c-126">See [known limitations](search-api-overview.md#known-limitations) for those combinations of two or more entity types that are supported in the same search request.</span></span> <span data-ttu-id="2e16c-127">必填。</span><span class="sxs-lookup"><span data-stu-id="2e16c-127">Required.</span></span>|
|<span data-ttu-id="2e16c-128">fields</span><span class="sxs-lookup"><span data-stu-id="2e16c-128">fields</span></span>|<span data-ttu-id="2e16c-129">String collection</span><span class="sxs-lookup"><span data-stu-id="2e16c-129">String collection</span></span> |<span data-ttu-id="2e16c-130">包含为 **entityTypes** 中指定的每个资源对象返回的字段，允许自定义默认情况下返回的字段，包括其他字段，如 SharePoint 和 OneDrive。</span><span class="sxs-lookup"><span data-stu-id="2e16c-130">Contains the fields to be returned for each resource object specified in **entityTypes**, allowing customization of the fields returned by default otherwise, including additional fields such as custom managed properties from SharePoint and OneDrive.</span></span> <span data-ttu-id="2e16c-131">可选。</span><span class="sxs-lookup"><span data-stu-id="2e16c-131">Optional.</span></span>|
|<span data-ttu-id="2e16c-132">起始数量</span><span class="sxs-lookup"><span data-stu-id="2e16c-132">from</span></span>|<span data-ttu-id="2e16c-133">Int32</span><span class="sxs-lookup"><span data-stu-id="2e16c-133">Int32</span></span>|<span data-ttu-id="2e16c-134">指定搜索结果的偏移量。</span><span class="sxs-lookup"><span data-stu-id="2e16c-134">Specifies the offset for the search results.</span></span> <span data-ttu-id="2e16c-135">偏移量 0 返回第一个结果。</span><span class="sxs-lookup"><span data-stu-id="2e16c-135">Offset 0 returns the very first result.</span></span> <span data-ttu-id="2e16c-136">可选。</span><span class="sxs-lookup"><span data-stu-id="2e16c-136">Optional.</span></span>|
|<span data-ttu-id="2e16c-137">查询</span><span class="sxs-lookup"><span data-stu-id="2e16c-137">query</span></span>|[<span data-ttu-id="2e16c-138">searchQuery</span><span class="sxs-lookup"><span data-stu-id="2e16c-138">searchQuery</span></span>](searchquery.md)|<span data-ttu-id="2e16c-139">包含查询词。</span><span class="sxs-lookup"><span data-stu-id="2e16c-139">Contains the query terms.</span></span> <span data-ttu-id="2e16c-140">必填。</span><span class="sxs-lookup"><span data-stu-id="2e16c-140">Required.</span></span>|
|<span data-ttu-id="2e16c-141">size</span><span class="sxs-lookup"><span data-stu-id="2e16c-141">size</span></span>|<span data-ttu-id="2e16c-142">Int32</span><span class="sxs-lookup"><span data-stu-id="2e16c-142">Int32</span></span>|<span data-ttu-id="2e16c-143">要检索的页面的大小。</span><span class="sxs-lookup"><span data-stu-id="2e16c-143">The size of the page to be retrieved.</span></span> <span data-ttu-id="2e16c-144">可选。</span><span class="sxs-lookup"><span data-stu-id="2e16c-144">Optional.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2e16c-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2e16c-145">JSON representation</span></span>

<span data-ttu-id="2e16c-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2e16c-146">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="2e16c-147">另请参阅</span><span class="sxs-lookup"><span data-stu-id="2e16c-147">See also</span></span>
- <span data-ttu-id="2e16c-148">搜索 [邮件](/graph/search-concept-messages)</span><span class="sxs-lookup"><span data-stu-id="2e16c-148">Search [mail messages](/graph/search-concept-messages)</span></span>
- <span data-ttu-id="2e16c-149">搜索 [日历事件](/graph/search-concept-events)</span><span class="sxs-lookup"><span data-stu-id="2e16c-149">Search [calendar events](/graph/search-concept-events)</span></span>
- <span data-ttu-id="2e16c-150">搜索网站[SharePoint OneDrive (、列表和网站) ](/graph/search-concept-files)</span><span class="sxs-lookup"><span data-stu-id="2e16c-150">Search content in SharePoint and OneDrive ([files, lists and sites](/graph/search-concept-files))</span></span>



<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


