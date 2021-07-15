---
title: 使用查询参数自定义响应
description: Microsoft Graph 提供可选的查询参数，可用于指定和控制响应中返回的数据量。
author: mumbi-o
localization_priority: Priority
ms.custom: graphiamtop20, scenarios:getting-started
ms.openlocfilehash: 2cf22e03f4134c1e4612433bf8190e89eea97bbf
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440665"
---
# <a name="use-query-parameters-to-customize-responses"></a><span data-ttu-id="156cc-103">使用查询参数自定义响应</span><span class="sxs-lookup"><span data-stu-id="156cc-103">Use query parameters to customize responses</span></span>

<span data-ttu-id="156cc-104">Microsoft Graph 支持可选的查询参数，可用于指定和控制响应中返回的数据量。</span><span class="sxs-lookup"><span data-stu-id="156cc-104">Microsoft Graph supports optional query parameters that you can use to specify and control the amount of data returned in a response.</span></span> <span data-ttu-id="156cc-105">对准确查询参数的支持因 API 操作不同而不同，并且可能会在 v1.0 和数据终结点之间不同，具体取决于 API。</span><span class="sxs-lookup"><span data-stu-id="156cc-105">The support for the exact query parameters varies from one API operation to another, and depending on the API, can differ between the v1.0 and beta endpoints.</span></span>

> [!TIP] 
> <span data-ttu-id="156cc-106">在 beta 终结点上，`$` 前缀是可选的。</span><span class="sxs-lookup"><span data-stu-id="156cc-106">On the beta endpoint, the `$` prefix is optional.</span></span> <span data-ttu-id="156cc-107">例如，可使用 `filter` 来代替 `$filter`。</span><span class="sxs-lookup"><span data-stu-id="156cc-107">For example, instead of `$filter`, you can use `filter`.</span></span> <span data-ttu-id="156cc-108">在 v1 终结点上, `$`前缀仅对 API 的一个子集是可选的。</span><span class="sxs-lookup"><span data-stu-id="156cc-108">On the v1 endpoint, the `$` prefix is optional for only a subset of APIs.</span></span> <span data-ttu-id="156cc-109">为简单起见, 如果使用 v1 终结点, 请始终包含`$`。</span><span class="sxs-lookup"><span data-stu-id="156cc-109">For simplicity, always include `$` if using the v1 endpoint.</span></span>

<span data-ttu-id="156cc-110">查询参数可以是 OData 系统查询选项，也可以是其他查询参数。</span><span class="sxs-lookup"><span data-stu-id="156cc-110">Query parameters can be OData system query options or other query parameters.</span></span> 

