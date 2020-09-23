---
title: Microsoft Graph 连接的注册架构
description: 了解如何使用 Microsoft Graph 为 Microsoft Graph 连接注册架构
localization_priority: Priority
author: rsamai
ms.prod: search
doc_type: conceptualPageType
ms.openlocfilehash: 0e70f712b7965e97df7255cda3dcf94c69f73691
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193679"
---
# <a name="register-schema-for-the-microsoft-graph-connection"></a><span data-ttu-id="d63e9-103">Microsoft Graph 连接的注册架构</span><span class="sxs-lookup"><span data-stu-id="d63e9-103">Register schema for the Microsoft Graph connection</span></span>

<span data-ttu-id="d63e9-104">连接[架构](/graph/api/resources/schema?view=graph-rest-beta&preserve-view=true)确定如何将内容用于各种 Microsoft Graph 体验。</span><span class="sxs-lookup"><span data-stu-id="d63e9-104">The connection [schema](/graph/api/resources/schema?view=graph-rest-beta&preserve-view=true) determines how your content will be used in various Microsoft Graph experiences.</span></span> <span data-ttu-id="d63e9-105">架构是计划添加到连接中的所有属性的简单列表及其属性、标签和别名。</span><span class="sxs-lookup"><span data-stu-id="d63e9-105">Schema is a flat list of all the properties that you plan to add to the connection along with their attributes, labels, and aliases.</span></span> <span data-ttu-id="d63e9-106">向连接添加项目前，必须注册架构。</span><span class="sxs-lookup"><span data-stu-id="d63e9-106">You must register the schema before adding items into the connection.</span></span>

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

## <a name="example-schema"></a><span data-ttu-id="d63e9-107">示例架构</span><span class="sxs-lookup"><span data-stu-id="d63e9-107">Example schema</span></span>

<span data-ttu-id="d63e9-108">下表提供了工作票据系统连接器可能的架构示例。</span><span class="sxs-lookup"><span data-stu-id="d63e9-108">The following table represents an example of a possible schema for a work ticket system connector.</span></span>

