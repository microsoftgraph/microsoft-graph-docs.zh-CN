---
title: 使用 Microsoft 搜索 API 查询数据
description: 使用搜索 API，应用可以在经过身份验证的用户的上下文中搜索 Office 365 数据
localization_priority: Priority
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: afbb9ba469dad7751422902ea4a9876b6ca6b904
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/19/2019
ms.locfileid: "38704127"
---
# <a name="use-the-microsoft-search-api-to-query-data"></a><span data-ttu-id="f8957-103">使用 Microsoft 搜索 API 查询数据</span><span class="sxs-lookup"><span data-stu-id="f8957-103">Use the Microsoft Search API to query data</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8957-104">使用 Microsoft 搜索 API，应用可以查询 Office 365 数据。</span><span class="sxs-lookup"><span data-stu-id="f8957-104">Using the Microsoft Search API, apps can query Office 365 data.</span></span>

<span data-ttu-id="f8957-105">搜索请求在登录用户的上下文中执行，并使用[包含委派权限的访问令牌](/graph/auth-v2-user)进行标识。</span><span class="sxs-lookup"><span data-stu-id="f8957-105">Search requests are executed in the context of the signed-in user, identified using an [access token with delegated permissions](/graph/auth-v2-user).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="common-use-cases"></a><span data-ttu-id="f8957-106">常见用例</span><span class="sxs-lookup"><span data-stu-id="f8957-106">Common use cases</span></span>

<span data-ttu-id="f8957-107">搜索 API 提供了[查询](../api/search-query.md)方法，可在 Microsoft 搜索中跨数据搜索。</span><span class="sxs-lookup"><span data-stu-id="f8957-107">The search API provides a [query](../api/search-query.md) method to search across your data in Microsoft Search.</span></span> <span data-ttu-id="f8957-108">本部分列出了常见用例，具体取决于在**查询**请求正文中设置的属性。</span><span class="sxs-lookup"><span data-stu-id="f8957-108">This section lists the common use cases, based on the properties you set in the **query** request body.</span></span>

<span data-ttu-id="f8957-109">代表用户执行搜索请求。</span><span class="sxs-lookup"><span data-stu-id="f8957-109">Search requests are executed on behalf of user.</span></span> <span data-ttu-id="f8957-110">削减搜索结果以强制执行应用到项目的任何访问控制。</span><span class="sxs-lookup"><span data-stu-id="f8957-110">Search results are trimmed down to enforce any access control applied to the items.</span></span>  <span data-ttu-id="f8957-111">例如，在文件的上下文中，将在搜索请求过程中评估对文件的权限。</span><span class="sxs-lookup"><span data-stu-id="f8957-111">For example, in the context of files, permissions on the files will be evaluated part of the search request.</span></span> <span data-ttu-id="f8957-112">用户可以访问搜索中的项目数少于可以通过枚举 API 访问的项目数。</span><span class="sxs-lookup"><span data-stu-id="f8957-112">Users cannot access more items in search than they would be able to from the enumeration API.</span></span>

