---
title: 使用 Microsoft 搜索 API 查询数据
description: 使用搜索 API，应用程序可以在已认证用户的上下文中搜索 Microsoft 365 数据
localization_priority: Priority
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: e77c0170487b0762538d98376921565857c9b3c8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985783"
---
# <a name="use-the-microsoft-search-api-to-query-data"></a><span data-ttu-id="af70b-103">使用 Microsoft 搜索 API 查询数据</span><span class="sxs-lookup"><span data-stu-id="af70b-103">Use the Microsoft Search API to query data</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af70b-104">可使用 Microsoft 搜索 API 来查询应用程序中的 Microsoft 365 数据。</span><span class="sxs-lookup"><span data-stu-id="af70b-104">You can use the Microsoft Search API to query Microsoft 365 data in your apps.</span></span>

<span data-ttu-id="af70b-105">搜索请求在登录用户的上下文中运行，并使用[包含委派权限的访问令牌](/graph/auth-v2-user)进行标识。</span><span class="sxs-lookup"><span data-stu-id="af70b-105">Search requests run in the context of the signed-in user, identified using an [access token with delegated permissions](/graph/auth-v2-user).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="common-use-cases"></a><span data-ttu-id="af70b-106">常见用例</span><span class="sxs-lookup"><span data-stu-id="af70b-106">Common use cases</span></span>

<span data-ttu-id="af70b-107">Microsoft 搜索 API 提供了[查询](../api/search-query.md)方法，可在 Microsoft 搜索中跨数据搜索。</span><span class="sxs-lookup"><span data-stu-id="af70b-107">The Microsoft Search API provides a [query](../api/search-query.md) method to search across your data in Microsoft Search.</span></span> <span data-ttu-id="af70b-108">本部分列出了常见用例，具体取决于在**查询**请求正文中设置的属性。</span><span class="sxs-lookup"><span data-stu-id="af70b-108">This section lists the common use cases, based on the properties you set in the **query** request body.</span></span>

<span data-ttu-id="af70b-109">代表用户运行搜索请求。</span><span class="sxs-lookup"><span data-stu-id="af70b-109">Search requests run on behalf of the user.</span></span> <span data-ttu-id="af70b-110">设定搜索结果范围，以强制执行应用到项目的任何访问控制。</span><span class="sxs-lookup"><span data-stu-id="af70b-110">Search results are scoped to enforce any access control applied to the items.</span></span>  <span data-ttu-id="af70b-111">例如，在文件的上下文中，将在搜索请求过程中评估对文件的权限。</span><span class="sxs-lookup"><span data-stu-id="af70b-111">For example, in the context of files, permissions on the files are evaluated as part of the search request.</span></span> <span data-ttu-id="af70b-112">用户在搜索中可访问的项目数不得多于其可通过枚举 API 调用的项目数。</span><span class="sxs-lookup"><span data-stu-id="af70b-112">Users cannot access more items in a search than they can from the enumeration API.</span></span>

