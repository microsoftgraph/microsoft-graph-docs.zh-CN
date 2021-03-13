---
title: 请求 Azure AD Graph 和 Microsoft Graph 之间的差异
description: 介绍 Microsoft Graph 请求与 Azure AD 请求的区别，这有助于将应用迁移到较新的服务。
author: dkershaw10
localization_priority: Normal
ms.prod: applications
ms.openlocfilehash: e30a0c98aaf7ec0d042787f511872d02529aaa5c
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760663"
---
# <a name="request-differences-between-azure-ad-graph-and-microsoft-graph"></a><span data-ttu-id="5671e-103">请求 Azure AD Graph 和 Microsoft Graph 之间的差异</span><span class="sxs-lookup"><span data-stu-id="5671e-103">Request differences between Azure AD Graph and Microsoft Graph</span></span>

<span data-ttu-id="5671e-104">本文是步骤 *1：查看迁移应用的* 过程的 API [差异的一部分](migrate-azure-ad-graph-planning-checklist.md)。</span><span class="sxs-lookup"><span data-stu-id="5671e-104">This article is part of *step 1: review API differences* of the [process to migrate apps](migrate-azure-ad-graph-planning-checklist.md).</span></span>

<span data-ttu-id="5671e-105">Microsoft Graph 和 Azure AD Graph API 都是 REST API，它们各自支持查询参数的 ODATA 约定。</span><span class="sxs-lookup"><span data-stu-id="5671e-105">Microsoft Graph and the Azure AD Graph API are both REST APIs and they each support ODATA conventions for query parameters.</span></span> <span data-ttu-id="5671e-106">但是，语法因这两个 API 而异。</span><span class="sxs-lookup"><span data-stu-id="5671e-106">However, the syntax varies between these two APIs.</span></span>

