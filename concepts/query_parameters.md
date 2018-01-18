# <a name="use-query-parameters-to-customize-responses"></a><span data-ttu-id="3dc8b-101">使用查询参数自定义响应</span><span class="sxs-lookup"><span data-stu-id="3dc8b-101">Use query parameters to customize responses</span></span>

<span data-ttu-id="3dc8b-p101">Microsoft Graph 提供可选的查询参数，可用于指定和控制响应中返回的数据量。支持以下查询参数。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-p101">Microsoft Graph provides optional query parameters that you can use to specify and control the amount of data returned in a response. The following query parameters are supported.</span></span>

><span data-ttu-id="3dc8b-104">**注意：**单击示例以在 [Graph 浏览器][graph-explorer]中试调用。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-104">**Note:** Click the examples to try them in [Graph Explorer][graph-explorer].</span></span>

| <span data-ttu-id="3dc8b-105">名称</span><span class="sxs-lookup"><span data-stu-id="3dc8b-105">Name</span></span>                     | <span data-ttu-id="3dc8b-106">说明</span><span class="sxs-lookup"><span data-stu-id="3dc8b-106">Description</span></span> | <span data-ttu-id="3dc8b-107">示例</span><span class="sxs-lookup"><span data-stu-id="3dc8b-107">Example</span></span>
|:-------------------------|:------------|:---------|
| [<span data-ttu-id="3dc8b-108">$count</span><span class="sxs-lookup"><span data-stu-id="3dc8b-108">$count</span></span>](#count-parameter)         | <span data-ttu-id="3dc8b-109">检索匹配资源的总数。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-109">Retrieves the total count of matching resources.</span></span> | [`/me/messages?$top=2&$count=true`][count-example]
| [<span data-ttu-id="3dc8b-110">$expand</span><span class="sxs-lookup"><span data-stu-id="3dc8b-110">$expand</span></span>](#expand-parameter)       | <span data-ttu-id="3dc8b-111">检索相关资源。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-111">Retrieves related resources.</span></span>|[`/groups?$expand=members`][expand-example]
| [<span data-ttu-id="3dc8b-112">$filter</span><span class="sxs-lookup"><span data-stu-id="3dc8b-112">$filter</span></span>](#filter-parameter)       | <span data-ttu-id="3dc8b-113">筛选结果（行）。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-113">Filters results (rows).</span></span>|[`/users?$filter=startswith(givenName,'J')`][filter-example]
| [<span data-ttu-id="3dc8b-114">$format</span><span class="sxs-lookup"><span data-stu-id="3dc8b-114">$format</span></span>](#format-parameter)       | <span data-ttu-id="3dc8b-115">返回指定媒体格式的结果。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-115">Returns the results in the specified media format.</span></span>|[`/users?$format=json`][format-example]
| [<span data-ttu-id="3dc8b-116">$orderby</span><span class="sxs-lookup"><span data-stu-id="3dc8b-116">$orderby</span></span>](#orderby-parameter)     | <span data-ttu-id="3dc8b-117">对结果进行排序。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-117">Orders results.</span></span>|[`/users?$orderby=displayName desc`][orderby-example]
| [<span data-ttu-id="3dc8b-118">$search</span><span class="sxs-lookup"><span data-stu-id="3dc8b-118">$search</span></span>](#search-parameter)       | <span data-ttu-id="3dc8b-p102">根据搜索条件返回结果。目前支持用于 **messages** 和 **person** 集合。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-p102">Returns results based on search criteria. Currently supported on **** and **** collections.</span></span>|[`/me/messages?$search=pizza`][search-example]
| [<span data-ttu-id="3dc8b-121">$select</span><span class="sxs-lookup"><span data-stu-id="3dc8b-121">$select</span></span>](#select-parameter)       | <span data-ttu-id="3dc8b-122">筛选属性（列）。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-122">Filters properties (columns).</span></span>|[`/users?$select=givenName,surname`][select-example]
| [<span data-ttu-id="3dc8b-123">$skip</span><span class="sxs-lookup"><span data-stu-id="3dc8b-123">$skip</span></span>](#skip-parameter)           | <span data-ttu-id="3dc8b-p103">对结果集建立索引。一些 API 也使用它来实现分页，并且可以与 `$top` 一起使用来手动对结果分页。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-p103">Indexes into a result set. Also used by some APIs to implement paging and can be used together with `$top` to manually page results.</span></span> | [`/me/messages?$skip=11`][skip-example]
| [<span data-ttu-id="3dc8b-126">$skipToken</span><span class="sxs-lookup"><span data-stu-id="3dc8b-126">$skipToken</span></span>](#skiptoken-parameter) | <span data-ttu-id="3dc8b-p104">从跨多页的结果集中检索下一页结果。（但某些 API 改为使用 `$skip`。）</span><span class="sxs-lookup"><span data-stu-id="3dc8b-p104">Retrieves the next page of results from result sets that span multiple pages. (Some APIs use `$skip` instead.)</span></span> | `/users?$skiptoken=X%274453707402000100000017...`|
| [<span data-ttu-id="3dc8b-129">$top</span><span class="sxs-lookup"><span data-stu-id="3dc8b-129">$top</span></span>](#top-parameter)             | <span data-ttu-id="3dc8b-130">设置结果的页面大小。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-130">Sets the page size of results.</span></span> |[`/users?$top=2`][top-example]



<span data-ttu-id="3dc8b-131">这些参数与 [OData V4 查询语言][odata-query]兼容。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-131">These parameters are compatible with the [OData V4 query language][odata-query].</span></span> <span data-ttu-id="3dc8b-132">并非所有的 Microsoft Graph API 都支持所有参数，而对 `v1.0` 和 `beta` 终结点的支持可能会显著不同。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-132">Not all parameters are supported across all Microsoft Graph APIs, and support might differ significantly between the `v1.0` and `beta` endpoints.</span></span> 

> <span data-ttu-id="3dc8b-p106">**注意：**在 `beta` 终结点上，`$` 前缀是可选的。例如，可使用 `filter` 来代替 `$filter`。有关更多详细信息和示例，请参阅 [Microsoft Graph 中支持不含 $ 前缀的查询参数](http://dev.office.com/queryparametersinMicrosoftGraph)。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-p106">**Note:** On the `beta` endpoint, the `$` prefix is optional. For example, instead of `$filter`, you can use `filter`. For more details and examples, see [Supporting query parameters without $ prefixes in Microsoft Graph](http://dev.office.com/queryparametersinMicrosoftGraph).</span></span>

## <a name="encoding-query-parameters"></a><span data-ttu-id="3dc8b-136">编码的查询参数</span><span class="sxs-lookup"><span data-stu-id="3dc8b-136">Encoding query parameters</span></span>

<span data-ttu-id="3dc8b-137">应对查询参数的值进行百分比编码。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-137">The values of query parameters should be percent-encoded.</span></span> <span data-ttu-id="3dc8b-138">许多 HTTP 客户端、浏览器和工具（例如，[Graph 浏览器][graph-explorer]）都可以帮助用户完成此操作。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-138">Many HTTP clients, browsers, and tools (such as the [Graph Explorer][graph-explorer]) will help you with this.</span></span> <span data-ttu-id="3dc8b-139">如果查询失败，可能原因之一是未正确编码查询参数值。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-139">If a query is failing, one possible cause is failure to encode the query parameter values appropriately.</span></span>

<span data-ttu-id="3dc8b-140">未编码的 URL 如下所示：</span><span class="sxs-lookup"><span data-stu-id="3dc8b-140">An unencoded URL looks like this:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName, 'J')
```

<span data-ttu-id="3dc8b-141">正确解码的 URL 如下所示：</span><span class="sxs-lookup"><span data-stu-id="3dc8b-141">A properly encoded URL looks like this:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName%2C+'J')
```

## <a name="count-parameter"></a><span data-ttu-id="3dc8b-142">count 参数</span><span class="sxs-lookup"><span data-stu-id="3dc8b-142">count parameter</span></span>

<span data-ttu-id="3dc8b-143">使用 `$count` 查询参数以包括集合中项总数的计数，以及从 Microsoft Graph 返回的数据值页。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-143">Use the `$count` query parameter to include a count of the total number of items in a collection alongside the page of data values returned from Microsoft Graph.</span></span> 

<span data-ttu-id="3dc8b-144">例如，下面的请求返回当前用户的 **contact** 集合，以及 `@odata.count` 属性中 **contact** 集合内的项数。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-144">For example, the following request will return both the **** collection of the current user, and the number of items in the **** collection in the `@odata.count` property.</span></span>

```http
GET  https://graph.microsoft.com/v1.0/me/contacts?$count=true
```

[<span data-ttu-id="3dc8b-145">在 Graph 浏览器中试调用</span><span class="sxs-lookup"><span data-stu-id="3dc8b-145">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/contacts?$count=true&method=GET&version=v1.0)


><span data-ttu-id="3dc8b-146">**注意：**派生自 [directoryObject](../api-reference/v1.0/resources/directoryobject.md) 的资源集合（如 [user](../api-reference/v1.0/resources/user.md) 或 [group](../api-reference/v1.0/resources/group.md) 集合）不支持 `$count`。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-146">Note:  is not supported for collections of resources that derive from    like collections of users or groups.</span></span>

## <a name="expand-parameter"></a><span data-ttu-id="3dc8b-147">expand 参数</span><span class="sxs-lookup"><span data-stu-id="3dc8b-147">expand parameter</span></span>

<span data-ttu-id="3dc8b-148">许多 Microsoft Graph 资源都会公开资源的已声明属性以及与其他资源的关系。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-148">Many Microsoft Graph resources expose both declared properties of the resource as well as its relationships with other resources.</span></span> <span data-ttu-id="3dc8b-149">这些关系也称为引用属性或导航属性，它们可以引用单个资源或资源集合。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-149">These relationships are also called reference properties or navigation properties, and they can reference either a single resource or a collection of resources.</span></span> <span data-ttu-id="3dc8b-150">例如，用户的邮件文件夹、管理者和直接下属都将作为关系公开。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-150">For example, the mail folders, manager, and direct reports of a user are all exposed as relationships.</span></span> 

<span data-ttu-id="3dc8b-p109">通常情况下，可以在单个请求中查询资源属性或其关系之一，但不能同时查询。可以使用 `$expand` 查询字符串参数以包含结果中单个关系（导航属性）引用的扩展资源或集合。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-p109">Normally, you can query either the properties of a resource or one of its relationships in a single request, but not both. You can use the `$expand` query string parameter to include the expanded resource or collection referenced by a single relationship (navigation property) in your results.</span></span>

<span data-ttu-id="3dc8b-153">以下示例在驱动器中获取根驱动器信息以及顶级子项：</span><span class="sxs-lookup"><span data-stu-id="3dc8b-153">The following example gets root drive information along with the top-level child items in a drive:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children
```

[<span data-ttu-id="3dc8b-154">在 Graph 浏览器中试调用</span><span class="sxs-lookup"><span data-stu-id="3dc8b-154">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/drive/root?$expand=children&method=GET&version=v1.0)

<span data-ttu-id="3dc8b-p110">使用一些资源集合，还可以添加 `$select` 参数，指定要在扩展资源中返回的属性。下面的示例执行与上一示例几乎相同的查询，不同之处在于使用 [`$select`](#select-parameter) 语句将为扩展子项返回的属性限制为 **id** 和 **name** 属性。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-p110">With some resource collections, you can also specify the properties to be returned in the expanded resources by adding a `$select` parameter. The following example performs the same query as the previous example but uses a [`$select`](#select-parameter) statement to limit the properties returned for the expanded child items to the **** and **** properties.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children($select=id,name)
```

<span data-ttu-id="3dc8b-157">[在 Graph 浏览器中试用][expand-example]</span><span class="sxs-lookup"><span data-stu-id="3dc8b-157">[Try in Graph Explorer][expand-example]</span></span>

> <span data-ttu-id="3dc8b-p111">**注意：**并不是所有关系和资源都支持 `$expand` 查询参数。例如，可以扩展用户的 **directReports**、**manager** 和 **memberOf** 关系，但无法扩展其 **events**、**messages** 或 **photo** 关系。并非所有资源或关系都支持对扩展项使用 `$select`。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-p111">**Note:** Not all relationships and resources support the `$expand` query parameter. For example, you can expand the ****, ****, and **** relationships on a user, but you cannot expand its ****, ****, or **** relationships. Not all resources or relationships support using `$select` on expanded items.</span></span> 
> 
> <span data-ttu-id="3dc8b-161">使用从 [directoryObject](../api-reference/v1.0/resources/directoryobject.md) 派生的 Azure AD 资源（如[user](../api-reference/v1.0/resources/user.md) 和 [group](../api-reference/v1.0/resources/group.md)），`$expand` 仅支持 `beta`，并且通常最多为扩展关系返回 20 个项。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-161">With Azure AD resources that derive from [directoryObject](../api-reference/v1.0/resources/directoryobject.md), like [user](../api-reference/v1.0/resources/user.md) and [group](../api-reference/v1.0/resources/group.md), `$expand` is only supported for `beta` and  typically returns a maximum of 20 items for the expanded relationship.</span></span>

## <a name="filter-parameter"></a><span data-ttu-id="3dc8b-162">filter 参数</span><span class="sxs-lookup"><span data-stu-id="3dc8b-162">filter parameter</span></span>

<span data-ttu-id="3dc8b-163">使用 `$filter` 查询参数，以仅检索集合的子集。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-163">Use the `$filter` query parameter to retrieve just a subset of a collection.</span></span> 

<span data-ttu-id="3dc8b-164">例如，若要查找显示名称以子母“J”开头的用户，请使用 `startswith`。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-164">For example, to find users whose display name starts with the letter 'J', use `startswith`.</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'J')
```

<span data-ttu-id="3dc8b-165">[在 Graph 浏览器中试用][filter-example]</span><span class="sxs-lookup"><span data-stu-id="3dc8b-165">[Try in Graph Explorer][filter-example]</span></span>

<span data-ttu-id="3dc8b-166">对 `$filter` 运算符的支持因 Microsoft Graph API 而异。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-166">Support for `$filter` operators varies across Microsoft Graph APIs.</span></span> <span data-ttu-id="3dc8b-167">通常支持下列逻辑运算符：</span><span class="sxs-lookup"><span data-stu-id="3dc8b-167">The following logical operators are generally supported:</span></span> 

- <span data-ttu-id="3dc8b-168">等于 (`eq`)</span><span class="sxs-lookup"><span data-stu-id="3dc8b-168">equals (`eq`)</span></span>
- <span data-ttu-id="3dc8b-169">不等于 (`ne`)</span><span class="sxs-lookup"><span data-stu-id="3dc8b-169">not equals (`ne`)</span></span>
- <span data-ttu-id="3dc8b-170">大于 (`gt`)</span><span class="sxs-lookup"><span data-stu-id="3dc8b-170">greater than (`gt`)</span></span>
- <span data-ttu-id="3dc8b-171">大于或等于 (`ge`)</span><span class="sxs-lookup"><span data-stu-id="3dc8b-171">greater than or equals (`ge`)</span></span>
- <span data-ttu-id="3dc8b-172">小于 (`lt`)，小于或等于 (`le`)</span><span class="sxs-lookup"><span data-stu-id="3dc8b-172">less than (`lt`), less than or equals (`le`)</span></span>
- <span data-ttu-id="3dc8b-173">且 (`and`)</span><span class="sxs-lookup"><span data-stu-id="3dc8b-173">and (`and`)</span></span>
- <span data-ttu-id="3dc8b-174">或 (`or`)</span><span class="sxs-lookup"><span data-stu-id="3dc8b-174">or (`or`)</span></span>
- <span data-ttu-id="3dc8b-175">非 (`not`)</span><span class="sxs-lookup"><span data-stu-id="3dc8b-175">not (`not`)</span></span>
 
<span data-ttu-id="3dc8b-176">通常支持 `startswith` 字符串运算符。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-176">The `startswith` string operator is often supported.</span></span> <span data-ttu-id="3dc8b-177">某些 API 支持 `any` lambda 运算符。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-177">The `any` lambda operator is supported for some APIs.</span></span> <span data-ttu-id="3dc8b-178">有关一些用法示例的信息，请参阅下表。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-178">For some  usage examples, see the following table.</span></span> <span data-ttu-id="3dc8b-179">有关 `$filter` 语法的其他详细信息，请参阅 [OData 协议][odata-filter]。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-179">For more details about `$filter` syntax, see the [OData protocol][odata-filter].</span></span>  

<span data-ttu-id="3dc8b-180">下表显示使用 `$filter` 查询参数的一些示例。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-180">The following table shows some examples that use the `$filter` query parameter.</span></span>

> <span data-ttu-id="3dc8b-181">**注意：**单击示例以在 [Graph 浏览器][graph-explorer]中试调用。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-181">**Note:** Click the examples to try them in [Graph Explorer][graph-explorer].</span></span>

| <span data-ttu-id="3dc8b-182">说明</span><span class="sxs-lookup"><span data-stu-id="3dc8b-182">Description</span></span> | <span data-ttu-id="3dc8b-183">示例</span><span class="sxs-lookup"><span data-stu-id="3dc8b-183">Example</span></span>
|:------------|:--------|
| <span data-ttu-id="3dc8b-184">跨多个属性搜索名为 Mary 的用户。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-184">Search for users with the name Mary across multiple properties.</span></span> | [`https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'mary') or startswith(givenName,'mary') or startswith(surname,'mary') or startswith(mail,'mary') or startswith(userPrincipalName,'mary')`](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(displayName,'mary')+or+startswith(givenName,'mary')+or+startswith(surname,'mary')+or+startswith(mail,'mary')+or+startswith(userPrincipalName,'mary')&method=GET&version=v1.0) 
| <span data-ttu-id="3dc8b-185">获取 2017 年 7 月 1 日之后开始的所有登录用户的事件。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-185">Get all the signed-in user's events that start after 7/1/2017.</span></span> | [`https://graph.microsoft.com/v1.0/me/events?$filter=start/dateTime ge '2017-07-01T08:00'`](https://developer.microsoft.com/graph/graph-explorer?request=me/events?$filter=start/dateTime+ge+'2017-07-01T08:00'&method=GET&version=v1.0) 
| <span data-ttu-id="3dc8b-186">获取登录用户收到的来自特定地址的所有电子邮件。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-186">Get all emails from a specific address received by the signed-in user.</span></span> | [`https://graph.microsoft.com/v1.0/me/messages?$filter=from/emailAddress/address eq 'someuser@example.com'`](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=from/emailAddress/address+eq+'someuser@.com'&method=GET&version=v1.0) 
| <span data-ttu-id="3dc8b-187">获取登录用户在 2017 年 4 月收到的所有电子邮件。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-187">Get all emails received by the signed-in user in April 2017.</span></span> | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=ReceivedDateTime ge 2017-04-01 and receivedDateTime lt 2017-05-01`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=ReceivedDateTime+ge+2017-04-01+and+receivedDateTime+lt+2017-05-01&method=GET&version=v1.0) 
| <span data-ttu-id="3dc8b-188">获取登录用户收件箱中的所有未读邮件。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-188">Get all unread mail in the signed-in user's Inbox.</span></span> | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=isRead eq false`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=isRead+eq+false&method=GET&version=v1.0) 
| <span data-ttu-id="3dc8b-189">列出组织中的所有 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-189">List all Office 365 groups in an organization.</span></span> | [`https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')`](https://developer.microsoft.com/graph/graph-explorer?request=groups?$filter=groupTypes/any(c:c+eq+'Unified')&method=GET&version=v1.0) 

> <span data-ttu-id="3dc8b-p114">**注意：**Azure AD 资源不支持以下 `$filter` 运算符：`ne`、`gt`、`ge`、`lt`、`le` 和 `not`。所有 Microsoft Graph 资源目前均不支持 `contains` 字符串运算符。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-p114">**Note:** The following `$filter` operators are not supported for Azure AD resources:  `ne`, `gt`, `ge`, `lt`, `le`, and `not`. The `contains` string operator is currently not supported on any Microsoft Graph resources.</span></span>

## <a name="format-parameter"></a><span data-ttu-id="3dc8b-192">format 参数</span><span class="sxs-lookup"><span data-stu-id="3dc8b-192">format parameter</span></span>

<span data-ttu-id="3dc8b-193">使用 `$format` 查询参数，指定 Microsoft Graph 返回的项的媒体格式。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-193">Use the `$format` query parameter to specify the media format of the items returned from Microsoft Graph.</span></span>

<span data-ttu-id="3dc8b-194">例如，下面的请求以 json 格式返回组织中的用户：</span><span class="sxs-lookup"><span data-stu-id="3dc8b-194">For example, the following request returns the users in the organization in the json format:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$format=json
```

<span data-ttu-id="3dc8b-195">[在 Graph 浏览器中试用][format-example]</span><span class="sxs-lookup"><span data-stu-id="3dc8b-195">[Try in Graph Explorer][format-example]</span></span>

> <span data-ttu-id="3dc8b-196">**注意：**`$format` 查询参数支持许多格式（例如，atom、xml 和 json），但可能无法返回所有格式的结果。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-196">**Note:** The `$format` query parameter supports a number of formats (for example, atom, xml, and json) but results may not be returned in all formats.</span></span>

## <a name="orderby-parameter"></a><span data-ttu-id="3dc8b-197">orderby 参数</span><span class="sxs-lookup"><span data-stu-id="3dc8b-197">orderby parameter</span></span>

<span data-ttu-id="3dc8b-198">使用 `$orderby` 查询参数指定从 Microsoft Graph 返回的项的排序顺序。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-198">Use the `$orderby` query parameter to specify the sort order of the items returned from Microsoft Graph.</span></span>

<span data-ttu-id="3dc8b-199">例如，以下请求返回按用户显示名称进行排序的组织中的用户：</span><span class="sxs-lookup"><span data-stu-id="3dc8b-199">For example, the following request returns the users in the organization ordered by their display name:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$orderby=displayName
```
<span data-ttu-id="3dc8b-200">[在 Graph 浏览器中试用][orderby-example]</span><span class="sxs-lookup"><span data-stu-id="3dc8b-200">[Try in Graph Explorer][orderby-example]</span></span>

<span data-ttu-id="3dc8b-p115">还可以按复杂类型实体进行排序。下面的请求获取邮件，并按 **from** 属性的 **address** 字段（复杂类型为 **emailAddress**）进行排序：</span><span class="sxs-lookup"><span data-stu-id="3dc8b-p115">You can also sort by complex type entities. The following example gets messages and sorts them by the **address** field of the **from** property, which is of the complex type **emailAddress**:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$orderby=from/emailAddress/address
```
[<span data-ttu-id="3dc8b-203">在 Graph 浏览器中试调用</span><span class="sxs-lookup"><span data-stu-id="3dc8b-203">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/address&method=GET&version=v1.0)

<span data-ttu-id="3dc8b-204">若要以升序或降序对结果进行排序，请向字段名称追加 `asc` 或 `desc`，并用空格隔开。例如，`?$orderby=name%20desc`。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-204">To sort the results in ascending or descending order, append either `asc` or `desc` to the field name, separated by a space; for example, `?$orderby=name%20desc`.</span></span>

<span data-ttu-id="3dc8b-205">通过一些 API，可以对多个属性的结果进行排序。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-205">With some APIs, you can order results on multiple properties.</span></span> <span data-ttu-id="3dc8b-206">例如，以下请求首先按发件人名称以降序（Z 到 A）排序用户收件箱中的邮件，然后按主题以升序（默认）排序邮件。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-206">For example, the following request orders the messages in the user's Inbox, first by the name of the person who sent it in descending order (Z to A), and then by subject in ascending order (default).</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/Inbox/messages?$orderby=from/emailAddress/name desc,subject
```

[<span data-ttu-id="3dc8b-207">在 Graph 浏览器中试调用</span><span class="sxs-lookup"><span data-stu-id="3dc8b-207">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/name%20desc,subject&method=GET&version=v1.0)

<span data-ttu-id="3dc8b-208">如果指定 $filter，服务器会推断结果的排序顺序。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-208">When you specify $filter the server will infer a sort order for the results.</span></span> <span data-ttu-id="3dc8b-209">如果同时使用 `$orderby` 和 `$filter`，由于服务器始终推断 `$filter` 结果的排序顺序，因此必须先在 `$orderby` 中列出 `$filter` 的属性，然后再列出其他任何属性，且必须按照它们在 `$filter` 参数中的顺序列出这些属性。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-209">If you use both `$orderby` and `$filter`, because the server always infers a sort order for the results of a `$filter`, the properties in the `$filter` must be listed first in the `$orderby` before any other properties, and they must be listed in the order that they appear in the `$filter` parameter.</span></span> 

<span data-ttu-id="3dc8b-210">下面的示例展示了如何按 **subject** 和 **importance** 属性筛选查询，再按 **subject**、**importance** 和 **receivedDateTime** 属性进行降序排序。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-210">The following example shows a query filtered by the **subject** and **importance** properties, and then sorted by the **subject**, **importance**, and **receivedDateTime** properties in descending order.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=Subject eq 'welcome to exchange unified messaging' and importance eq 'normal'&$orderby=subject,importance,receivedDateTime desc
```

[<span data-ttu-id="3dc8b-211">在 Graph 浏览器中试调用</span><span class="sxs-lookup"><span data-stu-id="3dc8b-211">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=subject%20eq%20%27welcome to exchange unified messaging%27%20and%20importance%20eq%20%27normal%27%20&$orderby=subject,importance,receivedDateTime%20desc&method=GET&version=v1.0)

 > <span data-ttu-id="3dc8b-212">**注意：**使用从 [directoryObject](../api-reference/v1.0/resources/directoryobject.md) 派生的 Azure AD 资源（如 [user](../api-reference/v1.0/resources/user.md) 和 [group](../api-reference/v1.0/resources/group.md)），则不能合并 `$orderby` 与 `$filter` 表达式。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-212">**Note:** With Azure AD resources that derive from [directoryObject](../api-reference/v1.0/resources/directoryobject.md), like [user](../api-reference/v1.0/resources/user.md) and [group](../api-reference/v1.0/resources/group.md), you cannot combine `$orderby` with `$filter` expressions.</span></span> 

## <a name="search-parameter"></a><span data-ttu-id="3dc8b-213">search 参数</span><span class="sxs-lookup"><span data-stu-id="3dc8b-213">search parameter</span></span>

<span data-ttu-id="3dc8b-214">使用 `$search` 查询参数限制与搜索条件匹配的请求结果。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-214">Use the `$search` query parameter to restrict the results of a request to match a search criterion.</span></span>

> <span data-ttu-id="3dc8b-p118">**注意：**目前**只**能搜索 [message](../api-reference/v1.0/resources/message.md) 和 [person](../api-reference/v1.0/resources/person.md) 集合。`$search` 请求最多可返回 250 个结果。不能在搜索请求中使用 [`$filter`](#filter-parameter) 或 [`$orderby`](#orderby-parameter)。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-p118">**Note:** You can currently search **only** [message](../api-reference/v1.0/resources/message.md) and [person](../api-reference/v1.0/resources/person.md) collections. A `$search` request returns up to 250 results. You cannot use [`$filter`](#filter-parameter) or [`$orderby`](#orderby-parameter) in a search request.</span></span>

### <a name="using-search-on-message-collections"></a><span data-ttu-id="3dc8b-218">对 message 集合使用 $search</span><span class="sxs-lookup"><span data-stu-id="3dc8b-218">Using $search on  collections</span></span>

<span data-ttu-id="3dc8b-219">Office 365 应用（如 Outlook 和 SharePoint）支持使用关键字查询语言 (KQL) 语法执行搜索。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-219">Office 365 applications, such as Outlook and SharePoint, support the Keyword Query Language (KQL) syntax to do searches.</span></span> <span data-ttu-id="3dc8b-220">这就方便常见发现域使用数据存储。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-220">This provides the convenience of a common discovery domain for their data stores.</span></span> 

<span data-ttu-id="3dc8b-221">搜索 message 集合时，结果按邮件发送日期和时间进行排序。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-221">When you search message collections, the results are sorted by the date and time that the message was sent.</span></span> 

<span data-ttu-id="3dc8b-222">可以在 `$search` 条件中对 **message** 指定下列属性：</span><span class="sxs-lookup"><span data-stu-id="3dc8b-222">You can specify the following properties on a **** in a `$search` criterion:</span></span>

- <span data-ttu-id="3dc8b-223">**attachments**</span><span class="sxs-lookup"><span data-stu-id="3dc8b-223">**attachments**</span></span>
- <span data-ttu-id="3dc8b-224">**bccRecipients**</span><span class="sxs-lookup"><span data-stu-id="3dc8b-224">**bccRecipients**</span></span>
- <span data-ttu-id="3dc8b-225">**body**</span><span class="sxs-lookup"><span data-stu-id="3dc8b-225">**body**</span></span>
- <span data-ttu-id="3dc8b-226">**category**</span><span class="sxs-lookup"><span data-stu-id="3dc8b-226">**Category**</span></span>
- <span data-ttu-id="3dc8b-227">**ccRecipients**</span><span class="sxs-lookup"><span data-stu-id="3dc8b-227">**ccRecipients**</span></span>
- <span data-ttu-id="3dc8b-228">**content**</span><span class="sxs-lookup"><span data-stu-id="3dc8b-228">**content**</span></span>
- <span data-ttu-id="3dc8b-229">**from**</span><span class="sxs-lookup"><span data-stu-id="3dc8b-229">**from**</span></span>
- <span data-ttu-id="3dc8b-230">**hasAttachments**</span><span class="sxs-lookup"><span data-stu-id="3dc8b-230">**hasAttachments**</span></span>
- <span data-ttu-id="3dc8b-231">**participants**</span><span class="sxs-lookup"><span data-stu-id="3dc8b-231">**participants**</span></span>
- <span data-ttu-id="3dc8b-232">**receivedDateTime**</span><span class="sxs-lookup"><span data-stu-id="3dc8b-232">**receivedDateTime**</span></span>
- <span data-ttu-id="3dc8b-233">**sender**</span><span class="sxs-lookup"><span data-stu-id="3dc8b-233">**sender**</span></span>
- <span data-ttu-id="3dc8b-234">**subject**</span><span class="sxs-lookup"><span data-stu-id="3dc8b-234">**subject**</span></span>
- <span data-ttu-id="3dc8b-235">**toRecipients**</span><span class="sxs-lookup"><span data-stu-id="3dc8b-235">**toRecipients**</span></span>

<span data-ttu-id="3dc8b-236">如果搜索邮件且仅指定值，将根据默认搜索属性 **from**、**subject** 和 **body** 进行搜索。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-236">If you do a search on messages and specify only a value, the search is carried out on the default search properties of **from**, **subject** and **body**.</span></span>

<span data-ttu-id="3dc8b-237">下面的示例返回登录用户收件箱中在三个默认搜索属性的任意一个中包含“pizza”的所有邮件：</span><span class="sxs-lookup"><span data-stu-id="3dc8b-237">The following example returns all messages in the signed-in user's Inbox that contains "pizza" in any of the three default search properties:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="pizza"
```

<span data-ttu-id="3dc8b-238">[在 Graph 浏览器中试用][search-example]</span><span class="sxs-lookup"><span data-stu-id="3dc8b-238">[Try in Graph Explorer][search-example]</span></span>

<span data-ttu-id="3dc8b-239">下一个示例在用户收件箱中搜索从指定电子邮件地址发送的所有邮件：</span><span class="sxs-lookup"><span data-stu-id="3dc8b-239">The next example searches all messages in the user's Inbox that were sent from a specific email address:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="from:help@contoso.com"
```
<span data-ttu-id="3dc8b-240">若要详细了解 KQL（如语法、支持的运算符和搜索提示），请参阅以下文章：</span><span class="sxs-lookup"><span data-stu-id="3dc8b-240">For more information about KQL such as the syntax, supported operators, and tips on searching, see the following articles:</span></span>

- [<span data-ttu-id="3dc8b-241">关键字查询语言 (KQL) 语法参考</span><span class="sxs-lookup"><span data-stu-id="3dc8b-241">Keyword Query Language (KQL) syntax reference</span></span>](https://docs.microsoft.com/zh-CN/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference)

- <span data-ttu-id="3dc8b-242">
  [Exchange 2016 中的就地电子数据展示的邮件属性和搜索运算符](https://technet.microsoft.com/en-us/library/dn774955(v=exchg.160).aspx)</span><span class="sxs-lookup"><span data-stu-id="3dc8b-242">[Message properties and search operators for In-Place eDiscovery in Exchange 2016](https://technet.microsoft.com/en-us/library/dn774955(v=exchg.160).aspx)</span></span>

### <a name="using-search-on-person-collections"></a><span data-ttu-id="3dc8b-243">对 person 集合使用 $search</span><span class="sxs-lookup"><span data-stu-id="3dc8b-243">Using $search on  collections</span></span>

<span data-ttu-id="3dc8b-p120">可以使用 Microsoft Graph People API 检索与用户相关度最高的人员。相关性由用户的通信和协作模式及业务关系决定。People API 支持 `$search` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-p120">You can use the Microsoft Graph People API to retrieve the people who are most relevant to a user. Relevance is determined by the user’s communication and collaboration patterns and business relationships. The People API supports the `$search` query parameter.</span></span>

<span data-ttu-id="3dc8b-247">人员搜索就是按 [person](../api-reference/v1.0/resources/person.md) 资源的 **displayName** 和 **emailAddress** 属性进行搜索。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-247">Searches on people occur on both the **displayName** and **emailAddress** properties of the [person](../api-reference/v1.0/resources/person.md) resource.</span></span> <span data-ttu-id="3dc8b-248">搜索实现模糊匹配算法。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-248">Searches implement a fuzzy matching algorithm.</span></span> <span data-ttu-id="3dc8b-249">它们根据完全匹配以及搜索意图推断返回结果。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-249">They will return results based on an exact match and also on inferences about the intent of the search.</span></span> <span data-ttu-id="3dc8b-250">例如，假设用户显示名称为“Tyler Lee”，电子邮件地址为 tylerle@example.com，用户位于登录用户的 **people** 集合中。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-250">For example, imagine a user with a display name of "Tyler Lee" and an email address of tylerle@example.com who is in the **people** collection of the signed-in user.</span></span> <span data-ttu-id="3dc8b-251">所有以下搜索将返回包含 Tyler 的结果。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-251">All of the following searches will return results that contain Tyler.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people?$search=tyler                //matches both Tyler's name and email
GET https://graph.microsoft.com/v1.0/me/people?$search=tylerle              //matches Tyler's email
GET https://graph.microsoft.com/v1.0/me/people?$search="tylerle@example.com"  //matches Tyler's email. Note the quotes to enclose '@'.
GET https://graph.microsoft.com/v1.0/me/people?$search=tiler                //fuzzy match with Tyler's name 
GET https://graph.microsoft.com/v1.0/me/people?$search="tyler lee"          //matches Tyler's name. Note the quotes to enclose the space.
```

<span data-ttu-id="3dc8b-p122">还可以搜索对特定主题感兴趣的人员。基于从用户的邮件对话派生的推断来执行搜索。例如，以下搜索将返回与登录用户相关的人员集合，在与该用户进行通信时，他表现出了对披萨的兴趣。请注意，搜索短语用引号括起来。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-p122">You can also perform searches for people who are interested in a particular topic. Searches are performed based on inferences derived from the user's mail conversations. For example, the following search will return a collection of people relevant to the signed-in user who have expressed an interest in pizza in communications with that user. Note that the search phrase is enclosed in quotes.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="topic:pizza"                
```

<span data-ttu-id="3dc8b-256">最后，可以通过组合两种类型的搜索表达式，在同一请求中合并人员搜索和主题搜索。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-256">Finally, you can combine both people searches and topic searches in the same request by combining the two types of search expression.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="tyl topic:pizza"                
```

<span data-ttu-id="3dc8b-257">此请求主要进行两次搜索：对登录用户的相关人员的 **displayName** 和 **emailAddress** 属性进行模糊搜索，以及对用户的相关人员进行“pizza”主题搜索。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-257">This request essentially conducts two searches: a fuzzy search against **** and **** properties of the signed-in user's relevant people, and a topic search for "pizza" against the user's relevant people.</span></span> <span data-ttu-id="3dc8b-258">然后，对结果进行排名、排序并返回。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-258">The results are then ranked, ordered, and returned.</span></span> <span data-ttu-id="3dc8b-259">请注意，该搜索没有限制；可能会得到包含模糊匹配“tyl”的人员的结果和/或对“披萨”感兴趣的人员的结果。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-259">Note that the search is not restrictive; you might get results that contain people that fuzzy match "tyl", or that are interested in "pizza", or both.</span></span>

<span data-ttu-id="3dc8b-260">若要了解有关 People API 的详细信息，请参阅[获取相关人员的信息](./people_example.md)。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-260">To learn more about the People API, see [Get information about relevant people](./people_example.md).</span></span>  

## <a name="select-parameter"></a><span data-ttu-id="3dc8b-261">select 参数</span><span class="sxs-lookup"><span data-stu-id="3dc8b-261">select parameter</span></span>

<span data-ttu-id="3dc8b-262">使用 `$select` 查询参数返回一组不同于单个资源的默认集或资源集合的属性。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-262">Use the `$select` query parameter to return a set of properties that are different than the default set for an individual resource or a collection of resources.</span></span> <span data-ttu-id="3dc8b-263">使用 $select，可以指定默认属性的子集或超集。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-263">With $select, you can specify a subset or a superset of the default properties.</span></span>

<span data-ttu-id="3dc8b-264">例如，检索登录用户的邮件时，可以指定仅返回 **from** 和 **subject** 属性：</span><span class="sxs-lookup"><span data-stu-id="3dc8b-264">For example, when retrieving the messages of the signed-in user, you can specify that only the **** and **** properties be returned:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$select=from,subject
```

<span data-ttu-id="3dc8b-265">[在 Graph 浏览器中试用][select-example]</span><span class="sxs-lookup"><span data-stu-id="3dc8b-265">[Try in Graph Explorer][select-example]</span></span>

> <span data-ttu-id="3dc8b-266">**重要说明：**一般来说，建议使用 `$select` 将查询返回的属性限制为应用所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-266">**Important:** In general, we recommend that you use `$select` to limit the properties returned by a query to those needed by your app.</span></span> <span data-ttu-id="3dc8b-267">这对于可能返回大型结果集的查询尤为有用。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-267">This is especially true of queries that might potentially return a large result set.</span></span> <span data-ttu-id="3dc8b-268">限制每行返回的属性将减少网络负载并帮助提升应用的性能。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-268">Limiting the properties returned in each row will reduce network load and help improve your app's performance.</span></span>
>
> <span data-ttu-id="3dc8b-p126">在 `v1.0` 中，从 [directoryObject](../api-reference/v1.0/resources/directoryobject.md) 派生的一些 Azure AD 资源（如 [user](../api-reference/v1.0/resources/user.md) 和 [group](../api-reference/v1.0/resources/group.md)）在读取时返回受限的默认属性子集。对于这些资源，必须使用 `$select` 将属性返回到默认集之外。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-p126">In `v1.0`, some Azure AD resources that derive from [directoryObject](../api-reference/v1.0/resources/directoryobject.md), like [user](../api-reference/v1.0/resources/user.md) and [group](../api-reference/v1.0/resources/group.md), return a limited, default subset of properties on reads. For these resources, you must use `$select` to return properties outside of the default set.</span></span>  

## <a name="skip-parameter"></a><span data-ttu-id="3dc8b-271">skip 参数</span><span class="sxs-lookup"><span data-stu-id="3dc8b-271">skip parameter</span></span>

<span data-ttu-id="3dc8b-p127">使用 `$skip` 查询参数设置要在集合开头跳过的项数。例如，以下请求返回按照创建日期排序的用户的事件，从集合中的第 21 个事件开始：</span><span class="sxs-lookup"><span data-stu-id="3dc8b-p127">Use the `$skip` query parameter to set the number of items to skip at the start of a collection. For example, the following request returns events for the user sorted by date created, starting with the 21st event in the collection:</span></span>

```http
GET  https://graph.microsoft.com/v1.0/me/events?$orderby=createdDateTime&$skip=20
```
<span data-ttu-id="3dc8b-274">[在 Graph 浏览器中试用][skip-example]</span><span class="sxs-lookup"><span data-stu-id="3dc8b-274">[Try in Graph Explorer][skip-example]</span></span>

> <span data-ttu-id="3dc8b-275">**注意：**一些 Microsoft Graph API 使用 `$skip` 实现分页，如 Outlook 邮件和日历（**message**、**event** 和 **calendar**）。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-275">**Note:** Some Microsoft Graph APIs, like Outlook Mail and Calendars (****, ****, and ****), use `$skip` to implement paging.</span></span> <span data-ttu-id="3dc8b-276">当查询结果跨多个页面时，这些 API 会返回 `@odata:nextLink` 属性，具有包含 `$skip` 参数的 URL。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-276">When results of a query span multiple pages, these APIs will return an `@odata:nextLink` property with a URL that contains a `$skip` parameter.</span></span> <span data-ttu-id="3dc8b-277">可以使用此 URL 返回下一页结果。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-277">You can use this URL to return the next page of results.</span></span> <span data-ttu-id="3dc8b-278">若要了解详细信息，请参阅[分页](./paging.md)。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-278">To learn more, see [Paging](./paging.md).</span></span>

## <a name="skiptoken-parameter"></a><span data-ttu-id="3dc8b-279">skipToken 参数</span><span class="sxs-lookup"><span data-stu-id="3dc8b-279">skipToken parameter</span></span>

<span data-ttu-id="3dc8b-p129">由于服务器端分页或由于使用 [`$top`](#top-parameter) 参数来限制响应的页面大小，致使一些请求返回多页数据。许多 Microsoft Graph API 使用 `skipToken` 查询参数来引用结果的后续页面。`$skiptoken` 参数包含引用下一页结果的不透明令牌，并在响应的 `@odata.nextLink` 属性中提供的 URL 中返回。若要了解详细信息，请参阅[分页](./paging.md)。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-p129">Some requests return multiple pages of data either due to server-side paging or due to the use of the [`$top`](#top-parameter) parameter to limit the page size of the response. Many Microsoft Graph APIs use the `skipToken` query parameter to reference subsequent pages of the result. The `$skiptoken` parameter contains an opaque token that references the next page of results and is returned in the URL provided in the `@odata.nextLink` property in the response. To learn more, see [Paging](./paging.md).</span></span>


## <a name="top-parameter"></a><span data-ttu-id="3dc8b-284">top 参数</span><span class="sxs-lookup"><span data-stu-id="3dc8b-284">top parameter</span></span>

<span data-ttu-id="3dc8b-285">使用 `$top` 查询参数指定结果集的页面大小。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-285">Use the `$top` query parameter to specify the page size of the result set.</span></span> 

<span data-ttu-id="3dc8b-286">如果结果集中还剩余多个项目，则响应正文将包含 `@odata.nextLink` 参数。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-286">If more items remain in the result set, the response body will contain an `@odata.nextLink` parameter.</span></span> <span data-ttu-id="3dc8b-287">此参数包含可用于获取下一页结果的 URL。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-287">This parameter contains a URL that you can use to get the next page of results.</span></span> <span data-ttu-id="3dc8b-288">若要了解详细信息，请参阅[分页](./paging.md)。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-288">To learn more, see [Paging](./paging.md).</span></span> 

<span data-ttu-id="3dc8b-289">例如，以下请求返回用户邮箱中的前 5 封邮件：</span><span class="sxs-lookup"><span data-stu-id="3dc8b-289">For example, the following request returns the first five messages in the user's mailbox:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$top=5
```

<span data-ttu-id="3dc8b-290">[在 Graph 浏览器中试用][top-example]</span><span class="sxs-lookup"><span data-stu-id="3dc8b-290">[Try in Graph Explorer][top-example]</span></span>


## <a name="error-handling-for-query-parameters"></a><span data-ttu-id="3dc8b-291">查询参数的错误处理</span><span class="sxs-lookup"><span data-stu-id="3dc8b-291">Error handling for query parameters</span></span>

<span data-ttu-id="3dc8b-p131">如果不支持指定的查询参数，某些请求将返回错误消息。例如，不能对 `user/photo` 关系使用 `$expand`。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-p131">Some requests will return an error message if a specified query parameter is not supported. For example, you cannot use `$expand` on the `user/photo` relationship.</span></span> 

```http
https://graph.microsoft.com/beta/me?$expand=photo
```

```json
{
    "error":{
        "code":"ExpandNotSupported",
        "message":"Expand is not allowed for property 'Photo' according to the entity schema.",
        "innerError":{
            "request-id":"1653fefd-bc31-484b-bb10-8dc33cb853ec",
            "date":"2017-07-31T20:55:01"
        }
    }
}
```

<span data-ttu-id="3dc8b-294">但是，值得注意的是请求中指定的查询参数可能会自行失败。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-294">However, it is important to note that query parameters specified in a request might fail silently.</span></span> <span data-ttu-id="3dc8b-295">不支持的查询参数以及不支持的查询参数组合的情况就是如此。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-295">This can be true for unsupported query parameters as well as for unsupported combinations of query parameters.</span></span> <span data-ttu-id="3dc8b-296">在这些情况下，应检查请求返回的数据，以确定指定的查询参数是否具有所需的效果。</span><span class="sxs-lookup"><span data-stu-id="3dc8b-296">In these cases, you should examine the data returned by the request to determine whether the query parameters you specified had the desired effect.</span></span> 

[graph-explorer]: https://developer.microsoft.com/graph/graph-explorer
[odata-filter]: http://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752358
[odata-query]: http://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752356
[count-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$top=2%26$count=true&method=GET&version=v1.0
[expand-example]: https://developer.microsoft.com/graph/graph-explorer?request=groups$expand=members&method=GET&version=v1.0
[filter-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(givenName,'J')&method=GET&version=v1.0
[format-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$format=json&method=GET&version=v1.0
[orderby-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$orderby=displayName%20DESC&method=GET&version=v1.0
[search-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=pizza&method=GET&version=v1.0
[select-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$select=givenName,surname&method=GET&version=v1.0
[skip-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$skip=11&method=GET&version=v1.0
[top-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$top=2&method=GET&version=v1.0


