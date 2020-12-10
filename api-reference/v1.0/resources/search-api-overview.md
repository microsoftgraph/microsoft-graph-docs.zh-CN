---
title: 使用 Microsoft 搜索 API 查询数据
description: 使用搜索 API，应用程序可以在已认证用户的上下文中搜索 Microsoft 365 数据
localization_priority: Priority
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: b616119d1b5c1dcc8bb56b65711468cceafd7d88
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523005"
---
# <a name="use-the-microsoft-search-api-to-query-data"></a><span data-ttu-id="a1330-103">使用 Microsoft 搜索 API 查询数据</span><span class="sxs-lookup"><span data-stu-id="a1330-103">Use the Microsoft Search API to query data</span></span>

<span data-ttu-id="a1330-104">可使用 Microsoft 搜索 API 来查询应用程序中的 Microsoft 365 数据。</span><span class="sxs-lookup"><span data-stu-id="a1330-104">You can use the Microsoft Search API to query Microsoft 365 data in your apps.</span></span>

<span data-ttu-id="a1330-105">搜索请求在登录用户的上下文中运行，并使用[包含委派权限的访问令牌](/graph/auth-v2-user)进行标识。</span><span class="sxs-lookup"><span data-stu-id="a1330-105">Search requests run in the context of the signed-in user, identified using an [access token with delegated permissions](/graph/auth-v2-user).</span></span>

## <a name="common-use-cases"></a><span data-ttu-id="a1330-106">常见用例</span><span class="sxs-lookup"><span data-stu-id="a1330-106">Common use cases</span></span>

<span data-ttu-id="a1330-107">Microsoft Search API 提供了[查询](../api/search-query.md)方法，可在 Microsoft Search 中搜索数据，在其请求正文中传递 [searchRequest](searchRequest.md) ，定义搜索的具体内容。</span><span class="sxs-lookup"><span data-stu-id="a1330-107">The Microsoft Search API provides a [query](../api/search-query.md) method to search across your data in Microsoft Search, where you pass a [searchRequest](searchRequest.md) in the request body, defining the specifics of your search.</span></span>

<span data-ttu-id="a1330-108">本部分列出了 **查询** 方法的常见用例，具体取决于在 **查询** [searchRequest](searchRequest.md)正文中设置的属性和参数。</span><span class="sxs-lookup"><span data-stu-id="a1330-108">This section lists the common use cases of the **query** method, based on the properties and parameters you set in the **query** [searchRequest](searchRequest.md) body.</span></span>

<span data-ttu-id="a1330-109">代表用户运行搜索请求。</span><span class="sxs-lookup"><span data-stu-id="a1330-109">Search requests run on behalf of the user.</span></span> <span data-ttu-id="a1330-110">设定搜索结果范围，以强制执行应用到项目的任何访问控制。</span><span class="sxs-lookup"><span data-stu-id="a1330-110">Search results are scoped to enforce any access control applied to the items.</span></span>  <span data-ttu-id="a1330-111">例如，在文件的上下文中，将在搜索请求过程中评估对文件的权限。</span><span class="sxs-lookup"><span data-stu-id="a1330-111">For example, in the context of files, permissions on the files are evaluated as part of the search request.</span></span> <span data-ttu-id="a1330-112">在搜索中，用户无法访问更多的项目，但可以从具有相同权限和访问控制的相应 GET 操作中获得这些项目。</span><span class="sxs-lookup"><span data-stu-id="a1330-112">Users cannot access more items in a search than they can otherwise obtain from a corresponding GET operation with the same permissions and access control.</span></span>