| <span data-ttu-id="d63e9-109">属性</span><span class="sxs-lookup"><span data-stu-id="d63e9-109">Property</span></span>       | <span data-ttu-id="d63e9-110">类型</span><span class="sxs-lookup"><span data-stu-id="d63e9-110">Type</span></span>             | <span data-ttu-id="d63e9-111">可搜索</span><span class="sxs-lookup"><span data-stu-id="d63e9-111">Searchable</span></span>         | <span data-ttu-id="d63e9-112">可查询</span><span class="sxs-lookup"><span data-stu-id="d63e9-112">Queryable</span></span>          | <span data-ttu-id="d63e9-113">可检索</span><span class="sxs-lookup"><span data-stu-id="d63e9-113">Retrievable</span></span>        | <span data-ttu-id="d63e9-114">可精简</span><span class="sxs-lookup"><span data-stu-id="d63e9-114">Refinable</span></span>          | <span data-ttu-id="d63e9-115">标签</span><span class="sxs-lookup"><span data-stu-id="d63e9-115">Labels</span></span>               | <span data-ttu-id="d63e9-116">别名</span><span class="sxs-lookup"><span data-stu-id="d63e9-116">Aliases</span></span>    |
|----------------|------------------|--------------------|--------------------|--------------------|--------------------|----------------------|------------|
| <span data-ttu-id="d63e9-117">ticketId</span><span class="sxs-lookup"><span data-stu-id="d63e9-117">ticketId</span></span>       | <span data-ttu-id="d63e9-118">String</span><span class="sxs-lookup"><span data-stu-id="d63e9-118">String</span></span>           |                    |                    |                    |                    |                      | <span data-ttu-id="d63e9-119">ID</span><span class="sxs-lookup"><span data-stu-id="d63e9-119">ID</span></span>         |
| <span data-ttu-id="d63e9-120">title</span><span class="sxs-lookup"><span data-stu-id="d63e9-120">title</span></span>          | <span data-ttu-id="d63e9-121">String</span><span class="sxs-lookup"><span data-stu-id="d63e9-121">String</span></span>           | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |                    | <span data-ttu-id="d63e9-125">title</span><span class="sxs-lookup"><span data-stu-id="d63e9-125">title</span></span>                |            |
| <span data-ttu-id="d63e9-126">createdBy</span><span class="sxs-lookup"><span data-stu-id="d63e9-126">createdBy</span></span>      | <span data-ttu-id="d63e9-127">String</span><span class="sxs-lookup"><span data-stu-id="d63e9-127">String</span></span>           | :heavy_check_mark: | :heavy_check_mark: |                    |                    | <span data-ttu-id="d63e9-130">createdBy</span><span class="sxs-lookup"><span data-stu-id="d63e9-130">createdBy</span></span>            | <span data-ttu-id="d63e9-131">Creator</span><span class="sxs-lookup"><span data-stu-id="d63e9-131">creator</span></span>    |
| <span data-ttu-id="d63e9-132">assignedTo</span><span class="sxs-lookup"><span data-stu-id="d63e9-132">assignedTo</span></span>     | <span data-ttu-id="d63e9-133">String</span><span class="sxs-lookup"><span data-stu-id="d63e9-133">String</span></span>           | :heavy_check_mark: | :heavy_check_mark: |                    |                    |                      |            |
| <span data-ttu-id="d63e9-136">lastEditedDate</span><span class="sxs-lookup"><span data-stu-id="d63e9-136">lastEditedDate</span></span> | <span data-ttu-id="d63e9-137">日期时间</span><span class="sxs-lookup"><span data-stu-id="d63e9-137">DateTime</span></span>         |                    | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | <span data-ttu-id="d63e9-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d63e9-141">lastModifiedDateTime</span></span> | <span data-ttu-id="d63e9-142">editedDate</span><span class="sxs-lookup"><span data-stu-id="d63e9-142">editedDate</span></span> |
| <span data-ttu-id="d63e9-143">lastEditedBy</span><span class="sxs-lookup"><span data-stu-id="d63e9-143">lastEditedBy</span></span>   | <span data-ttu-id="d63e9-144">String</span><span class="sxs-lookup"><span data-stu-id="d63e9-144">String</span></span>           | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |                    | <span data-ttu-id="d63e9-148">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="d63e9-148">lastModifiedBy</span></span>       | <span data-ttu-id="d63e9-149">已编辑</span><span class="sxs-lookup"><span data-stu-id="d63e9-149">edited</span></span>     |
| <span data-ttu-id="d63e9-150">workItemType</span><span class="sxs-lookup"><span data-stu-id="d63e9-150">workItemType</span></span>   | <span data-ttu-id="d63e9-151">String</span><span class="sxs-lookup"><span data-stu-id="d63e9-151">String</span></span>           |                    | :heavy_check_mark: | :heavy_check_mark: |                    |                      | <span data-ttu-id="d63e9-154">ticketType</span><span class="sxs-lookup"><span data-stu-id="d63e9-154">ticketType</span></span> |
| <span data-ttu-id="d63e9-155">priority</span><span class="sxs-lookup"><span data-stu-id="d63e9-155">priority</span></span>       | <span data-ttu-id="d63e9-156">Int64</span><span class="sxs-lookup"><span data-stu-id="d63e9-156">Int64</span></span>            | :heavy_check_mark: |                    |                    |                    |                      |            |
| <span data-ttu-id="d63e9-158">标记</span><span class="sxs-lookup"><span data-stu-id="d63e9-158">tags</span></span>           | <span data-ttu-id="d63e9-159">StringCollection</span><span class="sxs-lookup"><span data-stu-id="d63e9-159">StringCollection</span></span> |                    | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |                      |            |
| <span data-ttu-id="d63e9-163">状态</span><span class="sxs-lookup"><span data-stu-id="d63e9-163">status</span></span>         | <span data-ttu-id="d63e9-164">String</span><span class="sxs-lookup"><span data-stu-id="d63e9-164">String</span></span>           |                    | :heavy_check_mark: | :heavy_check_mark: |                    |                      |            |
| <span data-ttu-id="d63e9-167">url</span><span class="sxs-lookup"><span data-stu-id="d63e9-167">url</span></span>            | <span data-ttu-id="d63e9-168">String</span><span class="sxs-lookup"><span data-stu-id="d63e9-168">String</span></span>           |                    |                    |                    |                    | <span data-ttu-id="d63e9-169">url</span><span class="sxs-lookup"><span data-stu-id="d63e9-169">url</span></span>                  |            |
| <span data-ttu-id="d63e9-170">已解决</span><span class="sxs-lookup"><span data-stu-id="d63e9-170">resolved</span></span>       | <span data-ttu-id="d63e9-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="d63e9-171">Boolean</span></span>          |                    | :heavy_check_mark: | :heavy_check_mark: |                    |                      |            |

