---
title: 使用查询参数自定义响应
description: Microsoft Graph 提供可选的查询参数，可用于指定和控制响应中返回的数据量。
author: mumbi-o
localization_priority: Priority
ms.custom: graphiamtop20, scenarios:getting-started
ms.openlocfilehash: 51bf43360c3580011ab39e2c385b4c23d3bfc5a1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962411"
---
# <a name="use-query-parameters-to-customize-responses"></a><span data-ttu-id="ab3e3-103">使用查询参数自定义响应</span><span class="sxs-lookup"><span data-stu-id="ab3e3-103">Use query parameters to customize responses</span></span>

<span data-ttu-id="ab3e3-104">Microsoft Graph 支持可选的查询参数，可用于指定和控制响应中返回的数据量。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-104">Microsoft Graph supports optional query parameters that you can use to specify and control the amount of data returned in a response.</span></span> <span data-ttu-id="ab3e3-105">对准确查询参数的支持因 API 操作不同而不同，并且可能会在 v1.0 和数据终结点之间不同，具体取决于 API。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-105">The support for the exact query parameters varies from one API operation to another, and depending on the API, can differ between the v1.0 and beta endpoints.</span></span> 

> [!TIP] 
> <span data-ttu-id="ab3e3-106">在 beta 终结点上，`$` 前缀是可选的。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-106">On the beta endpoint, the `$` prefix is optional.</span></span> <span data-ttu-id="ab3e3-107">例如，可使用 `filter` 来代替 `$filter`。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-107">For example, instead of `$filter`, you can use `filter`.</span></span> <span data-ttu-id="ab3e3-108">在 v1 终结点上, `$`前缀仅对 API 的一个子集是可选的。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-108">On the v1 endpoint, the `$` prefix is optional for only a subset of APIs.</span></span> <span data-ttu-id="ab3e3-109">为简单起见, 如果使用 v1 终结点, 请始终包含`$`。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-109">For simplicity, always include `$` if using the v1 endpoint.</span></span>

<span data-ttu-id="ab3e3-110">查询参数可以是 OData 系统查询选项，也可以是其他查询参数。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-110">Query parameters can be OData system query options or other query parameters.</span></span> 