> [!VIDEO https://www.youtube-nocookie.com/embed/7BuFv3yETi4]

## <a name="odata-system-query-options"></a><span data-ttu-id="156cc-111">OData 系统查询选项</span><span class="sxs-lookup"><span data-stu-id="156cc-111">OData system query options</span></span>
<span data-ttu-id="156cc-112">Microsoft Graph API 操作可以支持以下一个或多个 OData 系统查询选项。</span><span class="sxs-lookup"><span data-stu-id="156cc-112">A Microsoft Graph API operation might support one or more of the following OData system query options.</span></span> <span data-ttu-id="156cc-113">这些查询选项与 [OData V4 查询语言][odata-query]兼容。</span><span class="sxs-lookup"><span data-stu-id="156cc-113">These query options are compatible with the [OData V4 query language][odata-query].</span></span>

><span data-ttu-id="156cc-114">**注意：** OData 4.0 仅在 GET 操作中支持系统查询选项。</span><span class="sxs-lookup"><span data-stu-id="156cc-114">**Note:** OData 4.0 supports system query options in only GET operations.</span></span>

<span data-ttu-id="156cc-115">单击示例可以在 [Graph 浏览器][graph-explorer]中试调用它们。</span><span class="sxs-lookup"><span data-stu-id="156cc-115">Click the examples to try them in [Graph Explorer][graph-explorer].</span></span>

| <span data-ttu-id="156cc-116">名称</span><span class="sxs-lookup"><span data-stu-id="156cc-116">Name</span></span>                     | <span data-ttu-id="156cc-117">说明</span><span class="sxs-lookup"><span data-stu-id="156cc-117">Description</span></span> | <span data-ttu-id="156cc-118">示例</span><span class="sxs-lookup"><span data-stu-id="156cc-118">Example</span></span>
|:-------------------------|:------------|:---------|
| [<span data-ttu-id="156cc-119">$count</span><span class="sxs-lookup"><span data-stu-id="156cc-119">$count</span></span>](#count-parameter)         | <span data-ttu-id="156cc-120">检索匹配资源的总数。</span><span class="sxs-lookup"><span data-stu-id="156cc-120">Retrieves the total count of matching resources.</span></span> | [`/me/messages?$top=2&$count=true`][count-example]
| [<span data-ttu-id="156cc-121">$expand</span><span class="sxs-lookup"><span data-stu-id="156cc-121">$expand</span></span>](#expand-parameter)       | <span data-ttu-id="156cc-122">检索相关资源。</span><span class="sxs-lookup"><span data-stu-id="156cc-122">Retrieves related resources.</span></span>|[`/groups?$expand=members`][expand-example]
| [<span data-ttu-id="156cc-123">$filter</span><span class="sxs-lookup"><span data-stu-id="156cc-123">$filter</span></span>](#filter-parameter)       | <span data-ttu-id="156cc-124">筛选结果（行）。</span><span class="sxs-lookup"><span data-stu-id="156cc-124">Filters results (rows).</span></span>|[`/users?$filter=startswith(givenName,'J')`][filter-example]
| [<span data-ttu-id="156cc-125">$format</span><span class="sxs-lookup"><span data-stu-id="156cc-125">$format</span></span>](#format-parameter)       | <span data-ttu-id="156cc-126">返回指定媒体格式的结果。</span><span class="sxs-lookup"><span data-stu-id="156cc-126">Returns the results in the specified media format.</span></span>|[`/users?$format=json`][format-example]
| [<span data-ttu-id="156cc-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="156cc-127">$orderby</span></span>](#orderby-parameter)     | <span data-ttu-id="156cc-128">对结果进行排序。</span><span class="sxs-lookup"><span data-stu-id="156cc-128">Orders results.</span></span>|[`/users?$orderby=displayName desc`][orderby-example]
| [<span data-ttu-id="156cc-129">$search</span><span class="sxs-lookup"><span data-stu-id="156cc-129">$search</span></span>](#search-parameter)       | <span data-ttu-id="156cc-130">返回基于搜索条件的结果。</span><span class="sxs-lookup"><span data-stu-id="156cc-130">Returns results based on search criteria.</span></span> |[`/me/messages?$search=pizza`][search-example]
| [<span data-ttu-id="156cc-131">$select</span><span class="sxs-lookup"><span data-stu-id="156cc-131">$select</span></span>](#select-parameter)       | <span data-ttu-id="156cc-132">筛选属性（列）。</span><span class="sxs-lookup"><span data-stu-id="156cc-132">Filters properties (columns).</span></span>|[`/users?$select=givenName,surname`][select-example]
| [<span data-ttu-id="156cc-133">$skip</span><span class="sxs-lookup"><span data-stu-id="156cc-133">$skip</span></span>](#skip-parameter)           | <span data-ttu-id="156cc-p104">对结果集建立索引。一些 API 也使用它来实现分页，并且可以与 `$top` 一起使用来手动对结果分页。</span><span class="sxs-lookup"><span data-stu-id="156cc-p104">Indexes into a result set. Also used by some APIs to implement paging and can be used together with `$top` to manually page results.</span></span> | [`/me/messages?$skip=11`][skip-example]
| [<span data-ttu-id="156cc-136">$top</span><span class="sxs-lookup"><span data-stu-id="156cc-136">$top</span></span>](#top-parameter)             | <span data-ttu-id="156cc-137">设置结果的页面大小。</span><span class="sxs-lookup"><span data-stu-id="156cc-137">Sets the page size of results.</span></span> |[`/users?$top=2`][top-example]


## <a name="other-query-parameters"></a><span data-ttu-id="156cc-138">其他查询参数</span><span class="sxs-lookup"><span data-stu-id="156cc-138">Other query parameters</span></span>

| <span data-ttu-id="156cc-139">名称</span><span class="sxs-lookup"><span data-stu-id="156cc-139">Name</span></span>                     | <span data-ttu-id="156cc-140">说明</span><span class="sxs-lookup"><span data-stu-id="156cc-140">Description</span></span> | <span data-ttu-id="156cc-141">示例</span><span class="sxs-lookup"><span data-stu-id="156cc-141">Example</span></span>
|:-------------------------|:------------|:---------|
| [<span data-ttu-id="156cc-142">$skipToken</span><span class="sxs-lookup"><span data-stu-id="156cc-142">$skipToken</span></span>](#skiptoken-parameter) | <span data-ttu-id="156cc-p105">从跨多页的结果集中检索下一页结果。（但某些 API 改为使用 `$skip`。）</span><span class="sxs-lookup"><span data-stu-id="156cc-p105">Retrieves the next page of results from result sets that span multiple pages. (Some APIs use `$skip` instead.)</span></span> | `/users?$skiptoken=X%274453707402000100000017...`|

## <a name="other-odata-url-capabilities"></a><span data-ttu-id="156cc-145">其他 OData URL 功能</span><span class="sxs-lookup"><span data-stu-id="156cc-145">Other OData URL capabilities</span></span>

<span data-ttu-id="156cc-146">下列 OData 4.0 功能是 URL 区段，不是查询参数。</span><span class="sxs-lookup"><span data-stu-id="156cc-146">The following OData 4.0 capabilities are URL segments, not query parameters.</span></span>

| <span data-ttu-id="156cc-147">名称</span><span class="sxs-lookup"><span data-stu-id="156cc-147">Name</span></span>                     | <span data-ttu-id="156cc-148">说明</span><span class="sxs-lookup"><span data-stu-id="156cc-148">Description</span></span> | <span data-ttu-id="156cc-149">示例</span><span class="sxs-lookup"><span data-stu-id="156cc-149">Example</span></span> 
|:-------------------------|:------------|:---------|
| [<span data-ttu-id="156cc-150">$count</span><span class="sxs-lookup"><span data-stu-id="156cc-150">$count</span></span>](/graph/api/user-list#example-3-get-only-a-count-of-users)| <span data-ttu-id="156cc-151">检索集合的整数总计。</span><span class="sxs-lookup"><span data-stu-id="156cc-151">Retrieves the integer total of the collection.</span></span> | `GET /users/$count` <br> `GET /groups/{id}/members/$count`|
| [<span data-ttu-id="156cc-152">$ref</span><span class="sxs-lookup"><span data-stu-id="156cc-152">$ref</span></span>](/graph/api/group-post-members) | <span data-ttu-id="156cc-153">更新实体成员身份至集合。</span><span class="sxs-lookup"><span data-stu-id="156cc-153">Updates entities membership to a collection.</span></span> | `POST /groups/{id}/members/$ref` |
| [<span data-ttu-id="156cc-154">$value</span><span class="sxs-lookup"><span data-stu-id="156cc-154">$value</span></span>](/graph/api/profilephoto-get) | <span data-ttu-id="156cc-155">检索或更新项的二进制值。</span><span class="sxs-lookup"><span data-stu-id="156cc-155">Retrieves or updates the binary value of an item.</span></span> | `GET /me/photo/$value` |

## <a name="encoding-query-parameters"></a><span data-ttu-id="156cc-156">对查询参数进行编码</span><span class="sxs-lookup"><span data-stu-id="156cc-156">Encoding query parameters</span></span>

<span data-ttu-id="156cc-157">应对查询参数的值进行百分比编码。</span><span class="sxs-lookup"><span data-stu-id="156cc-157">The values of query parameters should be percent-encoded.</span></span> <span data-ttu-id="156cc-158">许多 HTTP 客户端、浏览器和工具（如 [Graph 浏览器][graph-explorer]）将在这方面帮助你。</span><span class="sxs-lookup"><span data-stu-id="156cc-158">Many HTTP clients, browsers, and tools (such as the [Graph Explorer][graph-explorer]) will help you with this.</span></span> <span data-ttu-id="156cc-159">如果查询失败，可能原因之一是未正确编码查询参数值。</span><span class="sxs-lookup"><span data-stu-id="156cc-159">If a query is failing, one possible cause is failure to encode the query parameter values appropriately.</span></span>

<span data-ttu-id="156cc-160">未编码的 URL 如下所示：</span><span class="sxs-lookup"><span data-stu-id="156cc-160">An unencoded URL looks like this:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName, 'J')
```

<span data-ttu-id="156cc-161">正确解码的 URL 如下所示：</span><span class="sxs-lookup"><span data-stu-id="156cc-161">A properly encoded URL looks like this:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName%2C+'J')
```

### <a name="escaping-single-quotes"></a><span data-ttu-id="156cc-162">转义单引号</span><span class="sxs-lookup"><span data-stu-id="156cc-162">Escaping single quotes</span></span>

<span data-ttu-id="156cc-163">对于使用单引号的请求，如果任何参数值也包含单引号，则必须进行双转义；否则，由于语法无效，请求将失败。</span><span class="sxs-lookup"><span data-stu-id="156cc-163">For requests that use single quotes, if any parameter values also contain single quotes, those must be double escaped; otherwise, the request will fail due to invalid syntax.</span></span> <span data-ttu-id="156cc-164">在示例中，字符串值 `let''s meet for lunch?` 进行了单引号转义。</span><span class="sxs-lookup"><span data-stu-id="156cc-164">In the example, the string value `let''s meet for lunch?` has the single quote escaped.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=subject eq 'let''s meet for lunch?'
```

## <a name="count-parameter"></a><span data-ttu-id="156cc-165">count 参数</span><span class="sxs-lookup"><span data-stu-id="156cc-165">count parameter</span></span>

<span data-ttu-id="156cc-166">使用 `$count` 查询参数以包括集合中项总数的计数，以及从 Microsoft Graph 返回的数据值页。</span><span class="sxs-lookup"><span data-stu-id="156cc-166">Use the `$count` query parameter to include a count of the total number of items in a collection alongside the page of data values returned from Microsoft Graph.</span></span>

> [!NOTE]
> <span data-ttu-id="156cc-167">`$count` 还可以用作 [URL 段](#other-odata-url-capabilities) 以检索集合的整数总计。</span><span class="sxs-lookup"><span data-stu-id="156cc-167">`$count` can also be used as a [URL segment](#other-odata-url-capabilities) to retrieve the integer total of the collection.</span></span> <span data-ttu-id="156cc-168">在派生自[directoryObject](/graph/api/resources/directoryobject)的资源上，它仅适用于高级查询。</span><span class="sxs-lookup"><span data-stu-id="156cc-168">On resources that derive from [directoryObject](/graph/api/resources/directoryobject), is it only supported in an advanced query.</span></span> <span data-ttu-id="156cc-169">请参阅[Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。</span><span class="sxs-lookup"><span data-stu-id="156cc-169">See [Advanced query capabilities in Azure AD directory objects](/graph/aad-advanced-queries).</span></span>
>
> <span data-ttu-id="156cc-170">Azure AD B2C 租户不支持使用`$count`。</span><span class="sxs-lookup"><span data-stu-id="156cc-170">Use of `$count` is not supported in Azure AD B2C tenants.</span></span>

<span data-ttu-id="156cc-171">例如，下面的请求返回当前用户的 **contact** 集合，以及 `@odata.count` 属性中 **contact** 集合内的项数。</span><span class="sxs-lookup"><span data-stu-id="156cc-171">For example, the following request returns both the **contact** collection of the current user, and the number of items in the **contact** collection in the `@odata.count` property.</span></span>

```msgraph-interactive
GET  https://graph.microsoft.com/v1.0/me/contacts?$count=true
```

<span data-ttu-id="156cc-172">`$count`查询参数支持这些资源集合和派生自[directoryObject](/graph/api/resources/directoryobject)的关系，而且仅在[高级查询](/graph/filter-directory-objects)中支持:</span><span class="sxs-lookup"><span data-stu-id="156cc-172">The `$count` query parameter is supported for these collections of resources and their relationships that derive from [directoryObject](/graph/api/resources/directoryobject) and only in [advanced queries](/graph/filter-directory-objects):</span></span>
- [<span data-ttu-id="156cc-173">application</span><span class="sxs-lookup"><span data-stu-id="156cc-173">application</span></span>](/graph/api/resources/application)
- [<span data-ttu-id="156cc-174">orgContact</span><span class="sxs-lookup"><span data-stu-id="156cc-174">orgContact</span></span>](/graph/api/resources/orgcontact)
- [<span data-ttu-id="156cc-175">设备</span><span class="sxs-lookup"><span data-stu-id="156cc-175">device</span></span>](/graph/api/resources/device)
- [<span data-ttu-id="156cc-176">组</span><span class="sxs-lookup"><span data-stu-id="156cc-176">group</span></span>](/graph/api/resources/group)
- [<span data-ttu-id="156cc-177">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="156cc-177">servicePrincipal</span></span>](/graph/api/resources/serviceprincipal)
- [<span data-ttu-id="156cc-178">用户</span><span class="sxs-lookup"><span data-stu-id="156cc-178">user</span></span>](/graph/api/resources/user)

## <a name="expand-parameter"></a><span data-ttu-id="156cc-179">expand 参数</span><span class="sxs-lookup"><span data-stu-id="156cc-179">expand parameter</span></span>

<span data-ttu-id="156cc-180">许多 Microsoft Graph 资源都会公开资源的已声明属性以及与其他资源的关系。</span><span class="sxs-lookup"><span data-stu-id="156cc-180">Many Microsoft Graph resources expose both declared properties of the resource as well as its relationships with other resources.</span></span> <span data-ttu-id="156cc-181">这些关系也称为引用属性或导航属性，它们可以引用单个资源或资源集合。</span><span class="sxs-lookup"><span data-stu-id="156cc-181">These relationships are also called reference properties or navigation properties, and they can reference either a single resource or a collection of resources.</span></span> <span data-ttu-id="156cc-182">例如，用户的邮件文件夹、管理者和直接下属都将作为关系公开。</span><span class="sxs-lookup"><span data-stu-id="156cc-182">For example, the mail folders, manager, and direct reports of a user are all exposed as relationships.</span></span> 

<span data-ttu-id="156cc-183">通常情况下，可以在单个请求中查询资源属性或其关系之一，但不能同时查询。</span><span class="sxs-lookup"><span data-stu-id="156cc-183">Normally, you can query either the properties of a resource or one of its relationships in a single request, but not both.</span></span> <span data-ttu-id="156cc-184">可以使用 `$expand` 查询字符串参数以包含结果中单个关系（导航属性）引用的扩展资源或集合。</span><span class="sxs-lookup"><span data-stu-id="156cc-184">You can use the `$expand` query string parameter to include the expanded resource or collection referenced by a single relationship (navigation property) in your results.</span></span> <span data-ttu-id="156cc-185">在单个请求中只能扩展一个关系。</span><span class="sxs-lookup"><span data-stu-id="156cc-185">Only one relationship can be expanded in a single request.</span></span>

<span data-ttu-id="156cc-186">以下示例在驱动器中获取根驱动器信息以及顶级子项：</span><span class="sxs-lookup"><span data-stu-id="156cc-186">The following example gets root drive information along with the top-level child items in a drive:</span></span>

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children
```


<span data-ttu-id="156cc-p111">使用一些资源集合，还可以添加 `$select` 参数，指定要在扩展资源中返回的属性。下面的示例执行与上一示例几乎相同的查询，不同之处在于使用 [`$select`](#select-parameter) 语句将为扩展子项返回的属性限制为 **id** 和 **name** 属性。</span><span class="sxs-lookup"><span data-stu-id="156cc-p111">With some resource collections, you can also specify the properties to be returned in the expanded resources by adding a `$select` parameter. The following example performs the same query as the previous example but uses a [`$select`](#select-parameter) statement to limit the properties returned for the expanded child items to the **id** and **name** properties.</span></span>

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children($select=id,name)
```

> [!NOTE]
> <span data-ttu-id="156cc-189">并不是所有关系和资源都支持 `$expand` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="156cc-189">Not all relationships and resources support the `$expand` query parameter.</span></span> <span data-ttu-id="156cc-190">例如，可以展开一个用户的 **directReports**、 **manager** 和 **memberOf** 关系，但不能展开其 **events**、 **messages** 或 **photos** 关系。</span><span class="sxs-lookup"><span data-stu-id="156cc-190">For example, you can expand the **directReports**, **manager**, and **memberOf** relationships on a user, but you cannot expand its **events**, **messages**, or **photo** relationships.</span></span> <span data-ttu-id="156cc-191">并非所有资源或关系都支持在扩展项上使用 `$select`。</span><span class="sxs-lookup"><span data-stu-id="156cc-191">Not all resources or relationships support using `$select` on expanded items.</span></span> 
> 
> <span data-ttu-id="156cc-192">使用派生自 [directoryObject](/graph/api/resources/directoryobject) 的 Azure AD 资源(如[user](/graph/api/resources/user) 和 [group](/graph/api/resources/group))，`$expand` 通常最多为扩展关系返回 20 个项，并且没有 [@odata.nextLink](./paging.md)。</span><span class="sxs-lookup"><span data-stu-id="156cc-192">With Azure AD resources that derive from [directoryObject](/graph/api/resources/directoryobject), like [user](/graph/api/resources/user) and [group](/graph/api/resources/group), `$expand` typically returns a maximum of 20 items for the expanded relationship and has no [@odata.nextLink](./paging.md).</span></span> <span data-ttu-id="156cc-193">请参阅更多 [已知问题](known-issues.md#query-parameter-limitations)。</span><span class="sxs-lookup"><span data-stu-id="156cc-193">See more [known issues](known-issues.md#query-parameter-limitations).</span></span>

## <a name="filter-parameter"></a><span data-ttu-id="156cc-194">filter 参数</span><span class="sxs-lookup"><span data-stu-id="156cc-194">filter parameter</span></span>

<span data-ttu-id="156cc-195">使用 `$filter` 查询参数，以仅检索集合的子集。</span><span class="sxs-lookup"><span data-stu-id="156cc-195">Use the `$filter` query parameter to retrieve just a subset of a collection.</span></span> <span data-ttu-id="156cc-196">`$filter`查询参数还可以用于检索关系，例如members、memberOf、transitiveMembers和transitiveMemberOf。</span><span class="sxs-lookup"><span data-stu-id="156cc-196">The `$filter` query parameter can also be used to retrieve relationships like members, memberOf, transitiveMembers, and transitiveMemberOf.</span></span> <span data-ttu-id="156cc-197">例如，获取我所属的所有安全组。</span><span class="sxs-lookup"><span data-stu-id="156cc-197">For example, get all the security groups I'm a member of.</span></span>

<span data-ttu-id="156cc-198">以下示例查找显示名称以字母“J”开头的用户:</span><span class="sxs-lookup"><span data-stu-id="156cc-198">The following example finds users whose display name starts with the letter 'J':</span></span>

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=startsWith(displayName,'J')
```

<span data-ttu-id="156cc-199">对 `$filter` 运算符的支持因 Microsoft Graph API 不同而异。</span><span class="sxs-lookup"><span data-stu-id="156cc-199">Support for `$filter` operators varies across Microsoft Graph APIs.</span></span> <span data-ttu-id="156cc-200">通常支持下列逻辑运算符：</span><span class="sxs-lookup"><span data-stu-id="156cc-200">The following logical operators are generally supported:</span></span>

| <span data-ttu-id="156cc-201">运算符类型</span><span class="sxs-lookup"><span data-stu-id="156cc-201">Operator type</span></span> | <span data-ttu-id="156cc-202">运算符</span><span class="sxs-lookup"><span data-stu-id="156cc-202">Operator</span></span> |
| --- | --- |
| <span data-ttu-id="156cc-203">相等运算符</span><span class="sxs-lookup"><span data-stu-id="156cc-203">Equality operators</span></span> | <ul><li> <span data-ttu-id="156cc-204">等于 `eq`</span><span class="sxs-lookup"><span data-stu-id="156cc-204">equals `eq`</span></span> </li><li> <span data-ttu-id="156cc-205">不等于 `ne`</span><span class="sxs-lookup"><span data-stu-id="156cc-205">not equals `ne`</span></span></li><li> <span data-ttu-id="156cc-206">否定式 `not`</span><span class="sxs-lookup"><span data-stu-id="156cc-206">Negation `not`</span></span></li><li> <span data-ttu-id="156cc-207">在 `in` 内</span><span class="sxs-lookup"><span data-stu-id="156cc-207">in `in`</span></span></li></ul> |
| <span data-ttu-id="156cc-208">关系运算符</span><span class="sxs-lookup"><span data-stu-id="156cc-208">Relational operators</span></span> | <ul><li> <span data-ttu-id="156cc-209">小于 `lt`</span><span class="sxs-lookup"><span data-stu-id="156cc-209">less than `lt`</span></span> </li><li> <span data-ttu-id="156cc-210">大于 `gt`</span><span class="sxs-lookup"><span data-stu-id="156cc-210">greater than `gt`</span></span></li><li> <span data-ttu-id="156cc-211">小于或等于 `le`</span><span class="sxs-lookup"><span data-stu-id="156cc-211">less than or equal to `le`</span></span></li><li> <span data-ttu-id="156cc-212">大于或等于 `ge`</span><span class="sxs-lookup"><span data-stu-id="156cc-212">greater than or equal to `ge`</span></span></li></ul> |
| <span data-ttu-id="156cc-213">Lambda 运算符</span><span class="sxs-lookup"><span data-stu-id="156cc-213">Lambda operators</span></span> | <ul><li> <span data-ttu-id="156cc-214">任何 `any`</span><span class="sxs-lookup"><span data-stu-id="156cc-214">any `any`</span></span> </li><li> <span data-ttu-id="156cc-215">全部 `all`</span><span class="sxs-lookup"><span data-stu-id="156cc-215">all `all`</span></span></li></ul>|
| <span data-ttu-id="156cc-216">条件运算符</span><span class="sxs-lookup"><span data-stu-id="156cc-216">Conditional operators</span></span> | <ul><li> <span data-ttu-id="156cc-217">和 `and`</span><span class="sxs-lookup"><span data-stu-id="156cc-217">and `and`</span></span> </li><li> <span data-ttu-id="156cc-218">或 `or`</span><span class="sxs-lookup"><span data-stu-id="156cc-218">or `or`</span></span></li> |
| <span data-ttu-id="156cc-219">函数</span><span class="sxs-lookup"><span data-stu-id="156cc-219">Functions</span></span> | <ul><li> <span data-ttu-id="156cc-220">开头为 `startsWith`</span><span class="sxs-lookup"><span data-stu-id="156cc-220">Starts with `startsWith`</span></span> </li><li> <span data-ttu-id="156cc-221">结尾为 `endsWith`</span><span class="sxs-lookup"><span data-stu-id="156cc-221">Ends with `endsWith`</span></span></li><li> <span data-ttu-id="156cc-222">包含`contains`</span><span class="sxs-lookup"><span data-stu-id="156cc-222">Contains `contains`</span></span></li></ul>|


> <span data-ttu-id="156cc-223">**注意:** 对这些运算符的支持因实体而异，某些属性仅在 [高级查询](/graph/aad-advanced-queries)中支持`$filter`。</span><span class="sxs-lookup"><span data-stu-id="156cc-223">**Note:** Support for these operators varies by entity and some properties support `$filter` only in [advanced queries](/graph/aad-advanced-queries).</span></span> <span data-ttu-id="156cc-224">有关详细信息，请参阅特定实体文档。</span><span class="sxs-lookup"><span data-stu-id="156cc-224">See the specific entity documentation for details.</span></span>

### <a name="filter-using-lambda-operators"></a><span data-ttu-id="156cc-225">使用 lambda 运算符进行筛选</span><span class="sxs-lookup"><span data-stu-id="156cc-225">Filter using lambda operators</span></span>

<span data-ttu-id="156cc-226">OData 定义 `any` 和 `all` 运算符以评估多值属性的匹配项，即基元值(如字符串 类型或实体集合)的集合。</span><span class="sxs-lookup"><span data-stu-id="156cc-226">OData defines the `any` and `all` operators to evaluate matches on multi-valued properties, that is, either collection of primitive values such as String types or collection of entities.</span></span>

<span data-ttu-id="156cc-227">`any`运算符以迭代方式将布尔表达式应用于集合的每个成员，如果集合的 *任何成员* 的表达式为`true`，则返回`true`;否则返回`false`。</span><span class="sxs-lookup"><span data-stu-id="156cc-227">The `any` operator iteratively applies a Boolean expression to each member of a collection and returns `true` if the expression is `true` for *any member* of the collection, otherwise it returns `false`.</span></span> <span data-ttu-id="156cc-228">以下是`any`运算符的语法:</span><span class="sxs-lookup"><span data-stu-id="156cc-228">The following is the syntax of the `any` operator:</span></span>

```http
$filter=param/any(var:var/subparam eq 'value-to-match')
```

<span data-ttu-id="156cc-229">其中</span><span class="sxs-lookup"><span data-stu-id="156cc-229">Where</span></span>
+ <span data-ttu-id="156cc-230">*param* 是包含值集合或实体集合的属性。</span><span class="sxs-lookup"><span data-stu-id="156cc-230">*param* is the property that contains a collection of values or a collection of entities.</span></span>
+ <span data-ttu-id="156cc-231">*var:var* 是一个范围变量，用于在迭代期间保存集合的当前元素。</span><span class="sxs-lookup"><span data-stu-id="156cc-231">*var:var* is a range variable that holds the current element of the collection during iteration.</span></span> <span data-ttu-id="156cc-232">此变量几乎可以被命名为任何内容，例如， *adele:adele* 或 *x:x*。</span><span class="sxs-lookup"><span data-stu-id="156cc-232">This variable can be named almost anything, for example, *adele:adele* or *x:x*.</span></span>
+ <span data-ttu-id="156cc-233">当查询应用于实体集合时，*subparam* 是必需的。</span><span class="sxs-lookup"><span data-stu-id="156cc-233">*subparam* is required when the query applies to a collection of entities.</span></span> <span data-ttu-id="156cc-234">它表示正在匹配其值的复杂类型的属性。</span><span class="sxs-lookup"><span data-stu-id="156cc-234">It represents the property of the complex type whose value we are matching.</span></span>
+ <span data-ttu-id="156cc-235">*value-to-match* 表示要与之匹配的集合的成员。</span><span class="sxs-lookup"><span data-stu-id="156cc-235">*value-to-match* represents the member of the collection against which we are matching.</span></span>

<span data-ttu-id="156cc-236">例如，用户资源的 **imAddresses** 属性包含基元类型 String 的集合。</span><span class="sxs-lookup"><span data-stu-id="156cc-236">For example, the **imAddresses** property of the user resource contains a collection of primitive type String.</span></span> <span data-ttu-id="156cc-237">以下查询仅检索 imAddress 为 `admin@contoso.com`的用户。</span><span class="sxs-lookup"><span data-stu-id="156cc-237">The following query retrieves only users with an imAddress of `admin@contoso.com`.</span></span>

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=imAddresses/any(s:s eq 'admin@contoso.com')
```

<span data-ttu-id="156cc-238">用户资源的 **assignedLicenses** 属性包含 **assignedLicense** 对象的集合，一个包含两个属性 **skuId** 和 **disabledPlans** 的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="156cc-238">The **assignedLicenses** property of the user resource contains a collection of **assignedLicense** objects, a complex type with two properties, **skuId** and **disabledPlans**.</span></span> <span data-ttu-id="156cc-239">以下查询仅检索具有由 **skuId** `184efa21-98c3-4e5d-95ab-d07053a96e67`标识的已分配许可证的用户。</span><span class="sxs-lookup"><span data-stu-id="156cc-239">The following query retrieves only users with an assigned license identified by the **skuId** `184efa21-98c3-4e5d-95ab-d07053a96e67`.</span></span>

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=assignedLicenses/any(s:s/skuId eq 184efa21-98c3-4e5d-95ab-d07053a96e67)
```

<span data-ttu-id="156cc-240">若要对 `any` 子句内表达式的结果求反，请使用 `NOT` 运算符，而不是 `ne` 运算符。</span><span class="sxs-lookup"><span data-stu-id="156cc-240">To negate the result of the expression inside the `any` clause, use the `NOT` operator, not the `ne` operator.</span></span> <span data-ttu-id="156cc-241">例如，以下查询仅检索未分配 `admin@contoso.com` 的 **imAddress** 的用户。</span><span class="sxs-lookup"><span data-stu-id="156cc-241">For example, the following query retrieves only users who are not assigned the **imAddress** of `admin@contoso.com`.</span></span>
><span data-ttu-id="156cc-242">**注意:** 对于像用户这样的目录对象，`NOT` 和 `ne` 运算符仅在 [高级查询](/graph/aad-advanced-queries) 中受支持。</span><span class="sxs-lookup"><span data-stu-id="156cc-242">**Note:** For directory objects like users, the `NOT` and `ne` operators are supported only in [advanced queries](/graph/aad-advanced-queries).</span></span>

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=NOT(imAddresses/any(s:s eq 'admin@contoso.com'))&$count=true
ConsistencyLevel: eventual
```

<span data-ttu-id="156cc-243">`all`运算符以迭代方式将布尔表达式应用于集合的每个成员，如果集合的 *所有成员* 的表达式为`true`，则返回`true`;否则返回`false`。</span><span class="sxs-lookup"><span data-stu-id="156cc-243">The `all` operator applies a Boolean expression to each member of a collection and returns `true` if the expression is `true` for *all members* of the collection, otherwise it returns `false`.</span></span> <span data-ttu-id="156cc-244">任何属性都不支持它。</span><span class="sxs-lookup"><span data-stu-id="156cc-244">It is not supported by any property.</span></span>

### <a name="examples-using-the-filter-query-operator"></a><span data-ttu-id="156cc-245">使用筛选器查询运算符的示例</span><span class="sxs-lookup"><span data-stu-id="156cc-245">Examples using the filter query operator</span></span>

<span data-ttu-id="156cc-246">下表展示了一些使用 `$filter` 查询参数的示例。</span><span class="sxs-lookup"><span data-stu-id="156cc-246">The following table shows some examples that use the `$filter` query parameter.</span></span> <span data-ttu-id="156cc-247">如需了解 `$filter` 语法的更多详情，请参阅 [OData 协议][odata-filter]。</span><span class="sxs-lookup"><span data-stu-id="156cc-247">For more details about `$filter` syntax, see the [OData protocol][odata-filter].</span></span>

> <span data-ttu-id="156cc-248">**注意：** 单击示例可以在 [Graph 浏览器][graph-explorer]中试调用。</span><span class="sxs-lookup"><span data-stu-id="156cc-248">**Note:** Click the examples to try them in [Graph Explorer][graph-explorer].</span></span>

| <span data-ttu-id="156cc-249">说明</span><span class="sxs-lookup"><span data-stu-id="156cc-249">Description</span></span> | <span data-ttu-id="156cc-250">示例</span><span class="sxs-lookup"><span data-stu-id="156cc-250">Example</span></span>
|:------------|:--------|
| <span data-ttu-id="156cc-251">跨多个属性获取名为 Mary 的用户。</span><span class="sxs-lookup"><span data-stu-id="156cc-251">Get all users with the name Mary across multiple properties.</span></span> | <span data-ttu-id="156cc-252">[GET](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(displayName,'mary')+or+startswith(givenName,'mary')+or+startswith(surname,'mary')+or+startswith(mail,'mary')+or+startswith(userPrincipalName,'mary')&method=GET&version=v1.0) `../users?$filter=startswith(displayName,'mary') or startswith(givenName,'mary') or startswith(surname,'mary') or startswith(mail,'mary') or startswith(userPrincipalName,'mary')`</span><span class="sxs-lookup"><span data-stu-id="156cc-252">[GET](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(displayName,'mary')+or+startswith(givenName,'mary')+or+startswith(surname,'mary')+or+startswith(mail,'mary')+or+startswith(userPrincipalName,'mary')&method=GET&version=v1.0) `../users?$filter=startswith(displayName,'mary') or startswith(givenName,'mary') or startswith(surname,'mary') or startswith(mail,'mary') or startswith(userPrincipalName,'mary')`</span></span> |
| <span data-ttu-id="156cc-253">获取邮件域等于“hotmail.com”的所有用户</span><span class="sxs-lookup"><span data-stu-id="156cc-253">Get all users with mail domain equal to 'hotmail.com'</span></span> | <span data-ttu-id="156cc-254">
  [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24count%3Dtrue%26%24filter%3DendsWith(mail%2C'%40hotmail.com')%26%24select%3Did%2CdisplayName%2Cmail&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$count=true&$filter=endsWith(mail,'@hotmail.com')`。</span><span class="sxs-lookup"><span data-stu-id="156cc-254">[GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24count%3Dtrue%26%24filter%3DendsWith(mail%2C'%40hotmail.com')%26%24select%3Did%2CdisplayName%2Cmail&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$count=true&$filter=endsWith(mail,'@hotmail.com')`.</span></span> <span data-ttu-id="156cc-255">这是一个[高级查询](/graph/aad-advanced-queries)。</span><span class="sxs-lookup"><span data-stu-id="156cc-255">This is an [advanced query](/graph/aad-advanced-queries).</span></span> |
| <span data-ttu-id="156cc-256">获取 2017 年 7 月 1 日之后开始的所有登录用户的事件。</span><span class="sxs-lookup"><span data-stu-id="156cc-256">Get all the signed-in user's events that start after 7/1/2017.</span></span> | <span data-ttu-id="156cc-257">[GET](https://developer.microsoft.com/graph/graph-explorer?request=me/events?$filter=start/dateTime+ge+'2017-07-01T08:00'&method=GET&version=v1.0) `../me/events?$filter=start/dateTime ge '2017-07-01T08:00'`</span><span class="sxs-lookup"><span data-stu-id="156cc-257">[GET](https://developer.microsoft.com/graph/graph-explorer?request=me/events?$filter=start/dateTime+ge+'2017-07-01T08:00'&method=GET&version=v1.0) `../me/events?$filter=start/dateTime ge '2017-07-01T08:00'`</span></span> |
| <span data-ttu-id="156cc-258">获取登录用户收到的来自特定地址的所有电子邮件。</span><span class="sxs-lookup"><span data-stu-id="156cc-258">Get all emails from a specific address received by the signed-in user.</span></span> | <span data-ttu-id="156cc-259">[GET](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=from/emailAddress/address+eq+'someuser@.com'&method=GET&version=v1.0) `../me/messages?$filter=from/emailAddress/address eq 'someuser@example.com'`</span><span class="sxs-lookup"><span data-stu-id="156cc-259">[GET](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=from/emailAddress/address+eq+'someuser@.com'&method=GET&version=v1.0) `../me/messages?$filter=from/emailAddress/address eq 'someuser@example.com'`</span></span> |
| <span data-ttu-id="156cc-260">获取登录用户在 2017 年 4 月收到的所有电子邮件。</span><span class="sxs-lookup"><span data-stu-id="156cc-260">Get all emails received by the signed-in user in April 2017.</span></span> | <span data-ttu-id="156cc-261">[GET](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=ReceivedDateTime+ge+2017-04-01+and+receivedDateTime+lt+2017-05-01&method=GET&version=v1.0) `../me/mailFolders/inbox/messages?$filter=ReceivedDateTime ge 2017-04-01 and receivedDateTime lt 2017-05-01`</span><span class="sxs-lookup"><span data-stu-id="156cc-261">[GET](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=ReceivedDateTime+ge+2017-04-01+and+receivedDateTime+lt+2017-05-01&method=GET&version=v1.0) `../me/mailFolders/inbox/messages?$filter=ReceivedDateTime ge 2017-04-01 and receivedDateTime lt 2017-05-01`</span></span> |
| <span data-ttu-id="156cc-262">获取登录用户收件箱中的所有未读邮件。</span><span class="sxs-lookup"><span data-stu-id="156cc-262">Get all unread mail in the signed-in user's Inbox.</span></span> | <span data-ttu-id="156cc-263">[GET](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=isRead+eq+false&method=GET&version=v1.0) `../me/mailFolders/inbox/messages?$filter=isRead eq false`</span><span class="sxs-lookup"><span data-stu-id="156cc-263">[GET](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=isRead+eq+false&method=GET&version=v1.0) `../me/mailFolders/inbox/messages?$filter=isRead eq false`</span></span> |
| <span data-ttu-id="156cc-264">获取零售和销售部门中的所有用户。</span><span class="sxs-lookup"><span data-stu-id="156cc-264">Get all users in the Retail and Sales departments.</span></span> | <span data-ttu-id="156cc-265">
  [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24filter%3Ddepartment%20in%20('Retail'%2C%20'Sales')&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com) `../users?$filter=department in ('Retail', 'Sales')`</span><span class="sxs-lookup"><span data-stu-id="156cc-265">[GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24filter%3Ddepartment%20in%20('Retail'%2C%20'Sales')&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com) `../users?$filter=department in ('Retail', 'Sales')`</span></span>| 
| <span data-ttu-id="156cc-266">列出具有处于挂起状态的特定服务计划的用户。</span><span class="sxs-lookup"><span data-stu-id="156cc-266">List users with a particular service plan that is in a suspended state.</span></span> | <span data-ttu-id="156cc-267">
  [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24filter%3DassignedPlans%2Fany(a%3Aa%2FservicePlanId%20eq%202e2ddb96-6af9-4b1d-a3f0-d6ecfd22edb2%20and%20a%2FcapabilityStatus%20eq%20'Suspended')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=assignedPlans/any(a:a/servicePlanId eq 2e2ddb96-6af9-4b1d-a3f0-d6ecfd22edb2 and a/capabilityStatus eq 'Suspended')&$count=true`。</span><span class="sxs-lookup"><span data-stu-id="156cc-267">[GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24filter%3DassignedPlans%2Fany(a%3Aa%2FservicePlanId%20eq%202e2ddb96-6af9-4b1d-a3f0-d6ecfd22edb2%20and%20a%2FcapabilityStatus%20eq%20'Suspended')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=assignedPlans/any(a:a/servicePlanId eq 2e2ddb96-6af9-4b1d-a3f0-d6ecfd22edb2 and a/capabilityStatus eq 'Suspended')&$count=true`.</span></span> <span data-ttu-id="156cc-268">这是一个[高级查询](/graph/aad-advanced-queries)。</span><span class="sxs-lookup"><span data-stu-id="156cc-268">This is an [advanced query](/graph/aad-advanced-queries).</span></span> |
| <span data-ttu-id="156cc-269">列出组织中的所有非 Microsoft 365 组。</span><span class="sxs-lookup"><span data-stu-id="156cc-269">List all non-Microsoft 365 groups in an organization.</span></span> | <span data-ttu-id="156cc-270">
  [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=groups%3F%24filter%3DNOT%20groupTypes%2Fany(c%3Ac%20eq%20'Unified')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../groups?$filter=NOT groupTypes/any(c:c eq 'Unified')&$count=true`。</span><span class="sxs-lookup"><span data-stu-id="156cc-270">[GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=groups%3F%24filter%3DNOT%20groupTypes%2Fany(c%3Ac%20eq%20'Unified')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../groups?$filter=NOT groupTypes/any(c:c eq 'Unified')&$count=true`.</span></span> <span data-ttu-id="156cc-271">这是一个[高级查询](/graph/aad-advanced-queries)。</span><span class="sxs-lookup"><span data-stu-id="156cc-271">This is an [advanced query](/graph/aad-advanced-queries).</span></span> |
| <span data-ttu-id="156cc-272">列出其公司名称不是未定义(即，不是 `null` 值)或 Microsoft 的所有用户。</span><span class="sxs-lookup"><span data-stu-id="156cc-272">List all users whose company name is not undefined (that is, not a `null` value) or Microsoft.</span></span> | <span data-ttu-id="156cc-273">
  [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24filter%3DcompanyName%20ne%20null%20and%20NOT(companyName%20eq%20'Microsoft')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=companyName ne null and NOT(companyName eq 'Microsoft')&$count=true`。</span><span class="sxs-lookup"><span data-stu-id="156cc-273">[GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24filter%3DcompanyName%20ne%20null%20and%20NOT(companyName%20eq%20'Microsoft')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=companyName ne null and NOT(companyName eq 'Microsoft')&$count=true`.</span></span> <span data-ttu-id="156cc-274">这是一个[高级查询](/graph/aad-advanced-queries)。</span><span class="sxs-lookup"><span data-stu-id="156cc-274">This is an [advanced query](/graph/aad-advanced-queries).</span></span> |
| <span data-ttu-id="156cc-275">列出其公司名称是未定义或 Microsoft 的所有用户。</span><span class="sxs-lookup"><span data-stu-id="156cc-275">List all users whose company name is either undefined or Microsoft.</span></span> | <span data-ttu-id="156cc-276">
  [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24filter%3DcompanyName%20in%20(null%2C%20'Microsoft')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=companyName in (null, 'Microsoft')&$count=true`。</span><span class="sxs-lookup"><span data-stu-id="156cc-276">[GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24filter%3DcompanyName%20in%20(null%2C%20'Microsoft')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=companyName in (null, 'Microsoft')&$count=true`.</span></span> <span data-ttu-id="156cc-277">这是一个[高级查询](/graph/aad-advanced-queries)。</span><span class="sxs-lookup"><span data-stu-id="156cc-277">This is an [advanced query](/graph/aad-advanced-queries).</span></span> |
| <span data-ttu-id="156cc-278">使用 OData 转换可实现显示名称以“ a”开头(包括返回的对象数)的组中的临时成员资格。</span><span class="sxs-lookup"><span data-stu-id="156cc-278">Use OData cast to get transitive membership in groups with a display name that starts with 'a' including a count of returned objects.</span></span> | <span data-ttu-id="156cc-279">
  [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=me%2FtransitiveMemberOf%2Fmicrosoft.graph.group%3F%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../me/transitiveMemberOf/microsoft.graph.group?$count=true&$filter=startswith(displayName, 'a')`。</span><span class="sxs-lookup"><span data-stu-id="156cc-279">[GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=me%2FtransitiveMemberOf%2Fmicrosoft.graph.group%3F%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../me/transitiveMemberOf/microsoft.graph.group?$count=true&$filter=startswith(displayName, 'a')`.</span></span> <span data-ttu-id="156cc-280">这是一个[高级查询](/graph/aad-advanced-queries)。</span><span class="sxs-lookup"><span data-stu-id="156cc-280">This is an [advanced query](/graph/aad-advanced-queries).</span></span> |

## <a name="format-parameter"></a><span data-ttu-id="156cc-281">format 参数</span><span class="sxs-lookup"><span data-stu-id="156cc-281">format parameter</span></span>

<span data-ttu-id="156cc-282">使用 `$format` 查询参数，指定 Microsoft Graph 返回的项的媒体格式。</span><span class="sxs-lookup"><span data-stu-id="156cc-282">Use the `$format` query parameter to specify the media format of the items returned from Microsoft Graph.</span></span>

<span data-ttu-id="156cc-283">例如，下面的请求以 json 格式返回组织中的用户：</span><span class="sxs-lookup"><span data-stu-id="156cc-283">For example, the following request returns the users in the organization in the json format:</span></span>

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$format=json
```


> <span data-ttu-id="156cc-284">**注意：**`$format` 查询参数支持许多格式（例如，atom、xml 和 json），但可能无法返回所有格式的结果。</span><span class="sxs-lookup"><span data-stu-id="156cc-284">**Note:** The `$format` query parameter supports a number of formats (for example, atom, xml, and json) but results may not be returned in all formats.</span></span>

## <a name="orderby-parameter"></a><span data-ttu-id="156cc-285">orderby 参数</span><span class="sxs-lookup"><span data-stu-id="156cc-285">orderby parameter</span></span>

<span data-ttu-id="156cc-286">使用 `$orderby` 查询参数指定从 Microsoft Graph 返回的项的排序顺序。</span><span class="sxs-lookup"><span data-stu-id="156cc-286">Use the `$orderby` query parameter to specify the sort order of the items returned from Microsoft Graph.</span></span> <span data-ttu-id="156cc-287">默认顺序为升序。</span><span class="sxs-lookup"><span data-stu-id="156cc-287">The default order is ascending order.</span></span>

<span data-ttu-id="156cc-288">例如，以下请求返回按用户显示名称进行排序的组织中的用户：</span><span class="sxs-lookup"><span data-stu-id="156cc-288">For example, the following request returns the users in the organization ordered by their display name:</span></span>

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$orderby=displayName
```

<span data-ttu-id="156cc-p132">还可以按复杂类型实体进行排序。下面的请求获取邮件，并按 **from** 属性的 **address** 字段（复杂类型为 **emailAddress**）进行排序：</span><span class="sxs-lookup"><span data-stu-id="156cc-p132">You can also sort by complex type entities. The following request gets messages and sorts them by the **address** field of the **from** property, which is of the complex type **emailAddress**:</span></span>

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages?$orderby=from/emailAddress/address
```

<span data-ttu-id="156cc-291">若要以升序或降序对结果进行排序，请向字段名称追加 `asc` 或 `desc`，并用空格隔开。例如，`?$orderby=name%20desc`。</span><span class="sxs-lookup"><span data-stu-id="156cc-291">To sort the results in ascending or descending order, append either `asc` or `desc` to the field name, separated by a space; for example, `?$orderby=name%20desc`.</span></span> <span data-ttu-id="156cc-292">如果未指定排序顺序，则推断默认值(升序)。</span><span class="sxs-lookup"><span data-stu-id="156cc-292">If the sort order is not specified, the default (ascending order) is inferred.</span></span>

<span data-ttu-id="156cc-p134">通过一些 API，可以对多个属性的结果进行排序。例如，以下请求首先按发件人名称以降序(Z 到 A)排序用户收件箱中的邮件，然后按主题以升序(默认)排序邮件。</span><span class="sxs-lookup"><span data-stu-id="156cc-p134">With some APIs, you can order results on multiple properties. For example, the following request orders the messages in the user's Inbox, first by the name of the person who sent it in descending order (Z to A), and then by subject in ascending order (default).</span></span>

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailFolders/Inbox/messages?$orderby=from/emailAddress/name desc,subject
```

> <span data-ttu-id="156cc-295">**注意:** 如果指定 `$filter`，服务器会推断结果的排序顺序。</span><span class="sxs-lookup"><span data-stu-id="156cc-295">**Note:** When you specify `$filter` the server will infer a sort order for the results.</span></span> <span data-ttu-id="156cc-296">如果同时使用 `$orderby` 和 `$filter` 获取消息，因为服务器始终会推断 `$filter` 结果的排序顺序，必须[以特定的方式指定属性](/graph/api/user-list-messages#using-filter-and-orderby-in-the-same-query)。</span><span class="sxs-lookup"><span data-stu-id="156cc-296">If you use both `$orderby` and `$filter` to get messages, because the server always infers a sort order for the results of a `$filter`, you must [specify properties in certain ways](/graph/api/user-list-messages#using-filter-and-orderby-in-the-same-query).</span></span>


<span data-ttu-id="156cc-297">下面的示例展示了如何按 **subject** 和 **importance** 属性筛选查询，再按 **subject**、**importance** 和 **receivedDateTime** 属性进行降序排序。</span><span class="sxs-lookup"><span data-stu-id="156cc-297">The following example shows a query filtered by the **subject** and **importance** properties, and then sorted by the **subject**, **importance**, and **receivedDateTime** properties in descending order.</span></span>

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages?$filter=Subject eq 'welcome' and importance eq 'normal'&$orderby=subject,importance,receivedDateTime desc
```


> [!NOTE] 
> <span data-ttu-id="156cc-298">目录对象支持组合 `$orderby` 和 `$filter` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="156cc-298">Combining `$orderby` and `$filter` query parameters is supported for directory objects.</span></span> <span data-ttu-id="156cc-299">请参阅[Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。</span><span class="sxs-lookup"><span data-stu-id="156cc-299">See [Advanced query capabilities in Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

## <a name="search-parameter"></a><span data-ttu-id="156cc-300">search 参数</span><span class="sxs-lookup"><span data-stu-id="156cc-300">search parameter</span></span>

<span data-ttu-id="156cc-301">使用 `$search` 查询参数限制与搜索条件匹配的请求结果。</span><span class="sxs-lookup"><span data-stu-id="156cc-301">Use the `$search` query parameter to restrict the results of a request to match a search criterion.</span></span> <span data-ttu-id="156cc-302">它的语法和行为因 API 操作而异。</span><span class="sxs-lookup"><span data-stu-id="156cc-302">It's syntax and behavior varies from one API operation to another.</span></span> <span data-ttu-id="156cc-303">若要查看不同资源之间 `$search` 的语法，请参阅 [使用$search查询参数匹配搜索条件](/graph/search-query-parameter)。</span><span class="sxs-lookup"><span data-stu-id="156cc-303">To see the syntax for `$search` across different resources, see [Use the $search query parameter to match a search criterion](/graph/search-query-parameter).</span></span>

## <a name="select-parameter"></a><span data-ttu-id="156cc-304">select 参数</span><span class="sxs-lookup"><span data-stu-id="156cc-304">select parameter</span></span>

<span data-ttu-id="156cc-305">使用 `$select` 查询参数返回一组不同于单个资源的默认集或资源集合的属性。</span><span class="sxs-lookup"><span data-stu-id="156cc-305">Use the `$select` query parameter to return a set of properties that are different than the default set for an individual resource or a collection of resources.</span></span> <span data-ttu-id="156cc-306">使用 `$select`，可以指定默认属性的子集或超集。</span><span class="sxs-lookup"><span data-stu-id="156cc-306">With `$select`, you can specify a subset or a superset of the default properties.</span></span>

<span data-ttu-id="156cc-307">例如，检索登录用户的邮件时，可以指定仅返回 **from** 和 **subject** 属性：</span><span class="sxs-lookup"><span data-stu-id="156cc-307">For example, when retrieving the messages of the signed-in user, you can specify that only the **from** and **subject** properties be returned:</span></span>

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages?$select=from,subject
```


> <span data-ttu-id="156cc-308">**重要说明：** 一般来说，建议使用 `$select` 将查询返回的属性限制为应用所需的属性。</span><span class="sxs-lookup"><span data-stu-id="156cc-308">**Important:** In general, we recommend that you use `$select` to limit the properties returned by a query to those needed by your app.</span></span> <span data-ttu-id="156cc-309">这对于可能返回大型结果集的查询尤为有用。</span><span class="sxs-lookup"><span data-stu-id="156cc-309">This is especially true of queries that might potentially return a large result set.</span></span> <span data-ttu-id="156cc-310">限制每行返回的属性将减少网络负载并帮助提升应用的性能。</span><span class="sxs-lookup"><span data-stu-id="156cc-310">Limiting the properties returned in each row will reduce network load and help improve your app's performance.</span></span>
>
> <span data-ttu-id="156cc-p140">在 `v1.0` 中，从 [directoryObject](/graph/api/resources/directoryobject) 派生的一些 Azure AD 资源（如 [user](/graph/api/resources/user) 和 [group](/graph/api/resources/group)）在读取时返回受限的默认属性子集。对于这些资源，必须使用 `$select` 将属性返回到默认集之外。</span><span class="sxs-lookup"><span data-stu-id="156cc-p140">In `v1.0`, some Azure AD resources that derive from [directoryObject](/graph/api/resources/directoryobject), like [user](/graph/api/resources/user) and [group](/graph/api/resources/group), return a limited, default subset of properties on reads. For these resources, you must use `$select` to return properties outside of the default set.</span></span>  

## <a name="skip-parameter"></a><span data-ttu-id="156cc-313">skip 参数</span><span class="sxs-lookup"><span data-stu-id="156cc-313">skip parameter</span></span>

<span data-ttu-id="156cc-p141">使用 `$skip` 查询参数设置要在集合开头跳过的项数。例如，以下请求返回按照创建日期排序的用户的事件，从集合中的第 21 个事件开始：</span><span class="sxs-lookup"><span data-stu-id="156cc-p141">Use the `$skip` query parameter to set the number of items to skip at the start of a collection. For example, the following request returns events for the user sorted by date created, starting with the 21st event in the collection:</span></span>

```msgraph-interactive
GET  https://graph.microsoft.com/v1.0/me/events?$orderby=createdDateTime&$skip=20
```


> <span data-ttu-id="156cc-316">**注意：** 一些 Microsoft Graph API 使用 `$skip` 实现分页，如 Outlook 邮件和日历（**message**、**event** 和 **calendar**）。</span><span class="sxs-lookup"><span data-stu-id="156cc-316">**Note:** Some Microsoft Graph APIs, like Outlook Mail and Calendars (**message**, **event**, and **calendar**), use `$skip` to implement paging.</span></span> <span data-ttu-id="156cc-317">当查询结果跨多个页面时，这些 API 会返回 `@odata:nextLink` 属性，具有包含 `$skip` 参数的 URL。</span><span class="sxs-lookup"><span data-stu-id="156cc-317">When results of a query span multiple pages, these APIs will return an `@odata:nextLink` property with a URL that contains a `$skip` parameter.</span></span> <span data-ttu-id="156cc-318">可以使用此 URL 返回下一页结果。</span><span class="sxs-lookup"><span data-stu-id="156cc-318">You can use this URL to return the next page of results.</span></span> <span data-ttu-id="156cc-319">若要了解详细信息，请参阅[分页](./paging.md)。</span><span class="sxs-lookup"><span data-stu-id="156cc-319">To learn more, see [Paging](./paging.md).</span></span>
>
> <span data-ttu-id="156cc-320">默认情况下，针对目录对象的高级查询所需的 **ConsistencyLevel** 标头不包含在后续页面请求中。</span><span class="sxs-lookup"><span data-stu-id="156cc-320">The **ConsistencyLevel** header required for advanced queries against directory objects is not included by default in subsequent page requests.</span></span> <span data-ttu-id="156cc-321">必须在后续页面中显式设置它。</span><span class="sxs-lookup"><span data-stu-id="156cc-321">It must be set explicitly in subsequent pages.</span></span>

## <a name="skiptoken-parameter"></a><span data-ttu-id="156cc-322">skipToken 参数</span><span class="sxs-lookup"><span data-stu-id="156cc-322">skipToken parameter</span></span>

<span data-ttu-id="156cc-323">由于服务器端分页或由于使用 [`$top`](#top-parameter) 参数来限制响应的页面大小，致使一些请求返回多页数据。</span><span class="sxs-lookup"><span data-stu-id="156cc-323">Some requests return multiple pages of data, either due to server-side paging or due to the use of the [`$top`](#top-parameter) parameter to limit the page size of the response.</span></span> <span data-ttu-id="156cc-324">许多 Microsoft Graph API 使用 `skipToken` 查询参数来引用结果的后续页面。</span><span class="sxs-lookup"><span data-stu-id="156cc-324">Many Microsoft Graph APIs use the `skipToken` query parameter to reference subsequent pages of the result.</span></span>  
<span data-ttu-id="156cc-325">`$skiptoken` 参数包含引用下一页结果的不透明令牌，并在响应的 `@odata.nextLink` 属性中提供的 URL 中返回。</span><span class="sxs-lookup"><span data-stu-id="156cc-325">The `$skiptoken` parameter contains an opaque token that references the next page of results and is returned in the URL provided in the `@odata.nextLink` property in the response.</span></span> <span data-ttu-id="156cc-326">若要了解详细信息，请参阅[分页](./paging.md)。</span><span class="sxs-lookup"><span data-stu-id="156cc-326">To learn more, see [Paging](./paging.md).</span></span>
> <span data-ttu-id="156cc-327">**注意**:如果对目录对象的查询使用 OData 计数(在查询字符串中添加 `$count=true`)，则 `@odata.count` 属性将仅在第一页中出现。</span><span class="sxs-lookup"><span data-stu-id="156cc-327">**Note:** If you're using OData Count (adding `$count=true` in the query string) for queries against directory objects, the `@odata.count` property is present only in the first page.</span></span>
>
> <span data-ttu-id="156cc-328">默认情况下，针对目录对象的高级查询所需的 **ConsistencyLevel** 标头不包含在后续页面请求中。</span><span class="sxs-lookup"><span data-stu-id="156cc-328">The **ConsistencyLevel** header required for advanced queries against directory objects is not included by default in subsequent page requests.</span></span> <span data-ttu-id="156cc-329">必须在后续页面中显式设置它。</span><span class="sxs-lookup"><span data-stu-id="156cc-329">It must be set explicitly in subsequent pages.</span></span>

## <a name="top-parameter"></a><span data-ttu-id="156cc-330">top 参数</span><span class="sxs-lookup"><span data-stu-id="156cc-330">top parameter</span></span>

<span data-ttu-id="156cc-331">使用 `$top` 查询参数指定结果集的页面大小。</span><span class="sxs-lookup"><span data-stu-id="156cc-331">Use the `$top` query parameter to specify the page size of the result set.</span></span> 

<span data-ttu-id="156cc-332">如果结果集中还剩余多个项目，则响应正文将包含 `@odata.nextLink` 参数。</span><span class="sxs-lookup"><span data-stu-id="156cc-332">If more items remain in the result set, the response body will contain an `@odata.nextLink` parameter.</span></span> <span data-ttu-id="156cc-333">此参数包含可用于获取下一页结果的 URL。</span><span class="sxs-lookup"><span data-stu-id="156cc-333">This parameter contains a URL that you can use to get the next page of results.</span></span> <span data-ttu-id="156cc-334">若要了解详细信息，请参阅[分页](./paging.md)。</span><span class="sxs-lookup"><span data-stu-id="156cc-334">To learn more, see [Paging](./paging.md).</span></span> 

<span data-ttu-id="156cc-335">最小值为 $top 1，最大值取决于相应的 API。</span><span class="sxs-lookup"><span data-stu-id="156cc-335">The minimum value of $top is 1 and the maximum depends on the corresponding API.</span></span>  

<span data-ttu-id="156cc-336">例如，以下列表 [请求](/graph/api/user-list-messages) 返回用户邮箱中的前五条消息：</span><span class="sxs-lookup"><span data-stu-id="156cc-336">For example, the following [list messages](/graph/api/user-list-messages) request returns the first five messages in the user's mailbox:</span></span>

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages?$top=5
```


> <span data-ttu-id="156cc-337">默认情况下，针对目录对象的高级查询所需的 **ConsistencyLevel** 标头不包含在后续页面请求中。</span><span class="sxs-lookup"><span data-stu-id="156cc-337">The **ConsistencyLevel** header required for advanced queries against directory objects is not included by default in subsequent page requests.</span></span> <span data-ttu-id="156cc-338">必须在后续页面中显式设置它。</span><span class="sxs-lookup"><span data-stu-id="156cc-338">It must be set explicitly in subsequent pages.</span></span>

## <a name="error-handling-for-query-parameters"></a><span data-ttu-id="156cc-339">查询参数的错误处理</span><span class="sxs-lookup"><span data-stu-id="156cc-339">Error handling for query parameters</span></span>

<span data-ttu-id="156cc-p149">如果不支持指定的查询参数，某些请求将返回错误消息。例如，不能对 `user/photo` 关系使用 `$expand`。</span><span class="sxs-lookup"><span data-stu-id="156cc-p149">Some requests will return an error message if a specified query parameter is not supported. For example, you cannot use `$expand` on the `user/photo` relationship.</span></span> 

```http
https://graph.microsoft.com/v1.0/me?$expand=photo
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

<span data-ttu-id="156cc-342">但是，值得注意的是请求中指定的查询参数可能会自行失败。</span><span class="sxs-lookup"><span data-stu-id="156cc-342">However, it is important to note that query parameters specified in a request might fail silently.</span></span> <span data-ttu-id="156cc-343">不支持的查询参数以及不支持的查询参数组合的情况就是如此。</span><span class="sxs-lookup"><span data-stu-id="156cc-343">This can be true for unsupported query parameters as well as for unsupported combinations of query parameters.</span></span> <span data-ttu-id="156cc-344">在这些情况下，应检查请求返回的数据，以确定指定的查询参数是否具有所需的效果。</span><span class="sxs-lookup"><span data-stu-id="156cc-344">In these cases, you should examine the data returned by the request to determine whether the query parameters you specified had the desired effect.</span></span> 

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

## <a name="see-also"></a><span data-ttu-id="156cc-345">另请参阅</span><span class="sxs-lookup"><span data-stu-id="156cc-345">See also</span></span>

- [<span data-ttu-id="156cc-346">Azure AD 目录对象的高级查询功能</span><span class="sxs-lookup"><span data-stu-id="156cc-346">Advanced query capabilities on Azure AD directory objects</span></span>](/graph/aad-advanced-queries)
- [<span data-ttu-id="156cc-347">使用$search查询参数匹配搜索条件</span><span class="sxs-lookup"><span data-stu-id="156cc-347">Use the $search query parameter to match a search criterion</span></span>](/graph/search-query-parameter)
- [<span data-ttu-id="156cc-348">查询参数限制</span><span class="sxs-lookup"><span data-stu-id="156cc-348">Query parameter limitations</span></span>](known-issues.md#query-parameter-limitations)