| <span data-ttu-id="a1330-113">用例</span><span class="sxs-lookup"><span data-stu-id="a1330-113">Use cases</span></span> | <span data-ttu-id="a1330-114">要在查询请求正文中定义的属性</span><span class="sxs-lookup"><span data-stu-id="a1330-114">Properties to define in the query request body</span></span> |
|:------------------|:---------|
|[<span data-ttu-id="a1330-115">根据实体类型限定搜索范围</span><span class="sxs-lookup"><span data-stu-id="a1330-115">Scope search results based on entity types</span></span>](#scope-search-based-on-entity-types)| <span data-ttu-id="a1330-116">**entityTypes**</span><span class="sxs-lookup"><span data-stu-id="a1330-116">**entityTypes**</span></span> |
|[<span data-ttu-id="a1330-117">页面结果</span><span class="sxs-lookup"><span data-stu-id="a1330-117">Page results</span></span>](#page-search-results) | <span data-ttu-id="a1330-118">**起始数量** 和 **大小**</span><span class="sxs-lookup"><span data-stu-id="a1330-118">**from** and **size**</span></span> |
|[<span data-ttu-id="a1330-119">获取最相关的电子邮件</span><span class="sxs-lookup"><span data-stu-id="a1330-119">Get the most relevant emails</span></span>](#get-the-most-relevant-emails) | <span data-ttu-id="a1330-120">**enableTopResults**</span><span class="sxs-lookup"><span data-stu-id="a1330-120">**enableTopResults**</span></span> |
|[<span data-ttu-id="a1330-121">获取选定属性</span><span class="sxs-lookup"><span data-stu-id="a1330-121">Get selected properties</span></span>](#get-selected-properties) | <span data-ttu-id="a1330-122">**fields**</span><span class="sxs-lookup"><span data-stu-id="a1330-122">**fields**</span></span> |
|[<span data-ttu-id="a1330-123">在查询条款中使用 KQL</span><span class="sxs-lookup"><span data-stu-id="a1330-123">Use KQL in query terms</span></span>](#keyword-query-language-kql-support) | <span data-ttu-id="a1330-124">**查询**</span><span class="sxs-lookup"><span data-stu-id="a1330-124">**query**</span></span> |

## <a name="scope-search-based-on-entity-types"></a><span data-ttu-id="a1330-125">根据实体类型限定搜索范围</span><span class="sxs-lookup"><span data-stu-id="a1330-125">Scope search based on entity types</span></span>

<span data-ttu-id="a1330-126">使用 **查询** 请求有效负载中的 **entityTypes** 属性定义搜索请求的范围。</span><span class="sxs-lookup"><span data-stu-id="a1330-126">Define the scope of the search request using the **entityTypes** property in the **query** request payload.</span></span>
<span data-ttu-id="a1330-127">下表介绍了可用于查询的类型以及访问数据所支持的权限。</span><span class="sxs-lookup"><span data-stu-id="a1330-127">The following table describes the types available to query and the supported permissions to access the data.</span></span>

| <span data-ttu-id="a1330-128">EntityType</span><span class="sxs-lookup"><span data-stu-id="a1330-128">EntityType</span></span> | <span data-ttu-id="a1330-129">访问项目所需的权限范围</span><span class="sxs-lookup"><span data-stu-id="a1330-129">Permission scope required to access the items</span></span>| <span data-ttu-id="a1330-130">Source</span><span class="sxs-lookup"><span data-stu-id="a1330-130">Source</span></span>| <span data-ttu-id="a1330-131">评论</span><span class="sxs-lookup"><span data-stu-id="a1330-131">Comment</span></span>|
|:------------------|:---------|:---------|:---------|
|[<span data-ttu-id="a1330-132">message</span><span class="sxs-lookup"><span data-stu-id="a1330-132">message</span></span>](message.md)|<span data-ttu-id="a1330-133">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a1330-133">Mail.Read, Mail.ReadWrite</span></span>| <span data-ttu-id="a1330-134">Exchange Online</span><span class="sxs-lookup"><span data-stu-id="a1330-134">Exchange Online</span></span>| <span data-ttu-id="a1330-135">电子邮件。</span><span class="sxs-lookup"><span data-stu-id="a1330-135">Email messages.</span></span>|
|[<span data-ttu-id="a1330-136">event</span><span class="sxs-lookup"><span data-stu-id="a1330-136">event</span></span>](event.md) |<span data-ttu-id="a1330-137">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a1330-137">Calendars.Read, Calendars.ReadWrite</span></span>| <span data-ttu-id="a1330-138">Exchange Online</span><span class="sxs-lookup"><span data-stu-id="a1330-138">Exchange Online</span></span>|<span data-ttu-id="a1330-139">日历事件。</span><span class="sxs-lookup"><span data-stu-id="a1330-139">Calendar events.</span></span> |
|[<span data-ttu-id="a1330-140">drive</span><span class="sxs-lookup"><span data-stu-id="a1330-140">drive</span></span>](drive.md)|<span data-ttu-id="a1330-141">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1330-141">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>| <span data-ttu-id="a1330-142">SharePoint</span><span class="sxs-lookup"><span data-stu-id="a1330-142">SharePoint</span></span> | <span data-ttu-id="a1330-143">文档库。</span><span class="sxs-lookup"><span data-stu-id="a1330-143">Document libraries.</span></span>|
|[<span data-ttu-id="a1330-144">driveItem</span><span class="sxs-lookup"><span data-stu-id="a1330-144">driveItem</span></span>](driveitem.md)|<span data-ttu-id="a1330-145">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1330-145">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>| <span data-ttu-id="a1330-146">SharePoint 和 OneDrive</span><span class="sxs-lookup"><span data-stu-id="a1330-146">SharePoint and OneDrive</span></span> | <span data-ttu-id="a1330-147">文件、文件夹、页面和新闻。</span><span class="sxs-lookup"><span data-stu-id="a1330-147">Files, folders, pages, and news.</span></span> |
|[<span data-ttu-id="a1330-148">列表</span><span class="sxs-lookup"><span data-stu-id="a1330-148">list</span></span>](list.md)|<span data-ttu-id="a1330-149">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1330-149">Sites.Read.All, Sites.ReadWrite.All</span></span>| <span data-ttu-id="a1330-150">SharePoint 和 OneDrive</span><span class="sxs-lookup"><span data-stu-id="a1330-150">SharePoint and OneDrive</span></span> | <span data-ttu-id="a1330-151">列表。</span><span class="sxs-lookup"><span data-stu-id="a1330-151">Lists.</span></span> <span data-ttu-id="a1330-152">请注意，文档库也作为列表返回。</span><span class="sxs-lookup"><span data-stu-id="a1330-152">Note that document libraries are also returned as lists.</span></span> |
|[<span data-ttu-id="a1330-153">listItem</span><span class="sxs-lookup"><span data-stu-id="a1330-153">listItem</span></span>](listitem.md)|<span data-ttu-id="a1330-154">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1330-154">Sites.Read.All, Sites.ReadWrite.All</span></span>| <span data-ttu-id="a1330-155">SharePoint 和 OneDrive</span><span class="sxs-lookup"><span data-stu-id="a1330-155">SharePoint and OneDrive</span></span> | <span data-ttu-id="a1330-156">列表项。</span><span class="sxs-lookup"><span data-stu-id="a1330-156">List items.</span></span> <span data-ttu-id="a1330-157">请注意，文件和文件夹也作为列表项返回；**driveItem** 是 **driveItem** 的超类。</span><span class="sxs-lookup"><span data-stu-id="a1330-157">Note that files and folders are also returned as list items; **listItem** is the super class of **driveItem**.</span></span> |
|[<span data-ttu-id="a1330-158">网站</span><span class="sxs-lookup"><span data-stu-id="a1330-158">site</span></span>](site.md)|<span data-ttu-id="a1330-159">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1330-159">Sites.Read.All, Sites.ReadWrite.All</span></span>| <span data-ttu-id="a1330-160">SharePoint</span><span class="sxs-lookup"><span data-stu-id="a1330-160">SharePoint</span></span> | <span data-ttu-id="a1330-161">SharePoint 中的网站。</span><span class="sxs-lookup"><span data-stu-id="a1330-161">Sites in SharePoint.</span></span>|

## <a name="page-search-results"></a><span data-ttu-id="a1330-162">页面搜索结果</span><span class="sxs-lookup"><span data-stu-id="a1330-162">Page search results</span></span>

<span data-ttu-id="a1330-163">通过在 **查询** 请求正文中指定以下两个属性来控制搜索结果的分页：</span><span class="sxs-lookup"><span data-stu-id="a1330-163">Control pagination of the search results by specifying the following two properties in the **query** request body:</span></span>

- <span data-ttu-id="a1330-164">**起始数量** - 一个整数，它表示从 0 开始的起始数，在页面上列出搜索结果。</span><span class="sxs-lookup"><span data-stu-id="a1330-164">**from** - An integer that indicates the 0-based starting point to list search results on the page.</span></span> <span data-ttu-id="a1330-165">默认值为 0。</span><span class="sxs-lookup"><span data-stu-id="a1330-165">The default value is 0.</span></span>

- <span data-ttu-id="a1330-166">**大小** - 一个整数，它表示要为页面返回的结果数。</span><span class="sxs-lookup"><span data-stu-id="a1330-166">**size** - An integer that indicates the number of results to be returned for a page.</span></span> <span data-ttu-id="a1330-167">默认值为 25。</span><span class="sxs-lookup"><span data-stu-id="a1330-167">The default value is 25.</span></span>

<span data-ttu-id="a1330-168">如果你正在搜索 **event** 或 **message** 实体，则注意以下限制：</span><span class="sxs-lookup"><span data-stu-id="a1330-168">Note the following limits if you're searching the **event** or **message** entity:</span></span>

- <span data-ttu-id="a1330-169">**起始数量** 在第一个页面请求中必须从零开始，否则请求将导致出现 HTTP 400 `Bad request`。</span><span class="sxs-lookup"><span data-stu-id="a1330-169">**from** must start at zero in the first page request; otherwise, the request results in an HTTP 400 `Bad request`.</span></span>
- <span data-ttu-id="a1330-170">每页的 **message** 和 **event** 最大结果数（**大小**）为 25。</span><span class="sxs-lookup"><span data-stu-id="a1330-170">The maximum results per page (**size**) is 25 for **message** and **event**.</span></span> 

<span data-ttu-id="a1330-171">SharePoint 或 OneDrive 项没有上限。</span><span class="sxs-lookup"><span data-stu-id="a1330-171">There is no upper limit for SharePoint or OneDrive items.</span></span> <span data-ttu-id="a1330-172">合理的页面大小是 200。</span><span class="sxs-lookup"><span data-stu-id="a1330-172">A reasonable page size is 200.</span></span> <span data-ttu-id="a1330-173">较大的页面大小通常会导致更高的延迟。</span><span class="sxs-lookup"><span data-stu-id="a1330-173">A larger page size generally incurs higher latency.</span></span>

<span data-ttu-id="a1330-174">最佳实践：</span><span class="sxs-lookup"><span data-stu-id="a1330-174">Best practices:</span></span>

- <span data-ttu-id="a1330-175">指定初始请求中的较小的首页。</span><span class="sxs-lookup"><span data-stu-id="a1330-175">Specify a smaller first page in the initial request.</span></span> <span data-ttu-id="a1330-176">例如，将 **起始数量** 指定为 0，将 **大小** 指定为 25。</span><span class="sxs-lookup"><span data-stu-id="a1330-176">For example, specify **from** as 0, **size** as 25.</span></span>
- <span data-ttu-id="a1330-177">通过更新 **起始数量** 和 **大小** 属性来对后续页面进行分页。</span><span class="sxs-lookup"><span data-stu-id="a1330-177">Paginate subsequent pages by updating the **from** and **size** properties.</span></span> <span data-ttu-id="a1330-178">可以在每个后续请求中增加页面大小。</span><span class="sxs-lookup"><span data-stu-id="a1330-178">You can increase the page size in each subsequent request.</span></span> <span data-ttu-id="a1330-179">下表显示了一个示例。</span><span class="sxs-lookup"><span data-stu-id="a1330-179">The following table shows an example.</span></span>

    | <span data-ttu-id="a1330-180">页面</span><span class="sxs-lookup"><span data-stu-id="a1330-180">Page</span></span> | <span data-ttu-id="a1330-181">起始数量</span><span class="sxs-lookup"><span data-stu-id="a1330-181">from</span></span> | <span data-ttu-id="a1330-182">大小</span><span class="sxs-lookup"><span data-stu-id="a1330-182">size</span></span> |
    |:-----|:-----|:-----|
    | <span data-ttu-id="a1330-183">1</span><span class="sxs-lookup"><span data-stu-id="a1330-183">1</span></span>    | <span data-ttu-id="a1330-184">0</span><span class="sxs-lookup"><span data-stu-id="a1330-184">0</span></span> | <span data-ttu-id="a1330-185">25</span><span class="sxs-lookup"><span data-stu-id="a1330-185">25</span></span> |
    | <span data-ttu-id="a1330-186">2</span><span class="sxs-lookup"><span data-stu-id="a1330-186">2</span></span>    | <span data-ttu-id="a1330-187">25</span><span class="sxs-lookup"><span data-stu-id="a1330-187">25</span></span> | <span data-ttu-id="a1330-188">50</span><span class="sxs-lookup"><span data-stu-id="a1330-188">50</span></span> |
    | <span data-ttu-id="a1330-189">3</span><span class="sxs-lookup"><span data-stu-id="a1330-189">3</span></span>    | <span data-ttu-id="a1330-190">75</span><span class="sxs-lookup"><span data-stu-id="a1330-190">75</span></span> | <span data-ttu-id="a1330-191">75</span><span class="sxs-lookup"><span data-stu-id="a1330-191">75</span></span> |
    | <span data-ttu-id="a1330-192">4</span><span class="sxs-lookup"><span data-stu-id="a1330-192">4</span></span>    | <span data-ttu-id="a1330-193">150</span><span class="sxs-lookup"><span data-stu-id="a1330-193">150</span></span> | <span data-ttu-id="a1330-194">100</span><span class="sxs-lookup"><span data-stu-id="a1330-194">100</span></span> |

## <a name="get-the-most-relevant-emails"></a><span data-ttu-id="a1330-195">获取最相关的电子邮件</span><span class="sxs-lookup"><span data-stu-id="a1330-195">Get the most relevant emails</span></span>

<span data-ttu-id="a1330-196">搜索 **message** 实体时，将 **enableTopResults** 指定为 `true` 返回邮件的混合列表：响应中的前 3 封邮件按相关性排序，剩余邮件按日期/时间排序。</span><span class="sxs-lookup"><span data-stu-id="a1330-196">When searching the **message** entity, specifying **enableTopResults** as `true` returns a hybrid list of messages: the first three messages in the response are sorted by relevance; the remaining messages are sorted by date/time.</span></span>

## <a name="get-selected-properties"></a><span data-ttu-id="a1330-197">获取选定属性</span><span class="sxs-lookup"><span data-stu-id="a1330-197">Get selected properties</span></span>

<span data-ttu-id="a1330-198">搜索实体类型，如 **message**、**event**、**drive**、**driveItem**、**list**、**listItem**、**site**、**externalItem**，可以在 **fields** 属性中包含特定的实体属性，以便在搜索结果中返回。</span><span class="sxs-lookup"><span data-stu-id="a1330-198">When searching an entity type, such as **message**, **event**, **drive**, **driveItem**, **list**, **listItem**, **site**, **externalItem**, you can include in the **fields** property specific entity properties to return in the search results.</span></span> <span data-ttu-id="a1330-199">这类似于使用 [OData 系统查询选项，REST 请求中的 $select](/graph/query-parameters#select-parameter)。</span><span class="sxs-lookup"><span data-stu-id="a1330-199">This is similar to using the [OData system query option, $select](/graph/query-parameters#select-parameter) in REST requests.</span></span> <span data-ttu-id="a1330-200">搜索 API 技术上不支持这些查询选项，因为会在文章正文中表达该行为。</span><span class="sxs-lookup"><span data-stu-id="a1330-200">The search API does not technically support these query options because the behavior is expressed in the POST body.</span></span>

<span data-ttu-id="a1330-201">对于所有这些实体类型，指定 **fields** 属性可减少响应中返回的属性数，从而通过网络优化负载。</span><span class="sxs-lookup"><span data-stu-id="a1330-201">For all these entity types, specifying the **fields** property reduces the number of properties returned in the response, optimizing the payload over the wire.</span></span>

<span data-ttu-id="a1330-202">**listItem** 和 **externalItem** 实体是唯一支持的实体，可用于获取架构中配置的扩展字段。</span><span class="sxs-lookup"><span data-stu-id="a1330-202">The **listItem** and **externalItem** entities are the only supported entities that allow getting extended fields configured in the schema.</span></span> <span data-ttu-id="a1330-203">无法从所有其他实体检索扩展属性。</span><span class="sxs-lookup"><span data-stu-id="a1330-203">You cannot retrieve extended properties from all the other entities.</span></span> <span data-ttu-id="a1330-204">例如，如果在搜索架构中创建了 **externalItem** 的字段，或者 **listItem** 上有自定义列，则可以从搜索中检索这些属性。</span><span class="sxs-lookup"><span data-stu-id="a1330-204">For example, if you created a field for **externalItem** in the search schema, or if you have a custom column on a **listItem**, you can retrieve these properties from search.</span></span> <span data-ttu-id="a1330-205">若要检索文件的扩展属性，请在请求中指定 **listItem** 类型。</span><span class="sxs-lookup"><span data-stu-id="a1330-205">To retrieve an extended property on a file, specify the **listItem** type in the request.</span></span>

<span data-ttu-id="a1330-206">如果请求中指定的 **fields** 在架构中不存在，则在响应中将不会返回这些字段。</span><span class="sxs-lookup"><span data-stu-id="a1330-206">If the **fields** specified in the request are not present in the schema, they will not be returned in the response.</span></span> <span data-ttu-id="a1330-207">请求中的无效字段将忽略静默。</span><span class="sxs-lookup"><span data-stu-id="a1330-207">Invalid fields in the request are silently ignored.</span></span>

<span data-ttu-id="a1330-208">如果你在请求中未指定任何 **字段**，则将获得所有类型的默认属性集。</span><span class="sxs-lookup"><span data-stu-id="a1330-208">If you do not specify any **fields** in the request,  you will get the default set of properties for all types.</span></span> <span data-ttu-id="a1330-209">对于扩展属性，在请求中未传递任何 **字段** 时，**listItem** 和 **externalItem** 的行为不同：</span><span class="sxs-lookup"><span data-stu-id="a1330-209">For extended properties, **listItem** and **externalItem** behave differently when no **fields** are passed in the request:</span></span>

- <span data-ttu-id="a1330-210">**listItem** 不会返回任何自定义字段。</span><span class="sxs-lookup"><span data-stu-id="a1330-210">**listItem** will not return any custom field.</span></span>
- <span data-ttu-id="a1330-211">**externalItem** 将返回该特定连接的 Microsoft Graph 连接器架构中标记有 **retrievable** 属性的所有字段。</span><span class="sxs-lookup"><span data-stu-id="a1330-211">**externalItem** will return all the fields marked with the **retrievable** attribute in the Microsoft Graph connector schema for that particular connection.</span></span>

## <a name="keyword-query-language-kql-support"></a><span data-ttu-id="a1330-212">关键字查询语言 (KQL) 支持</span><span class="sxs-lookup"><span data-stu-id="a1330-212">Keyword Query Language (KQL) support</span></span>

<span data-ttu-id="a1330-213">在实际搜索查询字符串（**查询** 请求正文的 **查询** 属性）中的 KQL 语法中，指定自由文本关键字、运算符（例如 `AND`、`OR`）和属性限制。</span><span class="sxs-lookup"><span data-stu-id="a1330-213">Specify free text keywords, operators (such as `AND`, `OR`), and property restrictions in KQL syntax in the actual search query string (**query** property of the **query** request body).</span></span> <span data-ttu-id="a1330-214">语法和命令取决于在同一 **查询** 请求主体中指向的实体类型（在 **entityTypes** 属性中）。</span><span class="sxs-lookup"><span data-stu-id="a1330-214">The syntax and command depend on the entity types (in the **entityTypes** property) you target in the same **query** request body.</span></span>

<span data-ttu-id="a1330-215">可搜索的属性各不相同，具体取决于实体类型。</span><span class="sxs-lookup"><span data-stu-id="a1330-215">Depending on the entity type, the searchable properties vary.</span></span> <span data-ttu-id="a1330-216">有关详细信息，请参阅：</span><span class="sxs-lookup"><span data-stu-id="a1330-216">For details, see:</span></span>

- [<span data-ttu-id="a1330-217">电子邮件属性</span><span class="sxs-lookup"><span data-stu-id="a1330-217">Email properties</span></span>](/microsoft-365/compliance/keyword-queries-and-search-conditions#searchable-email-properties)
- [<span data-ttu-id="a1330-218">站点属性</span><span class="sxs-lookup"><span data-stu-id="a1330-218">Site properties</span></span>](/microsoft-365/compliance/keyword-queries-and-search-conditions#searchable-site-properties)

## <a name="error-handling"></a><span data-ttu-id="a1330-219">错误处理</span><span class="sxs-lookup"><span data-stu-id="a1330-219">Error handling</span></span>

<span data-ttu-id="a1330-220">搜索 API 将返回由 [OData 错误对象定义](http://docs.oasis-open.org/odata/odata-json-format/v4.01/cs01/odata-json-format-v4.01-cs01.html#sec_ErrorResponse)所定义的错误响应，其中每个是包含代码和消息的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="a1330-220">The search API returns error responses as defined by [OData error object definition](http://docs.oasis-open.org/odata/odata-json-format/v4.01/cs01/odata-json-format-v4.01-cs01.html#sec_ErrorResponse), each of which is a JSON object containing a code and a message.</span></span>

<!---TODOSEARCHAPI Describe the know errors: bad requests.--->

## <a name="known-limitations"></a><span data-ttu-id="a1330-221">已知限制</span><span class="sxs-lookup"><span data-stu-id="a1330-221">Known limitations</span></span>

<span data-ttu-id="a1330-222">搜索 API 存在以下限制：</span><span class="sxs-lookup"><span data-stu-id="a1330-222">The search API has the following limitations:</span></span>

- <span data-ttu-id="a1330-223">定义 **查询** 方法，以允许一次传递一个或多个 **searchRequest** 实例的集合。</span><span class="sxs-lookup"><span data-stu-id="a1330-223">The **query** method is defined to allow passing a collection of one or more **searchRequest** instances at once.</span></span> <span data-ttu-id="a1330-224">但是，该服务当前仅支持一次传递一个 [searchRequest](./searchrequest.md)。</span><span class="sxs-lookup"><span data-stu-id="a1330-224">However, the service currently supports only a single [searchRequest](./searchrequest.md) at a time.</span></span>

- <span data-ttu-id="a1330-225">[searchRequest](./searchrequest.md) 资源支持一次传递多个类型的实体。</span><span class="sxs-lookup"><span data-stu-id="a1330-225">The [searchRequest](./searchrequest.md) resource supports passing multiple types of entities at a time.</span></span> <span data-ttu-id="a1330-226">但是，目前仅支持 SharePoint 和 OneDrive entityTypes 的组合为：**driveItem**、**drive**、**site**、**list**、**listItem**。</span><span class="sxs-lookup"><span data-stu-id="a1330-226">However, currently the only supported combination is for SharePoint and OneDrive entityTypes: **driveItem**, **drive**, **site**, **list**, **listItem**.</span></span>
<span data-ttu-id="a1330-227">当前不支持任何涉及 **message**、**event**、Sharepoint 和 OneDrive 类型或 **externalItem** 的组合。</span><span class="sxs-lookup"><span data-stu-id="a1330-227">Any combinations involving **message**, **event**, SharePoint and OneDrive types , or **externalItem** are currently not supported.</span></span>  

- <span data-ttu-id="a1330-228">仅当将 **entityType** 指定为 `externalItem` 时，定义要使用的连接的 **contentSource** 属性才适用。</span><span class="sxs-lookup"><span data-stu-id="a1330-228">The **contentSource** property, which defines the connection to use, is only applicable when **entityType** is specified as `externalItem`.</span></span>

- <span data-ttu-id="a1330-229">搜索 API 不支持 **message**、**event** 或 **externalItem** 的自定义排序。</span><span class="sxs-lookup"><span data-stu-id="a1330-229">The search API does not support custom sort for **message**, **event** or  **externalItem**.</span></span>

- <span data-ttu-id="a1330-230">搜索 API 不支持 **message**、**event**、**site** 或 **drive** 的聚合。</span><span class="sxs-lookup"><span data-stu-id="a1330-230">The search API does not support aggregations for **message**, **event**, **site** or **drive**.</span></span>

## <a name="search-samples"></a><span data-ttu-id="a1330-231">搜索示例</span><span class="sxs-lookup"><span data-stu-id="a1330-231">Search samples</span></span>

- <span data-ttu-id="a1330-232">了解有关几个关键用例的详细信息：</span><span class="sxs-lookup"><span data-stu-id="a1330-232">Learn more about a few key use cases:</span></span>
  - [<span data-ttu-id="a1330-233">搜索 Outlook 邮件</span><span class="sxs-lookup"><span data-stu-id="a1330-233">Search Outlook messages</span></span>](/graph/search-concept-messages)
  - [<span data-ttu-id="a1330-234">搜索日历事件</span><span class="sxs-lookup"><span data-stu-id="a1330-234">Search calendar events</span></span>](/graph/search-concept-events)
  - [<span data-ttu-id="a1330-235">SharePoint 和 OneDrive 中的搜索内容</span><span class="sxs-lookup"><span data-stu-id="a1330-235">Search content in SharePoint and OneDrive</span></span>](/graph/search-concept-files)

- <span data-ttu-id="a1330-236">在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中探索搜索 API。</span><span class="sxs-lookup"><span data-stu-id="a1330-236">Explore the search APIs in  [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>


## <a name="whats-new"></a><span data-ttu-id="a1330-237">最近更新</span><span class="sxs-lookup"><span data-stu-id="a1330-237">What's new</span></span>

<span data-ttu-id="a1330-238">了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。</span><span class="sxs-lookup"><span data-stu-id="a1330-238">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>