## <a name="property-attributes"></a><span data-ttu-id="d63e9-174">Property 属性</span><span class="sxs-lookup"><span data-stu-id="d63e9-174">Property attributes</span></span>

### <a name="searchable"></a><span data-ttu-id="d63e9-175">可搜索</span><span class="sxs-lookup"><span data-stu-id="d63e9-175">Searchable</span></span>

<span data-ttu-id="d63e9-176">如果属性可搜索，则将其值添加到全文检索。</span><span class="sxs-lookup"><span data-stu-id="d63e9-176">If a property is searchable, its value is added to the full text index.</span></span> <span data-ttu-id="d63e9-177">当用户执行搜索时，如果其中一个可搜索字段或其[内容](search-index-manage-items.md#content)中有搜索命中率，则会返回结果。</span><span class="sxs-lookup"><span data-stu-id="d63e9-177">When a user performs a search, we return results if there is a search hit in one of the searchable fields or its [content](search-index-manage-items.md#content).</span></span>

<!-- markdownlint-disable MD036 -->
<span data-ttu-id="d63e9-178">![搜索“设计”，显示针对属性和内容的点击结果](./images/search-index-manage-items-schema-1.svg)</span><span class="sxs-lookup"><span data-stu-id="d63e9-178">![A search for "design" displaying results for hits against properties and content](./images/search-index-manage-items-schema-1.svg)</span></span>

<span data-ttu-id="d63e9-179">*搜索“设计”，显示针对属性（`title`, `tags`）和内容的点击结果*</span><span class="sxs-lookup"><span data-stu-id="d63e9-179">*A search for "design" displaying results for hits against properties (`title`, `tags`) and content*</span></span>

### <a name="queryable"></a><span data-ttu-id="d63e9-180">可查询</span><span class="sxs-lookup"><span data-stu-id="d63e9-180">Queryable</span></span>

<span data-ttu-id="d63e9-181">如果属性可查询，则可以使用知识查询语言 (KQL) 对其进行查询。</span><span class="sxs-lookup"><span data-stu-id="d63e9-181">If a property is queryable, you can query against it using knowledge query language (KQL).</span></span> <span data-ttu-id="d63e9-182">KQL 由一个或多个自由文本关键词（单词或短语）或属性限制组成。</span><span class="sxs-lookup"><span data-stu-id="d63e9-182">KQL consists of 1 or more free text keywords (words or phrases) or property restrictions.</span></span> <span data-ttu-id="d63e9-183">属性名称必须包含在查询中：在查询本身中指定或以编程方式包含在查询中。</span><span class="sxs-lookup"><span data-stu-id="d63e9-183">The property name must be included in the query, either specified in the query itself or included in the query programmatically.</span></span> <span data-ttu-id="d63e9-184">可将前缀与通配符 (\*) 搭配使用。</span><span class="sxs-lookup"><span data-stu-id="d63e9-184">You can use prefix matching with the wildcard operator(\*).</span></span>

> [!NOTE]
> <span data-ttu-id="d63e9-185">不支持后缀匹配。</span><span class="sxs-lookup"><span data-stu-id="d63e9-185">Suffix matching is not supported.</span></span>

![搜索“search ba\*”，显示与此前缀匹配的结果](./images/search-index-manage-items-schema-2.svg)

<span data-ttu-id="d63e9-187">*搜索“search ba*”，显示与此前缀 \* 匹配的结果</span><span class="sxs-lookup"><span data-stu-id="d63e9-187">*A search for "search ba*" displaying results that match this prefix\*</span></span>

![搜索“tags:design”，结果范围限定为 tags 属性中包含“design”的项](./images/search-index-manage-items-schema-3.svg)

<span data-ttu-id="d63e9-189">*搜索“tags:design”，结果范围限定为 tags 属性中包含“design”的项*</span><span class="sxs-lookup"><span data-stu-id="d63e9-189">*A search for "tags:design" scoping down results to items with "design" in the tags property*</span></span>

### <a name="retrievable"></a><span data-ttu-id="d63e9-190">可检索</span><span class="sxs-lookup"><span data-stu-id="d63e9-190">Retrievable</span></span>

<span data-ttu-id="d63e9-191">如果属性可检索，则其值可以在搜索结果中返回。</span><span class="sxs-lookup"><span data-stu-id="d63e9-191">If a property is retrievable, its value can be returned in search results.</span></span> <span data-ttu-id="d63e9-192">希望将任何属性添加到显示模板，或者从查询中返回，并且在搜索结果中相关，则该属性必须是可检索的。</span><span class="sxs-lookup"><span data-stu-id="d63e9-192">Any property that you want to add in the display template or be returned from the query and be relevant in search results must be retrievable.</span></span> <span data-ttu-id="d63e9-193">将较大的属性（如 `editHistory`或属性过多）标记为可检索会增加搜索延迟。</span><span class="sxs-lookup"><span data-stu-id="d63e9-193">Marking large properties, such as `editHistory`, or too many properties as retrievable will increase search latency.</span></span> <span data-ttu-id="d63e9-194">是可选择的并选择相关属性。</span><span class="sxs-lookup"><span data-stu-id="d63e9-194">Be selective and choose relevant properties.</span></span>

![结果所呈现的一组可检索属性](./images/search-index-manage-schema-4.svg)

<span data-ttu-id="d63e9-196">*结果所呈现的一组可检索属性（`title`、 `lastEditedBy` 等）*</span><span class="sxs-lookup"><span data-stu-id="d63e9-196">*A set of retrievable properties (`title`, `lastEditedBy` etc.) rendered as a result*</span></span>

### <a name="refinable"></a><span data-ttu-id="d63e9-197">可精简</span><span class="sxs-lookup"><span data-stu-id="d63e9-197">Refinable</span></span>

<span data-ttu-id="d63e9-198">如果属性是可精简的，则管理员可将其配置为 Microsoft 搜索结果页面中的自定义筛选器。</span><span class="sxs-lookup"><span data-stu-id="d63e9-198">If a property is refinable, an admin can configure it as a custom filter in the Microsoft Search results page.</span></span>

![按标记优化结果，可精简属性](./images/search-index-manage-schema-5.svg)

<span data-ttu-id="d63e9-200">*按`tags`优化结果，可精简属性*</span><span class="sxs-lookup"><span data-stu-id="d63e9-200">*Refine results by `tags`, a refinable property*</span></span>

## <a name="labels"></a><span data-ttu-id="d63e9-201">标签</span><span class="sxs-lookup"><span data-stu-id="d63e9-201">Labels</span></span>

<span data-ttu-id="d63e9-202">标签是 Microsoft 发布的众所周知的标记，可在架构中针对属性进行添加。</span><span class="sxs-lookup"><span data-stu-id="d63e9-202">A label is a well known tag published by Microsoft that you can add against a property in your schema.</span></span> <span data-ttu-id="d63e9-203">添加标签有助于各种 Microsoft 产品理解属性并提供更好的体验。</span><span class="sxs-lookup"><span data-stu-id="d63e9-203">Adding a label helps various Microsoft products understand the property and provide a better experience.</span></span>

| <span data-ttu-id="d63e9-204">标签</span><span class="sxs-lookup"><span data-stu-id="d63e9-204">Label</span></span>                 | <span data-ttu-id="d63e9-205">说明</span><span class="sxs-lookup"><span data-stu-id="d63e9-205">Description</span></span>                                                                          |
|---------------------- |------------------------------------------------------------------------------------- |
| <span data-ttu-id="d63e9-206">title</span><span class="sxs-lookup"><span data-stu-id="d63e9-206">title</span></span>                 | <span data-ttu-id="d63e9-207">要在搜索中显示的项目标题和其他体验</span><span class="sxs-lookup"><span data-stu-id="d63e9-207">The title of the item that you want shown in search & other experiences</span></span>              |
| <span data-ttu-id="d63e9-208">url</span><span class="sxs-lookup"><span data-stu-id="d63e9-208">url</span></span>                   | <span data-ttu-id="d63e9-209">数据源中的项的目标 URL</span><span class="sxs-lookup"><span data-stu-id="d63e9-209">The target URL of the item in the data source</span></span>                                        |
| <span data-ttu-id="d63e9-210">createdBy</span><span class="sxs-lookup"><span data-stu-id="d63e9-210">createdBy</span></span>             | <span data-ttu-id="d63e9-211">数据源中的项创建者的姓名</span><span class="sxs-lookup"><span data-stu-id="d63e9-211">Name of the person who created the item in the data source</span></span>                           |
| <span data-ttu-id="d63e9-212">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="d63e9-212">lastModifiedBy</span></span>        | <span data-ttu-id="d63e9-213">数据源中的项最近编辑者的姓名</span><span class="sxs-lookup"><span data-stu-id="d63e9-213">Name of the person who most recently edited the item in the data source</span></span>              |
| <span data-ttu-id="d63e9-214">authors</span><span class="sxs-lookup"><span data-stu-id="d63e9-214">authors</span></span>               | <span data-ttu-id="d63e9-215">数据源中的项参加/合作所有人员的姓名</span><span class="sxs-lookup"><span data-stu-id="d63e9-215">Name of all the people who participated/collaborated on the item in the data source</span></span>  |
| <span data-ttu-id="d63e9-216">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d63e9-216">createdDateTime</span></span>       | <span data-ttu-id="d63e9-217">在数据源中创建项的日期和时间</span><span class="sxs-lookup"><span data-stu-id="d63e9-217">Date & time that the item was created in the data source</span></span>                             |
| <span data-ttu-id="d63e9-218">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d63e9-218">lastModifiedDateTime</span></span>  | <span data-ttu-id="d63e9-219">在数据源中修正项的日期和时间</span><span class="sxs-lookup"><span data-stu-id="d63e9-219">Date & time the item was last modified in the data source</span></span>                            |
| <span data-ttu-id="d63e9-220">fileName</span><span class="sxs-lookup"><span data-stu-id="d63e9-220">fileName</span></span>              | <span data-ttu-id="d63e9-221">对于文件，则为数据源中的文件名称</span><span class="sxs-lookup"><span data-stu-id="d63e9-221">In case of a file, the name of the file in the data source</span></span>                           |
| <span data-ttu-id="d63e9-222">FileExtension</span><span class="sxs-lookup"><span data-stu-id="d63e9-222">fileExtension</span></span>         | <span data-ttu-id="d63e9-223">对于文件，则为数据源中的文件扩展</span><span class="sxs-lookup"><span data-stu-id="d63e9-223">In case of a file, the extension of the file in the data source</span></span>                      |

<span data-ttu-id="d63e9-224">例如，*lastEditedBy* 连接属性与 Microsoft label *lastModifiedBy*的含义相同。</span><span class="sxs-lookup"><span data-stu-id="d63e9-224">For example, the connection property *lastEditedBy* has the same meaning as the Microsoft label *lastModifiedBy*.</span></span>

<span data-ttu-id="d63e9-225">添加尽可能多的标签，但要确保它们准确地映射到属性。</span><span class="sxs-lookup"><span data-stu-id="d63e9-225">Add as many labels as you can, but ensure that they are accurately mapped to properties.</span></span> <span data-ttu-id="d63e9-226">如果标签没有意义，请不要向属性中添加。</span><span class="sxs-lookup"><span data-stu-id="d63e9-226">Do not add a label to a property if it doesn't make sense.</span></span> <span data-ttu-id="d63e9-227">不正确的映射将降低体验。</span><span class="sxs-lookup"><span data-stu-id="d63e9-227">Incorrect mappings will deteriorate the experience.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="d63e9-228">所有映射到标签的属性都必须可供检索。</span><span class="sxs-lookup"><span data-stu-id="d63e9-228">All properties that you map to labels must be retrievable.</span></span>

### <a name="relevance"></a><span data-ttu-id="d63e9-229">相关性</span><span class="sxs-lookup"><span data-stu-id="d63e9-229">Relevance</span></span>

<span data-ttu-id="d63e9-230">通过应用尽可能多地正确映射的标签，你还可以通过搜索改进内容的发现。</span><span class="sxs-lookup"><span data-stu-id="d63e9-230">By applying as many accurately mapped labels as possible, you can also improve the discovery of your content through search.</span></span> <span data-ttu-id="d63e9-231">我们极力建议你尽可能多地定义如下所示的标签，并按对发现顺序的潜在影响进行降序：</span><span class="sxs-lookup"><span data-stu-id="d63e9-231">We highly recommend defining as many of the below labels as possible, listed by potential impact on discovery in descending order:</span></span>

- <span data-ttu-id="d63e9-232">title</span><span class="sxs-lookup"><span data-stu-id="d63e9-232">title</span></span>
- <span data-ttu-id="d63e9-233">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d63e9-233">lastModifiedDateTime</span></span>
- <span data-ttu-id="d63e9-234">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="d63e9-234">lastModifiedBy</span></span>
- <span data-ttu-id="d63e9-235">url</span><span class="sxs-lookup"><span data-stu-id="d63e9-235">url</span></span>
- <span data-ttu-id="d63e9-236">文件名</span><span class="sxs-lookup"><span data-stu-id="d63e9-236">filename</span></span>
- <span data-ttu-id="d63e9-237">FileExtension</span><span class="sxs-lookup"><span data-stu-id="d63e9-237">fileExtension</span></span>

<span data-ttu-id="d63e9-238">对于发现，即搜索方案，请注意：</span><span class="sxs-lookup"><span data-stu-id="d63e9-238">For discovery, i.e. search scenarios, please note:</span></span>

- <span data-ttu-id="d63e9-239">确保你的映射准确。</span><span class="sxs-lookup"><span data-stu-id="d63e9-239">Ensure that your mappings are accurate.</span></span>
- <span data-ttu-id="d63e9-240">将属性用作包含大型内容的标签时，可能会增加搜索延迟，并且必须等待更长的时间才能使搜索返回结果。</span><span class="sxs-lookup"><span data-stu-id="d63e9-240">When you use a property as label that contains large content, you might increase search latency and have to wait longer for search to return results.</span></span>
- <span data-ttu-id="d63e9-241">尤其是在配置自定义垂直的情况下允许通过多个连接进行搜索的情况下，搜索结果在指定尽可能多的标签时占有优势。</span><span class="sxs-lookup"><span data-stu-id="d63e9-241">Especially in the scenario where you configure a custom vertical that allows search over more than one connection, the search outcomes greatly benefit from appointing as many labels as possible.</span></span>

### <a name="default-result-types"></a><span data-ttu-id="d63e9-242">默认结果类型</span><span class="sxs-lookup"><span data-stu-id="d63e9-242">Default result types</span></span>

<span data-ttu-id="d63e9-243">标签还会影响生成默认结果类型的方式。</span><span class="sxs-lookup"><span data-stu-id="d63e9-243">Labels also affect how default result types are generated.</span></span> <span data-ttu-id="d63e9-244">尽可能少添加标题和内容标签可确保为连接创建结果类型。</span><span class="sxs-lookup"><span data-stu-id="d63e9-244">Adding the title and content labels at a minimum will ensure that a result type is created for your connection.</span></span>

![带有标题和结果片段的默认结果类型](./images/search-index-manage-schema-6.svg)

<span data-ttu-id="d63e9-246">*带有标题和`title`结果片段的默认结果类型*</span><span class="sxs-lookup"><span data-stu-id="d63e9-246">*A default result type with `title` and a result snippet*</span></span>

<span data-ttu-id="d63e9-247">当你定义这些标签时，你的默认结果类型将提供更好的体验（适用时按升序排列）：</span><span class="sxs-lookup"><span data-stu-id="d63e9-247">Your default result type will provide a better experience when you define these labels, when applicable, listed by ascending order:</span></span>

- <span data-ttu-id="d63e9-248">title</span><span class="sxs-lookup"><span data-stu-id="d63e9-248">title</span></span>
- <span data-ttu-id="d63e9-249">url</span><span class="sxs-lookup"><span data-stu-id="d63e9-249">url</span></span>
- <span data-ttu-id="d63e9-250">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="d63e9-250">lastModifiedBy</span></span>
- <span data-ttu-id="d63e9-251">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d63e9-251">lastModifiedDateTime</span></span>
- <span data-ttu-id="d63e9-252">fileName</span><span class="sxs-lookup"><span data-stu-id="d63e9-252">fileName</span></span>
- <span data-ttu-id="d63e9-253">FileExtension</span><span class="sxs-lookup"><span data-stu-id="d63e9-253">fileExtension</span></span>

<span data-ttu-id="d63e9-254">最后，在分配标签时，请确保以下内容：</span><span class="sxs-lookup"><span data-stu-id="d63e9-254">Finally, when assigning labels, ensure the following:</span></span>

- <span data-ttu-id="d63e9-255">需要将选择用作标签的属性标记为可检索。</span><span class="sxs-lookup"><span data-stu-id="d63e9-255">The properties that you select to function as labels need to be marked retrievable.</span></span>
- <span data-ttu-id="d63e9-256">属性及其分配的标签必须具有相同的数据类型。</span><span class="sxs-lookup"><span data-stu-id="d63e9-256">The properties and their assigned labels must have the same datatype.</span></span>
- <span data-ttu-id="d63e9-257">只能将一个标签正好映射到一个属性。</span><span class="sxs-lookup"><span data-stu-id="d63e9-257">You can map exactly one label to exactly one property.</span></span>

## <a name="aliases"></a><span data-ttu-id="d63e9-258">别名</span><span class="sxs-lookup"><span data-stu-id="d63e9-258">Aliases</span></span>

<span data-ttu-id="d63e9-259">别名是你所分配属性的好记的名称。</span><span class="sxs-lookup"><span data-stu-id="d63e9-259">Aliases are friendly names for properties that you assign.</span></span> <span data-ttu-id="d63e9-260">它们将用于可精简属性筛选器中的查询和选择。</span><span class="sxs-lookup"><span data-stu-id="d63e9-260">These will be used in queries and selections in refinable property filters.</span></span>

## <a name="next-steps"></a><span data-ttu-id="d63e9-261">后续步骤</span><span class="sxs-lookup"><span data-stu-id="d63e9-261">Next steps</span></span>

- [<span data-ttu-id="d63e9-262">向连接添加项目</span><span class="sxs-lookup"><span data-stu-id="d63e9-262">Add items to the connection</span></span>](/graph/concepts/search-index-manage-items.md)
- [<span data-ttu-id="d63e9-263">查看 Microsoft Graph 连接器 API 参考</span><span class="sxs-lookup"><span data-stu-id="d63e9-263">Review the Microsoft Graph connectors API reference</span></span>](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true)
- [<span data-ttu-id="d63e9-264">自定义 Microsoft 搜索结果页</span><span class="sxs-lookup"><span data-stu-id="d63e9-264">Customize Microsoft Search results page</span></span>](/MicrosoftSearch/configure-connector#next-steps-customize-the-search-results-page)
- [<span data-ttu-id="d63e9-265">搜索自定义类型 (externalItem)</span><span class="sxs-lookup"><span data-stu-id="d63e9-265">Search custom types (externalItem)</span></span>](search-concept-custom-types.md)
- <span data-ttu-id="d63e9-266">从 GitHub 下载[示例搜索连接器](https://github.com/microsoftgraph/msgraph-search-connector-sample)</span><span class="sxs-lookup"><span data-stu-id="d63e9-266">Download the [sample search connector](https://github.com/microsoftgraph/msgraph-search-connector-sample) from GitHub</span></span>