| <span data-ttu-id="af70b-113">用例</span><span class="sxs-lookup"><span data-stu-id="af70b-113">Use cases</span></span> | <span data-ttu-id="af70b-114">要在查询请求正文中定义的属性</span><span class="sxs-lookup"><span data-stu-id="af70b-114">Properties to define in the query request body</span></span> |
|:------------------|:---------|
|[<span data-ttu-id="af70b-115">根据实体类型限定搜索范围</span><span class="sxs-lookup"><span data-stu-id="af70b-115">Scope search based on entity types</span></span>](#scope-search-based-on-entity-types)| <span data-ttu-id="af70b-116">**entityTypes**</span><span class="sxs-lookup"><span data-stu-id="af70b-116">**entityTypes**</span></span> |
|[<span data-ttu-id="af70b-117">页面结果</span><span class="sxs-lookup"><span data-stu-id="af70b-117">Page results</span></span>](#page-search-results) | <span data-ttu-id="af70b-118">**起始数量**和**大小**</span><span class="sxs-lookup"><span data-stu-id="af70b-118">**from** and **size**</span></span> |
|[<span data-ttu-id="af70b-119">获取最相关的电子邮件</span><span class="sxs-lookup"><span data-stu-id="af70b-119">Get the most relevant emails</span></span>](#get-the-most-relevant-emails) | <span data-ttu-id="af70b-120">**enableTopResults**</span><span class="sxs-lookup"><span data-stu-id="af70b-120">**enableTopResults**</span></span> |
|[<span data-ttu-id="af70b-121">获取选定属性</span><span class="sxs-lookup"><span data-stu-id="af70b-121">Get selected properties</span></span>](#get-selected-properties) | <span data-ttu-id="af70b-122">**stored_fields**</span><span class="sxs-lookup"><span data-stu-id="af70b-122">**stored_fields**</span></span> |
|[<span data-ttu-id="af70b-123">在查询条款中使用 KQL</span><span class="sxs-lookup"><span data-stu-id="af70b-123">Use KQL in query terms</span></span>](#keyword-query-language-kql-support) | <span data-ttu-id="af70b-124">**查询**</span><span class="sxs-lookup"><span data-stu-id="af70b-124">**query**</span></span> |
|[<span data-ttu-id="af70b-125">搜索外部文件</span><span class="sxs-lookup"><span data-stu-id="af70b-125">Search external Files</span></span>](/graph/search-concept-files)| <span data-ttu-id="af70b-126">**entityTypes**</span><span class="sxs-lookup"><span data-stu-id="af70b-126">**entityTypes**</span></span> |
|[<span data-ttu-id="af70b-127">在特定 contentSource 中搜索（索引 API）</span><span class="sxs-lookup"><span data-stu-id="af70b-127">Search within a specific contentSource (indexing API)</span></span>](/graph/search-concept-custom-types)| <span data-ttu-id="af70b-128">**contentSources**</span><span class="sxs-lookup"><span data-stu-id="af70b-128">**contentSources**</span></span> |

### <a name="scope-search-based-on-entity-types"></a><span data-ttu-id="af70b-129">根据实体类型限定搜索范围</span><span class="sxs-lookup"><span data-stu-id="af70b-129">Scope search based on entity types</span></span>

<span data-ttu-id="af70b-130">使用**查询**请求有效负载中的 **entityTypes** 属性定义搜索请求的范围。</span><span class="sxs-lookup"><span data-stu-id="af70b-130">Define the scope of the search request using the **entityTypes** property in the **query** request payload.</span></span>
<span data-ttu-id="af70b-131">下面是支持的实体类型：</span><span class="sxs-lookup"><span data-stu-id="af70b-131">The following are the supported entity types:</span></span>

- [<span data-ttu-id="af70b-132">event</span><span class="sxs-lookup"><span data-stu-id="af70b-132">event</span></span>](event.md)
- [<span data-ttu-id="af70b-133">message</span><span class="sxs-lookup"><span data-stu-id="af70b-133">message</span></span>](message.md)
- [<span data-ttu-id="af70b-134">driveItem</span><span class="sxs-lookup"><span data-stu-id="af70b-134">driveItem</span></span>](driveitem.md)
- [<span data-ttu-id="af70b-135">externalFile</span><span class="sxs-lookup"><span data-stu-id="af70b-135">externalFile</span></span>](externalfile.md)
- [<span data-ttu-id="af70b-136">externalItem</span><span class="sxs-lookup"><span data-stu-id="af70b-136">externalItem</span></span>](externalitem.md)

### <a name="page-search-results"></a><span data-ttu-id="af70b-137">页面搜索结果</span><span class="sxs-lookup"><span data-stu-id="af70b-137">Page search results</span></span>

<span data-ttu-id="af70b-138">通过在**查询**请求正文中指定以下两个属性来控制搜索结果的分页：</span><span class="sxs-lookup"><span data-stu-id="af70b-138">Control pagination of the search results by specifying the following two properties in the **query** request body:</span></span>

- <span data-ttu-id="af70b-139">**起始数量** - 一个整数，它表示从 0 开始的起始数，在页面上列出搜索结果。</span><span class="sxs-lookup"><span data-stu-id="af70b-139">**from** - An integer that indicates the 0-based starting point to list search results on the page.</span></span> <span data-ttu-id="af70b-140">默认值为 0。</span><span class="sxs-lookup"><span data-stu-id="af70b-140">The default value is 0.</span></span>

- <span data-ttu-id="af70b-141">**大小** - 一个整数，它表示要为页面返回的结果数。</span><span class="sxs-lookup"><span data-stu-id="af70b-141">**size** - An integer that indicates the number of results to be returned for a page.</span></span> <span data-ttu-id="af70b-142">默认值为 25。</span><span class="sxs-lookup"><span data-stu-id="af70b-142">The default value is 25.</span></span>

<span data-ttu-id="af70b-143">如果你正在搜索 **event** 或 **message** 实体，则注意以下限制：</span><span class="sxs-lookup"><span data-stu-id="af70b-143">Note the following limits if you're searching the **event** or **message** entity:</span></span>

- <span data-ttu-id="af70b-144">**起始数量**在第一个页面请求中必须从零开始，否则请求将导致出现 HTTP 400 `Bad request`。</span><span class="sxs-lookup"><span data-stu-id="af70b-144">**from** must start at zero in the first page request; otherwise, the request results in an HTTP 400 `Bad request`.</span></span>
- <span data-ttu-id="af70b-145">每页的最大结果数（**大小**）为 200。</span><span class="sxs-lookup"><span data-stu-id="af70b-145">The maximum results per page (**size**) is 200.</span></span>
- <span data-ttu-id="af70b-146">分页可返回的最大总项数为 1000。</span><span class="sxs-lookup"><span data-stu-id="af70b-146">The maximum total number of items that can be returned by paginating is 1000.</span></span>
- <span data-ttu-id="af70b-147">超出限制将返回最佳响应。</span><span class="sxs-lookup"><span data-stu-id="af70b-147">Going beyond the limits returns a best effort response.</span></span> <span data-ttu-id="af70b-148">请求不会导致 HTTP 400。</span><span class="sxs-lookup"><span data-stu-id="af70b-148">The request does not result in an HTTP 400.</span></span>

<span data-ttu-id="af70b-149">最佳实践：</span><span class="sxs-lookup"><span data-stu-id="af70b-149">Best practices:</span></span>

- <span data-ttu-id="af70b-150">指定初始请求中的较小的首页。</span><span class="sxs-lookup"><span data-stu-id="af70b-150">Specify a smaller first page in the initial request.</span></span> <span data-ttu-id="af70b-151">例如，将**起始数量**指定为 0，将**大小**指定为 25。</span><span class="sxs-lookup"><span data-stu-id="af70b-151">For example, specify **from** as 0, **size** as 25.</span></span>
- <span data-ttu-id="af70b-152">通过更新**起始数量**和**大小**属性来对后续页面进行分页。</span><span class="sxs-lookup"><span data-stu-id="af70b-152">Paginate subsequent pages by updating the **from** and **size** properties.</span></span> <span data-ttu-id="af70b-153">可以在每个后续请求中增加页面大小。</span><span class="sxs-lookup"><span data-stu-id="af70b-153">You can increase the page size in each subsequent request.</span></span> <span data-ttu-id="af70b-154">下表显示了一个示例。</span><span class="sxs-lookup"><span data-stu-id="af70b-154">The following table shows an example.</span></span>

    | <span data-ttu-id="af70b-155">页面</span><span class="sxs-lookup"><span data-stu-id="af70b-155">Page</span></span> | <span data-ttu-id="af70b-156">起始数量</span><span class="sxs-lookup"><span data-stu-id="af70b-156">from</span></span> | <span data-ttu-id="af70b-157">大小</span><span class="sxs-lookup"><span data-stu-id="af70b-157">size</span></span> |
    |:-----|:-----|:-----|
    | <span data-ttu-id="af70b-158">1</span><span class="sxs-lookup"><span data-stu-id="af70b-158">1</span></span>    | <span data-ttu-id="af70b-159">0</span><span class="sxs-lookup"><span data-stu-id="af70b-159">0</span></span> | <span data-ttu-id="af70b-160">25</span><span class="sxs-lookup"><span data-stu-id="af70b-160">25</span></span> |
    | <span data-ttu-id="af70b-161">2</span><span class="sxs-lookup"><span data-stu-id="af70b-161">2</span></span>    | <span data-ttu-id="af70b-162">25</span><span class="sxs-lookup"><span data-stu-id="af70b-162">25</span></span> | <span data-ttu-id="af70b-163">50</span><span class="sxs-lookup"><span data-stu-id="af70b-163">50</span></span> |
    | <span data-ttu-id="af70b-164">3</span><span class="sxs-lookup"><span data-stu-id="af70b-164">3</span></span>    | <span data-ttu-id="af70b-165">75</span><span class="sxs-lookup"><span data-stu-id="af70b-165">75</span></span> | <span data-ttu-id="af70b-166">75</span><span class="sxs-lookup"><span data-stu-id="af70b-166">75</span></span> |
    | <span data-ttu-id="af70b-167">4</span><span class="sxs-lookup"><span data-stu-id="af70b-167">4</span></span>    | <span data-ttu-id="af70b-168">150</span><span class="sxs-lookup"><span data-stu-id="af70b-168">150</span></span> | <span data-ttu-id="af70b-169">100</span><span class="sxs-lookup"><span data-stu-id="af70b-169">100</span></span> |

### <a name="get-the-most-relevant-emails"></a><span data-ttu-id="af70b-170">获取最相关的电子邮件</span><span class="sxs-lookup"><span data-stu-id="af70b-170">Get the most relevant emails</span></span>

<span data-ttu-id="af70b-171">搜索 **message** 实体时，将 **enableTopResults** 指定为 `true` 返回邮件的混合列表：响应中的前 3 封邮件按相关性排序，剩余邮件按日期排序。</span><span class="sxs-lookup"><span data-stu-id="af70b-171">When searching the **message** entity, specifying **enableTopResults** as `true` returns a hybrid list of messages: the first three messages in the response are sorted by relevance; the remaining messages are sorted by date.</span></span>

### <a name="get-selected-properties"></a><span data-ttu-id="af70b-172">获取选定属性</span><span class="sxs-lookup"><span data-stu-id="af70b-172">Get selected properties</span></span>

<span data-ttu-id="af70b-173">搜索 **externalItem** 实体时，使用 **stored_fields** 属性指定要在响应中返回的字段。</span><span class="sxs-lookup"><span data-stu-id="af70b-173">When searching an **externalItem** entity, use the **stored_fields** property to specify the fields to be returned in the response.</span></span>

<span data-ttu-id="af70b-174">**stored_fields** 中指定的字段应为可检索的托管属性，且它们已通过 Microsoft 搜索租户管理针对连接进行了配置。</span><span class="sxs-lookup"><span data-stu-id="af70b-174">The fields specified in **stored_fields** should be retrievable managed properties that have been configured for the connection via the Microsoft Search tenant administration.</span></span>

### <a name="keyword-query-language-kql-support"></a><span data-ttu-id="af70b-175">关键字查询语言 (KQL) 支持</span><span class="sxs-lookup"><span data-stu-id="af70b-175">Keyword Query Language (KQL) support</span></span>

<span data-ttu-id="af70b-176">在实际搜索查询字符串（**查询**请求正文的**查询**属性）中的 KQL 语法中，指定自由文本关键字、运算符（例如 `AND`、`OR`）和属性限制。</span><span class="sxs-lookup"><span data-stu-id="af70b-176">Specify free text keywords, operators (such as `AND`, `OR`), and property restrictions in KQL syntax in the actual search query string (**query** property of the **query** request body).</span></span> <span data-ttu-id="af70b-177">语法和命令取决于在同一**查询**请求主体中指向的实体类型（在 **entityTypes** 属性中）。</span><span class="sxs-lookup"><span data-stu-id="af70b-177">The syntax and command depend on the entity types (in the **entityTypes** property) you target in the same **query** request body.</span></span>

<span data-ttu-id="af70b-178">可搜索的属性各不相同，具体取决于实体类型。</span><span class="sxs-lookup"><span data-stu-id="af70b-178">Depending on the entity type, the searchable properties vary.</span></span> <span data-ttu-id="af70b-179">有关详细信息，请参阅：</span><span class="sxs-lookup"><span data-stu-id="af70b-179">For details, see:</span></span>

- [<span data-ttu-id="af70b-180">电子邮件属性</span><span class="sxs-lookup"><span data-stu-id="af70b-180">Email properties</span></span>](/microsoft-365/compliance/keyword-queries-and-search-conditions#searchable-email-properties)
- [<span data-ttu-id="af70b-181">站点属性</span><span class="sxs-lookup"><span data-stu-id="af70b-181">Site properties</span></span>](/microsoft-365/compliance/keyword-queries-and-search-conditions#searchable-site-properties)

## <a name="error-handling"></a><span data-ttu-id="af70b-182">错误处理</span><span class="sxs-lookup"><span data-stu-id="af70b-182">Error handling</span></span>

<span data-ttu-id="af70b-183">搜索 API 将返回由 [OData 错误对象定义](http://docs.oasis-open.org/odata/odata-json-format/v4.01/cs01/odata-json-format-v4.01-cs01.html#sec_ErrorResponse)所定义的错误响应，其中每个是包含代码和消息的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="af70b-183">The search API returns error responses as defined by [OData error object definition](http://docs.oasis-open.org/odata/odata-json-format/v4.01/cs01/odata-json-format-v4.01-cs01.html#sec_ErrorResponse), each of which is a JSON object containing a code and a message.</span></span>

<!---TODO Describe the know errors : bad requests.--->

## <a name="known-limitations"></a><span data-ttu-id="af70b-184">已知限制</span><span class="sxs-lookup"><span data-stu-id="af70b-184">Known limitations</span></span>

<span data-ttu-id="af70b-185">搜索 API 存在以下限制：</span><span class="sxs-lookup"><span data-stu-id="af70b-185">The search API has the following limitations:</span></span>

- <span data-ttu-id="af70b-186">定义**查询**方法，以允许一次传递一个或多个 **searchRequest** 实例的集合。</span><span class="sxs-lookup"><span data-stu-id="af70b-186">The **query** method is defined to allow passing a collection of one or more **searchRequest** instances at once.</span></span> <span data-ttu-id="af70b-187">但是，该服务当前仅支持一次传递一个 [searchRequest](./searchrequest.md)。</span><span class="sxs-lookup"><span data-stu-id="af70b-187">However, the service currently supports only a single [searchRequest](./searchrequest.md) at a time.</span></span>

- <span data-ttu-id="af70b-188">[searchRequest](./searchrequest.md) 资源支持一次传递多个类型的实体。</span><span class="sxs-lookup"><span data-stu-id="af70b-188">The [searchRequest](./searchrequest.md) resource supports passing multiple types of entities at a time.</span></span> <span data-ttu-id="af70b-189">但是，当前唯一支持的组合是 **driveItem** 和 **externalFile**。</span><span class="sxs-lookup"><span data-stu-id="af70b-189">However, currently the only supported combination is **driveItem** and **externalFile**.</span></span> <span data-ttu-id="af70b-190">其他组合无效。</span><span class="sxs-lookup"><span data-stu-id="af70b-190">Other combinations are invalid.</span></span>

- <span data-ttu-id="af70b-191">仅当将 **entityType** 指定为 `externalItem` 时，定义要使用的连接的 **contentSource** 属性才适用。</span><span class="sxs-lookup"><span data-stu-id="af70b-191">The **contentSource** property, which defines the connection to use, is only applicable when **entityType** is specified as `externalItem`.</span></span>
<!--todo nmoreauteam Fix the link to ContentSource  pls provide the content source url--->

- <span data-ttu-id="af70b-192">搜索 API 不支持自定义排序，并且始终通过以下方式对结果进行排序：</span><span class="sxs-lookup"><span data-stu-id="af70b-192">The search API does not support custom sort and always sorts results in the following ways:</span></span>

  - <span data-ttu-id="af70b-193">按日期对 **message** 或 **event** 类型结果进行排序。</span><span class="sxs-lookup"><span data-stu-id="af70b-193">Sort **message** or **event** type results by date.</span></span>

  - <span data-ttu-id="af70b-194">按相关性对 **driveItem**、**externalFile** 或 **externalItem** 类型结果进行排序。</span><span class="sxs-lookup"><span data-stu-id="af70b-194">Sort **driveItem**, **externalFile**, or **externalItem** type results by relevance.</span></span>

## <a name="whats-new"></a><span data-ttu-id="af70b-195">最近更新</span><span class="sxs-lookup"><span data-stu-id="af70b-195">What's new</span></span>
<span data-ttu-id="af70b-196">了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。</span><span class="sxs-lookup"><span data-stu-id="af70b-196">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>