> [!VIDEO https://www.youtube-nocookie.com/embed/7BuFv3yETi4]

## <a name="odata-system-query-options"></a><span data-ttu-id="ab3e3-111">OData 系统查询选项</span><span class="sxs-lookup"><span data-stu-id="ab3e3-111">OData system query options</span></span>
<span data-ttu-id="ab3e3-112">Microsoft Graph API 操作可以支持以下一个或多个 OData 系统查询选项。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-112">A Microsoft Graph API operation might support one or more of the following OData system query options.</span></span> <span data-ttu-id="ab3e3-113">这些查询选项与 [OData V4 查询语言][odata-query]兼容。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-113">These query options are compatible with the [OData V4 query language][odata-query].</span></span>

><span data-ttu-id="ab3e3-114">**注意：** OData 4.0 仅在 GET 操作中支持系统查询选项。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-114">**Note:** OData 4.0 supports system query options in only GET operations.</span></span>

<span data-ttu-id="ab3e3-115">单击示例可以在 [Graph 浏览器][graph-explorer]中试调用它们。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-115">Click the examples to try them in [Graph Explorer][graph-explorer].</span></span>

| <span data-ttu-id="ab3e3-116">名称</span><span class="sxs-lookup"><span data-stu-id="ab3e3-116">Name</span></span>                     | <span data-ttu-id="ab3e3-117">说明</span><span class="sxs-lookup"><span data-stu-id="ab3e3-117">Description</span></span> | <span data-ttu-id="ab3e3-118">示例</span><span class="sxs-lookup"><span data-stu-id="ab3e3-118">Example</span></span>
|:-------------------------|:------------|:---------|
| [<span data-ttu-id="ab3e3-119">$count</span><span class="sxs-lookup"><span data-stu-id="ab3e3-119">$count</span></span>](#count-parameter)         | <span data-ttu-id="ab3e3-120">检索匹配资源的总数。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-120">Retrieves the total count of matching resources.</span></span> | [`/me/messages?$top=2&$count=true`][count-example]
| [<span data-ttu-id="ab3e3-121">$expand</span><span class="sxs-lookup"><span data-stu-id="ab3e3-121">$expand</span></span>](#expand-parameter)       | <span data-ttu-id="ab3e3-122">检索相关资源。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-122">Retrieves related resources.</span></span>|[`/groups?$expand=members`][expand-example]
| [<span data-ttu-id="ab3e3-123">$filter</span><span class="sxs-lookup"><span data-stu-id="ab3e3-123">$filter</span></span>](#filter-parameter)       | <span data-ttu-id="ab3e3-124">筛选结果（行）。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-124">Filters results (rows).</span></span>|[`/users?$filter=startswith(givenName,'J')`][filter-example]
| [<span data-ttu-id="ab3e3-125">$format</span><span class="sxs-lookup"><span data-stu-id="ab3e3-125">$format</span></span>](#format-parameter)       | <span data-ttu-id="ab3e3-126">返回指定媒体格式的结果。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-126">Returns the results in the specified media format.</span></span>|[`/users?$format=json`][format-example]
| [<span data-ttu-id="ab3e3-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="ab3e3-127">$orderby</span></span>](#orderby-parameter)     | <span data-ttu-id="ab3e3-128">对结果进行排序。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-128">Orders results.</span></span>|[`/users?$orderby=displayName desc`][orderby-example]
| [<span data-ttu-id="ab3e3-129">$search</span><span class="sxs-lookup"><span data-stu-id="ab3e3-129">$search</span></span>](#search-parameter)       | <span data-ttu-id="ab3e3-130">返回基于搜索条件的结果。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-130">Returns results based on search criteria.</span></span> |[`/me/messages?$search=pizza`][search-example]
| [<span data-ttu-id="ab3e3-131">$select</span><span class="sxs-lookup"><span data-stu-id="ab3e3-131">$select</span></span>](#select-parameter)       | <span data-ttu-id="ab3e3-132">筛选属性（列）。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-132">Filters properties (columns).</span></span>|[`/users?$select=givenName,surname`][select-example]
| [<span data-ttu-id="ab3e3-133">$skip</span><span class="sxs-lookup"><span data-stu-id="ab3e3-133">$skip</span></span>](#skip-parameter)           | <span data-ttu-id="ab3e3-p104">对结果集建立索引。一些 API 也使用它来实现分页，并且可以与 `$top` 一起使用来手动对结果分页。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-p104">Indexes into a result set. Also used by some APIs to implement paging and can be used together with `$top` to manually page results.</span></span> | [`/me/messages?$skip=11`][skip-example]
| [<span data-ttu-id="ab3e3-136">$top</span><span class="sxs-lookup"><span data-stu-id="ab3e3-136">$top</span></span>](#top-parameter)             | <span data-ttu-id="ab3e3-137">设置结果的页面大小。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-137">Sets the page size of results.</span></span> |[`/users?$top=2`][top-example]


## <a name="other-query-parameters"></a><span data-ttu-id="ab3e3-138">其他查询参数</span><span class="sxs-lookup"><span data-stu-id="ab3e3-138">Other query parameters</span></span>

| <span data-ttu-id="ab3e3-139">名称</span><span class="sxs-lookup"><span data-stu-id="ab3e3-139">Name</span></span>                     | <span data-ttu-id="ab3e3-140">说明</span><span class="sxs-lookup"><span data-stu-id="ab3e3-140">Description</span></span> | <span data-ttu-id="ab3e3-141">示例</span><span class="sxs-lookup"><span data-stu-id="ab3e3-141">Example</span></span>
|:-------------------------|:------------|:---------|
| [<span data-ttu-id="ab3e3-142">$skipToken</span><span class="sxs-lookup"><span data-stu-id="ab3e3-142">$skipToken</span></span>](#skiptoken-parameter) | <span data-ttu-id="ab3e3-p105">从跨多页的结果集中检索下一页结果。（但某些 API 改为使用 `$skip`。）</span><span class="sxs-lookup"><span data-stu-id="ab3e3-p105">Retrieves the next page of results from result sets that span multiple pages. (Some APIs use `$skip` instead.)</span></span> | `/users?$skiptoken=X%274453707402000100000017...`|

## <a name="other-odata-url-capabilities"></a><span data-ttu-id="ab3e3-145">其他 OData URL 功能</span><span class="sxs-lookup"><span data-stu-id="ab3e3-145">Other OData URL capabilities</span></span>

<span data-ttu-id="ab3e3-146">下列 OData 4.0 功能是 URL 区段，不是查询参数。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-146">The following OData 4.0 capabilities are URL segments, not query parameters.</span></span>

| <span data-ttu-id="ab3e3-147">名称</span><span class="sxs-lookup"><span data-stu-id="ab3e3-147">Name</span></span>                     | <span data-ttu-id="ab3e3-148">说明</span><span class="sxs-lookup"><span data-stu-id="ab3e3-148">Description</span></span> | <span data-ttu-id="ab3e3-149">示例</span><span class="sxs-lookup"><span data-stu-id="ab3e3-149">Example</span></span> 
|:-------------------------|:------------|:---------|
| [<span data-ttu-id="ab3e3-150">$ref</span><span class="sxs-lookup"><span data-stu-id="ab3e3-150">$ref</span></span>](/graph/api/group-post-members) | <span data-ttu-id="ab3e3-151">更新实体成员身份至集合。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-151">Updates entities membership to a collection.</span></span> | `POST /groups/{id}/members/$ref` |
| [<span data-ttu-id="ab3e3-152">$value</span><span class="sxs-lookup"><span data-stu-id="ab3e3-152">$value</span></span>](/graph/api/profilephoto-get) | <span data-ttu-id="ab3e3-153">检索或更新项的二进制值。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-153">Retrieves or updates the binary value of an item.</span></span> | `GET /me/photo/$value` |

## <a name="encoding-query-parameters"></a><span data-ttu-id="ab3e3-154">对查询参数进行编码</span><span class="sxs-lookup"><span data-stu-id="ab3e3-154">Encoding query parameters</span></span>

<span data-ttu-id="ab3e3-155">应对查询参数的值进行百分比编码。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-155">The values of query parameters should be percent-encoded.</span></span> <span data-ttu-id="ab3e3-156">许多 HTTP 客户端、浏览器和工具（如 [Graph 浏览器][graph-explorer]）将在这方面帮助你。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-156">Many HTTP clients, browsers, and tools (such as the [Graph Explorer][graph-explorer]) will help you with this.</span></span> <span data-ttu-id="ab3e3-157">如果查询失败，可能原因之一是未正确编码查询参数值。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-157">If a query is failing, one possible cause is failure to encode the query parameter values appropriately.</span></span>

<span data-ttu-id="ab3e3-158">未编码的 URL 如下所示：</span><span class="sxs-lookup"><span data-stu-id="ab3e3-158">An unencoded URL looks like this:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName, 'J')
```

<span data-ttu-id="ab3e3-159">正确解码的 URL 如下所示：</span><span class="sxs-lookup"><span data-stu-id="ab3e3-159">A properly encoded URL looks like this:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName%2C+'J')
```

### <a name="escaping-single-quotes"></a><span data-ttu-id="ab3e3-160">转义单引号</span><span class="sxs-lookup"><span data-stu-id="ab3e3-160">Escaping single quotes</span></span>

<span data-ttu-id="ab3e3-161">对于使用单引号的请求，如果任何参数值也包含单引号，则必须进行双转义；否则，由于语法无效，请求将失败。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-161">For requests that use single quotes, if any parameter values also contain single quotes, those must be double escaped; otherwise, the request will fail due to invalid syntax.</span></span> <span data-ttu-id="ab3e3-162">在示例中，字符串值 `let''s meet for lunch?` 进行了单引号转义。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-162">In the example, the string value `let''s meet for lunch?` has the single quote escaped.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=subject eq 'let''s meet for lunch?'
```

## <a name="count-parameter"></a><span data-ttu-id="ab3e3-163">count 参数</span><span class="sxs-lookup"><span data-stu-id="ab3e3-163">count parameter</span></span>

<span data-ttu-id="ab3e3-164">使用 `$count` 查询参数以包括集合中项总数的计数，以及从 Microsoft Graph 返回的数据值页。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-164">Use the `$count` query parameter to include a count of the total number of items in a collection alongside the page of data values returned from Microsoft Graph.</span></span> 

<span data-ttu-id="ab3e3-165">例如，下面的请求返回当前用户的 **contact** 集合，以及 `@odata.count` 属性中 **contact** 集合内的项数。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-165">For example, the following request returns both the **contact** collection of the current user, and the number of items in the **contact** collection in the `@odata.count` property.</span></span>

```http
GET  https://graph.microsoft.com/v1.0/me/contacts?$count=true
```

[<span data-ttu-id="ab3e3-166">在 Graph 浏览器中试调用</span><span class="sxs-lookup"><span data-stu-id="ab3e3-166">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/contacts?$count=true&method=GET&version=v1.0)


<span data-ttu-id="ab3e3-167">`$count`查询参数支持这些资源集合和它们的关系派生[自directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta&preserve-view=true)：</span><span class="sxs-lookup"><span data-stu-id="ab3e3-167">The `$count` query parameter is supported for these collections of resources and their relationships that derive from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta&preserve-view=true):</span></span>
- [<span data-ttu-id="ab3e3-168">application</span><span class="sxs-lookup"><span data-stu-id="ab3e3-168">application</span></span>](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true)
- [<span data-ttu-id="ab3e3-169">orgContact</span><span class="sxs-lookup"><span data-stu-id="ab3e3-169">orgContact</span></span>](/graph/api/resources/orgcontact?view=graph-rest-beta&preserve-view=true)
- [<span data-ttu-id="ab3e3-170">设备</span><span class="sxs-lookup"><span data-stu-id="ab3e3-170">device</span></span>](/graph/api/resources/device?view=graph-rest-beta&preserve-view=true)
- [<span data-ttu-id="ab3e3-171">组</span><span class="sxs-lookup"><span data-stu-id="ab3e3-171">group</span></span>](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true)
- [<span data-ttu-id="ab3e3-172">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="ab3e3-172">servicePrincipal</span></span>](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true)
- <span data-ttu-id="ab3e3-173">[用户](/graph/api/resources/user?view=graph-rest-beta&preserve-view=true)。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-173">[users](/graph/api/resources/user?view=graph-rest-beta&preserve-view=true).</span></span>

## <a name="expand-parameter"></a><span data-ttu-id="ab3e3-174">expand 参数</span><span class="sxs-lookup"><span data-stu-id="ab3e3-174">expand parameter</span></span>

<span data-ttu-id="ab3e3-175">许多 Microsoft Graph 资源都会公开资源的已声明属性以及与其他资源的关系。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-175">Many Microsoft Graph resources expose both declared properties of the resource as well as its relationships with other resources.</span></span> <span data-ttu-id="ab3e3-176">这些关系也称为引用属性或导航属性，它们可以引用单个资源或资源集合。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-176">These relationships are also called reference properties or navigation properties, and they can reference either a single resource or a collection of resources.</span></span> <span data-ttu-id="ab3e3-177">例如，用户的邮件文件夹、管理者和直接下属都将作为关系公开。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-177">For example, the mail folders, manager, and direct reports of a user are all exposed as relationships.</span></span> 

<span data-ttu-id="ab3e3-p109">通常情况下，可以在单个请求中查询资源属性或其关系之一，但不能同时查询。可以使用 `$expand` 查询字符串参数以包含结果中单个关系（导航属性）引用的扩展资源或集合。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-p109">Normally, you can query either the properties of a resource or one of its relationships in a single request, but not both. You can use the `$expand` query string parameter to include the expanded resource or collection referenced by a single relationship (navigation property) in your results.</span></span>

<span data-ttu-id="ab3e3-180">以下示例在驱动器中获取根驱动器信息以及顶级子项：</span><span class="sxs-lookup"><span data-stu-id="ab3e3-180">The following example gets root drive information along with the top-level child items in a drive:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children
```

[<span data-ttu-id="ab3e3-181">在 Graph 浏览器中试调用</span><span class="sxs-lookup"><span data-stu-id="ab3e3-181">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/drive/root?$expand=children&method=GET&version=v1.0)

<span data-ttu-id="ab3e3-p110">使用一些资源集合，还可以添加 `$select` 参数，指定要在扩展资源中返回的属性。下面的示例执行与上一示例几乎相同的查询，不同之处在于使用 [`$select`](#select-parameter) 语句将为扩展子项返回的属性限制为 **id** 和 **name** 属性。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-p110">With some resource collections, you can also specify the properties to be returned in the expanded resources by adding a `$select` parameter. The following example performs the same query as the previous example but uses a [`$select`](#select-parameter) statement to limit the properties returned for the expanded child items to the **id** and **name** properties.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children($select=id,name)
```

<span data-ttu-id="ab3e3-184">[在 Graph 浏览器中试调用][expand-example]</span><span class="sxs-lookup"><span data-stu-id="ab3e3-184">[Try in Graph Explorer][expand-example]</span></span>

> <span data-ttu-id="ab3e3-p111">**注意：** 并不是所有关系和资源都支持 `$expand` 查询参数。例如，可以扩展用户的 **directReports**、**manager** 和 **memberOf** 关系，但无法扩展其 **events**、**messages** 或 **photo** 关系。并非所有资源或关系都支持对扩展项使用 `$select`。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-p111">**Note:** Not all relationships and resources support the `$expand` query parameter. For example, you can expand the **directReports**, **manager**, and **memberOf** relationships on a user, but you cannot expand its **events**, **messages**, or **photo** relationships. Not all resources or relationships support using `$select` on expanded items.</span></span> 
> 
> <span data-ttu-id="ab3e3-188">使用从 [directoryObject](/graph/api/resources/directoryobject) 派生的 Azure AD 资源（如[user](/graph/api/resources/user) 和 [group](/graph/api/resources/group)），`$expand` 仅支持 `beta`，并且通常最多为扩展关系返回 20 个项。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-188">With Azure AD resources that derive from [directoryObject](/graph/api/resources/directoryobject), like [user](/graph/api/resources/user) and [group](/graph/api/resources/group), `$expand` is only supported for `beta` and  typically returns a maximum of 20 items for the expanded relationship.</span></span>

## <a name="filter-parameter"></a><span data-ttu-id="ab3e3-189">filter 参数</span><span class="sxs-lookup"><span data-stu-id="ab3e3-189">filter parameter</span></span>

<span data-ttu-id="ab3e3-190">使用 `$filter` 查询参数，以仅检索集合的子集。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-190">Use the `$filter` query parameter to retrieve just a subset of a collection.</span></span> <span data-ttu-id="ab3e3-191">`$filter`查询参数还可以用于检索关系，例如members、memberOf、transitiveMembers和transitiveMemberOf。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-191">The `$filter` query parameter can also be used to retrieve relationships like members, memberOf, transitiveMembers, and transitiveMemberOf.</span></span> <span data-ttu-id="ab3e3-192">例如，获取我所属的所有安全组。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-192">For example, get all the security groups I'm a member of.</span></span>

<span data-ttu-id="ab3e3-193">以下例子可用于查找显示名称以子母“J”开头的用户，请使用 `startsWith`。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-193">The following example can be used to find users whose display name starts with the letter 'J', use `startsWith`.</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startsWith(displayName,'J')
```

<span data-ttu-id="ab3e3-194">[在 Graph 浏览器中试调用][filter-example]</span><span class="sxs-lookup"><span data-stu-id="ab3e3-194">[Try in Graph Explorer][filter-example]</span></span>

<span data-ttu-id="ab3e3-195">对 `$filter` 运算符的支持因 Microsoft Graph API 不同而异。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-195">Support for `$filter` operators varies across Microsoft Graph APIs.</span></span> <span data-ttu-id="ab3e3-196">通常支持下列逻辑运算符：</span><span class="sxs-lookup"><span data-stu-id="ab3e3-196">The following logical operators are generally supported:</span></span>

- <span data-ttu-id="ab3e3-197">等于 `eq`/不等于 `ne`</span><span class="sxs-lookup"><span data-stu-id="ab3e3-197">equals `eq` / not equals `ne`</span></span>
- <span data-ttu-id="ab3e3-198">小于 `lt`/大于 `gt`</span><span class="sxs-lookup"><span data-stu-id="ab3e3-198">less than `lt` / greater than `gt`</span></span>
- <span data-ttu-id="ab3e3-199">小于或等于 `le`/大于或等于 `ge`</span><span class="sxs-lookup"><span data-stu-id="ab3e3-199">less than or equal to `le` / greater than or equal to `ge`</span></span>
- <span data-ttu-id="ab3e3-200">和 `and`/或 `or`</span><span class="sxs-lookup"><span data-stu-id="ab3e3-200">and `and` / or `or`</span></span>
- <span data-ttu-id="ab3e3-201">属于 `in`</span><span class="sxs-lookup"><span data-stu-id="ab3e3-201">in `in`</span></span>
- <span data-ttu-id="ab3e3-202">否定式 `not`</span><span class="sxs-lookup"><span data-stu-id="ab3e3-202">Negation `not`</span></span>
- <span data-ttu-id="ab3e3-203">l匿名函数运算符 any `any`</span><span class="sxs-lookup"><span data-stu-id="ab3e3-203">lambda operator any `any`</span></span>
- <span data-ttu-id="ab3e3-204">l匿名函数运算符 all `all`</span><span class="sxs-lookup"><span data-stu-id="ab3e3-204">lambda operator all `all`</span></span>
- <span data-ttu-id="ab3e3-205">开头为 `startsWith`</span><span class="sxs-lookup"><span data-stu-id="ab3e3-205">Starts with `startsWith`</span></span>
- <span data-ttu-id="ab3e3-206">结尾为 `endsWith`</span><span class="sxs-lookup"><span data-stu-id="ab3e3-206">Ends with `endsWith`</span></span>

> <span data-ttu-id="ab3e3-207">**注意：** 对这些运算符的支持因实体而异。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-207">**Note:** Support for these operators varies by entity.</span></span> <span data-ttu-id="ab3e3-208">有关详细信息，请参阅特定实体文档。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-208">See the specific entity documentation for details.</span></span> 
>
> <span data-ttu-id="ab3e3-209">所有 Microsoft Graph 资源目前均不支持 `contains` 字符串运算符。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-209">The `contains` string operator is currently not supported on any Microsoft Graph resources.</span></span>

<span data-ttu-id="ab3e3-210">有关一些用法示例的信息，请参阅下表。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-210">For some usage examples, see the following table.</span></span> <span data-ttu-id="ab3e3-211">如需了解 `$filter` 语法的更多详情，请参阅 [OData 协议][odata-filter]。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-211">For more details about `$filter` syntax, see the [OData protocol][odata-filter].</span></span>  
<span data-ttu-id="ab3e3-212">下表展示了一些使用 `$filter` 查询参数的示例。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-212">The following table shows some examples that use the `$filter` query parameter.</span></span>

> <span data-ttu-id="ab3e3-213">**注意：** 单击示例可以在 [Graph 浏览器][graph-explorer]中试调用。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-213">**Note:** Click the examples to try them in [Graph Explorer][graph-explorer].</span></span>

| <span data-ttu-id="ab3e3-214">说明</span><span class="sxs-lookup"><span data-stu-id="ab3e3-214">Description</span></span> | <span data-ttu-id="ab3e3-215">示例</span><span class="sxs-lookup"><span data-stu-id="ab3e3-215">Example</span></span>
|:------------|:--------|
| <span data-ttu-id="ab3e3-216">跨多个属性获取名为 Mary 的用户。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-216">Get all users with the name Mary across multiple properties.</span></span> | [`https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'mary') or startswith(givenName,'mary') or startswith(surname,'mary') or startswith(mail,'mary') or startswith(userPrincipalName,'mary')`](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(displayName,'mary')+or+startswith(givenName,'mary')+or+startswith(surname,'mary')+or+startswith(mail,'mary')+or+startswith(userPrincipalName,'mary')&method=GET&version=v1.0) |
| <span data-ttu-id="ab3e3-217">获取邮件域等于“hotmail.com”的所有用户</span><span class="sxs-lookup"><span data-stu-id="ab3e3-217">Get all users with mail domain equal to 'hotmail.com'</span></span> | [`https://graph.microsoft.com/v1.0/users?$count=true&$filter=endsWith(mail,'@hotmail.com')`](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24count%3Dtrue%26%24filter%3DendsWith(mail%2C'%40hotmail.com')%26%24select%3Did%2CdisplayName%2Cmail&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) |
| <span data-ttu-id="ab3e3-218">获取 2017 年 7 月 1 日之后开始的所有登录用户的事件。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-218">Get all the signed-in user's events that start after 7/1/2017.</span></span> | [`https://graph.microsoft.com/v1.0/me/events?$filter=start/dateTime ge '2017-07-01T08:00'`](https://developer.microsoft.com/graph/graph-explorer?request=me/events?$filter=start/dateTime+ge+'2017-07-01T08:00'&method=GET&version=v1.0) |
| <span data-ttu-id="ab3e3-219">获取登录用户收到的来自特定地址的所有电子邮件。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-219">Get all emails from a specific address received by the signed-in user.</span></span> | [`https://graph.microsoft.com/v1.0/me/messages?$filter=from/emailAddress/address eq 'someuser@example.com'`](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=from/emailAddress/address+eq+'someuser@.com'&method=GET&version=v1.0) |
| <span data-ttu-id="ab3e3-220">获取登录用户在 2017 年 4 月收到的所有电子邮件。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-220">Get all emails received by the signed-in user in April 2017.</span></span> | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=ReceivedDateTime ge 2017-04-01 and receivedDateTime lt 2017-05-01`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=ReceivedDateTime+ge+2017-04-01+and+receivedDateTime+lt+2017-05-01&method=GET&version=v1.0) |
| <span data-ttu-id="ab3e3-221">获取登录用户收件箱中的所有未读邮件。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-221">Get all unread mail in the signed-in user's Inbox.</span></span> | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=isRead eq false`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=isRead+eq+false&method=GET&version=v1.0) |
| <span data-ttu-id="ab3e3-222">列出组织中的所有 Microsoft 365 组。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-222">List all Microsoft 365 groups in an organization.</span></span> | [`https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')`](https://developer.microsoft.com/graph/graph-explorer?request=groups?$filter=groupTypes/any(c:c+eq+'Unified')&method=GET&version=v1.0) |
| <span data-ttu-id="ab3e3-223">使用 OData 转换可实现显示名称以“ a”开头（包括返回的对象数）的组中的临时成员资格。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-223">Use OData cast to get transitive membership in groups with a display name that starts with 'a' including a count of returned objects.</span></span> | [`https://graph.microsoft.com/beta/me/transitiveMemberOf/microsoft.graph.group?$count=true&$filter=startswith(displayName, 'a')`](https://developer.microsoft.com/graph/graph-explorer?request=me/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName,'a')&method=GET&version=v1.0) |

## <a name="format-parameter"></a><span data-ttu-id="ab3e3-224">format 参数</span><span class="sxs-lookup"><span data-stu-id="ab3e3-224">format parameter</span></span>

<span data-ttu-id="ab3e3-225">使用 `$format` 查询参数，指定 Microsoft Graph 返回的项的媒体格式。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-225">Use the `$format` query parameter to specify the media format of the items returned from Microsoft Graph.</span></span>

<span data-ttu-id="ab3e3-226">例如，下面的请求以 json 格式返回组织中的用户：</span><span class="sxs-lookup"><span data-stu-id="ab3e3-226">For example, the following request returns the users in the organization in the json format:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$format=json
```

<span data-ttu-id="ab3e3-227">[在 Graph 浏览器中试调用][format-example]</span><span class="sxs-lookup"><span data-stu-id="ab3e3-227">[Try in Graph Explorer][format-example]</span></span>

> <span data-ttu-id="ab3e3-228">**注意：**`$format` 查询参数支持许多格式（例如，atom、xml 和 json），但可能无法返回所有格式的结果。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-228">**Note:** The `$format` query parameter supports a number of formats (for example, atom, xml, and json) but results may not be returned in all formats.</span></span>

## <a name="orderby-parameter"></a><span data-ttu-id="ab3e3-229">orderby 参数</span><span class="sxs-lookup"><span data-stu-id="ab3e3-229">orderby parameter</span></span>

<span data-ttu-id="ab3e3-230">使用 `$orderby` 查询参数指定从 Microsoft Graph 返回的项的排序顺序。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-230">Use the `$orderby` query parameter to specify the sort order of the items returned from Microsoft Graph.</span></span>

<span data-ttu-id="ab3e3-231">例如，以下请求返回按用户显示名称进行排序的组织中的用户：</span><span class="sxs-lookup"><span data-stu-id="ab3e3-231">For example, the following request returns the users in the organization ordered by their display name:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$orderby=displayName
```
<span data-ttu-id="ab3e3-232">[在 Graph 浏览器中试调用][orderby-example]</span><span class="sxs-lookup"><span data-stu-id="ab3e3-232">[Try in Graph Explorer][orderby-example]</span></span>

<span data-ttu-id="ab3e3-p116">还可以按复杂类型实体进行排序。下面的请求获取邮件，并按 **from** 属性的 **address** 字段（复杂类型为 **emailAddress**）进行排序：</span><span class="sxs-lookup"><span data-stu-id="ab3e3-p116">You can also sort by complex type entities. The following request gets messages and sorts them by the **address** field of the **from** property, which is of the complex type **emailAddress**:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$orderby=from/emailAddress/address
```
[<span data-ttu-id="ab3e3-235">在 Graph 浏览器中试调用</span><span class="sxs-lookup"><span data-stu-id="ab3e3-235">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/address&method=GET&version=v1.0)

<span data-ttu-id="ab3e3-236">若要以升序或降序对结果进行排序，请向字段名称追加 `asc` 或 `desc`，并用空格隔开。例如，`?$orderby=name%20desc`。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-236">To sort the results in ascending or descending order, append either `asc` or `desc` to the field name, separated by a space; for example, `?$orderby=name%20desc`.</span></span>

<span data-ttu-id="ab3e3-237">通过一些 API，可以对多个属性的结果进行排序。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-237">With some APIs, you can order results on multiple properties.</span></span> <span data-ttu-id="ab3e3-238">例如，以下请求首先按发件人名称以降序（Z 到 A）排序用户收件箱中的邮件，然后按主题以升序（默认）排序邮件。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-238">For example, the following request orders the messages in the user's Inbox, first by the name of the person who sent it in descending order (Z to A), and then by subject in ascending order (default).</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/Inbox/messages?$orderby=from/emailAddress/name desc,subject
```

[<span data-ttu-id="ab3e3-239">在 Graph 浏览器中试调用</span><span class="sxs-lookup"><span data-stu-id="ab3e3-239">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/name%20desc,subject&method=GET&version=v1.0)

> <span data-ttu-id="ab3e3-240">**注意：** 如果指定 $filter，服务器会推断结果的排序顺序。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-240">**Note:** When you specify $filter the server will infer a sort order for the results.</span></span> <span data-ttu-id="ab3e3-241">如果同时使用 `$orderby` 和 `$filter` 获取消息，因为服务器始终会推断 `$filter` 结果的排序顺序，必须[以特定的方式指定属性](/graph/api/user-list-messages#using-filter-and-orderby-in-the-same-query)。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-241">If you use both `$orderby` and `$filter` to get messages, because the server always infers a sort order for the results of a `$filter`, you must [specify properties in certain ways](/graph/api/user-list-messages#using-filter-and-orderby-in-the-same-query).</span></span>


<span data-ttu-id="ab3e3-242">下面的示例展示了如何按 **subject** 和 **importance** 属性筛选查询，再按 **subject**、**importance** 和 **receivedDateTime** 属性进行降序排序。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-242">The following example shows a query filtered by the **subject** and **importance** properties, and then sorted by the **subject**, **importance**, and **receivedDateTime** properties in descending order.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=Subject eq 'welcome' and importance eq 'normal'&$orderby=subject,importance,receivedDateTime desc
```

[<span data-ttu-id="ab3e3-243">在 Graph 浏览器中试调用</span><span class="sxs-lookup"><span data-stu-id="ab3e3-243">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=subject%20eq%20%27welcome%27%20and%20importance%20eq%20%27normal%27%20&$orderby=subject,importance,receivedDateTime%20desc&method=GET&version=v1.0)

> <span data-ttu-id="ab3e3-244">**注意：** 对于以下 AD 资源及其从 [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta&preserve-view=true) 派生的关系，在 Beta 终结点上支持组合 `$orderby` 和 `$filter` 查询参数：</span><span class="sxs-lookup"><span data-stu-id="ab3e3-244">**Note:** Combining `$orderby` and `$filter` query parameters is supported on the beta endpoint for the following AD resources and their relationships that derive from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta&preserve-view=true):</span></span>
>
>- [<span data-ttu-id="ab3e3-245">application</span><span class="sxs-lookup"><span data-stu-id="ab3e3-245">application</span></span>](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true)
>- [<span data-ttu-id="ab3e3-246">orgContact</span><span class="sxs-lookup"><span data-stu-id="ab3e3-246">orgContact</span></span>](/graph/api/resources/orgcontact?view=graph-rest-beta&preserve-view=true)
>- [<span data-ttu-id="ab3e3-247">设备</span><span class="sxs-lookup"><span data-stu-id="ab3e3-247">device</span></span>](/graph/api/resources/device?view=graph-rest-beta&preserve-view=true)
>- [<span data-ttu-id="ab3e3-248">组</span><span class="sxs-lookup"><span data-stu-id="ab3e3-248">group</span></span>](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true)
>- [<span data-ttu-id="ab3e3-249">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="ab3e3-249">servicePrincipal</span></span>](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true)
>- [<span data-ttu-id="ab3e3-250">用户</span><span class="sxs-lookup"><span data-stu-id="ab3e3-250">user</span></span>](/graph/api/resources/user?view=graph-rest-beta&preserve-view=true)
>
> <span data-ttu-id="ab3e3-251">若要将`$orderby``$filter`、或`$filter`与`endsWith`一，则需要：</span><span class="sxs-lookup"><span data-stu-id="ab3e3-251">To use `$orderby` and `$filter` together, or `$filter` with `endsWith` you need to:</span></span>
>
> - <span data-ttu-id="ab3e3-252">将 `$count=true` 添加到查询参数</span><span class="sxs-lookup"><span data-stu-id="ab3e3-252">Add `$count=true` to the query parameters</span></span>
> - <span data-ttu-id="ab3e3-253">添加 `ConsistencyLevel: eventual` 请求标题</span><span class="sxs-lookup"><span data-stu-id="ab3e3-253">Add `ConsistencyLevel: eventual` request header</span></span>
>
> <span data-ttu-id="ab3e3-254">有关更多信息，请参见[可选用户查询参数](/graph/api/user-list?view=graph-rest-beta&preserve-view=true#optional-query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-254">See [optional user query parameters](/graph/api/user-list?view=graph-rest-beta&preserve-view=true#optional-query-parameters) for more information.</span></span>

## <a name="search-parameter"></a><span data-ttu-id="ab3e3-255">search 参数</span><span class="sxs-lookup"><span data-stu-id="ab3e3-255">search parameter</span></span>

<span data-ttu-id="ab3e3-256">使用 `$search` 查询参数限制与搜索条件匹配的请求结果。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-256">Use the `$search` query parameter to restrict the results of a request to match a search criterion.</span></span>

### <a name="using-search-on-message-collections"></a><span data-ttu-id="ab3e3-257">对 message 集合使用 $search</span><span class="sxs-lookup"><span data-stu-id="ab3e3-257">Using $search on message collections</span></span>

<span data-ttu-id="ab3e3-258">可根据特定邮件属性值搜索邮件。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-258">You can search messages based on a value in specific message properties.</span></span> <span data-ttu-id="ab3e3-259">搜索结果按邮件发送日期和时间进行排序。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-259">The results of the search are sorted by the date and time that the message was sent.</span></span> <span data-ttu-id="ab3e3-260">`$search` 请求最多可返回 250 个结果。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-260">A `$search` request returns up to 250 results.</span></span>

<span data-ttu-id="ab3e3-261">如果确实要搜索邮件，且仅指定值，而未指定特定邮件属性，搜索依据为默认搜索属性 **from**、**subject** 和 **body**。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-261">If you do a search on messages and specify only a value without specific message properties, the search is carried out on the default search properties of **from**, **subject**, and **body**.</span></span>

<span data-ttu-id="ab3e3-262">下面的示例返回登录用户收件箱中三个默认搜索属性中有任意一个包含“pizza”的所有邮件：</span><span class="sxs-lookup"><span data-stu-id="ab3e3-262">The following example returns all messages in the signed-in user's Inbox that contains "pizza" in any of the three default search properties:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="pizza"
```

<span data-ttu-id="ab3e3-263">[在 Graph 浏览器中试调用][search-example]</span><span class="sxs-lookup"><span data-stu-id="ab3e3-263">[Try in Graph Explorer][search-example]</span></span>

<span data-ttu-id="ab3e3-264">也可以指定下表中的邮件属性名来搜索邮件，这些属性名可由关键字查询语言 (KQL) 语法识别。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-264">Alternatively, you can search messages by specifying message property names in the following table, that are recognized by the Keyword Query Language (KQL) syntax.</span></span> <span data-ttu-id="ab3e3-265">这些属性名对应于 Microsoft Graph **message** 实体中定义的属性。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-265">These property names correspond to properties defined in the **message** entity of Microsoft Graph.</span></span> <span data-ttu-id="ab3e3-266">Outlook 和其他 Microsoft 365 应用程序（如 SharePoint）支持 KQL 语法，从而为数据存储提供了方便使用的公共发现域。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-266">Outlook and other Microsoft 365 applications such as SharePoint support KQL syntax, providing the convenience of a common discovery domain for their data stores.</span></span>


| <span data-ttu-id="ab3e3-267">可搜索的电子邮件属性</span><span class="sxs-lookup"><span data-stu-id="ab3e3-267">Searchable email property</span></span>                | <span data-ttu-id="ab3e3-268">说明</span><span class="sxs-lookup"><span data-stu-id="ab3e3-268">Description</span></span> | <span data-ttu-id="ab3e3-269">示例</span><span class="sxs-lookup"><span data-stu-id="ab3e3-269">Example</span></span> 
|:-------------------------|:------------|:---------|
| <span data-ttu-id="ab3e3-270">**attachment**</span><span class="sxs-lookup"><span data-stu-id="ab3e3-270">**attachment**</span></span>           | <span data-ttu-id="ab3e3-271">电子邮件附件的文件名。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-271">The names of files attached to an email message.</span></span>|[`me/messages?$search="attachment:api-catalog.md"`][search-att-example]
| <span data-ttu-id="ab3e3-272">**bcc**</span><span class="sxs-lookup"><span data-stu-id="ab3e3-272">**bcc**</span></span>           | <span data-ttu-id="ab3e3-273">电子邮件的 **bcc** 字段，可指定为 SMTP 地址、显示名称或别名。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-273">The **bcc** field of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="bcc:samanthab@contoso.com"&$select=subject,bccRecipients`][search-bcc-example]
| <span data-ttu-id="ab3e3-274">**body**</span><span class="sxs-lookup"><span data-stu-id="ab3e3-274">**body**</span></span>           | <span data-ttu-id="ab3e3-275">电子邮件正文。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-275">The body of an email message.</span></span>|[`me/messages?$search="body:excitement"`][search-body-example]
| <span data-ttu-id="ab3e3-276">**cc**</span><span class="sxs-lookup"><span data-stu-id="ab3e3-276">**cc**</span></span>           | <span data-ttu-id="ab3e3-277">电子邮件的 **cc** 字段，可指定为 SMTP 地址、显示名称或别名。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-277">The **cc** field of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="cc:danas"&$select=subject,ccRecipients`][search-cc-example]
| <span data-ttu-id="ab3e3-278">**from**</span><span class="sxs-lookup"><span data-stu-id="ab3e3-278">**from**</span></span>           | <span data-ttu-id="ab3e3-279">电子邮件的发件人，可指定为 SMTP 地址、显示名称或别名。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-279">The sender of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="from:randiw"&$select=subject,from`][search-from-example]
| <span data-ttu-id="ab3e3-280">**hasAttachment**</span><span class="sxs-lookup"><span data-stu-id="ab3e3-280">**hasAttachment**</span></span> | <span data-ttu-id="ab3e3-281">如果电子邮件附件不是内联附件，则为 true；否则，为 false。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-281">True if an email message contains an attachment that is not an inline attachment, false otherwise.</span></span> |[`me/messages?$search="hasAttachments:true"`][search-from-example]
| <span data-ttu-id="ab3e3-282">**importance**</span><span class="sxs-lookup"><span data-stu-id="ab3e3-282">**importance**</span></span>           | <span data-ttu-id="ab3e3-283">发件人在发送邮件时可以指定的电子邮件重要性。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-283">The importance of an email message, which a sender can specify when sending a message.</span></span> <span data-ttu-id="ab3e3-284">可取值包括 `low`、`medium` 或 `high`。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-284">The possible values are `low`, `medium`, or `high`.</span></span>|[`me/messages?$search="importance:high"&$select=subject,importance`][search-imp-example]
| <span data-ttu-id="ab3e3-285">**Kind**</span><span class="sxs-lookup"><span data-stu-id="ab3e3-285">**kind**</span></span>           | <span data-ttu-id="ab3e3-286">邮件类型。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-286">The type of message.</span></span> <span data-ttu-id="ab3e3-287">可取值包括 `contacts`、`docs`、`email`、`faxes`、`im`、`journals`、`meetings`、`notes`、`posts`、`rssfeeds`、`tasks` 或 `voicemail`。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-287">The possible values are `contacts`, `docs`, `email`, `faxes`, `im`, `journals`, `meetings`, `notes`, `posts`, `rssfeeds`, `tasks`, or `voicemail`.</span></span>|[`me/messages?$search="kind:voicemail"`][search-kind-example]
| <span data-ttu-id="ab3e3-288">**participants**</span><span class="sxs-lookup"><span data-stu-id="ab3e3-288">**participants**</span></span>           | <span data-ttu-id="ab3e3-289">电子邮件的 **from**、**to**、**cc** 和 **bcc** 字段，可指定为 SMTP 地址、显示名称或别名。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-289">The **from**, **to**, **cc**, and **bcc** fields of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="participants:danas"`][search-part-example]
| <span data-ttu-id="ab3e3-290">**received**</span><span class="sxs-lookup"><span data-stu-id="ab3e3-290">**received**</span></span>           | <span data-ttu-id="ab3e3-291">收件人接收电子邮件的日期。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-291">The date that an email message was received by a recipient.</span></span>|[`me/messages?$search="received:07/23/2018"&$select=subject,receivedDateTime`][search-rcvd-example]
| <span data-ttu-id="ab3e3-292">**recipients**</span><span class="sxs-lookup"><span data-stu-id="ab3e3-292">**recipients**</span></span>           | <span data-ttu-id="ab3e3-293">电子邮件的 **to**、**cc** 和 **bcc** 字段，可指定为 SMTP 地址、显示名称或别名。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-293">The **to**, **cc**, and **bcc** fields of an email meesage, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="recipients:randiq"&$select=subject,toRecipients,ccRecipients,bccRecipients`][search-rcpts-example]
| <span data-ttu-id="ab3e3-294">**sent**</span><span class="sxs-lookup"><span data-stu-id="ab3e3-294">**sent**</span></span>           | <span data-ttu-id="ab3e3-295">发件人发送电子邮件的日期。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-295">The date that an email message was sent by the sender.</span></span>|[`me/messages?$search="sent:07/23/2018"&$select=subject,sentDateTime`][search-sent-example]
| <span data-ttu-id="ab3e3-296">**size**</span><span class="sxs-lookup"><span data-stu-id="ab3e3-296">**size**</span></span>           | <span data-ttu-id="ab3e3-297">邮件大小（以字节为单位）。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-297">The size of an item in bytes.</span></span>|[`me/messages?$search="size:1..500000"`][search-size-example]
| <span data-ttu-id="ab3e3-298">**subject**</span><span class="sxs-lookup"><span data-stu-id="ab3e3-298">**subject**</span></span>           | <span data-ttu-id="ab3e3-299">电子邮件主题行中的文本。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-299">The text in the subject line of an email message.</span></span> <span data-ttu-id="ab3e3-300">.</span><span class="sxs-lookup"><span data-stu-id="ab3e3-300">.</span></span>|[`me/messages?$search="subject:has"&$select=subject`][search-sbj-example]
| <span data-ttu-id="ab3e3-301">**to**</span><span class="sxs-lookup"><span data-stu-id="ab3e3-301">**to**</span></span>           | <span data-ttu-id="ab3e3-302">电子邮件的 **to** 字段，可指定为 SMTP 地址、显示名称或别名。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-302">The **to** field of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="to:randiw"&$select=subject,toRecipients`][search-to-example]


<span data-ttu-id="ab3e3-303">若要详细了解 可搜索的电子邮件属性、KQL 语法、受支持的运算符和搜索技巧，请参阅以下文章：</span><span class="sxs-lookup"><span data-stu-id="ab3e3-303">For more information about searchable email properties, KQL syntax, supported operators, and tips on searching, see the following articles:</span></span>

- <span data-ttu-id="ab3e3-304">[Exchange 中的可搜索属性](/Exchange/policy-and-compliance/ediscovery/message-properties-and-search-operators#searchable-properties-in-exchange)。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-304">[Searchable properties in Exchange](/Exchange/policy-and-compliance/ediscovery/message-properties-and-search-operators#searchable-properties-in-exchange).</span></span>

- [<span data-ttu-id="ab3e3-305">关键字查询语言 (KQL) 语法参考</span><span class="sxs-lookup"><span data-stu-id="ab3e3-305">Keyword Query Language (KQL) syntax reference</span></span>](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference)

- [<span data-ttu-id="ab3e3-306">Exchange 2016 中的就地电子数据展示的邮件属性和搜索运算符</span><span class="sxs-lookup"><span data-stu-id="ab3e3-306">Message properties and search operators for In-Place eDiscovery in Exchange 2016</span></span>](/Exchange/policy-and-compliance/ediscovery/message-properties-and-search-operators)

### <a name="using-search-on-person-collections"></a><span data-ttu-id="ab3e3-307">对 person 集合使用 $search</span><span class="sxs-lookup"><span data-stu-id="ab3e3-307">Using $search on person collections</span></span>

<span data-ttu-id="ab3e3-308">可以使用 Microsoft Graph People API 检索与用户相关度最高的人员。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-308">You can use the Microsoft Graph People API to retrieve the people who are most relevant to a user.</span></span> <span data-ttu-id="ab3e3-309">相关性由用户的通信和协作模式及业务关系决定。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-309">Relevance is determined by the user’s communication and collaboration patterns and business relationships.</span></span> <span data-ttu-id="ab3e3-310">People API 支持 `$search` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-310">The People API supports the `$search` query parameter.</span></span> <span data-ttu-id="ab3e3-311">`$search` 请求最多可返回 250 个结果。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-311">A `$search` request returns up to 250 results.</span></span>

<span data-ttu-id="ab3e3-312">人员搜索就是按 [person](/graph/api/resources/person) 资源的 **displayName** 和 **emailAddress** 属性进行搜索。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-312">Searches on people occur on both the **displayName** and **emailAddress** properties of the [person](/graph/api/resources/person) resource.</span></span>

<span data-ttu-id="ab3e3-313">以下请求在已登录用户的 **人员** 集合中的每个人员的 **displayName** 和 **emailAddress** 属性中，为名为“Irene McGowen”的人员执行搜索。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-313">The following request does a search for a person named "Irene McGowen" in the **displayName** and **emailAddress** properties in each person in the **people** collection of the signed-in user.</span></span> <span data-ttu-id="ab3e3-314">由于一个名为“Irene McGowan”的人员与登录用户相关，因此返回了“Irene McGowan”的信息。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-314">Because a person named "Irene McGowan" is relevant to the signed-in user, the information for "Irene McGowan" is returned.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="Irene McGowen"
```

<span data-ttu-id="ab3e3-315">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-315">The following example shows the response.</span></span> 

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

<span data-ttu-id="ab3e3-316">若要了解有关 People API 的详细信息，请参阅[获取相关人员的信息](./people-example.md#search-people)。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-316">To learn more about the People API, see [Get information about relevant people](./people-example.md#search-people).</span></span>  

### <a name="using-search-on-directory-object-collections"></a><span data-ttu-id="ab3e3-317">在目录对象集合上使用 $search</span><span class="sxs-lookup"><span data-stu-id="ab3e3-317">Using $search on directory object collections</span></span>

<span data-ttu-id="ab3e3-318">可使用 `$search` 查询参数来使用标记筛选结果。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-318">You can use a `$search` query parameter to filter results using tokenization.</span></span> <span data-ttu-id="ab3e3-319">标记化搜索的工作原理是提取输入和输出字符串中的单词，并使用空格、数字、不同的大小写和符号分隔这些词，如下所示：</span><span class="sxs-lookup"><span data-stu-id="ab3e3-319">Tokenized search works by extracting words from your input and output string, using spaces, numbers, different casing, and symbols to separate the words, as follow:</span></span>

* <span data-ttu-id="ab3e3-320">**空格**：`hello world` => `hello`、 `world`</span><span class="sxs-lookup"><span data-stu-id="ab3e3-320">**Spaces**: `hello world` => `hello`, `world`</span></span>
* <span data-ttu-id="ab3e3-321">**不同的大小写**⁽¹⁾：`HelloWorld` 或 `helloWORLD` => `hello`、`world`</span><span class="sxs-lookup"><span data-stu-id="ab3e3-321">**Different casing**⁽¹⁾: `HelloWorld` or `helloWORLD` => `hello`, `world`</span></span>
* <span data-ttu-id="ab3e3-322">**符号**⁽⁾：`hello.world` => `hello`、`.`、`world`， `helloworld`</span><span class="sxs-lookup"><span data-stu-id="ab3e3-322">**Symbols**⁽²⁾: `hello.world` => `hello`, `.`, `world`, `helloworld`</span></span>
* <span data-ttu-id="ab3e3-323">**数字**：`hello123world` => `hello`、`123`、 `world`</span><span class="sxs-lookup"><span data-stu-id="ab3e3-323">**Numbers**: `hello123world` => `hello`, `123`, `world`</span></span>

<span data-ttu-id="ab3e3-324">⁽¹⁾ 目前，标记化仅在大小写从小写转换为大写时才有效，因此 `HELLOworld` 被视为一个标记：`helloworld`，`HelloWORld` 是两个标记：`hello`、`world`。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-324">⁽¹⁾ Currently, tokenization only works when the casing is changing from lowercase to uppercase, so `HELLOworld` is considered a single token: `helloworld`, and `HelloWORld` is two tokens: `hello`, `world`.</span></span> <span data-ttu-id="ab3e3-325">⁽²⁾ 标记化逻辑还会合并仅由符号分隔的单词；例如，搜索 `helloworld` 将找到 `hello-world` 和 `hello.world`。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-325">⁽²⁾ Tokenization logic also combines words that are separated only by symbols; for example, searching for `helloworld` will find `hello-world` and `hello.world`.</span></span>

> <span data-ttu-id="ab3e3-326">**注意**：标记化后，标记将独立于原始大小写进行匹配，并且将以任何顺序匹配。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-326">**Note**: after tokenization, the tokens are matched independently of the original casing, and they are matched in any order.</span></span>
> <span data-ttu-id="ab3e3-327">`$search` 目录对象集合上的查询参数 **需要** 特殊的请求标头：`ConsistencyLevel: eventual`。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-327">`$search` query parameter on directory objects collections **requires** a special request header: `ConsistencyLevel: eventual`.</span></span>

<span data-ttu-id="ab3e3-328">标记化搜索支持仅适用于 **displayName** 和 **description** 字段。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-328">The tokenized search support works only on the **displayName** and **description** fields.</span></span> <span data-ttu-id="ab3e3-329">任何字段都可以放入 `$search`；非 **displayName** 和 **description** 的字段默认为 `$filter` startswith 行为。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-329">Any field can be put in `$search`; fields other than **displayName** and **description** default to `$filter` startswith behavior.</span></span> <span data-ttu-id="ab3e3-330">例如：</span><span class="sxs-lookup"><span data-stu-id="ab3e3-330">For example:</span></span>

`https://graph.microsoft.com/beta/groups/?$search="displayName:OneVideo"`

<span data-ttu-id="ab3e3-331">这将查找显示名称看起来像 "OneVideo" 的所有组。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-331">This looks for all groups with display names that look like "OneVideo".</span></span> <span data-ttu-id="ab3e3-332">也可与`$search`配合使用`$filter`。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-332">`$search` can be used together with `$filter` as well.</span></span> <span data-ttu-id="ab3e3-333">例如：</span><span class="sxs-lookup"><span data-stu-id="ab3e3-333">For example:</span></span>

`https://graph.microsoft.com/beta/groups/?$filter=mailEnabled eq true&$search="displayName:OneVideo"`

<span data-ttu-id="ab3e3-334">这将查找显示名称类似于“OneVideo”的所有启用邮件的组。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-334">This looks for all mail-enabled groups with display names that look like "OneVideo".</span></span> <span data-ttu-id="ab3e3-335">结果是根据逻辑结合（"AND"）和`$filter`整个查询`$search`来限制。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-335">The results are restricted based on a logical conjunction (an "AND") of the `$filter` and the entire query in the `$search`.</span></span> <span data-ttu-id="ab3e3-336">搜索文本基于大小写进行标记，但是匹配以不区分大小写的方式执行。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-336">The search text is tokenized based on casing, but matches are performed in a case-insensitive manner.</span></span> <span data-ttu-id="ab3e3-337">例如，“OneVideo”将被分割成两个输入标记“one”和“video”，但是匹配不区分大小写的属性。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-337">For example, "OneVideo" would be split into two input tokens "one" and "video", but matches properties insensitive to case.</span></span>

<span data-ttu-id="ab3e3-338">搜索的语法遵循以下规则：</span><span class="sxs-lookup"><span data-stu-id="ab3e3-338">The syntax of search follows these rules:</span></span>

* <span data-ttu-id="ab3e3-339">通用格式：$search="clause1" \[AND \| OR\] "\[clauseX\]"\.</span><span class="sxs-lookup"><span data-stu-id="ab3e3-339">Generic format: $search="clause1" \[AND \| OR\] "\[clauseX\]"\.</span></span>
* <span data-ttu-id="ab3e3-340">支持任何子句。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-340">Any number of clauses is supported.</span></span> <span data-ttu-id="ab3e3-341">支持适用于优先级的括号。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-341">Parentheses for precedence is also supported.</span></span>
* <span data-ttu-id="ab3e3-342">每个子句的语法是："\<property>:\<text to search>"。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-342">The syntax for each clause is: "\<property>:\<text to search>".</span></span>
* <span data-ttu-id="ab3e3-343">必须在子句中指定属性名称。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-343">The property name must be specified in clause.</span></span> <span data-ttu-id="ab3e3-344">可以在中使用的任何属性`$filter`也可以在内使用 `$search`。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-344">Any property that can be used in `$filter` can also be used inside `$search`.</span></span> <span data-ttu-id="ab3e3-345">根据属性的不同，如果属性不支持搜索，那么搜索行为要么是“search”，要么是“start with”。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-345">Depending on the property, the search behavior is either "search" or "startswith" if search is not supported on the property.</span></span>
* <span data-ttu-id="ab3e3-346">必须将完整子句部分置于双引号内。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-346">The whole clause part must be put inside double quotes.</span></span>
* <span data-ttu-id="ab3e3-347">必须将逻辑运算符 "AND" 和 "OR" 置于双引号之外。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-347">Logical operator 'AND' 'OR' must be put outside double quotes.</span></span> <span data-ttu-id="ab3e3-348">它们必须处于大写形式。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-348">They must be in upper case.</span></span>
* <span data-ttu-id="ab3e3-349">考虑到整个子句部分需要放在双引号内，如果包含双引号和反斜杠，则需要使用反斜杠对其进行转义。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-349">Given that the whole clause part needs to be put inside double quotes, if it contains double quote and backslash, it needs to be escaped with a backslash.</span></span> <span data-ttu-id="ab3e3-350">无需转义其他字符。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-350">No other characters need to be escaped.</span></span>

<span data-ttu-id="ab3e3-351">下表显示了一些示例。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-351">The following table shows some examples.</span></span>

| <span data-ttu-id="ab3e3-352">对象类</span><span class="sxs-lookup"><span data-stu-id="ab3e3-352">Object class</span></span> | <span data-ttu-id="ab3e3-353">说明</span><span class="sxs-lookup"><span data-stu-id="ab3e3-353">Description</span></span> | <span data-ttu-id="ab3e3-354">示例</span><span class="sxs-lookup"><span data-stu-id="ab3e3-354">Example</span></span> |
| ------------ | ----------- | ------- |
| <span data-ttu-id="ab3e3-355">用户</span><span class="sxs-lookup"><span data-stu-id="ab3e3-355">User</span></span> | <span data-ttu-id="ab3e3-356">通讯簿显示用户的名称。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-356">Address book display name of the user.</span></span> | `https://graph.microsoft.com/beta/users?$search="displayName:Guthr"` |
| <span data-ttu-id="ab3e3-357">用户</span><span class="sxs-lookup"><span data-stu-id="ab3e3-357">User</span></span> | <span data-ttu-id="ab3e3-358">通讯簿显示用户的名称或邮件。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-358">Address book display name or mail of the user.</span></span> | `https://graph.microsoft.com/beta/users?$search="displayName:Guthr" OR "mail:Guthr"` |
| <span data-ttu-id="ab3e3-359">Group</span><span class="sxs-lookup"><span data-stu-id="ab3e3-359">Group</span></span> | <span data-ttu-id="ab3e3-360">通讯簿显群组的名称或说明。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-360">Address book display name or description of the group.</span></span> | `https://graph.microsoft.com/beta/groups?$search="description:One" AND ("displayName:Video" OR "displayName:Drive")` |
| <span data-ttu-id="ab3e3-361">Group</span><span class="sxs-lookup"><span data-stu-id="ab3e3-361">Group</span></span> | <span data-ttu-id="ab3e3-362">通讯簿在启用邮件组上显示名称。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-362">Address book display name on a mail-enabled group.</span></span> | `https://graph.microsoft.com/beta/groups?$filter=mailEnabled eq true&$search="displayName:OneVideo"` |

<span data-ttu-id="ab3e3-363">你在 `$search` 中提供的字符串输入以及可搜索属性都按空格、不同的大小写和字符类型（数字和特殊字符）划分为多个部分。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-363">Both the string inputs you provide in `$search`, as well as the searchable properties, are split up into parts by spaces, different casing, and character types (numbers and special characters).</span></span>

## <a name="select-parameter"></a><span data-ttu-id="ab3e3-364">select 参数</span><span class="sxs-lookup"><span data-stu-id="ab3e3-364">select parameter</span></span>

<span data-ttu-id="ab3e3-365">使用 `$select` 查询参数返回一组不同于单个资源的默认集或资源集合的属性。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-365">Use the `$select` query parameter to return a set of properties that are different than the default set for an individual resource or a collection of resources.</span></span> <span data-ttu-id="ab3e3-366">使用 $select，可以指定默认属性的子集或超集。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-366">With $select, you can specify a subset or a superset of the default properties.</span></span>

<span data-ttu-id="ab3e3-367">例如，检索登录用户的邮件时，可以指定仅返回 **from** 和 **subject** 属性：</span><span class="sxs-lookup"><span data-stu-id="ab3e3-367">For example, when retrieving the messages of the signed-in user, you can specify that only the **from** and **subject** properties be returned:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$select=from,subject
```

<span data-ttu-id="ab3e3-368">[在 Graph 浏览器中试调用][select-example]</span><span class="sxs-lookup"><span data-stu-id="ab3e3-368">[Try in Graph Explorer][select-example]</span></span>

> <span data-ttu-id="ab3e3-369">**重要说明：** 一般来说，建议使用 `$select` 将查询返回的属性限制为应用所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-369">**Important:** In general, we recommend that you use `$select` to limit the properties returned by a query to those needed by your app.</span></span> <span data-ttu-id="ab3e3-370">这对于可能返回大型结果集的查询尤为有用。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-370">This is especially true of queries that might potentially return a large result set.</span></span> <span data-ttu-id="ab3e3-371">限制每行返回的属性将减少网络负载并帮助提升应用的性能。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-371">Limiting the properties returned in each row will reduce network load and help improve your app's performance.</span></span>
>
> <span data-ttu-id="ab3e3-p138">在 `v1.0` 中，从 [directoryObject](/graph/api/resources/directoryobject) 派生的一些 Azure AD 资源（如 [user](/graph/api/resources/user) 和 [group](/graph/api/resources/group)）在读取时返回受限的默认属性子集。对于这些资源，必须使用 `$select` 将属性返回到默认集之外。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-p138">In `v1.0`, some Azure AD resources that derive from [directoryObject](/graph/api/resources/directoryobject), like [user](/graph/api/resources/user) and [group](/graph/api/resources/group), return a limited, default subset of properties on reads. For these resources, you must use `$select` to return properties outside of the default set.</span></span>  

## <a name="skip-parameter"></a><span data-ttu-id="ab3e3-374">skip 参数</span><span class="sxs-lookup"><span data-stu-id="ab3e3-374">skip parameter</span></span>

<span data-ttu-id="ab3e3-p139">使用 `$skip` 查询参数设置要在集合开头跳过的项数。例如，以下请求返回按照创建日期排序的用户的事件，从集合中的第 21 个事件开始：</span><span class="sxs-lookup"><span data-stu-id="ab3e3-p139">Use the `$skip` query parameter to set the number of items to skip at the start of a collection. For example, the following request returns events for the user sorted by date created, starting with the 21st event in the collection:</span></span>

```http
GET  https://graph.microsoft.com/v1.0/me/events?$orderby=createdDateTime&$skip=20
```
<span data-ttu-id="ab3e3-377">[在 Graph 浏览器中试调用][skip-example]</span><span class="sxs-lookup"><span data-stu-id="ab3e3-377">[Try in Graph Explorer][skip-example]</span></span>

> <span data-ttu-id="ab3e3-378">**注意：** 一些 Microsoft Graph API 使用 `$skip` 实现分页，如 Outlook 邮件和日历（**message**、**event** 和 **calendar**）。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-378">**Note:** Some Microsoft Graph APIs, like Outlook Mail and Calendars (**message**, **event**, and **calendar**), use `$skip` to implement paging.</span></span> <span data-ttu-id="ab3e3-379">当查询结果跨多个页面时，这些 API 会返回 `@odata:nextLink` 属性，具有包含 `$skip` 参数的 URL。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-379">When results of a query span multiple pages, these APIs will return an `@odata:nextLink` property with a URL that contains a `$skip` parameter.</span></span> <span data-ttu-id="ab3e3-380">可以使用此 URL 返回下一页结果。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-380">You can use this URL to return the next page of results.</span></span> <span data-ttu-id="ab3e3-381">若要了解详细信息，请参阅[分页](./paging.md)。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-381">To learn more, see [Paging](./paging.md).</span></span>

## <a name="skiptoken-parameter"></a><span data-ttu-id="ab3e3-382">skipToken 参数</span><span class="sxs-lookup"><span data-stu-id="ab3e3-382">skipToken parameter</span></span>

<span data-ttu-id="ab3e3-383">由于服务器端分页或由于使用 [`$top`](#top-parameter) 参数来限制响应的页面大小，致使一些请求返回多页数据。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-383">Some requests return multiple pages of data, either due to server-side paging or due to the use of the [`$top`](#top-parameter) parameter to limit the page size of the response.</span></span> <span data-ttu-id="ab3e3-384">许多 Microsoft Graph API 使用 `skipToken` 查询参数来引用结果的后续页面。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-384">Many Microsoft Graph APIs use the `skipToken` query parameter to reference subsequent pages of the result.</span></span>  
<span data-ttu-id="ab3e3-385">`$skiptoken` 参数包含引用下一页结果的不透明令牌，并在响应的 `@odata.nextLink` 属性中提供的 URL 中返回。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-385">The `$skiptoken` parameter contains an opaque token that references the next page of results and is returned in the URL provided in the `@odata.nextLink` property in the response.</span></span> <span data-ttu-id="ab3e3-386">若要了解详细信息，请参阅[分页](./paging.md)。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-386">To learn more, see [Paging](./paging.md).</span></span>
> <span data-ttu-id="ab3e3-387">**注意**：如果你使用的是 OData 计数（在查询字符串中添加 `$count=true`），则 `@odata.count` 属性将仅在第一页中出现。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-387">**Note:** if you're using OData Count (adding `$count=true` in the querystring), the `@odata.count` property will be present only in the first page.</span></span>

## <a name="top-parameter"></a><span data-ttu-id="ab3e3-388">top 参数</span><span class="sxs-lookup"><span data-stu-id="ab3e3-388">top parameter</span></span>

<span data-ttu-id="ab3e3-389">使用 `$top` 查询参数指定结果集的页面大小。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-389">Use the `$top` query parameter to specify the page size of the result set.</span></span> 

<span data-ttu-id="ab3e3-390">如果结果集中还剩余多个项目，则响应正文将包含 `@odata.nextLink` 参数。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-390">If more items remain in the result set, the response body will contain an `@odata.nextLink` parameter.</span></span> <span data-ttu-id="ab3e3-391">此参数包含可用于获取下一页结果的 URL。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-391">This parameter contains a URL that you can use to get the next page of results.</span></span> <span data-ttu-id="ab3e3-392">若要了解详细信息，请参阅[分页](./paging.md)。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-392">To learn more, see [Paging](./paging.md).</span></span> 

<span data-ttu-id="ab3e3-393">最小值为 $top 1，最大值取决于相应的 API。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-393">The minimum value of $top is 1 and the maximum depends on the corresponding API.</span></span>  

<span data-ttu-id="ab3e3-394">例如，以下列表 [请求](/graph/api/user-list-messages) 返回用户邮箱中的前五条消息：</span><span class="sxs-lookup"><span data-stu-id="ab3e3-394">For example, the following [list messages](/graph/api/user-list-messages) request returns the first five messages in the user's mailbox:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$top=5
```

<span data-ttu-id="ab3e3-395">[在 Graph 浏览器中试调用][top-example]</span><span class="sxs-lookup"><span data-stu-id="ab3e3-395">[Try in Graph Explorer][top-example]</span></span>


## <a name="error-handling-for-query-parameters"></a><span data-ttu-id="ab3e3-396">查询参数的错误处理</span><span class="sxs-lookup"><span data-stu-id="ab3e3-396">Error handling for query parameters</span></span>

<span data-ttu-id="ab3e3-p144">如果不支持指定的查询参数，某些请求将返回错误消息。例如，不能对 `user/photo` 关系使用 `$expand`。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-p144">Some requests will return an error message if a specified query parameter is not supported. For example, you cannot use `$expand` on the `user/photo` relationship.</span></span> 

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

<span data-ttu-id="ab3e3-399">但是，值得注意的是请求中指定的查询参数可能会自行失败。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-399">However, it is important to note that query parameters specified in a request might fail silently.</span></span> <span data-ttu-id="ab3e3-400">不支持的查询参数以及不支持的查询参数组合的情况就是如此。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-400">This can be true for unsupported query parameters as well as for unsupported combinations of query parameters.</span></span> <span data-ttu-id="ab3e3-401">在这些情况下，应检查请求返回的数据，以确定指定的查询参数是否具有所需的效果。</span><span class="sxs-lookup"><span data-stu-id="ab3e3-401">In these cases, you should examine the data returned by the request to determine whether the query parameters you specified had the desired effect.</span></span> 

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

[search-sbj-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22subject%3Ahas%22%26$select=subject&method=GET&version=v1.0
[search-to-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22to%3Arandiw%22%26$select=subject,toRecipients&method=GET&version=v1.0



## <a name="see-also"></a><span data-ttu-id="ab3e3-402">另请参阅</span><span class="sxs-lookup"><span data-stu-id="ab3e3-402">See also</span></span>

- [<span data-ttu-id="ab3e3-403">查询参数限制</span><span class="sxs-lookup"><span data-stu-id="ab3e3-403">Query parameter limitations</span></span>](known-issues.md#query-parameter-limitations)
