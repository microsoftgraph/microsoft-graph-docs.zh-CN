---
title: 使用查询参数自定义响应
description: Microsoft Graph 提供可选的查询参数，可用于指定和控制响应中返回的数据量。支持以下查询参数。
author: piotrci
localization_priority: Priority
ms.openlocfilehash: 749415c25e03e3c29cdfb4b48ff66c562de0b84a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818912"
---
# <a name="use-query-parameters-to-customize-responses"></a><span data-ttu-id="3fb51-104">使用查询参数自定义响应</span><span class="sxs-lookup"><span data-stu-id="3fb51-104">Use query parameters to customize responses</span></span>

<span data-ttu-id="3fb51-105">Microsoft Graph 支持可选的查询参数，可用于指定和控制响应中返回的数据量。</span><span class="sxs-lookup"><span data-stu-id="3fb51-105">Microsoft Graph supports optional query parameters that you can use to specify and control the amount of data returned in a response.</span></span> <span data-ttu-id="3fb51-106">对准确查询参数的支持因 API 操作不同而不同，并且可能会在 v1.0 和数据终结点之间不同，具体取决于 API。</span><span class="sxs-lookup"><span data-stu-id="3fb51-106">The support for the exact query parameters varies from one API operation to another, and depending on the API, can differ between the v1.0 and beta endpoints.</span></span> 

> <span data-ttu-id="3fb51-107">**注释：** 在 v1.0 和 beta 终结点上，`$` 前缀为可选。</span><span class="sxs-lookup"><span data-stu-id="3fb51-107">**Note:** On the v1.0 and beta endpoints, the `$` prefix is optional.</span></span> <span data-ttu-id="3fb51-108">例如，可使用 `filter` 来代替 `$filter`。</span><span class="sxs-lookup"><span data-stu-id="3fb51-108">For example, instead of `$filter`, you can use `filter`.</span></span>

<span data-ttu-id="3fb51-109">查询参数可以是 OData 系统查询选项，也可以是其他查询参数。</span><span class="sxs-lookup"><span data-stu-id="3fb51-109">Query parameters can be OData system query options or other query parameters.</span></span> 

## <a name="odata-system-query-options"></a><span data-ttu-id="3fb51-110">OData 系统查询选项</span><span class="sxs-lookup"><span data-stu-id="3fb51-110">OData system query options</span></span>
<span data-ttu-id="3fb51-111">Microsoft Graph API 操作可以支持以下一个或多个 OData 系统查询选项。</span><span class="sxs-lookup"><span data-stu-id="3fb51-111">A Microsoft Graph API operation might support one or more of the following OData system query options.</span></span> <span data-ttu-id="3fb51-112">这些查询选项与 [OData V4 查询语言][odata-query]兼容。</span><span class="sxs-lookup"><span data-stu-id="3fb51-112">These query options are compatible with the [OData V4 query language][odata-query].</span></span>

><span data-ttu-id="3fb51-113">**注意：** 单击示例以在 [Graph 浏览器][graph-explorer]中试调用。</span><span class="sxs-lookup"><span data-stu-id="3fb51-113">**Note:** Click the examples to try them in [Graph Explorer][graph-explorer].</span></span>