| <span data-ttu-id="f8957-113">用例</span><span class="sxs-lookup"><span data-stu-id="f8957-113">Use cases</span></span> | <span data-ttu-id="f8957-114">要在查询请求正文中定义的属性</span><span class="sxs-lookup"><span data-stu-id="f8957-114">Properties to define in the query request body</span></span> |
|:------------------|:---------|
|[<span data-ttu-id="f8957-115">根据实体类型限定搜索范围</span><span class="sxs-lookup"><span data-stu-id="f8957-115">Scope search based on entity types</span></span>](#scope-search-based-on-entity-types)| <span data-ttu-id="f8957-116">**entityTypes**</span><span class="sxs-lookup"><span data-stu-id="f8957-116">**entityTypes**</span></span> |
|[<span data-ttu-id="f8957-117">页面结果</span><span class="sxs-lookup"><span data-stu-id="f8957-117">Page results</span></span>](#page-search-results) | <span data-ttu-id="f8957-118">**起始数量**和**大小**</span><span class="sxs-lookup"><span data-stu-id="f8957-118">**from** and **size**</span></span> |
|[<span data-ttu-id="f8957-119">获取最相关的电子邮件</span><span class="sxs-lookup"><span data-stu-id="f8957-119">Get the most relevant emails</span></span>](#get-the-most-relevant-emails) | <span data-ttu-id="f8957-120">**enableTopResults**</span><span class="sxs-lookup"><span data-stu-id="f8957-120">**enableTopResults**</span></span> |
|[<span data-ttu-id="f8957-121">获取选定属性</span><span class="sxs-lookup"><span data-stu-id="f8957-121">Get selected properties</span></span>](#get-selected-properties) | <span data-ttu-id="f8957-122">**stored_fields**</span><span class="sxs-lookup"><span data-stu-id="f8957-122">**stored_fields**</span></span> |
|[<span data-ttu-id="f8957-123">在查询条款中使用 KQL</span><span class="sxs-lookup"><span data-stu-id="f8957-123">Use KQL in query terms</span></span>](#keyword-query-language-kql-support) | <span data-ttu-id="f8957-124">**查询**</span><span class="sxs-lookup"><span data-stu-id="f8957-124">**query**</span></span> |
|[<span data-ttu-id="f8957-125">搜索外部文件</span><span class="sxs-lookup"><span data-stu-id="f8957-125">Search external Files</span></span>](/graph/search-concept-files)| <span data-ttu-id="f8957-126">**entityTypes**</span><span class="sxs-lookup"><span data-stu-id="f8957-126">**entityTypes**</span></span> |
|[<span data-ttu-id="f8957-127">在特定 contentSource 中搜索（索引 API）</span><span class="sxs-lookup"><span data-stu-id="f8957-127">Search within a specific contentSource (indexing API)</span></span>](/graph/search-concept-custom-types)| <span data-ttu-id="f8957-128">**contentSources**</span><span class="sxs-lookup"><span data-stu-id="f8957-128">**contentSources**</span></span> |

### <a name="scope-search-based-on-entity-types"></a><span data-ttu-id="f8957-129">根据实体类型限定搜索范围</span><span class="sxs-lookup"><span data-stu-id="f8957-129">Scope search based on entity types</span></span>

<span data-ttu-id="f8957-130">使用**查询**请求有效负载中的 **entityTypes** 属性定义搜索请求的范围。</span><span class="sxs-lookup"><span data-stu-id="f8957-130">Define the scope of the search request using the **entityTypes** property in the **query** request payload.</span></span>
<span data-ttu-id="f8957-131">下面是支持的实体类型：</span><span class="sxs-lookup"><span data-stu-id="f8957-131">The following are the supported entity types:</span></span>

- [<span data-ttu-id="f8957-132">event</span><span class="sxs-lookup"><span data-stu-id="f8957-132">event</span></span>](event.md)
- [<span data-ttu-id="f8957-133">message</span><span class="sxs-lookup"><span data-stu-id="f8957-133">message</span></span>](message.md)
- [<span data-ttu-id="f8957-134">driveItem</span><span class="sxs-lookup"><span data-stu-id="f8957-134">driveItem</span></span>](driveitem.md)
- [<span data-ttu-id="f8957-135">externalFile</span><span class="sxs-lookup"><span data-stu-id="f8957-135">externalFile</span></span>](externalfile.md)
- [<span data-ttu-id="f8957-136">externalItem</span><span class="sxs-lookup"><span data-stu-id="f8957-136">externalItem</span></span>](externalitem.md)

### <a name="page-search-results"></a><span data-ttu-id="f8957-137">页面搜索结果</span><span class="sxs-lookup"><span data-stu-id="f8957-137">Page search results</span></span>

<span data-ttu-id="f8957-138">通过在**查询**请求正文中指定以下两个属性来控制搜索结果的分页：</span><span class="sxs-lookup"><span data-stu-id="f8957-138">Control pagination of the search results by specifying the following two properties in the **query** request body:</span></span>

- <span data-ttu-id="f8957-139">**起始数量**，该值是从 0 开始的整数，在页面上列出搜索结果。</span><span class="sxs-lookup"><span data-stu-id="f8957-139">**from** which is an integer that indicates the 0-based starting point to list search results on the page.</span></span> <span data-ttu-id="f8957-140">默认值为 0。</span><span class="sxs-lookup"><span data-stu-id="f8957-140">The default value is 0.</span></span>

- <span data-ttu-id="f8957-141">**大小**，该值是指示要为页面返回的结果数的整数。</span><span class="sxs-lookup"><span data-stu-id="f8957-141">**size** which is an integer that indicates the number of results to be returned for a page.</span></span> <span data-ttu-id="f8957-142">默认值为 25。</span><span class="sxs-lookup"><span data-stu-id="f8957-142">The default value is 25.</span></span>

<span data-ttu-id="f8957-143">如果你正在搜索 **event** 或 **message** 实体，则注意以下限制：</span><span class="sxs-lookup"><span data-stu-id="f8957-143">Note the following limits if you're searching the **event** or **message** entity:</span></span>

- <span data-ttu-id="f8957-144">**起始数量**在第一个页面请求中必须从零开始，否则请求将导致出现 HTTP 400 `Bad request`。</span><span class="sxs-lookup"><span data-stu-id="f8957-144">**from** must start at zero in the first page request, otherwise the request results in HTTP 400 `Bad request`.</span></span>
- <span data-ttu-id="f8957-145">每页的最大结果数（**大小**）为 200。</span><span class="sxs-lookup"><span data-stu-id="f8957-145">The maximum results per page (**size**) is 200.</span></span>
- <span data-ttu-id="f8957-146">分页可返回的最大总项数为 1000。</span><span class="sxs-lookup"><span data-stu-id="f8957-146">The maximum total number of items that can be returned by paginating is 1000.</span></span>
- <span data-ttu-id="f8957-147">超出限制将返回最佳响应。</span><span class="sxs-lookup"><span data-stu-id="f8957-147">Going beyond the limits returns a best effort response.</span></span> <span data-ttu-id="f8957-148">请求不会导致 HTTP 400。</span><span class="sxs-lookup"><span data-stu-id="f8957-148">The request does not result in HTTP 400.</span></span>

<span data-ttu-id="f8957-149">最佳实践：</span><span class="sxs-lookup"><span data-stu-id="f8957-149">Best practices:</span></span>

- <span data-ttu-id="f8957-150">指定初始请求中的较小的首页。</span><span class="sxs-lookup"><span data-stu-id="f8957-150">Specify a smaller first page in the initial request.</span></span> <span data-ttu-id="f8957-151">例如，将**起始数量**指定为 0，将**大小**指定为 25。</span><span class="sxs-lookup"><span data-stu-id="f8957-151">For example, specify **from** as 0, **size** as 25.</span></span>
- <span data-ttu-id="f8957-152">通过更新**起始数量**和**大小**属性来对后续页面进行分页。</span><span class="sxs-lookup"><span data-stu-id="f8957-152">Paginate subsequent pages by updating the **from** and **size** properties.</span></span> <span data-ttu-id="f8957-153">可以在每个后续请求中增加页面大小。</span><span class="sxs-lookup"><span data-stu-id="f8957-153">You can increase the page size in each subsequent request.</span></span> <span data-ttu-id="f8957-154">下表显示了一个示例。</span><span class="sxs-lookup"><span data-stu-id="f8957-154">The following table shows an example.</span></span>

    | <span data-ttu-id="f8957-155">页面</span><span class="sxs-lookup"><span data-stu-id="f8957-155">Page</span></span> | <span data-ttu-id="f8957-156">起始数量</span><span class="sxs-lookup"><span data-stu-id="f8957-156">from</span></span> | <span data-ttu-id="f8957-157">大小</span><span class="sxs-lookup"><span data-stu-id="f8957-157">size</span></span> |
    |:-----|:-----|:-----|
    | <span data-ttu-id="f8957-158">1</span><span class="sxs-lookup"><span data-stu-id="f8957-158">1</span></span>    | <span data-ttu-id="f8957-159">0</span><span class="sxs-lookup"><span data-stu-id="f8957-159">0</span></span> | <span data-ttu-id="f8957-160">25</span><span class="sxs-lookup"><span data-stu-id="f8957-160">25</span></span> |
    | <span data-ttu-id="f8957-161">2</span><span class="sxs-lookup"><span data-stu-id="f8957-161">2</span></span>    | <span data-ttu-id="f8957-162">25</span><span class="sxs-lookup"><span data-stu-id="f8957-162">25</span></span> | <span data-ttu-id="f8957-163">50</span><span class="sxs-lookup"><span data-stu-id="f8957-163">50</span></span> |
    | <span data-ttu-id="f8957-164">3</span><span class="sxs-lookup"><span data-stu-id="f8957-164">3</span></span>    | <span data-ttu-id="f8957-165">75</span><span class="sxs-lookup"><span data-stu-id="f8957-165">75</span></span> | <span data-ttu-id="f8957-166">75</span><span class="sxs-lookup"><span data-stu-id="f8957-166">75</span></span> |
    | <span data-ttu-id="f8957-167">4</span><span class="sxs-lookup"><span data-stu-id="f8957-167">4</span></span>    | <span data-ttu-id="f8957-168">150</span><span class="sxs-lookup"><span data-stu-id="f8957-168">150</span></span> | <span data-ttu-id="f8957-169">100</span><span class="sxs-lookup"><span data-stu-id="f8957-169">100</span></span> |

### <a name="get-the-most-relevant-emails"></a><span data-ttu-id="f8957-170">获取最相关的电子邮件</span><span class="sxs-lookup"><span data-stu-id="f8957-170">Get the most relevant emails</span></span>

<span data-ttu-id="f8957-171">搜索 **message** 实体时，将 **enableTopResults** 指定为 `true` 返回邮件的混合列表：响应中的前 3 封邮件按相关性排序，剩余邮件按日期排序。</span><span class="sxs-lookup"><span data-stu-id="f8957-171">When searching the **message** entity, specifying **enableTopResults** as `true` returns a hybrid list of messages : the first 3 messages in the response are sorted by relevance, the remaining messages are sorted by date.</span></span>

### <a name="get-selected-properties"></a><span data-ttu-id="f8957-172">获取选定属性</span><span class="sxs-lookup"><span data-stu-id="f8957-172">Get selected properties</span></span>

<span data-ttu-id="f8957-173">搜索 **externalItem** 实体时，使用 **stored_fields** 属性指定要在响应中返回的字段。</span><span class="sxs-lookup"><span data-stu-id="f8957-173">When searching an **externalItem** entity, use the **stored_fields** property to specify the fields to be returned in the response.</span></span>

<span data-ttu-id="f8957-174">**stored_fields** 中指定的名称应为可检索的托管属性。</span><span class="sxs-lookup"><span data-stu-id="f8957-174">The names specified in **stored_fields** should be the retrievable Managed Property.</span></span> <span data-ttu-id="f8957-175">已针对 Microsoft 搜索的租户管理中的连接配置了这些属性名称。</span><span class="sxs-lookup"><span data-stu-id="f8957-175">These property names have been configured for the connection in the  tenant administration of Microsoft Search.</span></span>

### <a name="keyword-query-language-kql-support"></a><span data-ttu-id="f8957-176">关键字查询语言 (KQL) 支持</span><span class="sxs-lookup"><span data-stu-id="f8957-176">Keyword Query Language (KQL) support</span></span>

<span data-ttu-id="f8957-177">在实际搜索查询字符串（**查询**请求正文的**查询**属性）中的 KQL 语法中，指定自由文本关键字、运算符（例如 `AND`、`OR`）和属性限制。</span><span class="sxs-lookup"><span data-stu-id="f8957-177">Specify free text keywords, operators (such as `AND`, `OR`), and property restrictions in KQL syntax in the actual search query string (**query** property of the **query** request body).</span></span> <span data-ttu-id="f8957-178">语法和命令取决于在同一**查询**请求主体中指向的实体类型（在 **entityTypes** 属性中）。</span><span class="sxs-lookup"><span data-stu-id="f8957-178">The syntax and command depend on the entity types (in the **entityTypes** property) you target in the same **query** request body.</span></span>

<span data-ttu-id="f8957-179">可搜索的属性各不相同，具体取决于实体类型：</span><span class="sxs-lookup"><span data-stu-id="f8957-179">Depending on the entity type, the searchable properties vary:</span></span>

- [<span data-ttu-id="f8957-180">邮件属性</span><span class="sxs-lookup"><span data-stu-id="f8957-180">message properties</span></span>](/microsoft-365/compliance/keyword-queries-and-search-conditions#searchable-email-properties)
- [<span data-ttu-id="f8957-181">driveItem 属性</span><span class="sxs-lookup"><span data-stu-id="f8957-181">driveItem properties</span></span>](/microsoft-365/compliance/keyword-queries-and-search-conditions#searchable-site-properties)

## <a name="error-handling"></a><span data-ttu-id="f8957-182">错误处理</span><span class="sxs-lookup"><span data-stu-id="f8957-182">Error handling</span></span>

<span data-ttu-id="f8957-183">搜索 API 将返回由 [OData 错误对象定义](http://docs.oasis-open.org/odata/odata-json-format/v4.01/cs01/odata-json-format-v4.01-cs01.html#sec_ErrorResponse)所定义的错误响应，其中每个是包含代码和消息的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="f8957-183">The search API returns error responses as defined by [OData error object definition](http://docs.oasis-open.org/odata/odata-json-format/v4.01/cs01/odata-json-format-v4.01-cs01.html#sec_ErrorResponse), each of which is a JSON object containing a code and a message.</span></span>

<!---TODO Describe the know errors : bad requests.--->

## <a name="known-limitations"></a><span data-ttu-id="f8957-184">已知限制</span><span class="sxs-lookup"><span data-stu-id="f8957-184">Known limitations</span></span>

<span data-ttu-id="f8957-185">搜索 API 存在以下限制：</span><span class="sxs-lookup"><span data-stu-id="f8957-185">The search API has the following limitations:</span></span>

- <span data-ttu-id="f8957-186">定义**查询**方法，以允许一次传递一个或多个 **searchRequest** 实例的集合。</span><span class="sxs-lookup"><span data-stu-id="f8957-186">The **query** method is defined to allow passing a collection of one or more **searchRequest** instances at once.</span></span> <span data-ttu-id="f8957-187">但是，该服务当前仅支持一次传递一个 [searchRequest](./searchrequest.md)。</span><span class="sxs-lookup"><span data-stu-id="f8957-187">However, the service currently supports only a single [searchRequest](./searchrequest.md) at a time.</span></span>

- <span data-ttu-id="f8957-188">[searchRequest](./searchrequest.md) 资源支持一次传递多个类型的实体。</span><span class="sxs-lookup"><span data-stu-id="f8957-188">The [searchRequest](./searchrequest.md) resource supports passing multiple types of entities at a time.</span></span> <span data-ttu-id="f8957-189">但是，当前唯一支持的组合是 **driveItem** 和 **externalFile**。</span><span class="sxs-lookup"><span data-stu-id="f8957-189">However, currently the only supported combination is **driveItem** and **externalFile**.</span></span> <span data-ttu-id="f8957-190">其他组合无效。</span><span class="sxs-lookup"><span data-stu-id="f8957-190">Other combinations are invalid.</span></span>

- <span data-ttu-id="f8957-191">仅当将 **entityType** 指定为 `externalItem` 时，定义要使用的连接的 **contentSource** 属性才适用。</span><span class="sxs-lookup"><span data-stu-id="f8957-191">The **contentSource** property, which defines the connection to use, is only applicable when **entityType** is specified as `externalItem`.</span></span>
<!--todo nmoreauteam Fix the link to ContentSource  pls provide the content source url--->

- <span data-ttu-id="f8957-192">搜索 API 不支持自定义排序，并且始终通过以下方式对结果进行排序：</span><span class="sxs-lookup"><span data-stu-id="f8957-192">The search API does not support custom sort and always sorts results in the following ways:</span></span>

  - <span data-ttu-id="f8957-193">按日期对 **message** 或 **event** 类型结果进行排序。</span><span class="sxs-lookup"><span data-stu-id="f8957-193">Sort **message** or **event** type results by date.</span></span>

  - <span data-ttu-id="f8957-194">按相关性对 **driveItem**、**externalFile** 或 **externalItem** 类型结果进行排序。</span><span class="sxs-lookup"><span data-stu-id="f8957-194">Sort **driveItem**, **externalFile**, or **externalItem** type results by relevance.</span></span>
