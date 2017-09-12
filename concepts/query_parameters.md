# <a name="use-query-parameters-to-customize-responses"></a><span data-ttu-id="2ff29-101">使用查询参数自定义响应</span><span class="sxs-lookup"><span data-stu-id="2ff29-101">Use query parameters to customize responses</span></span>

<span data-ttu-id="2ff29-p101">Microsoft Graph 提供可选的查询参数，可用于指定和控制响应中返回的数据量。支持以下查询参数。</span><span class="sxs-lookup"><span data-stu-id="2ff29-p101">Microsoft Graph provides optional query parameters that you can use to specify and control the amount of data returned in a response. The following following query parameters are supported.</span></span>

|<span data-ttu-id="2ff29-104">名称</span><span class="sxs-lookup"><span data-stu-id="2ff29-104">Name</span></span>|<span data-ttu-id="2ff29-105">说明</span><span class="sxs-lookup"><span data-stu-id="2ff29-105">Description</span></span>|<span data-ttu-id="2ff29-106">示例（单击示例可在 [Graph 浏览器][graph-explorer]中试调用）</span><span class="sxs-lookup"><span data-stu-id="2ff29-106">Example (click examples to try in [Graph Explorer][graph-explorer])</span></span>
|:---------------|:--------|:-------|
|[<span data-ttu-id="2ff29-107">$count</span><span class="sxs-lookup"><span data-stu-id="2ff29-107">$count</span></span>](#count)|<span data-ttu-id="2ff29-108">检索匹配资源的总数。</span><span class="sxs-lookup"><span data-stu-id="2ff29-108">Retrieves the total count of matching resources.</span></span>|[`/me/messages?$top=2&$count=true`](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$top=2%26$count=true&method=GET&version=v1.0)
|[<span data-ttu-id="2ff29-109">$expand</span><span class="sxs-lookup"><span data-stu-id="2ff29-109">$expand</span></span>](#expand)|<span data-ttu-id="2ff29-110">检索相关资源。</span><span class="sxs-lookup"><span data-stu-id="2ff29-110">Retrieves related resources.</span></span>|[`/groups?$expand=members`](https://developer.microsoft.com/graph/graph-explorer?request=groups$expand=members&method=GET&version=v1.0)
|[<span data-ttu-id="2ff29-111">$filter</span><span class="sxs-lookup"><span data-stu-id="2ff29-111">$filter</span></span>](#filter)|<span data-ttu-id="2ff29-112">筛选结果（行）。</span><span class="sxs-lookup"><span data-stu-id="2ff29-112">Filters results (rows).</span></span>|[`/users?$filter=startswith(givenName,'J')`](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(givenName,'J')&method=GET&version=v1.0)
|[<span data-ttu-id="2ff29-113">$orderby</span><span class="sxs-lookup"><span data-stu-id="2ff29-113">$orderby</span></span>](#orderby)|<span data-ttu-id="2ff29-114">对结果进行排序。</span><span class="sxs-lookup"><span data-stu-id="2ff29-114">Orders results.</span></span>|[`/users?$orderby=displayName desc`](https://developer.microsoft.com/graph/graph-explorer?request=users?$orderby=displayName%20DESC&method=GET&version=v1.0)
|[<span data-ttu-id="2ff29-115">$search</span><span class="sxs-lookup"><span data-stu-id="2ff29-115">Search</span></span>](#search)| <span data-ttu-id="2ff29-p102">返回基于搜索条件的结果。目前在 `messages` 和 `person` 集合上受到支持。</span><span class="sxs-lookup"><span data-stu-id="2ff29-p102">Returns results based on search criteria. Currently supported on `messages` and `person` collections.</span></span>|[`/me/messages?$search=pizza`](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=pizza&method=GET&version=v1.0)
|[<span data-ttu-id="2ff29-118">$select</span><span class="sxs-lookup"><span data-stu-id="2ff29-118">$select</span></span>](#select)|<span data-ttu-id="2ff29-119">筛选属性（列）。</span><span class="sxs-lookup"><span data-stu-id="2ff29-119">Filters properties (columns).</span></span>|[`/users?$select=givenName,surname`](https://developer.microsoft.com/graph/graph-explorer?request=users?$select=givenName,surname&method=GET&version=v1.0)
|[<span data-ttu-id="2ff29-120">$skip</span><span class="sxs-lookup"><span data-stu-id="2ff29-120">$skip</span></span>](#skip)|<span data-ttu-id="2ff29-p103">对结果集建立索引。一些 API 也使用它来实现分页，并且可以与 `$top` 一起使用来手动对结果分页。</span><span class="sxs-lookup"><span data-stu-id="2ff29-p103">Indexes into a result set. Also used by some APIs to implement paging and can be used together with `$top` to manually page results.</span></span>  | [`/me/messages?$skip=11`](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$skip=11&method=GET&version=v1.0)
|[<span data-ttu-id="2ff29-123">$skipToken</span><span class="sxs-lookup"><span data-stu-id="2ff29-123">$skipToken</span></span>](#skiptoken)|<span data-ttu-id="2ff29-p104">从跨多页的结果集中检索下一页结果。（但某些 API 改为使用 `$skip`。）</span><span class="sxs-lookup"><span data-stu-id="2ff29-p104">Retrieves the next page of results from result sets that span multiple pages. (Some APIs use `$skip` instead.)</span></span> | `https://graph.microsoft.com/v1.0/users?$skiptoken=X%274453707402000100000017 ... 65612D643839392D343230372D613033662D306332623836633432363932B900000000000000000000%27`
|[<span data-ttu-id="2ff29-126">$top</span><span class="sxs-lookup"><span data-stu-id="2ff29-126">$top</span></span>](#top)|<span data-ttu-id="2ff29-127">设置结果的页面大小。</span><span class="sxs-lookup"><span data-stu-id="2ff29-127">Sets the page size of results.</span></span> |[`/users?$top=2`](https://developer.microsoft.com/graph/graph-explorer?request=users?$top=2&method=GET&version=v1.0)

<span data-ttu-id="2ff29-p105">这些参数与 [OData V4 查询语言][odata-query]兼容。并非所有的 Microsoft Graph API 都支持所有参数，而对 `v1.0` 和 `beta` 终结点的支持可能会显著不同。</span><span class="sxs-lookup"><span data-stu-id="2ff29-p105">These parameters are compatible with the [OData V4 query language][odata-query]. Not all parameters are supported across all Microsoft Graph APIs and support may differ significantly between the `v1.0` and `beta` endpoints.</span></span> 

> <span data-ttu-id="2ff29-p106">**注意：**在 `beta` 终结点上，`$` 前缀是可选的。例如，可使用 `filter` 来代替 `$filter`。有关更多详细信息和示例，请参阅 [Microsoft Graph 中支持不含 $ 前缀的查询参数](http://dev.office.com/queryparametersinMicrosoftGraph)。</span><span class="sxs-lookup"><span data-stu-id="2ff29-p106">**Note:** On the `beta` endpoint, the `$` prefix is optional. For example, instead of `$filter`, you can use `filter`. For more details and examples, see [Supporting query parameters without $ prefixes in Microsoft Graph](http://dev.office.com/queryparametersinMicrosoftGraph).</span></span>

<span data-ttu-id="2ff29-133">**编码查询参数：**</span><span class="sxs-lookup"><span data-stu-id="2ff29-133">**Encoding query parameters:**</span></span>

<span data-ttu-id="2ff29-p107">应对查询参数的值进行百分比编码。许多 HTTP 客户端、浏览器和工具（例如，[Graph 浏览器][graph-explorer]）都可以帮助你完成此操作。如果查询失败，可能原因之一是未正确编码查询参数的值。</span><span class="sxs-lookup"><span data-stu-id="2ff29-p107">The values of query parameters should be percent-encoded. Many HTTP clients, browsers and tools (e.g., the [Graph Explorer][graph-explorer]) will help you with this. If a query is failing, one possible reason is failure to encode the values of query parameters appropriately.</span></span>

<span data-ttu-id="2ff29-137">未编码的 URL 如下所示：</span><span class="sxs-lookup"><span data-stu-id="2ff29-137">An unencoded URL looks like this:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName, 'J')
```

<span data-ttu-id="2ff29-138">正确解码的 URL 如下所示：</span><span class="sxs-lookup"><span data-stu-id="2ff29-138">A properly encoded URL looks like this:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName%2C+'J')
```

## <a name="count"></a><span data-ttu-id="2ff29-139">count</span><span class="sxs-lookup"><span data-stu-id="2ff29-139">count</span></span>

<span data-ttu-id="2ff29-140">使用 `$count` 查询参数以包括集合中项总数的计数，以及从 Microsoft Graph 返回的数据值页。</span><span class="sxs-lookup"><span data-stu-id="2ff29-140">Use `$count` as a query parameter to include a count of the total number of items in a collection alongside the page of data values returned from the Graph, as in the following example:</span></span> 

<span data-ttu-id="2ff29-141">例如，以下请求将返回当前用户的 `contacts` 集合以及 `@odata.count` 属性的 `contacts` 集合中的项目数。</span><span class="sxs-lookup"><span data-stu-id="2ff29-141">For example, the following request will return both the `contacts` collection of the current user, and the number of items in the `contacts` collection in the `@odata.count` property.</span></span>

```http
GET  https://graph.microsoft.com/v1.0/me/contacts?$count=true
```

[<span data-ttu-id="2ff29-142">在 Graph 浏览器中试调用</span><span class="sxs-lookup"><span data-stu-id="2ff29-142">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/contacts?$count=true&method=GET&version=v1.0)


><span data-ttu-id="2ff29-143">**注意：**派生自 [`directoryObject`](../api-reference/v1.0/resources/directoryobject.md) 的资源集合（如 [user](../api-reference/v1.0/resources/user.md) 或 [group](../api-reference/v1.0/resources/group.md) 集合）不支持 `$count`。</span><span class="sxs-lookup"><span data-stu-id="2ff29-143">**Note:** `$count` is not supported for collections of resources that derive from [`directoryObject`](../api-reference/v1.0/resources/directoryobject.md) like collections of [user](../api-reference/v1.0/resources/user.md) or [group](../api-reference/v1.0/resources/group.md).</span></span>

## <a name="expand"></a><span data-ttu-id="2ff29-144">expand</span><span class="sxs-lookup"><span data-stu-id="2ff29-144">expand</span></span>

<span data-ttu-id="2ff29-p108">许多 Microsoft Graph 资源都会暴露资源的声明属性以及其与其他资源的关系。这些关系也称为引用属性或导航属性，它们可以引用单个资源或资源集合。例如，用户的邮件文件夹、管理者和直接下属都将作为关系公开。</span><span class="sxs-lookup"><span data-stu-id="2ff29-p108">Many Microsoft Graph resources expose both declared properties of the resource as well as its relationships with other resources. These relationships are also called reference properties or navigation properties and they can reference either a single resource or a collection of resources. For example, the mail folders, manager, and direct reports of a user are all exposed as relationships.</span></span> 

<span data-ttu-id="2ff29-p109">通常情况下，可以在单个请求中查询资源属性或其关系之一，但不能同时查询。可以使用 `$expand` 查询字符串参数以包含结果中单个关系（导航属性）引用的扩展资源或集合。</span><span class="sxs-lookup"><span data-stu-id="2ff29-p109">Normally, you can query either the properties of a resource or one of its relationships in a single request, but not both. You can use the `$expand` query string parameter to include the expanded resource or collection referenced by a single relationship (navigation property) in your results.</span></span>

<span data-ttu-id="2ff29-150">以下示例在驱动器中获取根驱动器信息以及顶级子项：</span><span class="sxs-lookup"><span data-stu-id="2ff29-150">The following example gets root drive information along with the top level child items in a drive:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children
```

[<span data-ttu-id="2ff29-151">在 Graph 浏览器中试调用</span><span class="sxs-lookup"><span data-stu-id="2ff29-151">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/drive/root?$expand=children&method=GET&version=v1.0)

<span data-ttu-id="2ff29-p110">使用某些资源集合，还可以通过添加 `$select` 参数来指定要在扩展资源中返回的属性。以下示例执行与上一示例相同的查询，但使用 [`$select`](#select) 语句将为扩展子项返回的属性限制为 `id` 和 `name` 属性。</span><span class="sxs-lookup"><span data-stu-id="2ff29-p110">With some resource collections, you can also specify the properties to be returned in the expanded resources by adding a `$select` parameter. The following example performs the same query as the previous example but uses a [`$select`](#select) statement to limit the properties returned for the expanded child items to the `id` and `name` properties.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children($select=id,name)
```

<span data-ttu-id="2ff29-154">[在 Graph 浏览器中试调用](https://developer.microsoft.com/graph/graph-explorer?request=me/drive/root?$expand=children($select=id,name)&method=GET&version=v1.0)</span><span class="sxs-lookup"><span data-stu-id="2ff29-154">[Try in Graph Explorer](https://developer.microsoft.com/graph/graph-explorer?request=me/drive/root?$expand=children($select=id,name)&method=GET&version=v1.0)</span></span>

> <span data-ttu-id="2ff29-p111">**注意：**并不是所有关系和资源都支持 `$expand` 查询参数。例如，可以扩展用户的 `directReports`、`manager` 和 `memberOf` 关系，但无法扩展其 `events`、`messages` 或 `photo` 关系。并非所有资源或关系都支持在扩展项上使用 `$select`。</span><span class="sxs-lookup"><span data-stu-id="2ff29-p111">**Note:** Not all relationships and resources support the `$expand` query parameter. For example, you can expand the `directReports`, `manager`, and `memberOf` relationships on a user, but you cannot expand its `events`, `messages`, or `photo` relationships. Not all resources or relationships support using `$select` on expanded items.</span></span> 
> 
> <span data-ttu-id="2ff29-158">使用从 [directoryObject](../api-reference/v1.0/resources/directoryobject.md) 派生的 Azure AD 资源（如[user](../api-reference/v1.0/resources/user.md) 和 [group](../api-reference/v1.0/resources/group.md)），`$expand` 仅支持 `beta`，并且通常最多为扩展关系返回 20 个项。</span><span class="sxs-lookup"><span data-stu-id="2ff29-158">With Azure AD resources that derive from [directoryObject](../api-reference/v1.0/resources/directoryobject.md), like [user](../api-reference/v1.0/resources/user.md) and [group](../api-reference/v1.0/resources/group.md), `$expand` is only supported for `beta` and  typically returns a maximum of 20 items for the expanded relationship.</span></span>

## <a name="filter"></a><span data-ttu-id="2ff29-159">筛选器</span><span class="sxs-lookup"><span data-stu-id="2ff29-159">filter</span></span>

<span data-ttu-id="2ff29-160">使用 `$filter` 查询参数，以仅检索集合的子集。</span><span class="sxs-lookup"><span data-stu-id="2ff29-160">Use the `$filter` query parameter to retrieve just a subset of a collection.</span></span> 

<span data-ttu-id="2ff29-161">例如，若要查找显示名称以子母“J”开头的用户，请使用 `startswith`。</span><span class="sxs-lookup"><span data-stu-id="2ff29-161">For example, to find users whose display name starts with the letter 'J', use `startswith`.</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'J')
```

<span data-ttu-id="2ff29-162">[在 Graph 浏览器中试调用](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(givenName,'J')&method=GET&version=v1.0)</span><span class="sxs-lookup"><span data-stu-id="2ff29-162">[Try in Graph Explorer](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(givenName,'J')&method=GET&version=v1.0)</span></span>

<span data-ttu-id="2ff29-p112">对 `$filter` 运算符的支持因 Microsoft Graph API 不同而异。通常支持下列逻辑运算符：等于 (`eq`)、不等于 (`ne`)、大于 (`gt`)、大于或等于 (`ge`)、小于 (`lt`)、小于或等于 (`le`)、和 (`and`)、或 (`or`) 以及非 (`not`)。通常支持 `startswith` 字符串运算符。某些 API 支持 `any` lambda 运算符。有关一些用法示例的信息，请参阅下表。有关 `$filter` 语法的其他详细信息，请参阅 [OData 协议][odata-filter]。</span><span class="sxs-lookup"><span data-stu-id="2ff29-p112">Support for `$filter` operators varies across Microsoft Graph APIs. The following logical operators are generally supported: equals (`eq`), not equals (`ne`), greater than (`gt`), greater than or equals (`ge`), less than (`lt`), less than or equals (`le`), and (`and`), or (`or`), and not (`not`). The `startswith` string operator is often supported. The `any` lambda operator is supported for some APIs. For some  usage examples, see the table below. For additional details on `$filter` syntax, see the [OData protocol][odata-filter].</span></span>  

<span data-ttu-id="2ff29-169">下表显示使用 `$filter` 查询参数的一些示例。</span><span class="sxs-lookup"><span data-stu-id="2ff29-169">The following table shows some examples using the `$filter` query parameter.</span></span>

|<span data-ttu-id="2ff29-170">说明</span><span class="sxs-lookup"><span data-stu-id="2ff29-170">Description</span></span>|<span data-ttu-id="2ff29-171">示例（单击示例可在 [Graph 浏览器][graph-explorer]中试调用）</span><span class="sxs-lookup"><span data-stu-id="2ff29-171">Example (click examples to try in [Graph Explorer][graph-explorer])</span></span>|
|:--------|:-------|
|  <span data-ttu-id="2ff29-172">跨多个属性搜索名为 Mary 的用户。</span><span class="sxs-lookup"><span data-stu-id="2ff29-172">Search for users with the name Mary across multiple properties.</span></span> | [`https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'mary') or startswith(givenName,'mary') or startswith(surname,'mary') or startswith(mail,'mary') or startswith(userPrincipalName,'mary')`](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(displayName,'mary')+or+startswith(givenName,'mary')+or+startswith(surname,'mary')+or+startswith(mail,'mary')+or+startswith(userPrincipalName,'mary')&method=GET&version=v1.0) |
| <span data-ttu-id="2ff29-173">获取 2017 年 7 月 1 日之后开始的所有登录用户的事件。</span><span class="sxs-lookup"><span data-stu-id="2ff29-173">Get all of the signed-in user's events that start after 7/1/2017.</span></span> | [`https://graph.microsoft.com/v1.0/me/events?$filter=start/dateTime ge '2017-07-01T08:00'`](https://developer.microsoft.com/graph/graph-explorer?request=me/events?$filter=start/dateTime+ge+'2017-07-01T08:00'&method=GET&version=v1.0) |
| <span data-ttu-id="2ff29-174">获取登录用户收到的来自特定地址的所有电子邮件。</span><span class="sxs-lookup"><span data-stu-id="2ff29-174">Get all emails from a specific address received by the signed-in user.</span></span> | [`https://graph.microsoft.com/v1.0/me/messages?$filter=from/emailAddress/address eq 'someuser@example.com'`](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=from/emailAddress/address+eq+'someuser@.com'&method=GET&version=v1.0) |
| <span data-ttu-id="2ff29-175">获取登录用户在 2017 年 4 月收到的所有电子邮件</span><span class="sxs-lookup"><span data-stu-id="2ff29-175">Get all emails received by the signed-in user in April 2017</span></span> | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=ReceivedDateTime ge 2017-04-01 and receivedDateTime lt 2017-05-01`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=ReceivedDateTime+ge+2017-04-01+and+receivedDateTime+lt+2017-05-01&method=GET&version=v1.0) |
| <span data-ttu-id="2ff29-176">获取登录用户收件箱中的所有未读邮件。</span><span class="sxs-lookup"><span data-stu-id="2ff29-176">Get all unread mails in the signed-in user's Inbox.</span></span> | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=isRead eq false`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=isRead+eq+false&method=GET&version=v1.0) |
| <span data-ttu-id="2ff29-177">列出组织中的所有 Office 365 组</span><span class="sxs-lookup"><span data-stu-id="2ff29-177">List all Office 365 groups in an organization</span></span> | [`https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')`](https://developer.microsoft.com/graph/graph-explorer?request=groups?$filter=groupTypes/any(c:c+eq+'Unified')&method=GET&version=v1.0) |

> <span data-ttu-id="2ff29-p113">**注意：**Azure AD 资源不支持以下 `$filter` 运算符：`ne`、`gt`、`ge`、`lt`、`le` 和 `not`。所有 Microsoft Graph 资源目前均不支持 `contains` 字符串运算符。</span><span class="sxs-lookup"><span data-stu-id="2ff29-p113">**Note:** The following `$filter` operators are not supported for Azure AD resources:  `ne`, `gt`, `ge`, `lt`, `le`, and `not`. The `contains` string operator is currently not supported on any Microsoft Graph resources.</span></span>

## <a name="orderby"></a><span data-ttu-id="2ff29-180">orderby</span><span class="sxs-lookup"><span data-stu-id="2ff29-180">orderby</span></span>

<span data-ttu-id="2ff29-181">使用 `$orderby` 查询参数指定从 Microsoft Graph 返回的项的排序顺序。</span><span class="sxs-lookup"><span data-stu-id="2ff29-181">Use the `$orderby` query parameter to specify the sort order of the items returned from Microsoft Graph.</span></span>

<span data-ttu-id="2ff29-182">例如，以下请求返回按用户显示名称进行排序的组织中的用户：</span><span class="sxs-lookup"><span data-stu-id="2ff29-182">For example, to return the users in the organization ordered by their display name, the syntax is as follows:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$orderby=displayName
```
[<span data-ttu-id="2ff29-183">在 Graph 浏览器中试调用</span><span class="sxs-lookup"><span data-stu-id="2ff29-183">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=users?$orderby=displayName&method=GET&version=v1.0)

<span data-ttu-id="2ff29-p114">还可以按复杂类型实体进行排序。下面的请求获取邮件，然后按 `from` 属性的 `address` 字段（属于复杂类型 `emailAddress`）对这些邮件进行排序：</span><span class="sxs-lookup"><span data-stu-id="2ff29-p114">You can also sort by complex type entities. The following example gets messages and sorts them by the `address` field of the `from` property, which is of the complex type `emailAddress`:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$orderby=from/emailAddress/address
```
[<span data-ttu-id="2ff29-186">在 Graph 浏览器中试调用</span><span class="sxs-lookup"><span data-stu-id="2ff29-186">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/address&method=GET&version=v1.0)

<span data-ttu-id="2ff29-187">若要以升序或降序对结果进行排序，请向字段名称追加 `asc` 或 `desc`，并用空格隔开。例如，`?$orderby=name%20desc`。</span><span class="sxs-lookup"><span data-stu-id="2ff29-187">To sort the results in ascending or descending order, append either `asc` or `desc` to the field name, separated by a space, for example, `?$orderby=name%20desc`.</span></span>

<span data-ttu-id="2ff29-p115">通过一些 API，可以对多个属性的结果进行排序。例如，以下请求首先按发件人名称以降序（Z 到 A）排序用户收件箱中的邮件，然后按主题以升序（默认）排序邮件。</span><span class="sxs-lookup"><span data-stu-id="2ff29-p115">With some APIs, you can order results on multiple properties. For example, the following request orders the messages in the user's Inbox first by the name of the person who sent it in descending order (Z to A) and then by subject in ascending order (default).</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/Inbox/messages?$orderby=from/emailAddress/name desc,subject
```
[<span data-ttu-id="2ff29-190">在 Graph 浏览器中试调用</span><span class="sxs-lookup"><span data-stu-id="2ff29-190">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/name%20desc,subject&method=GET&version=v1.0)


 > <span data-ttu-id="2ff29-191">**注意：**使用从 [directoryObject](../api-reference/v1.0/resources/directoryobject.md) 派生的 Azure AD 资源（如 [user](../api-reference/v1.0/resources/user.md) 和 [group](../api-reference/v1.0/resources/group.md)），则不能合并 `$orderby` 与 `$filter` 表达式。</span><span class="sxs-lookup"><span data-stu-id="2ff29-191">**Note:** With Azure AD resources that derive from [directoryObject](../api-reference/v1.0/resources/directoryobject.md), like [user](../api-reference/v1.0/resources/user.md) and [group](../api-reference/v1.0/resources/group.md), you cannot combine `$orderby` with `$filter` expressions.</span></span> 

## <a name="search"></a><span data-ttu-id="2ff29-192">search</span><span class="sxs-lookup"><span data-stu-id="2ff29-192">search</span></span>

<span data-ttu-id="2ff29-193">使用 `$search` 查询参数限制与搜索条件匹配的请求结果。</span><span class="sxs-lookup"><span data-stu-id="2ff29-193">Use the `$search` query parameter to restrict the results of a request to match a search criterion.</span></span>

> <span data-ttu-id="2ff29-p116">**注意：**目前**只**能搜索 [message](../api-reference/v1.0/resources/message.md) 和 [person](../api-reference/v1.0/resources/person.md) 集合。`$search` 请求最多可返回 250 个结果。不能在搜索请求中使用 [`$filter`](#filter) 或 [`$orderby`](#orderby)。</span><span class="sxs-lookup"><span data-stu-id="2ff29-p116">**Note:** You can currently **only** search [message](../api-reference/v1.0/resources/message.md) and [person](../api-reference/v1.0/resources/person.md) collections. A `$search` request returns up to 250 results. You cannot use [`$filter`](#filter) or [`$orderby`](#orderby) in a search request.</span></span>

### <a name="using-search-on-message-collections"></a><span data-ttu-id="2ff29-197">针对 `message` 集合使用 $search</span><span class="sxs-lookup"><span data-stu-id="2ff29-197">Using $search on `message` collections</span></span>

<span data-ttu-id="2ff29-p117">邮件的搜索条件使用[高级查询语法 (AQS)](https://support.office.com/article/Search-Mail-and-People-in-Outlook-com-and-Outlook-on-the-web-for-business-88108edf-028e-4306-b87e-7400bbb40aa7) 进行表示。结果按邮件发送日期和时间进行排序。</span><span class="sxs-lookup"><span data-stu-id="2ff29-p117">Search criteria are expressed using Advanced Query Syntax (AQS). The results are sorted by the date and time that the message was sent.</span></span>

<span data-ttu-id="2ff29-200">可以在 `$search` 条件中对 `message` 指定下列属性：`attachments`、`bccRecipients`、`body`、`category`、`ccRecipients`、`content`、`from`、`hasAttachments`、`participants`、`receivedDateTime`、`sender`、`subject`、`toRecipients`</span><span class="sxs-lookup"><span data-stu-id="2ff29-200">You can specify the following properties on a `message` in a `$search` criterion: `attachments`, `bccRecipients`, `body`, `category`, `ccRecipients`, `content`, `from`, `hasAttachments`, `participants`, `receivedDateTime`, `sender`, `subject`, `toRecipients`</span></span>

<span data-ttu-id="2ff29-201">如果要搜索邮件并且仅指定了一个值，那么会根据默认搜索属性 `from`、`subject` 和 `body` 进行搜索。</span><span class="sxs-lookup"><span data-stu-id="2ff29-201">If you do a search on messages and specify only a value, the search is carried out on the default search properties of `from`, `subject` and `body`.</span></span>

<span data-ttu-id="2ff29-202">下面的示例返回登录用户收件箱中在三个默认搜索属性的任意一个中包含“pizza”的的所有邮件：</span><span class="sxs-lookup"><span data-stu-id="2ff29-202">The following example returns all messages in the signed-in user's Inbox that contains "pizza" in any of the three default search properties:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="pizza"
```

<span data-ttu-id="2ff29-203">下一个示例在用户收件箱中搜索从指定电子邮件地址发送的所有邮件：</span><span class="sxs-lookup"><span data-stu-id="2ff29-203">The next example searches all messages in the user's Inbox that were sent from a specific email address:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="from:help@contoso.com"
```

### <a name="using-search-on-person-collections"></a><span data-ttu-id="2ff29-204">针对 `person` 集合使用 $search</span><span class="sxs-lookup"><span data-stu-id="2ff29-204">Using $search on `person` collections</span></span>

<span data-ttu-id="2ff29-p118">可以使用 Microsoft Graph People API 检索与用户相关度最高的人员。相关性由用户的通信和协作模式及业务关系决定。People API 支持 `$search` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="2ff29-p118">You can use the Microsoft Graph People API to retrieve the people who are most relevant to a user. Relevance is determined by the user’s communication and collaboration patterns and business relationships. The People API supports the `$search` query parameter.</span></span>

<span data-ttu-id="2ff29-p119">搜索 [person](../api-reference/v1.0/resources/person.md) 资源的 `displayName` 和 `emailAddress` 属性上的人员。搜索实现模糊匹配算法。它们将基于完全匹配以及关于搜索意图的推断返回结果。例如，假设用户显示名称为“Tyler Lee”，电子邮件地址为 tylerle@example.com，该用户位于已登录用户的 `people` 集合中。所有以下搜索将返回包含 Tyler 的结果。</span><span class="sxs-lookup"><span data-stu-id="2ff29-p119">Searches on people occur on both the `displayName` and `emailAddress` properties of the [person](../api-reference/v1.0/resources/person.md) resource. Searches implement a fuzzy matching algorithm. They will return results based on an exact match and also on inferences about the intent of the search. For example, imagine a user with a display name of "Tyler Lee" and an email address of tylerle@example.com who is in the `people` collection of the signed-in user. All of the following searches will return results that contain Tyler.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people?$search=tyler                //matches both Tyler's name and email
GET https://graph.microsoft.com/v1.0/me/people?$search=tylerle              //matches Tyler's email
GET https://graph.microsoft.com/v1.0/me/people?$search="tylerle@example.com"  //matches Tyler's email. Note the quotes to enclose '@'.
GET https://graph.microsoft.com/v1.0/me/people?$search=tiler                //fuzzy match with Tyler's name 
GET https://graph.microsoft.com/v1.0/me/people?$search="tyler lee"          //matches Tyler's name. Note the quotes to enclose the space.
```

<span data-ttu-id="2ff29-p120">还可以搜索对特定主题感兴趣的人员。基于从用户的邮件对话派生的推断来执行搜索。例如，以下搜索将返回与登录用户相关的人员集合，在与该用户进行通信时，他表现出了对披萨的兴趣。请注意，搜索短语用引号括起来。</span><span class="sxs-lookup"><span data-stu-id="2ff29-p120">You can also perform searches for people who are interested in a particular topic. Searches are performed based on inferences derived from the user's mail conversations. For example, the following search will return a collection of people relevant to the signed-in user who have expressed an interest in pizza in communications with that user. Note that the search phrase is enclosed in quotes.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="topic:pizza"                
```

<span data-ttu-id="2ff29-217">最后，可以通过组合两种类型的搜索表达式，在同一请求中合并人员搜索和主题搜索。</span><span class="sxs-lookup"><span data-stu-id="2ff29-217">Finally, you can combine both people searches and topic searches in the same request by combining the two types of search expression.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="tyl topic:pizza"                
```
<span data-ttu-id="2ff29-p121">该请求主要进行两次搜索：对登录用户的相关人员的 `displayName` 和 `emailAddress` 属性进行模糊搜索，以及对该用户相关人员进行“披萨”主题搜索。然后对结果进行排名、排序并返回。请注意，该搜索没有限制；可能会得到包含模糊匹配“tyl”的人员的结果和/或对“披萨”感兴趣的人员的结果。</span><span class="sxs-lookup"><span data-stu-id="2ff29-p121">This request essentially conducts two searches: a fuzzy search against `displayName` and `emailAddress` properties of the signed-in user's relevant people and a topic search for "pizza" against the user's relevant people. The results are then ranked, ordered, and returned. Note that the search is not restrictive; you may get results that contain people that fuzzy match "tyl", or that are interested in "pizza", or both.</span></span>

<span data-ttu-id="2ff29-221">若要了解有关 People API 的详细信息，请参阅[获取相关人员的信息](./people_example.md)。</span><span class="sxs-lookup"><span data-stu-id="2ff29-221">To learn more about the People API, see [Get information about relevant people](./people_example.md).</span></span>  

## <a name="select"></a><span data-ttu-id="2ff29-222">select</span><span class="sxs-lookup"><span data-stu-id="2ff29-222">select</span></span>

<span data-ttu-id="2ff29-p122">使用 `$select` 查询参数返回一组不同于单个资源的默认集合或资源集合的属性。使用 $select 可以指定默认属性的子集或超集。</span><span class="sxs-lookup"><span data-stu-id="2ff29-p122">Use the `$select` query parameter to return a set of properties different than the default set for an individual resource or a collection of resources. With $select you can specify a subset or a superset of the default properties.</span></span>

<span data-ttu-id="2ff29-225">例如，在检索登录用户的邮件时，可以指定仅返回 `from` 和 `subject` 属性：</span><span class="sxs-lookup"><span data-stu-id="2ff29-225">For example, when retrieving the messages of the signed-in user, you can specify that only the `from` and `subject` properties be returned:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$select=from,subject
```

[<span data-ttu-id="2ff29-226">在 Graph 浏览器中试调用</span><span class="sxs-lookup"><span data-stu-id="2ff29-226">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$select=from,subject&method=GET&version=v1.0)

> <span data-ttu-id="2ff29-p123">**重要说明：**一般来说，建议使用 `$select` 将查询返回的属性限制为应用所需的属性。这对于可能返回大型结果集的查询尤为有用。限制每行返回的属性将减少网络负载并帮助提升应用的性能。</span><span class="sxs-lookup"><span data-stu-id="2ff29-p123">**Important:** In general, we recommend that you use `$select` to limit the properties returned by a query to those needed by your app. This is especially true of queries that may potentially return a large result set. Limiting the properties returned in each row will reduce network load and help improve your app's performance.</span></span>
>
> <span data-ttu-id="2ff29-p124">在 `v1.0` 中，从 [directoryObject](../api-reference/v1.0/resources/directoryobject.md) 派生的一些 Azure AD 资源（如 [user](../api-reference/v1.0/resources/user.md) 和 [group](../api-reference/v1.0/resources/group.md)）在读取时返回受限的默认属性子集。对于这些资源，必须使用 `$select` 将属性返回到默认集之外。</span><span class="sxs-lookup"><span data-stu-id="2ff29-p124">In `v1.0`, some Azure AD resources that derive from [directoryObject](../api-reference/v1.0/resources/directoryobject.md), like [user](../api-reference/v1.0/resources/user.md) and [group](../api-reference/v1.0/resources/group.md), return a limited, default subset of properties on reads. For these resources, you must use `$select` to return properties outside of the default set.</span></span>  

## <a name="skip"></a><span data-ttu-id="2ff29-232">skip</span><span class="sxs-lookup"><span data-stu-id="2ff29-232">skip</span></span>

<span data-ttu-id="2ff29-p125">使用 `$skip` 查询参数设置要在集合开头跳过的项数。例如，以下请求返回按照创建日期排序的用户的事件，从集合中的第 21 个事件开始：</span><span class="sxs-lookup"><span data-stu-id="2ff29-p125">Use the `$skip` query parameter to set the number of items to skip at the start of a collection. For example, the following request returns events for the user sorted by date created, starting with the 21st event in the collection:</span></span>

```http
GET  https://graph.microsoft.com/v1.0/me/events?$orderby=createdDateTime&$skip=20
```
[<span data-ttu-id="2ff29-235">在 Graph 浏览器中试调用</span><span class="sxs-lookup"><span data-stu-id="2ff29-235">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/events?$orderby=createdDateTime&$skip=20&method=GET&version=v1.0)

> <span data-ttu-id="2ff29-p126">**注意：**一些 Microsoft Graph API，如 Outlook 邮件和 Outlook 日历（`message``event` 和 `calendar`），使用 `$skip` 来实现分页。当查询的结果跨多个页面时，这些 API 将返回一个具有包含 `$skip` 参数的 URL 的 `@odata:nextLink` 属性。可以使用此 URL 返回下一页结果。若要了解详细信息，请参阅[分页](./paging.md)。</span><span class="sxs-lookup"><span data-stu-id="2ff29-p126">**Note:** Some Microsoft Graph APIs, like Outlook Mail and Calendars (`message`, `event`, and, `calendar`), use `$skip` to implement paging. When results of a query span multiple pages, these APIs will return an `@odata:nextLink` property with a URL that contains a `$skip` parameter. You can use this URL to return the next page of results. To learn more, see [Paging](./paging.md).</span></span>

## <a name="skiptoken"></a><span data-ttu-id="2ff29-240">skipToken</span><span class="sxs-lookup"><span data-stu-id="2ff29-240">skipToken</span></span>

<span data-ttu-id="2ff29-p127">由于服务器端分页或由于使用 [`$top`](#top) 参数来限制响应的页面大小，致使一些请求返回多页数据。许多 Microsoft Graph API 使用 `skipToken` 查询参数来引用结果的后续页面。`$skiptoken` 参数包含引用下一页结果的不透明令牌，并在响应的 `@odata.nextLink` 属性中提供的 URL 中返回。若要了解详细信息，请参阅[分页](./paging.md)。</span><span class="sxs-lookup"><span data-stu-id="2ff29-p127">Some requests return multiple pages of data either due to server-side paging or due to the use of the [`$top`](#top) parameter to limit the page size of the response. Many Microsoft Graph APIs use the `skipToken` query parameter to reference subsequent pages of the result. The `$skiptoken` parameter contains an opaque token that references the next page of results and is returned in the URL provided in the `@odata.nextLink` property in the response. To learn more, see [Paging](./paging.md).</span></span>


## <a name="top"></a><span data-ttu-id="2ff29-245">top</span><span class="sxs-lookup"><span data-stu-id="2ff29-245">top</span></span>

<span data-ttu-id="2ff29-246">使用 `$top` 查询参数指定结果集的页面大小。</span><span class="sxs-lookup"><span data-stu-id="2ff29-246">Use the `$top` query parameter to specify the page size of the result set.</span></span> 

<span data-ttu-id="2ff29-p128">如果结果集中还剩余多个项目，则响应正文将包含 `@odata.nextLink` 参数。此参数包含可用于获取下一页结果的 URL。若要了解详细信息，请参阅[分页](./paging.md)。</span><span class="sxs-lookup"><span data-stu-id="2ff29-p128">If there are more items remaining in the result set, the response body will contain an `@odata.nextLink` parameter. This parameter contains a URL that you can use to get the next page of results. To learn more, see [Paging](./paging.md).</span></span> 

<span data-ttu-id="2ff29-250">例如，以下请求返回用户邮箱中的前 5 封邮件：</span><span class="sxs-lookup"><span data-stu-id="2ff29-250">For example, the following request returns the first five messages in the user's mailbox:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$top=5
```

[<span data-ttu-id="2ff29-251">在 Graph 浏览器中试调用</span><span class="sxs-lookup"><span data-stu-id="2ff29-251">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$top=5&method=GET&version=v1.0)


## <a name="error-handling-for-query-parameters"></a><span data-ttu-id="2ff29-252">查询参数的错误处理</span><span class="sxs-lookup"><span data-stu-id="2ff29-252">Error handling for query parameters</span></span>

<span data-ttu-id="2ff29-p129">如果不支持指定的查询参数，某些请求将返回错误消息。例如，不能对 `user/photo` 关系使用 `$expand`。</span><span class="sxs-lookup"><span data-stu-id="2ff29-p129">Some requests will return an error message if a specified query parameter is not supported. For example, you cannot use `$expand` on the `user/photo` relationship.</span></span> 

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

<span data-ttu-id="2ff29-p130">但是，值得注意的是请求中指定的查询参数可能会自行失败。不支持的查询参数以及不支持的查询参数组合的情况就是如此。在这些情况下，应检查请求返回的数据，以确定指定的查询参数是否具有所需的效果。</span><span class="sxs-lookup"><span data-stu-id="2ff29-p130">However, it is important to note that query parameters specified in a request may fail silently. This can be true for unsupported query parameters as well as for unsupported combinations of query parameters. In these cases, you should examine the data returned by the request to determine whether the query parameters you specified had the desired effect.</span></span> 

[graph-explorer]: https://developer.microsoft.com/graph/graph-explorer
[odata-filter]: http://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752358
[odata-query]: http://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752356