| <span data-ttu-id="3fb51-114">名称</span><span class="sxs-lookup"><span data-stu-id="3fb51-114">Name</span></span>                     | <span data-ttu-id="3fb51-115">说明</span><span class="sxs-lookup"><span data-stu-id="3fb51-115">Description</span></span> | <span data-ttu-id="3fb51-116">示例</span><span class="sxs-lookup"><span data-stu-id="3fb51-116">Example</span></span>
|:-------------------------|:------------|:---------|
| [<span data-ttu-id="3fb51-117">$count</span><span class="sxs-lookup"><span data-stu-id="3fb51-117">$count</span></span>](#count-parameter)         | <span data-ttu-id="3fb51-118">检索匹配资源的总数。</span><span class="sxs-lookup"><span data-stu-id="3fb51-118">Retrieves the total count of matching resources.</span></span> | [`/me/messages?$top=2&$count=true`][count-example]
| [<span data-ttu-id="3fb51-119">$expand</span><span class="sxs-lookup"><span data-stu-id="3fb51-119">$expand</span></span>](#expand-parameter)       | <span data-ttu-id="3fb51-120">检索相关资源。</span><span class="sxs-lookup"><span data-stu-id="3fb51-120">Retrieves related resources.</span></span>|[`/groups?$expand=members`][expand-example]
| [<span data-ttu-id="3fb51-121">$filter</span><span class="sxs-lookup"><span data-stu-id="3fb51-121">$filter</span></span>](#filter-parameter)       | <span data-ttu-id="3fb51-122">筛选结果（行）。</span><span class="sxs-lookup"><span data-stu-id="3fb51-122">Filters results (rows).</span></span>|[`/users?$filter=startswith(givenName,'J')`][filter-example]
| [<span data-ttu-id="3fb51-123">$format</span><span class="sxs-lookup"><span data-stu-id="3fb51-123">$format</span></span>](#format-parameter)       | <span data-ttu-id="3fb51-124">返回指定媒体格式的结果。</span><span class="sxs-lookup"><span data-stu-id="3fb51-124">Returns the results in the specified media format.</span></span>|[`/users?$format=json`][format-example]
| [<span data-ttu-id="3fb51-125">$orderby</span><span class="sxs-lookup"><span data-stu-id="3fb51-125">$orderby</span></span>](#orderby-parameter)     | <span data-ttu-id="3fb51-126">对结果进行排序。</span><span class="sxs-lookup"><span data-stu-id="3fb51-126">Orders results.</span></span>|[`/users?$orderby=displayName desc`][orderby-example]
| [<span data-ttu-id="3fb51-127">$search</span><span class="sxs-lookup"><span data-stu-id="3fb51-127">$search</span></span>](#search-parameter)       | <span data-ttu-id="3fb51-p105">根据搜索条件返回结果。目前支持用于 **messages** 和 **person** 集合。</span><span class="sxs-lookup"><span data-stu-id="3fb51-p105">Returns results based on search criteria. Currently supported on **messages** and **person** collections.</span></span>|[`/me/messages?$search=pizza`][search-example]
| [<span data-ttu-id="3fb51-130">$select</span><span class="sxs-lookup"><span data-stu-id="3fb51-130">$select</span></span>](#select-parameter)       | <span data-ttu-id="3fb51-131">筛选属性（列）。</span><span class="sxs-lookup"><span data-stu-id="3fb51-131">Filters properties (columns).</span></span>|[`/users?$select=givenName,surname`][select-example]
| [<span data-ttu-id="3fb51-132">$skip</span><span class="sxs-lookup"><span data-stu-id="3fb51-132">$skip</span></span>](#skip-parameter)           | <span data-ttu-id="3fb51-p106">对结果集建立索引。一些 API 也使用它来实现分页，并且可以与 `$top` 一起使用来手动对结果分页。</span><span class="sxs-lookup"><span data-stu-id="3fb51-p106">Indexes into a result set. Also used by some APIs to implement paging and can be used together with `$top` to manually page results.</span></span> | [`/me/messages?$skip=11`][skip-example]
| [<span data-ttu-id="3fb51-135">$top</span><span class="sxs-lookup"><span data-stu-id="3fb51-135">$top</span></span>](#top-parameter)             | <span data-ttu-id="3fb51-136">设置结果的页面大小。</span><span class="sxs-lookup"><span data-stu-id="3fb51-136">Sets the page size of results.</span></span> |[`/users?$top=2`][top-example]


## <a name="other-query-parameters"></a><span data-ttu-id="3fb51-137">其他查询参数</span><span class="sxs-lookup"><span data-stu-id="3fb51-137">Other query parameters</span></span>

| <span data-ttu-id="3fb51-138">名称</span><span class="sxs-lookup"><span data-stu-id="3fb51-138">Name</span></span>                     | <span data-ttu-id="3fb51-139">说明</span><span class="sxs-lookup"><span data-stu-id="3fb51-139">Description</span></span> | <span data-ttu-id="3fb51-140">示例</span><span class="sxs-lookup"><span data-stu-id="3fb51-140">Example</span></span>
|:-------------------------|:------------|:---------|
| [<span data-ttu-id="3fb51-141">$skipToken</span><span class="sxs-lookup"><span data-stu-id="3fb51-141">$skipToken</span></span>](#skiptoken-parameter) | <span data-ttu-id="3fb51-p107">从跨多页的结果集中检索下一页结果。（但某些 API 改为使用 `$skip`。）</span><span class="sxs-lookup"><span data-stu-id="3fb51-p107">Retrieves the next page of results from result sets that span multiple pages. (Some APIs use `$skip` instead.)</span></span> | `/users?$skiptoken=X%274453707402000100000017...`|

## <a name="encoding-query-parameters"></a><span data-ttu-id="3fb51-144">对查询参数进行编码</span><span class="sxs-lookup"><span data-stu-id="3fb51-144">Encoding query parameters</span></span>

<span data-ttu-id="3fb51-145">应对查询参数的值进行百分比编码。</span><span class="sxs-lookup"><span data-stu-id="3fb51-145">The values of query parameters should be percent-encoded.</span></span> <span data-ttu-id="3fb51-146">许多 HTTP 客户端、浏览器和工具（例如，[Graph 浏览器][graph-explorer]）都可以帮助用户完成此操作。</span><span class="sxs-lookup"><span data-stu-id="3fb51-146">Many HTTP clients, browsers, and tools (such as the [Graph Explorer][graph-explorer]) will help you with this.</span></span> <span data-ttu-id="3fb51-147">如果查询失败，可能原因之一是未正确编码查询参数值。</span><span class="sxs-lookup"><span data-stu-id="3fb51-147">If a query is failing, one possible cause is failure to encode the query parameter values appropriately.</span></span>

<span data-ttu-id="3fb51-148">未编码的 URL 如下所示：</span><span class="sxs-lookup"><span data-stu-id="3fb51-148">An unencoded URL looks like this:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName, 'J')
```

<span data-ttu-id="3fb51-149">正确解码的 URL 如下所示：</span><span class="sxs-lookup"><span data-stu-id="3fb51-149">A properly encoded URL looks like this:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName%2C+'J')
```

## <a name="count-parameter"></a><span data-ttu-id="3fb51-150">count 参数</span><span class="sxs-lookup"><span data-stu-id="3fb51-150">count parameter</span></span>

<span data-ttu-id="3fb51-151">使用 `$count` 查询参数以包括集合中项总数的计数，以及从 Microsoft Graph 返回的数据值页。</span><span class="sxs-lookup"><span data-stu-id="3fb51-151">Use the `$count` query parameter to include a count of the total number of items in a collection alongside the page of data values returned from Microsoft Graph.</span></span> 

<span data-ttu-id="3fb51-152">例如，下面的请求返回当前用户的 **contact** 集合，以及 `@odata.count` 属性中 **contact** 集合内的项数。</span><span class="sxs-lookup"><span data-stu-id="3fb51-152">For example, the following request will return both the **contact** collection of the current user, and the number of items in the **contact** collection in the `@odata.count` property.</span></span>

```http
GET  https://graph.microsoft.com/v1.0/me/contacts?$count=true
```

[<span data-ttu-id="3fb51-153">在 Graph 浏览器中试调用</span><span class="sxs-lookup"><span data-stu-id="3fb51-153">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/contacts?$count=true&method=GET&version=v1.0)


><span data-ttu-id="3fb51-154">**注意：** 派生自 [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0) 的资源集合（如 [user](/graph/api/resources/user?view=graph-rest-1.0) 或 [group](/graph/api/resources/group?view=graph-rest-1.0) 集合）不支持 `$count`。</span><span class="sxs-lookup"><span data-stu-id="3fb51-154">**Note:** `$count` is not supported for collections of resources that derive from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0) like collections of [users](/graph/api/resources/user?view=graph-rest-1.0) or [groups](/graph/api/resources/group?view=graph-rest-1.0).</span></span>

## <a name="expand-parameter"></a><span data-ttu-id="3fb51-155">expand 参数</span><span class="sxs-lookup"><span data-stu-id="3fb51-155">expand parameter</span></span>

<span data-ttu-id="3fb51-156">许多 Microsoft Graph 资源都会公开资源的已声明属性以及与其他资源的关系。</span><span class="sxs-lookup"><span data-stu-id="3fb51-156">Many Microsoft Graph resources expose both declared properties of the resource as well as its relationships with other resources.</span></span> <span data-ttu-id="3fb51-157">这些关系也称为引用属性或导航属性，它们可以引用单个资源或资源集合。</span><span class="sxs-lookup"><span data-stu-id="3fb51-157">These relationships are also called reference properties or navigation properties, and they can reference either a single resource or a collection of resources.</span></span> <span data-ttu-id="3fb51-158">例如，用户的邮件文件夹、管理者和直接下属都将作为关系公开。</span><span class="sxs-lookup"><span data-stu-id="3fb51-158">For example, the mail folders, manager, and direct reports of a user are all exposed as relationships.</span></span> 

<span data-ttu-id="3fb51-p110">通常情况下，可以在单个请求中查询资源属性或其关系之一，但不能同时查询。可以使用 `$expand` 查询字符串参数以包含结果中单个关系（导航属性）引用的扩展资源或集合。</span><span class="sxs-lookup"><span data-stu-id="3fb51-p110">Normally, you can query either the properties of a resource or one of its relationships in a single request, but not both. You can use the `$expand` query string parameter to include the expanded resource or collection referenced by a single relationship (navigation property) in your results.</span></span>

<span data-ttu-id="3fb51-161">以下示例在驱动器中获取根驱动器信息以及顶级子项：</span><span class="sxs-lookup"><span data-stu-id="3fb51-161">The following example gets root drive information along with the top-level child items in a drive:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children
```

[<span data-ttu-id="3fb51-162">在 Graph 浏览器中试调用</span><span class="sxs-lookup"><span data-stu-id="3fb51-162">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/drive/root?$expand=children&method=GET&version=v1.0)

<span data-ttu-id="3fb51-p111">使用一些资源集合，还可以添加 `$select` 参数，指定要在扩展资源中返回的属性。下面的示例执行与上一示例几乎相同的查询，不同之处在于使用 [`$select`](#select-parameter) 语句将为扩展子项返回的属性限制为 **id** 和 **name** 属性。</span><span class="sxs-lookup"><span data-stu-id="3fb51-p111">With some resource collections, you can also specify the properties to be returned in the expanded resources by adding a `$select` parameter. The following example performs the same query as the previous example but uses a [`$select`](#select-parameter) statement to limit the properties returned for the expanded child items to the **id** and **name** properties.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children($select=id,name)
```

<span data-ttu-id="3fb51-165">[在 Graph 浏览器中试用][expand-example]</span><span class="sxs-lookup"><span data-stu-id="3fb51-165">[Try in Graph Explorer][expand-example]</span></span>

> <span data-ttu-id="3fb51-p112">**注意：** 并不是所有关系和资源都支持 `$expand` 查询参数。例如，可以扩展用户的 **directReports**、**manager** 和 **memberOf** 关系，但无法扩展其 **events**、**messages** 或 **photo** 关系。并非所有资源或关系都支持对扩展项使用 `$select`。</span><span class="sxs-lookup"><span data-stu-id="3fb51-p112">**Note:** Not all relationships and resources support the `$expand` query parameter. For example, you can expand the **directReports**, **manager**, and **memberOf** relationships on a user, but you cannot expand its **events**, **messages**, or **photo** relationships. Not all resources or relationships support using `$select` on expanded items.</span></span> 
> 
> <span data-ttu-id="3fb51-169">使用从 [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0) 派生的 Azure AD 资源（如[user](/graph/api/resources/user?view=graph-rest-1.0) 和 [group](/graph/api/resources/group?view=graph-rest-1.0)），`$expand` 仅支持 `beta`，并且通常最多为扩展关系返回 20 个项。</span><span class="sxs-lookup"><span data-stu-id="3fb51-169">With Azure AD resources that derive from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0), like [user](/graph/api/resources/user?view=graph-rest-1.0) and [group](/graph/api/resources/group?view=graph-rest-1.0), `$expand` is only supported for `beta` and  typically returns a maximum of 20 items for the expanded relationship.</span></span>

## <a name="filter-parameter"></a><span data-ttu-id="3fb51-170">filter 参数</span><span class="sxs-lookup"><span data-stu-id="3fb51-170">filter parameter</span></span>

<span data-ttu-id="3fb51-171">使用 `$filter` 查询参数，以仅检索集合的子集。</span><span class="sxs-lookup"><span data-stu-id="3fb51-171">Use the `$filter` query parameter to retrieve just a subset of a collection.</span></span> 

<span data-ttu-id="3fb51-172">例如，若要查找显示名称以子母“J”开头的用户，请使用 `startswith`。</span><span class="sxs-lookup"><span data-stu-id="3fb51-172">For example, to find users whose display name starts with the letter 'J', use `startswith`.</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'J')
```

<span data-ttu-id="3fb51-173">[在 Graph 浏览器中试用][filter-example]</span><span class="sxs-lookup"><span data-stu-id="3fb51-173">[Try in Graph Explorer][filter-example]</span></span>

<span data-ttu-id="3fb51-174">对 `$filter` 运算符的支持因 Microsoft Graph API 而异。</span><span class="sxs-lookup"><span data-stu-id="3fb51-174">Support for `$filter` operators varies across Microsoft Graph APIs.</span></span> <span data-ttu-id="3fb51-175">通常支持下列逻辑运算符：</span><span class="sxs-lookup"><span data-stu-id="3fb51-175">The following logical operators are generally supported:</span></span> 

- <span data-ttu-id="3fb51-176">等于 (`eq`)</span><span class="sxs-lookup"><span data-stu-id="3fb51-176">equals (`eq`)</span></span>
- <span data-ttu-id="3fb51-177">不等于 (`ne`)</span><span class="sxs-lookup"><span data-stu-id="3fb51-177">not equals (`ne`)</span></span>
- <span data-ttu-id="3fb51-178">大于 (`gt`)</span><span class="sxs-lookup"><span data-stu-id="3fb51-178">greater than (`gt`)</span></span>
- <span data-ttu-id="3fb51-179">大于或等于 (`ge`)</span><span class="sxs-lookup"><span data-stu-id="3fb51-179">greater than or equals (`ge`)</span></span>
- <span data-ttu-id="3fb51-180">小于 (`lt`)，小于或等于 (`le`)</span><span class="sxs-lookup"><span data-stu-id="3fb51-180">less than (`lt`), less than or equals (`le`)</span></span>
- <span data-ttu-id="3fb51-181">且 (`and`)</span><span class="sxs-lookup"><span data-stu-id="3fb51-181">and (`and`)</span></span>
- <span data-ttu-id="3fb51-182">或 (`or`)</span><span class="sxs-lookup"><span data-stu-id="3fb51-182">or (`or`)</span></span>
- <span data-ttu-id="3fb51-183">非 (`not`)</span><span class="sxs-lookup"><span data-stu-id="3fb51-183">not (`not`)</span></span>
 
<span data-ttu-id="3fb51-184">通常支持 `startswith` 字符串运算符。</span><span class="sxs-lookup"><span data-stu-id="3fb51-184">The `startswith` string operator is often supported.</span></span> <span data-ttu-id="3fb51-185">某些 API 支持 `any` lambda 运算符。</span><span class="sxs-lookup"><span data-stu-id="3fb51-185">The `any` lambda operator is supported for some APIs.</span></span> <span data-ttu-id="3fb51-186">有关一些用法示例的信息，请参阅下表。</span><span class="sxs-lookup"><span data-stu-id="3fb51-186">For some  usage examples, see the following table.</span></span> <span data-ttu-id="3fb51-187">有关 `$filter` 语法的其他详细信息，请参阅 [OData 协议][odata-filter]。</span><span class="sxs-lookup"><span data-stu-id="3fb51-187">For more details about `$filter` syntax, see the [OData protocol][odata-filter].</span></span>  

<span data-ttu-id="3fb51-188">下表显示使用 `$filter` 查询参数的一些示例。</span><span class="sxs-lookup"><span data-stu-id="3fb51-188">The following table shows some examples that use the `$filter` query parameter.</span></span>

> <span data-ttu-id="3fb51-189">**注意：** 单击示例以在 [Graph 浏览器][graph-explorer]中试调用。</span><span class="sxs-lookup"><span data-stu-id="3fb51-189">**Note:** Click the examples to try them in [Graph Explorer][graph-explorer].</span></span>

| <span data-ttu-id="3fb51-190">说明</span><span class="sxs-lookup"><span data-stu-id="3fb51-190">Description</span></span> | <span data-ttu-id="3fb51-191">示例</span><span class="sxs-lookup"><span data-stu-id="3fb51-191">Example</span></span>
|:------------|:--------|
| <span data-ttu-id="3fb51-192">跨多个属性搜索名为 Mary 的用户。</span><span class="sxs-lookup"><span data-stu-id="3fb51-192">Search for users with the name Mary across multiple properties.</span></span> | [`https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'mary') or startswith(givenName,'mary') or startswith(surname,'mary') or startswith(mail,'mary') or startswith(userPrincipalName,'mary')`](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(displayName,'mary')+or+startswith(givenName,'mary')+or+startswith(surname,'mary')+or+startswith(mail,'mary')+or+startswith(userPrincipalName,'mary')&method=GET&version=v1.0) 
| <span data-ttu-id="3fb51-193">获取 2017 年 7 月 1 日之后开始的所有登录用户的事件。</span><span class="sxs-lookup"><span data-stu-id="3fb51-193">Get all the signed-in user's events that start after 7/1/2017.</span></span> | [`https://graph.microsoft.com/v1.0/me/events?$filter=start/dateTime ge '2017-07-01T08:00'`](https://developer.microsoft.com/graph/graph-explorer?request=me/events?$filter=start/dateTime+ge+'2017-07-01T08:00'&method=GET&version=v1.0) 
| <span data-ttu-id="3fb51-194">获取登录用户收到的来自特定地址的所有电子邮件。</span><span class="sxs-lookup"><span data-stu-id="3fb51-194">Get all emails from a specific address received by the signed-in user.</span></span> | [`https://graph.microsoft.com/v1.0/me/messages?$filter=from/emailAddress/address eq 'someuser@example.com'`](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=from/emailAddress/address+eq+'someuser@.com'&method=GET&version=v1.0) 
| <span data-ttu-id="3fb51-195">获取登录用户在 2017 年 4 月收到的所有电子邮件。</span><span class="sxs-lookup"><span data-stu-id="3fb51-195">Get all emails received by the signed-in user in April 2017.</span></span> | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=ReceivedDateTime ge 2017-04-01 and receivedDateTime lt 2017-05-01`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=ReceivedDateTime+ge+2017-04-01+and+receivedDateTime+lt+2017-05-01&method=GET&version=v1.0) 
| <span data-ttu-id="3fb51-196">获取登录用户收件箱中的所有未读邮件。</span><span class="sxs-lookup"><span data-stu-id="3fb51-196">Get all unread mail in the signed-in user's Inbox.</span></span> | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=isRead eq false`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=isRead+eq+false&method=GET&version=v1.0) 
| <span data-ttu-id="3fb51-197">列出组织中的所有 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="3fb51-197">List all Office 365 groups in an organization.</span></span> | [`https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')`](https://developer.microsoft.com/graph/graph-explorer?request=groups?$filter=groupTypes/any(c:c+eq+'Unified')&method=GET&version=v1.0) 

> <span data-ttu-id="3fb51-p115">**注意：** Azure AD 资源不支持以下 `$filter` 运算符：`ne`、`gt`、`ge`、`lt`、`le` 和 `not`。所有 Microsoft Graph 资源目前均不支持 `contains` 字符串运算符。</span><span class="sxs-lookup"><span data-stu-id="3fb51-p115">**Note:** The following `$filter` operators are not supported for Azure AD resources:  `ne`, `gt`, `ge`, `lt`, `le`, and `not`. The `contains` string operator is currently not supported on any Microsoft Graph resources.</span></span>

## <a name="format-parameter"></a><span data-ttu-id="3fb51-200">format 参数</span><span class="sxs-lookup"><span data-stu-id="3fb51-200">format parameter</span></span>

<span data-ttu-id="3fb51-201">使用 `$format` 查询参数，指定 Microsoft Graph 返回的项的媒体格式。</span><span class="sxs-lookup"><span data-stu-id="3fb51-201">Use the `$format` query parameter to specify the media format of the items returned from Microsoft Graph.</span></span>

<span data-ttu-id="3fb51-202">例如，下面的请求以 json 格式返回组织中的用户：</span><span class="sxs-lookup"><span data-stu-id="3fb51-202">For example, the following request returns the users in the organization in the json format:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$format=json
```

<span data-ttu-id="3fb51-203">[在 Graph 浏览器中试用][format-example]</span><span class="sxs-lookup"><span data-stu-id="3fb51-203">[Try in Graph Explorer][format-example]</span></span>

> <span data-ttu-id="3fb51-204">**注意：**`$format` 查询参数支持许多格式（例如，atom、xml 和 json），但可能无法返回所有格式的结果。</span><span class="sxs-lookup"><span data-stu-id="3fb51-204">**Note:** The `$format` query parameter supports a number of formats (for example, atom, xml, and json) but results may not be returned in all formats.</span></span>

## <a name="orderby-parameter"></a><span data-ttu-id="3fb51-205">orderby 参数</span><span class="sxs-lookup"><span data-stu-id="3fb51-205">orderby parameter</span></span>

<span data-ttu-id="3fb51-206">使用 `$orderby` 查询参数指定从 Microsoft Graph 返回的项的排序顺序。</span><span class="sxs-lookup"><span data-stu-id="3fb51-206">Use the `$orderby` query parameter to specify the sort order of the items returned from Microsoft Graph.</span></span>

<span data-ttu-id="3fb51-207">例如，以下请求返回按用户显示名称进行排序的组织中的用户：</span><span class="sxs-lookup"><span data-stu-id="3fb51-207">For example, the following request returns the users in the organization ordered by their display name:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$orderby=displayName
```
<span data-ttu-id="3fb51-208">[在 Graph 浏览器中试用][orderby-example]</span><span class="sxs-lookup"><span data-stu-id="3fb51-208">[Try in Graph Explorer][orderby-example]</span></span>

<span data-ttu-id="3fb51-p116">还可以按复杂类型实体进行排序。下面的请求获取邮件，并按 **from** 属性的 **address** 字段（复杂类型为 **emailAddress**）进行排序：</span><span class="sxs-lookup"><span data-stu-id="3fb51-p116">You can also sort by complex type entities. The following request gets messages and sorts them by the **address** field of the **from** property, which is of the complex type **emailAddress**:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$orderby=from/emailAddress/address
```
[<span data-ttu-id="3fb51-211">在 Graph 浏览器中试调用</span><span class="sxs-lookup"><span data-stu-id="3fb51-211">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/address&method=GET&version=v1.0)

<span data-ttu-id="3fb51-212">若要以升序或降序对结果进行排序，请向字段名称追加 `asc` 或 `desc`，并用空格隔开。例如，`?$orderby=name%20desc`。</span><span class="sxs-lookup"><span data-stu-id="3fb51-212">To sort the results in ascending or descending order, append either `asc` or `desc` to the field name, separated by a space; for example, `?$orderby=name%20desc`.</span></span>

<span data-ttu-id="3fb51-213">通过一些 API，可以对多个属性的结果进行排序。</span><span class="sxs-lookup"><span data-stu-id="3fb51-213">With some APIs, you can order results on multiple properties.</span></span> <span data-ttu-id="3fb51-214">例如，以下请求首先按发件人名称以降序（Z 到 A）排序用户收件箱中的邮件，然后按主题以升序（默认）排序邮件。</span><span class="sxs-lookup"><span data-stu-id="3fb51-214">For example, the following request orders the messages in the user's Inbox, first by the name of the person who sent it in descending order (Z to A), and then by subject in ascending order (default).</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/Inbox/messages?$orderby=from/emailAddress/name desc,subject
```

[<span data-ttu-id="3fb51-215">在 Graph 浏览器中试调用</span><span class="sxs-lookup"><span data-stu-id="3fb51-215">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/name%20desc,subject&method=GET&version=v1.0)

<span data-ttu-id="3fb51-216">如果指定 $filter，服务器会推断结果的排序顺序。</span><span class="sxs-lookup"><span data-stu-id="3fb51-216">When you specify $filter the server will infer a sort order for the results.</span></span> <span data-ttu-id="3fb51-217">如果同时使用 `$orderby` 和 `$filter`，由于服务器始终推断 `$filter` 结果的排序顺序，因此必须先在 `$orderby` 中列出 `$filter` 的属性，然后再列出其他任何属性，且必须按照它们在 `$filter` 参数中的顺序列出这些属性。</span><span class="sxs-lookup"><span data-stu-id="3fb51-217">If you use both `$orderby` and `$filter`, because the server always infers a sort order for the results of a `$filter`, the properties in the `$filter` must be listed first in the `$orderby` before any other properties, and they must be listed in the order that they appear in the `$filter` parameter.</span></span> 

<span data-ttu-id="3fb51-218">下面的示例展示了如何按 **subject** 和 **importance** 属性筛选查询，再按 **subject**、**importance** 和 **receivedDateTime** 属性进行降序排序。</span><span class="sxs-lookup"><span data-stu-id="3fb51-218">The following example shows a query filtered by the **subject** and **importance** properties, and then sorted by the **subject**, **importance**, and **receivedDateTime** properties in descending order.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=Subject eq 'welcome' and importance eq 'normal'&$orderby=subject,importance,receivedDateTime desc
```

[<span data-ttu-id="3fb51-219">在 Graph 浏览器中试调用</span><span class="sxs-lookup"><span data-stu-id="3fb51-219">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=subject%20eq%20%27welcome%27%20and%20importance%20eq%20%27normal%27%20&$orderby=subject,importance,receivedDateTime%20desc&method=GET&version=v1.0)

 > <span data-ttu-id="3fb51-220">**注意：** 使用从 [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0) 派生的 Azure AD 资源（如 [user](/graph/api/resources/user?view=graph-rest-1.0) 和 [group](/graph/api/resources/group?view=graph-rest-1.0)），则不能合并 `$orderby` 与 `$filter` 表达式。</span><span class="sxs-lookup"><span data-stu-id="3fb51-220">**Note:** With Azure AD resources that derive from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0), like [user](/graph/api/resources/user?view=graph-rest-1.0) and [group](/graph/api/resources/group?view=graph-rest-1.0), you cannot combine `$orderby` with `$filter` expressions.</span></span> 

## <a name="search-parameter"></a><span data-ttu-id="3fb51-221">search 参数</span><span class="sxs-lookup"><span data-stu-id="3fb51-221">search parameter</span></span>

<span data-ttu-id="3fb51-222">使用 `$search` 查询参数限制与搜索条件匹配的请求结果。</span><span class="sxs-lookup"><span data-stu-id="3fb51-222">Use the `$search` query parameter to restrict the results of a request to match a search criterion.</span></span>

> <span data-ttu-id="3fb51-p119">**注意：** 目前**只**能搜索 [message](/graph/api/resources/message?view=graph-rest-1.0) 和 [person](/graph/api/resources/person?view=graph-rest-1.0) 集合。`$search` 请求最多可返回 250 个结果。不能在搜索请求中使用 [`$filter`](#filter-parameter) 或 [`$orderby`](#orderby-parameter)。</span><span class="sxs-lookup"><span data-stu-id="3fb51-p119">**Note:** You can currently search **only** [message](/graph/api/resources/message?view=graph-rest-1.0) and [person](/graph/api/resources/person?view=graph-rest-1.0) collections. A `$search` request returns up to 250 results. You cannot use [`$filter`](#filter-parameter) or [`$orderby`](#orderby-parameter) in a search request.</span></span>

### <a name="using-search-on-message-collections"></a><span data-ttu-id="3fb51-226">对 message 集合使用 $search</span><span class="sxs-lookup"><span data-stu-id="3fb51-226">Using $search on message collections</span></span>

<span data-ttu-id="3fb51-227">可根据特定邮件属性值搜索邮件。</span><span class="sxs-lookup"><span data-stu-id="3fb51-227">You can search messages based on a value in specific message properties.</span></span> <span data-ttu-id="3fb51-228">搜索结果按邮件发送日期和时间进行排序。</span><span class="sxs-lookup"><span data-stu-id="3fb51-228">The results of the search are sorted by the date and time that the message was sent.</span></span>

<span data-ttu-id="3fb51-229">如果确实要搜索邮件，且仅指定值，而未指定特定邮件属性，搜索依据为默认搜索属性 **from**、**subject** 和 **body**。</span><span class="sxs-lookup"><span data-stu-id="3fb51-229">If you do a search on messages and specify only a value without specific message properties, the search is carried out on the default search properties of **from**, **subject**, and **body**.</span></span>

<span data-ttu-id="3fb51-230">下面的示例返回登录用户收件箱中三个默认搜索属性中有任意一个包含“pizza”的所有邮件：</span><span class="sxs-lookup"><span data-stu-id="3fb51-230">The following example returns all messages in the signed-in user's Inbox that contains "pizza" in any of the three default search properties:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="pizza"
```

<span data-ttu-id="3fb51-231">[在 Graph 浏览器中试调用][search-example]</span><span class="sxs-lookup"><span data-stu-id="3fb51-231">[Try in Graph Explorer][search-example]</span></span>

<span data-ttu-id="3fb51-232">也可以指定下表中的邮件属性名来搜索邮件，这些属性名可由关键字查询语言 (KQL) 语法识别。</span><span class="sxs-lookup"><span data-stu-id="3fb51-232">Alternatively, you can search messages by specifying message property names in the following table, that are recognized by the Keyword Query Language (KQL) syntax.</span></span> <span data-ttu-id="3fb51-233">这些属性名对应于 Microsoft Graph **message** 实体中定义的属性。</span><span class="sxs-lookup"><span data-stu-id="3fb51-233">These property names correspond to properties defined in the **message** entity of Microsoft Graph.</span></span> <span data-ttu-id="3fb51-234">Outlook 和其他 Office 365 应用程序（如 SharePoint）支持 KQL 语法，从而为数据存储提供了方便使用的公共发现域。</span><span class="sxs-lookup"><span data-stu-id="3fb51-234">Outlook and other Office 365 applications such as SharePoint support KQL syntax, providing the convenience of a common discovery domain for their data stores.</span></span>


| <span data-ttu-id="3fb51-235">可搜索的电子邮件属性</span><span class="sxs-lookup"><span data-stu-id="3fb51-235">Searchable email property</span></span>                | <span data-ttu-id="3fb51-236">说明</span><span class="sxs-lookup"><span data-stu-id="3fb51-236">Description</span></span> | <span data-ttu-id="3fb51-237">示例</span><span class="sxs-lookup"><span data-stu-id="3fb51-237">Example</span></span> 
|:-------------------------|:------------|:---------|
| <span data-ttu-id="3fb51-238">**attachment**</span><span class="sxs-lookup"><span data-stu-id="3fb51-238">**attachment**</span></span>           | <span data-ttu-id="3fb51-239">电子邮件附件的文件名。</span><span class="sxs-lookup"><span data-stu-id="3fb51-239">The names of files attached to an email message.</span></span>|[`me/messages?$search="attachment:api-catalog.md"`][search-att-example]
| <span data-ttu-id="3fb51-240">**bcc**</span><span class="sxs-lookup"><span data-stu-id="3fb51-240">**bcc**</span></span>           | <span data-ttu-id="3fb51-241">电子邮件的 **bcc** 字段，可指定为 SMTP 地址、显示名称或别名。</span><span class="sxs-lookup"><span data-stu-id="3fb51-241">The **bcc** field of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="bcc:samanthab@contoso.com"&$select=subject,bccRecipients`][search-bcc-example]
| <span data-ttu-id="3fb51-242">**body**</span><span class="sxs-lookup"><span data-stu-id="3fb51-242">**body**</span></span>           | <span data-ttu-id="3fb51-243">电子邮件正文。</span><span class="sxs-lookup"><span data-stu-id="3fb51-243">The body of an email message.</span></span>|[`me/messages?$search="body:excitement"`][search-body-example]
| <span data-ttu-id="3fb51-244">**cc**</span><span class="sxs-lookup"><span data-stu-id="3fb51-244">**cc**</span></span>           | <span data-ttu-id="3fb51-245">电子邮件的 **cc** 字段，可指定为 SMTP 地址、显示名称或别名。</span><span class="sxs-lookup"><span data-stu-id="3fb51-245">The **cc** field of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="cc:danas"&$select=subject,ccRecipients`][search-cc-example]
| <span data-ttu-id="3fb51-246">**from**</span><span class="sxs-lookup"><span data-stu-id="3fb51-246">**from**</span></span>           | <span data-ttu-id="3fb51-247">电子邮件的发件人，可指定为 SMTP 地址、显示名称或别名。</span><span class="sxs-lookup"><span data-stu-id="3fb51-247">The sender of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="from:randiw"&$select=subject,from`][search-from-example]
| <span data-ttu-id="3fb51-248">**hasAttachment**</span><span class="sxs-lookup"><span data-stu-id="3fb51-248">**hasAttachment**</span></span> | <span data-ttu-id="3fb51-249">如果电子邮件附件不是内联附件，则为 true；否则，为 false。</span><span class="sxs-lookup"><span data-stu-id="3fb51-249">True if an email message contains an attachment that is not an inline attachment, false otherwise.</span></span> |[`me/messages?$search="hasAttachments=true"`][search-from-example]
| <span data-ttu-id="3fb51-250">**importance**</span><span class="sxs-lookup"><span data-stu-id="3fb51-250">**importance**</span></span>           | <span data-ttu-id="3fb51-251">发件人在发送邮件时可以指定的电子邮件重要性。</span><span class="sxs-lookup"><span data-stu-id="3fb51-251">The importance of an email message, which a sender can specify when sending a message.</span></span> <span data-ttu-id="3fb51-252">可取值包括 `low`、`medium` 或 `high`。</span><span class="sxs-lookup"><span data-stu-id="3fb51-252">The possible values are `low`, `medium`, or `high`.</span></span>|[`me/messages?$search="importance:high"&$select=subject,importance`][search-imp-example]
| <span data-ttu-id="3fb51-253">**Kind**</span><span class="sxs-lookup"><span data-stu-id="3fb51-253">**kind**</span></span>           | <span data-ttu-id="3fb51-254">邮件类型。</span><span class="sxs-lookup"><span data-stu-id="3fb51-254">The type of message.</span></span> <span data-ttu-id="3fb51-255">可取值包括 `contacts`、`docs`、`email`、`faxes`、`im`、`journals`、`meetings`、`notes`、`posts`、`rssfeeds`、`tasks` 或 `voicemail`。</span><span class="sxs-lookup"><span data-stu-id="3fb51-255">The possible values are `contacts`, `docs`, `email`, `faxes`, `im`, `journals`, `meetings`, `notes`, `posts`, `rssfeeds`, `tasks`, or `voicemail`.</span></span>|[`me/messages?$search="kind:voicemail"`][search-kind-example]
| <span data-ttu-id="3fb51-256">**participants**</span><span class="sxs-lookup"><span data-stu-id="3fb51-256">**participants**</span></span>           | <span data-ttu-id="3fb51-257">电子邮件的 **from**、**to**、**cc** 和 **bcc** 字段，可指定为 SMTP 地址、显示名称或别名。</span><span class="sxs-lookup"><span data-stu-id="3fb51-257">The **from**, **to**, **cc**, and **bcc** fields of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="participants:danas"`][search-part-example]
| <span data-ttu-id="3fb51-258">**received**</span><span class="sxs-lookup"><span data-stu-id="3fb51-258">**received**</span></span>           | <span data-ttu-id="3fb51-259">收件人接收电子邮件的日期。</span><span class="sxs-lookup"><span data-stu-id="3fb51-259">The date that an email message was received by a recipient.</span></span>|[`me/messages?$search="received:07/23/2018"&$select=subject,receivedDateTime`][search-rcvd-example]
| <span data-ttu-id="3fb51-260">**recipients**</span><span class="sxs-lookup"><span data-stu-id="3fb51-260">**recipients**</span></span>           | <span data-ttu-id="3fb51-261">电子邮件的 **to**、**cc** 和 **bcc** 字段，可指定为 SMTP 地址、显示名称或别名。</span><span class="sxs-lookup"><span data-stu-id="3fb51-261">The **to**, **cc**, and **bcc** fields of an email meesage, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="recipients:randiq"&$select=subject,toRecipients,ccRecipients,bccRecipients`][search-rcpts-example]
| <span data-ttu-id="3fb51-262">**sent**</span><span class="sxs-lookup"><span data-stu-id="3fb51-262">**sent**</span></span>           | <span data-ttu-id="3fb51-263">发件人发送电子邮件的日期。</span><span class="sxs-lookup"><span data-stu-id="3fb51-263">The date that an email message was sent by the sender.</span></span>|[`me/messages?$search="sent:07/23/2018"&$select=subject,sentDateTime`][search-sent-example]
| <span data-ttu-id="3fb51-264">**size**</span><span class="sxs-lookup"><span data-stu-id="3fb51-264">**size**</span></span>           | <span data-ttu-id="3fb51-265">邮件大小（以字节为单位）。</span><span class="sxs-lookup"><span data-stu-id="3fb51-265">The size of an item in bytes.</span></span>|[`me/messages?$search="size:1..500000"`][search-size-example]
| <span data-ttu-id="3fb51-266">**subject**</span><span class="sxs-lookup"><span data-stu-id="3fb51-266">**subject**</span></span>           | <span data-ttu-id="3fb51-267">电子邮件主题行中的文本。</span><span class="sxs-lookup"><span data-stu-id="3fb51-267">The text in the subject line of an email message.</span></span> <span data-ttu-id="3fb51-268">.</span><span class="sxs-lookup"><span data-stu-id="3fb51-268">.</span></span>|[`me/messages?$search="subject:has"&$select=subject`][search-sbj-example]
| <span data-ttu-id="3fb51-269">**to**</span><span class="sxs-lookup"><span data-stu-id="3fb51-269">**to**</span></span>           | <span data-ttu-id="3fb51-270">电子邮件的 **to** 字段，可指定为 SMTP 地址、显示名称或别名。</span><span class="sxs-lookup"><span data-stu-id="3fb51-270">The **to** field of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="to:randiw"&$select=subject,toRecipients`][search-to-example]


<span data-ttu-id="3fb51-271">若要详细了解 可搜索的电子邮件属性、KQL 语法、受支持的运算符和搜索技巧，请参阅以下文章：</span><span class="sxs-lookup"><span data-stu-id="3fb51-271">For more information about searchable email properties, KQL syntax, supported operators, and tips on searching, see the following articles:</span></span>

- <span data-ttu-id="3fb51-272">[Exchange 中的可搜索属性](https://docs.microsoft.com/zh-CN/Exchange/policy-and-compliance/ediscovery/message-properties-and-search-operators#searchable-properties-in-exchange)。</span><span class="sxs-lookup"><span data-stu-id="3fb51-272">[Searchable properties in Exchange](https://docs.microsoft.com/zh-CN/Exchange/policy-and-compliance/ediscovery/message-properties-and-search-operators#searchable-properties-in-exchange).</span></span>

- [<span data-ttu-id="3fb51-273">关键字查询语言 (KQL) 语法参考</span><span class="sxs-lookup"><span data-stu-id="3fb51-273">Keyword Query Language (KQL) syntax reference</span></span>](https://docs.microsoft.com/zh-CN/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference)

- <span data-ttu-id="3fb51-274">
  [Exchange 2016 中的就地电子数据展示的邮件属性和搜索运算符](https://technet.microsoft.com/en-us/library/dn774955(v=exchg.160).aspx)</span><span class="sxs-lookup"><span data-stu-id="3fb51-274">[Message properties and search operators for In-Place eDiscovery in Exchange 2016](https://technet.microsoft.com/en-us/library/dn774955(v=exchg.160).aspx)</span></span>

### <a name="using-search-on-person-collections"></a><span data-ttu-id="3fb51-275">对 person 集合使用 $search</span><span class="sxs-lookup"><span data-stu-id="3fb51-275">Using $search on person collections</span></span>

<span data-ttu-id="3fb51-p125">可以使用 Microsoft Graph People API 检索与用户相关度最高的人员。相关性由用户的通信和协作模式及业务关系决定。People API 支持 `$search` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="3fb51-p125">You can use the Microsoft Graph People API to retrieve the people who are most relevant to a user. Relevance is determined by the user’s communication and collaboration patterns and business relationships. The People API supports the `$search` query parameter.</span></span>

<span data-ttu-id="3fb51-279">人员搜索就是按 [person](/graph/api/resources/person?view=graph-rest-1.0) 资源的 **displayName** 和 **emailAddress** 属性进行搜索。</span><span class="sxs-lookup"><span data-stu-id="3fb51-279">Searches on people occur on both the **displayName** and **emailAddress** properties of the [person](/graph/api/resources/person?view=graph-rest-1.0) resource.</span></span>

<span data-ttu-id="3fb51-280">以下请求在已登录用户的**人员**集合中的每个人员的 **displayName** 和 **emailAddress** 属性中，为名为“Irene McGowen”的人员执行搜索。</span><span class="sxs-lookup"><span data-stu-id="3fb51-280">The following request does a search for a person named "Irene McGowen" in the **displayName** and **emailAddress** properties in each person in the **people** collection of the signed-in user.</span></span> <span data-ttu-id="3fb51-281">由于一个名为“Irene McGowan”的人员与登录用户相关，因此返回了“Irene McGowan”的信息。</span><span class="sxs-lookup"><span data-stu-id="3fb51-281">Because a person named "Irene McGowan" is relevant to the signed-in user, the information for "Irene McGowan" is returned.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="Irene McGowen"
```

<span data-ttu-id="3fb51-282">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="3fb51-282">The following example shows the response.</span></span> 

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
       {
           "id": "C0BD1BA1-A84E-4796-9C65-F8A0293741D1",
           "displayName": "Irene McGowan",
           "givenName": "Irene",
           "surname": "McGowan",
           "birthday": "",
           "personNotes": "",
           "isFavorite": false,
           "jobTitle": "Auditor",
           "companyName": null,
           "yomiCompany": "",
           "department": "Finance",
           "officeLocation": "12/1110",
           "profession": "",
           "userPrincipalName": "irenem@contoso.onmicrosoft.com",
           "imAddress": "sip:irenem@contoso.onmicrosoft.com",
           "scoredEmailAddresses": [
               {
                   "address": "irenem@contoso.onmicrosoft.com",
                   "relevanceScore": -16.446060612802224
               }
           ],
           "phones": [
               {
                   "type": "Business",
                   "number": "+1 412 555 0109"
               }
           ],
           "postalAddresses": [],
           "websites": [],
           "personType": {
               "class": "Person",
               "subclass": "OrganizationUser"
           }
       }
   ]
}
```

<span data-ttu-id="3fb51-283">若要了解有关 People API 的详细信息，请参阅[获取相关人员的信息](./people-example.md#search-people)。</span><span class="sxs-lookup"><span data-stu-id="3fb51-283">To learn more about the People API, see [Get information about relevant people](./people-example.md#search-people).</span></span>  

## <a name="select-parameter"></a><span data-ttu-id="3fb51-284">select 参数</span><span class="sxs-lookup"><span data-stu-id="3fb51-284">select parameter</span></span>

<span data-ttu-id="3fb51-285">使用 `$select` 查询参数返回一组不同于单个资源的默认集或资源集合的属性。</span><span class="sxs-lookup"><span data-stu-id="3fb51-285">Use the `$select` query parameter to return a set of properties that are different than the default set for an individual resource or a collection of resources.</span></span> <span data-ttu-id="3fb51-286">使用 $select，可以指定默认属性的子集或超集。</span><span class="sxs-lookup"><span data-stu-id="3fb51-286">With $select, you can specify a subset or a superset of the default properties.</span></span>

<span data-ttu-id="3fb51-287">例如，检索登录用户的邮件时，可以指定仅返回 **from** 和 **subject** 属性：</span><span class="sxs-lookup"><span data-stu-id="3fb51-287">For example, when retrieving the messages of the signed-in user, you can specify that only the **from** and **subject** properties be returned:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$select=from,subject
```

<span data-ttu-id="3fb51-288">[在 Graph 浏览器中试用][select-example]</span><span class="sxs-lookup"><span data-stu-id="3fb51-288">[Try in Graph Explorer][select-example]</span></span>

> <span data-ttu-id="3fb51-289">**重要说明：** 一般来说，建议使用 `$select` 将查询返回的属性限制为应用所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3fb51-289">**Important:** In general, we recommend that you use `$select` to limit the properties returned by a query to those needed by your app.</span></span> <span data-ttu-id="3fb51-290">这对于可能返回大型结果集的查询尤为有用。</span><span class="sxs-lookup"><span data-stu-id="3fb51-290">This is especially true of queries that might potentially return a large result set.</span></span> <span data-ttu-id="3fb51-291">限制每行返回的属性将减少网络负载并帮助提升应用的性能。</span><span class="sxs-lookup"><span data-stu-id="3fb51-291">Limiting the properties returned in each row will reduce network load and help improve your app's performance.</span></span>
>
> <span data-ttu-id="3fb51-p129">在 `v1.0` 中，从 [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0) 派生的一些 Azure AD 资源（如 [user](/graph/api/resources/user?view=graph-rest-1.0) 和 [group](/graph/api/resources/group?view=graph-rest-1.0)）在读取时返回受限的默认属性子集。对于这些资源，必须使用 `$select` 将属性返回到默认集之外。</span><span class="sxs-lookup"><span data-stu-id="3fb51-p129">In `v1.0`, some Azure AD resources that derive from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0), like [user](/graph/api/resources/user?view=graph-rest-1.0) and [group](/graph/api/resources/group?view=graph-rest-1.0), return a limited, default subset of properties on reads. For these resources, you must use `$select` to return properties outside of the default set.</span></span>  

## <a name="skip-parameter"></a><span data-ttu-id="3fb51-294">skip 参数</span><span class="sxs-lookup"><span data-stu-id="3fb51-294">skip parameter</span></span>

<span data-ttu-id="3fb51-p130">使用 `$skip` 查询参数设置要在集合开头跳过的项数。例如，以下请求返回按照创建日期排序的用户的事件，从集合中的第 21 个事件开始：</span><span class="sxs-lookup"><span data-stu-id="3fb51-p130">Use the `$skip` query parameter to set the number of items to skip at the start of a collection. For example, the following request returns events for the user sorted by date created, starting with the 21st event in the collection:</span></span>

```http
GET  https://graph.microsoft.com/v1.0/me/events?$orderby=createdDateTime&$skip=20
```
<span data-ttu-id="3fb51-297">[在 Graph 浏览器中试用][skip-example]</span><span class="sxs-lookup"><span data-stu-id="3fb51-297">[Try in Graph Explorer][skip-example]</span></span>

> <span data-ttu-id="3fb51-298">**注意：** 一些 Microsoft Graph API 使用 `$skip` 实现分页，如 Outlook 邮件和日历（**message**、**event** 和 **calendar**）。</span><span class="sxs-lookup"><span data-stu-id="3fb51-298">**Note:** Some Microsoft Graph APIs, like Outlook Mail and Calendars (**message**, **event**, and **calendar**), use `$skip` to implement paging.</span></span> <span data-ttu-id="3fb51-299">当查询结果跨多个页面时，这些 API 会返回 `@odata:nextLink` 属性，具有包含 `$skip` 参数的 URL。</span><span class="sxs-lookup"><span data-stu-id="3fb51-299">When results of a query span multiple pages, these APIs will return an `@odata:nextLink` property with a URL that contains a `$skip` parameter.</span></span> <span data-ttu-id="3fb51-300">可以使用此 URL 返回下一页结果。</span><span class="sxs-lookup"><span data-stu-id="3fb51-300">You can use this URL to return the next page of results.</span></span> <span data-ttu-id="3fb51-301">若要了解详细信息，请参阅[分页](./paging.md)。</span><span class="sxs-lookup"><span data-stu-id="3fb51-301">To learn more, see [Paging](./paging.md).</span></span>

## <a name="skiptoken-parameter"></a><span data-ttu-id="3fb51-302">skipToken 参数</span><span class="sxs-lookup"><span data-stu-id="3fb51-302">skipToken parameter</span></span>

<span data-ttu-id="3fb51-p132">由于服务器端分页或由于使用 [`$top`](#top-parameter) 参数来限制响应的页面大小，致使一些请求返回多页数据。许多 Microsoft Graph API 使用 `skipToken` 查询参数来引用结果的后续页面。`$skiptoken` 参数包含引用下一页结果的不透明令牌，并在响应的 `@odata.nextLink` 属性中提供的 URL 中返回。若要了解详细信息，请参阅[分页](./paging.md)。</span><span class="sxs-lookup"><span data-stu-id="3fb51-p132">Some requests return multiple pages of data either due to server-side paging or due to the use of the [`$top`](#top-parameter) parameter to limit the page size of the response. Many Microsoft Graph APIs use the `skipToken` query parameter to reference subsequent pages of the result. The `$skiptoken` parameter contains an opaque token that references the next page of results and is returned in the URL provided in the `@odata.nextLink` property in the response. To learn more, see [Paging](./paging.md).</span></span>


## <a name="top-parameter"></a><span data-ttu-id="3fb51-307">top 参数</span><span class="sxs-lookup"><span data-stu-id="3fb51-307">top parameter</span></span>

<span data-ttu-id="3fb51-308">使用 `$top` 查询参数指定结果集的页面大小。</span><span class="sxs-lookup"><span data-stu-id="3fb51-308">Use the `$top` query parameter to specify the page size of the result set.</span></span> 

<span data-ttu-id="3fb51-309">如果结果集中还剩余多个项目，则响应正文将包含 `@odata.nextLink` 参数。</span><span class="sxs-lookup"><span data-stu-id="3fb51-309">If more items remain in the result set, the response body will contain an `@odata.nextLink` parameter.</span></span> <span data-ttu-id="3fb51-310">此参数包含可用于获取下一页结果的 URL。</span><span class="sxs-lookup"><span data-stu-id="3fb51-310">This parameter contains a URL that you can use to get the next page of results.</span></span> <span data-ttu-id="3fb51-311">若要了解详细信息，请参阅[分页](./paging.md)。</span><span class="sxs-lookup"><span data-stu-id="3fb51-311">To learn more, see [Paging](./paging.md).</span></span> 

<span data-ttu-id="3fb51-312">例如，以下请求返回用户邮箱中的前 5 封邮件：</span><span class="sxs-lookup"><span data-stu-id="3fb51-312">For example, the following request returns the first five messages in the user's mailbox:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$top=5
```

<span data-ttu-id="3fb51-313">[在 Graph 浏览器中试用][top-example]</span><span class="sxs-lookup"><span data-stu-id="3fb51-313">[Try in Graph Explorer][top-example]</span></span>


## <a name="error-handling-for-query-parameters"></a><span data-ttu-id="3fb51-314">查询参数的错误处理</span><span class="sxs-lookup"><span data-stu-id="3fb51-314">Error handling for query parameters</span></span>

<span data-ttu-id="3fb51-p134">如果不支持指定的查询参数，某些请求将返回错误消息。例如，不能对 `user/photo` 关系使用 `$expand`。</span><span class="sxs-lookup"><span data-stu-id="3fb51-p134">Some requests will return an error message if a specified query parameter is not supported. For example, you cannot use `$expand` on the `user/photo` relationship.</span></span> 

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

<span data-ttu-id="3fb51-317">但是，值得注意的是请求中指定的查询参数可能会自行失败。</span><span class="sxs-lookup"><span data-stu-id="3fb51-317">However, it is important to note that query parameters specified in a request might fail silently.</span></span> <span data-ttu-id="3fb51-318">不支持的查询参数以及不支持的查询参数组合的情况就是如此。</span><span class="sxs-lookup"><span data-stu-id="3fb51-318">This can be true for unsupported query parameters as well as for unsupported combinations of query parameters.</span></span> <span data-ttu-id="3fb51-319">在这些情况下，应检查请求返回的数据，以确定指定的查询参数是否具有所需的效果。</span><span class="sxs-lookup"><span data-stu-id="3fb51-319">In these cases, you should examine the data returned by the request to determine whether the query parameters you specified had the desired effect.</span></span> 

[graph-explorer]: https://developer.microsoft.com/graph/graph-explorer
[odata-filter]: https://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752358
[odata-query]: https://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752356
[count-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$top=2%26$count=true&method=GET&version=v1.0
[expand-example]: https://developer.microsoft.com/graph/graph-explorer?request=groups?$expand=members&method=GET&version=v1.0
[filter-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(givenName,'J')&method=GET&version=v1.0
[format-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$format=json&method=GET&version=v1.0
[orderby-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$orderby=displayName%20DESC&method=GET&version=v1.0
[search-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=pizza&method=GET&version=v1.0
[select-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$select=givenName,surname&method=GET&version=v1.0
[skip-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$skip=11&method=GET&version=v1.0
[top-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$top=2&method=GET&version=v1.0

[search-att-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22attachment%3Aapi-catalog%2Emd%22&method=GET&version=v1.0
[search-bcc-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22bcc%3Asamanthab%40contoso%2Ecom%22%26$select=subject,bccRecipients&method=GET&version=v1.0
[search-body-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22body%3Aexcitement%22&method=GET&version=v1.0
[search-cc-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22cc%3Adanas%22%26$select=subject,ccRecipients&method=GET&version=v1.0
[search-from-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22from%3Arandiw%22%26$select=subject,from&method=GET&version=v1.0
[search-hasatt-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22hasAttachments=true%22&method=GET&version=v1.0
[search-imp-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22importance%3Ahigh%22%26$select=subject,importance&method=GET&version=v1.0
[search-kind-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22kind%3Avoicemail%22&method=GET&version=v1.0
[search-part-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22participants%3Adanas%22&method=GET&version=v1.0

[search-rcvd-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22received%3A07/23/2018%22%26$select=subject,receivedDateTime&method=GET&version=v1.0

[search-rcpts-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22recipients%3Arandiw%22%26$select=subject,toRecipients,ccRecipients,bccRecipients&method=GET&version=v1.0
[search-sent-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22sent%3A07/23/2018%22%26$select=subject,sentDateTime&method=GET&version=v1.0
[search-size-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22size%3A1%2E%2E500000%22&method=GET&version=v1.0

[search-sbj-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22subject%3Ahas%22%26$select=subject&method=GET&version=v1.
[search-to-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22to%3Arandiw%22%26$select=subject,toRecipients&method=GET&version=v1.0