<span data-ttu-id="5671e-107">使用 [Graph 浏览器](https://aka.ms/ge) 针对你自己的数据尝试这些请求模式，因为它是了解请求和响应差异的一种很好的方法。</span><span class="sxs-lookup"><span data-stu-id="5671e-107">Use the [Graph Explorer](https://aka.ms/ge) to try these request patterns against your own data, as it's a great way to learn about the request and response differences.</span></span>

## <a name="basic-requests"></a><span data-ttu-id="5671e-108">基本请求</span><span class="sxs-lookup"><span data-stu-id="5671e-108">Basic requests</span></span>

<span data-ttu-id="5671e-109">下表突出显示了两个 API 之间的主要请求差异：</span><span class="sxs-lookup"><span data-stu-id="5671e-109">The following table highlights the main request differences between the two APIs:</span></span>

|<span data-ttu-id="5671e-110">请求详细信息</span><span class="sxs-lookup"><span data-stu-id="5671e-110">Request details</span></span>| <span data-ttu-id="5671e-111">Azure AD Graph</span><span class="sxs-lookup"><span data-stu-id="5671e-111">Azure AD Graph</span></span> | <span data-ttu-id="5671e-112">Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="5671e-112">Microsoft Graph</span></span> |
|---|---|---|
|<span data-ttu-id="5671e-113">请求语法</span><span class="sxs-lookup"><span data-stu-id="5671e-113">Request syntax</span></span>| `https://graph.windows.net/{tenant_id}/` <br> `{resource}?{version}&query-parameters` | `https://graph.microsoft.com/`<br>`{version}/{resource}?query-parameters`|
|<span data-ttu-id="5671e-114">服务 &nbsp; 终结点：</span><span class="sxs-lookup"><span data-stu-id="5671e-114">Service&nbsp;endpoints:</span></span>||
|<span data-ttu-id="5671e-115">-&nbsp;全局</span><span class="sxs-lookup"><span data-stu-id="5671e-115">-&nbsp;Global</span></span>|`https://graph.windows.net`|`https://graph.microsoft.com`|
|<span data-ttu-id="5671e-116">-&nbsp;美国 &nbsp; Gov &nbsp; L4</span><span class="sxs-lookup"><span data-stu-id="5671e-116">-&nbsp;US&nbsp;Gov&nbsp;L4</span></span>|`https://graph.microsoftazure.us`|`https://graph.microsoft.us`|
|<span data-ttu-id="5671e-117">-&nbsp;美国 &nbsp; Gov &nbsp; L5 &nbsp; (DOD) </span><span class="sxs-lookup"><span data-stu-id="5671e-117">-&nbsp;US&nbsp;Gov&nbsp;L5&nbsp;(DOD)</span></span>|`https://graph.microsoftazure.us`|`https://dod-graph.microsoft.us`|
|<span data-ttu-id="5671e-118">-&nbsp;德国</span><span class="sxs-lookup"><span data-stu-id="5671e-118">-&nbsp;Germany</span></span>|`https://graph.cloudapi.de`|`https://graph.microsoft.de`|
|<span data-ttu-id="5671e-119">-&nbsp;中国 &nbsp; (世纪) </span><span class="sxs-lookup"><span data-stu-id="5671e-119">-&nbsp;China&nbsp;(21Vianet)</span></span>| `https://graph.chinacloudapi.cn`|`https://microsoftgraph.chinacloudapi.cn`|
|<span data-ttu-id="5671e-120">{tenant_id}</span><span class="sxs-lookup"><span data-stu-id="5671e-120">{tenant_id}</span></span>|<span data-ttu-id="5671e-121">在请求中指定租户的 ID。</span><span class="sxs-lookup"><span data-stu-id="5671e-121">Specify the ID of the tenant in the request.</span></span>|<span data-ttu-id="5671e-122">可以选择在请求中指定租户 ID，因为这是从访问令牌推断出来的。</span><span class="sxs-lookup"><span data-stu-id="5671e-122">It's optional to specify a tenant ID in the request as it is inferred from the access token.</span></span><br><br><span data-ttu-id="5671e-123">如果指定租户 ID，它将在 请求 URL 中的 `{version}` `{resource}` 和 之间。</span><span class="sxs-lookup"><span data-stu-id="5671e-123">If you specify the tenant ID, it goes between the `{version}` and the `{resource}` in the request URL.</span></span>|
|<span data-ttu-id="5671e-124">{version}</span><span class="sxs-lookup"><span data-stu-id="5671e-124">{version}</span></span>|<span data-ttu-id="5671e-125">使用必需的查询参数在请求中指定 Azure AD Graph 的发布版本。</span><span class="sxs-lookup"><span data-stu-id="5671e-125">Specify the release version of Azure AD Graph in the request using a required query parameter.</span></span>|<span data-ttu-id="5671e-126">在请求中指定 Microsoft Graph 的发布版本作为 URL 路径的一部分，就在服务终结点之后。</span><span class="sxs-lookup"><span data-stu-id="5671e-126">Specify the release version of Microsoft Graph in the request as part of the URL path just after the service endpoint.</span></span>|

<span data-ttu-id="5671e-127">可以在 Microsoft Graph 中继续使用与 Azure AD Graph 相同的查询参数。</span><span class="sxs-lookup"><span data-stu-id="5671e-127">You can continue to use the same query parameters in Microsoft Graph as Azure AD Graph.</span></span>

### <a name="example-request-comparison"></a><span data-ttu-id="5671e-128">示例请求比较</span><span class="sxs-lookup"><span data-stu-id="5671e-128">Example request comparison</span></span>

<span data-ttu-id="5671e-129">假设您需要一个名称以"Dan"开头的所有用户的列表。</span><span class="sxs-lookup"><span data-stu-id="5671e-129">Suppose you want a list of all users with names beginning with "Dan".</span></span>

<span data-ttu-id="5671e-130">在 Azure AD Graph 中，可以使用此请求：</span><span class="sxs-lookup"><span data-stu-id="5671e-130">In Azure AD Graph, you might use this request:</span></span>

<span data-ttu-id="5671e-131">`GET https://graph.windows.net/contoso.com/users?$filter=startswith(givenName,'Dan')&api-version=1.6` 或 </span><span class="sxs-lookup"><span data-stu-id="5671e-131">`GET https://graph.windows.net/contoso.com/users?$filter=startswith(givenName,'Dan')&api-version=1.6` or</span></span>

`GET https://graph.windows.net/myOrganization/users?$filter=startswith(givenName,'Dan')&api-version=1.6`


<span data-ttu-id="5671e-132">此请求：</span><span class="sxs-lookup"><span data-stu-id="5671e-132">This request:</span></span>

- <span data-ttu-id="5671e-133">面向 Azure AD Graph 版本 1.6。</span><span class="sxs-lookup"><span data-stu-id="5671e-133">Targets version 1.6 of Azure AD Graph.</span></span>
- <span data-ttu-id="5671e-134">指定为 `contoso.com` 租户 ID。</span><span class="sxs-lookup"><span data-stu-id="5671e-134">Specifies `contoso.com` as the tenant ID.</span></span> <span data-ttu-id="5671e-135">替代项显示根据访问 `myOrganization` 令牌中的租户 ID 使用别名。</span><span class="sxs-lookup"><span data-stu-id="5671e-135">The alternative shows the use of an alias `myOrganization` based on the tenant ID in the access token.</span></span>
- <span data-ttu-id="5671e-136">调用 users 资源。</span><span class="sxs-lookup"><span data-stu-id="5671e-136">Calls the users resource.</span></span>
- <span data-ttu-id="5671e-137">使用 `$filter` query 参数将响应限制为以 开头的给定名称 `Dan` 。</span><span class="sxs-lookup"><span data-stu-id="5671e-137">Uses the `$filter` query parameter to limit the response to given names that begin with `Dan`.</span></span>

<span data-ttu-id="5671e-138">结果包括用户名为 Daniel、Danforth、Danielle、Danerys 等的用户。</span><span class="sxs-lookup"><span data-stu-id="5671e-138">Results include users with names like Daniel, Danforth, Danielle, Danerys, and so on.</span></span>

<span data-ttu-id="5671e-139">对 Microsoft Graph 的类似请求是：</span><span class="sxs-lookup"><span data-stu-id="5671e-139">A similar request for Microsoft Graph would be:</span></span>

`GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName,'Dan')`

<span data-ttu-id="5671e-140">此处：</span><span class="sxs-lookup"><span data-stu-id="5671e-140">Here:</span></span>

- <span data-ttu-id="5671e-141">版本为 `v1.0` 。</span><span class="sxs-lookup"><span data-stu-id="5671e-141">The version is `v1.0`.</span></span>
- <span data-ttu-id="5671e-142">租户 ID 从访问令牌推断 (未) 。</span><span class="sxs-lookup"><span data-stu-id="5671e-142">The tenant ID is inferred from the access token (not shown).</span></span>
- <span data-ttu-id="5671e-143">resource 和 `$filter` query 参数与 Azure AD 查询相同。</span><span class="sxs-lookup"><span data-stu-id="5671e-143">The resource and `$filter` query parameter are the same as the Azure AD query.</span></span>

> <span data-ttu-id="5671e-144">**注意**：如果你使用的是 Azure AD Graph .NET 客户端库，请参阅 [.NET](migrate-azure-ad-graph-client-libraries.md) 客户端库，了解更具体的策略和移动到 Microsoft Graph .NET 客户端库的帮助。</span><span class="sxs-lookup"><span data-stu-id="5671e-144">**NOTE**: If you're using the Azure AD Graph .NET client library, see [.NET client libraries](migrate-azure-ad-graph-client-libraries.md) for more specific strategies and assistance to move to the Microsoft Graph .NET client library.</span></span>

### <a name="key-identifiers-objectid-vs-id"></a><span data-ttu-id="5671e-145">密钥标识符：objectId 与 id</span><span class="sxs-lookup"><span data-stu-id="5671e-145">Key identifiers: objectId vs id</span></span>

<span data-ttu-id="5671e-146">在 Azure AD Graph 中，所有实体资源类型都有一个唯一标识符 (或密钥) **objectId**。</span><span class="sxs-lookup"><span data-stu-id="5671e-146">In Azure AD Graph, all entity resource types have a unique identifier (or key) called **objectId**.</span></span>  <span data-ttu-id="5671e-147">大多数情况下， (除非另有) 在 Microsoft Graph 中称为 **id。**</span><span class="sxs-lookup"><span data-stu-id="5671e-147">For the most part (unless otherwise stated) this same identifier is called **id** in Microsoft Graph.</span></span>

## <a name="default-properties-and-select"></a><span data-ttu-id="5671e-148">默认属性和$select</span><span class="sxs-lookup"><span data-stu-id="5671e-148">Default properties and $select</span></span>

<span data-ttu-id="5671e-149">在 `$select` GET 请求中，使用查询参数自定义响应以包含应用需要的所有属性。</span><span class="sxs-lookup"><span data-stu-id="5671e-149">Use the `$select` query parameter, in GET requests, to customize the response to include all the properties that your app requires.</span></span>

<span data-ttu-id="5671e-150">用户 **或** 组 **资源的** Microsoft Graph 获取或列表操作仅返回所有属性的子集，称为 _默认属性_。</span><span class="sxs-lookup"><span data-stu-id="5671e-150">Microsoft Graph **get** or **list** operations for user or group resources returns only a subset of all properties, known as the _default properties_.</span></span> <span data-ttu-id="5671e-151">默认属性表示资源最常用的属性。</span><span class="sxs-lookup"><span data-stu-id="5671e-151">The default properties represent the most commonly-used properties for a resource.</span></span> <span data-ttu-id="5671e-152">另一方面，Azure AD Graph 返回相应资源的所有属性的完整集。</span><span class="sxs-lookup"><span data-stu-id="5671e-152">On the other hand, Azure AD Graph returns the full set of all properties for the respective resource.</span></span>

<span data-ttu-id="5671e-153">若要获取 v1.0 中的其他属性，你的应用需要使用查询参数显式请求 `$select` 它们。</span><span class="sxs-lookup"><span data-stu-id="5671e-153">To get other properties in v1.0, your app needs to explicitly request them, using the `$select` query parameter.</span></span> <span data-ttu-id="5671e-154">这包括你的应用可能使用的任何目录架构扩展。</span><span class="sxs-lookup"><span data-stu-id="5671e-154">This includes any directory schema extensions your app might be using.</span></span> <span data-ttu-id="5671e-155">最佳做法是仅请求应用真正需要的属性。</span><span class="sxs-lookup"><span data-stu-id="5671e-155">It's a best practice to only request the properties your app really needs.</span></span>

<span data-ttu-id="5671e-156">为了说明这一区别，请使用 Graph 浏览器运行以下请求并比较不同的响应。</span><span class="sxs-lookup"><span data-stu-id="5671e-156">To illustrate the difference, use Graph Explorer to run the following requests and compare the different responses.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/
GET https://graph.microsoft.com/beta/me/
```

<span data-ttu-id="5671e-157">查看每个查询的响应。</span><span class="sxs-lookup"><span data-stu-id="5671e-157">Review the responses from each query.</span></span> <span data-ttu-id="5671e-158">你会注意到地址信息由 /beta 版本而不是 /v1.0 版本返回。</span><span class="sxs-lookup"><span data-stu-id="5671e-158">You'll notice that address information is returned by the /beta version, but not the /v1.0 version.</span></span>  <span data-ttu-id="5671e-159">这是因为地址属性不在默认属性集内。</span><span class="sxs-lookup"><span data-stu-id="5671e-159">That's because the address properties aren't in the default property set.</span></span>

<span data-ttu-id="5671e-160">如果你的应用依赖于地址属性，则需要更新 v1.0 请求以包含 `$select` 查询参数：</span><span class="sxs-lookup"><span data-stu-id="5671e-160">If your app relies on the address properties, you need to update your v1.0 requests to include the `$select` query parameter:</span></span>

```http
https://graph.microsoft.com/v1.0/me/?$select=displayName,streetAddress,city,state,postalCode
```

<span data-ttu-id="5671e-161">此请求的响应将包括地址属性。</span><span class="sxs-lookup"><span data-stu-id="5671e-161">The response for this request would include the address properties.</span></span>  <span data-ttu-id="5671e-162">它还包括 **displayName** 属性，但仅仅是因为它由查询参数指定。</span><span class="sxs-lookup"><span data-stu-id="5671e-162">It also includes the **displayName** property, but only because it was specified by the query parameter.</span></span>

<span data-ttu-id="5671e-163">若要了解有关：</span><span class="sxs-lookup"><span data-stu-id="5671e-163">To learn more about:</span></span>

- <span data-ttu-id="5671e-164">用户的默认属性，请参阅 [用户](/graph/api/resources/users?view=graph-rest-1.0)</span><span class="sxs-lookup"><span data-stu-id="5671e-164">Default properties on user, see [users](/graph/api/resources/users?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="5671e-165">参数 `$select` 和其他支持的 ODATA 查询参数，请参阅使用 [查询参数自定义响应](./query-parameters.md)。</span><span class="sxs-lookup"><span data-stu-id="5671e-165">The `$select` parameter and other supported ODATA query parameters, see [Use query parameters to customize responses](./query-parameters.md).</span></span>
- <span data-ttu-id="5671e-166">这和其他建议的优化，请参阅 [最佳做法](./best-practices-concept.md)。</span><span class="sxs-lookup"><span data-stu-id="5671e-166">This and other recommended optimizations, see [Best practices](./best-practices-concept.md).</span></span>

## <a name="relationships-and-navigation-properties"></a><span data-ttu-id="5671e-167">关系和导航属性</span><span class="sxs-lookup"><span data-stu-id="5671e-167">Relationships and navigation properties</span></span>

<span data-ttu-id="5671e-168">关系 (或导航) 是 Azure AD Graph 和 Microsoft Graph 中的关键概念，用于创建相关资源网络。</span><span class="sxs-lookup"><span data-stu-id="5671e-168">Relationships (or navigation properties) are a key concept in Azure AD Graph and Microsoft Graph, creating a network of related resources.</span></span> <span data-ttu-id="5671e-169">例如 **，manager 和** **directReports** 属性扩展用户资源以提供组织层次结构。</span><span class="sxs-lookup"><span data-stu-id="5671e-169">For example, the **manager** and **directReports** properties extend the user resource to provide organizational hierarchy.</span></span>

<span data-ttu-id="5671e-170">关系还定义成员身份，如用户所属的组、属于组或目录角色的成员等。</span><span class="sxs-lookup"><span data-stu-id="5671e-170">Relationships also define memberships, such as the groups a user belongs to, the members belonging to a group or a directory role, and so on.</span></span>

<span data-ttu-id="5671e-171">Azure AD Graph 请求 `$link` 用于指示资源之间的关系。</span><span class="sxs-lookup"><span data-stu-id="5671e-171">Azure AD Graph requests use `$link` to indicate relationships between resources.</span></span>  <span data-ttu-id="5671e-172">在 Microsoft Graph 中，它改为使用 ODATA 4.01 `$ref` 表示法。</span><span class="sxs-lookup"><span data-stu-id="5671e-172">In Microsoft Graph this uses the ODATA 4.01 `$ref` notation instead.</span></span>

<span data-ttu-id="5671e-173">下表显示了几个示例：</span><span class="sxs-lookup"><span data-stu-id="5671e-173">The following table shows several examples:</span></span>

| <span data-ttu-id="5671e-174">任务</span><span class="sxs-lookup"><span data-stu-id="5671e-174">Task</span></span> | <span data-ttu-id="5671e-175">Azure AD Graph</span><span class="sxs-lookup"><span data-stu-id="5671e-175">Azure AD Graph</span></span> | <span data-ttu-id="5671e-176">Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="5671e-176">Microsoft Graph</span></span> |
|------|----------------|-----------------|
| <span data-ttu-id="5671e-177">添加成员</span><span class="sxs-lookup"><span data-stu-id="5671e-177">Add member</span></span>        | ```POST /groups/{id}/$link/members```        | ```POST /groups/{id}/members/$ref```        |
| <span data-ttu-id="5671e-178">列出成员链接</span><span class="sxs-lookup"><span data-stu-id="5671e-178">List member links</span></span> | ```GET /groups/{id}/$link/members```         | ```GET /groups/{id}/members/$ref```         |
| <span data-ttu-id="5671e-179">列出成员</span><span class="sxs-lookup"><span data-stu-id="5671e-179">List members</span></span>      | ```GET /groups/{id}/members```                | ```GET /groups/{id}/members```               |
| <span data-ttu-id="5671e-180">删除成员</span><span class="sxs-lookup"><span data-stu-id="5671e-180">Remove member</span></span>     | ```DELETE /groups/{id}/$link/members/{id}``` | ```DELETE /groups/{id}/members/{id}/$ref``` |

<span data-ttu-id="5671e-181">将应用迁移到 Microsoft Graph 时，查找用于关联资源的请求; `$link` 将其更改为 `$ref` 使用。</span><span class="sxs-lookup"><span data-stu-id="5671e-181">When migrating your apps to Microsoft Graph, look for requests that use `$link` to associate resources; change these to use `$ref` instead.</span></span>

## <a name="next-steps"></a><span data-ttu-id="5671e-182">后续步骤</span><span class="sxs-lookup"><span data-stu-id="5671e-182">Next Steps</span></span>

- <span data-ttu-id="5671e-183">了解 Azure AD Graph [和](migrate-azure-ad-graph-feature-differences.md) Microsoft Graph 之间的服务功能差异。</span><span class="sxs-lookup"><span data-stu-id="5671e-183">Learn about [service feature differences](migrate-azure-ad-graph-feature-differences.md) between Azure AD Graph and Microsoft Graph.</span></span>
- <span data-ttu-id="5671e-184">再次查看 [检查](migrate-azure-ad-graph-planning-checklist.md) 表。</span><span class="sxs-lookup"><span data-stu-id="5671e-184">Review the [checklist](migrate-azure-ad-graph-planning-checklist.md) again.</span></span>