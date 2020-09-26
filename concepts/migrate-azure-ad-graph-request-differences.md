---
title: 请求 Azure AD Graph 和 Microsoft Graph 之间的差异
description: 介绍 Microsoft Graph 请求与 Azure AD 请求的不同之处，这有助于将应用迁移到较新的服务。。
author: dkershaw10
localization_priority: Normal
ms.prod: azure-active-directory
ms.openlocfilehash: ae393192961c61890e7dc3963a82727b6aea0557
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2020
ms.locfileid: "48289104"
---
# <a name="request-differences-between-azure-ad-graph-and-microsoft-graph"></a><span data-ttu-id="7af57-103">请求 Azure AD Graph 和 Microsoft Graph 之间的差异</span><span class="sxs-lookup"><span data-stu-id="7af57-103">Request differences between Azure AD Graph and Microsoft Graph</span></span>

<span data-ttu-id="7af57-104">本文是*第1步：查看*[迁移应用程序](migrate-azure-ad-graph-planning-checklist.md)的 API 差异的过程的一部分。</span><span class="sxs-lookup"><span data-stu-id="7af57-104">This article is part of *step 1: review API differences* of the [process to migrate apps](migrate-azure-ad-graph-planning-checklist.md).</span></span>

<span data-ttu-id="7af57-105">Microsoft Graph 和 Azure AD Graph API 都是 REST Api，它们分别支持查询参数的 ODATA 约定。</span><span class="sxs-lookup"><span data-stu-id="7af57-105">Microsoft Graph and the Azure AD Graph API are both REST APIs and they each support ODATA conventions for query parameters.</span></span> <span data-ttu-id="7af57-106">但是，这两个 Api 的语法各不相同。</span><span class="sxs-lookup"><span data-stu-id="7af57-106">However, the syntax varies between these two APIs.</span></span>

<span data-ttu-id="7af57-107">使用 [Graph 浏览器](https://aka.ms/ge) 针对您自己的数据尝试这些请求模式，因为这是了解请求和响应差异的一种很好的方法。</span><span class="sxs-lookup"><span data-stu-id="7af57-107">Use the [Graph Explorer](https://aka.ms/ge) to try these request patterns against your own data, as it's a great way to learn about the request and response differences.</span></span>

## <a name="basic-requests"></a><span data-ttu-id="7af57-108">基本请求</span><span class="sxs-lookup"><span data-stu-id="7af57-108">Basic requests</span></span>

<span data-ttu-id="7af57-109">下表突出显示了这两个 Api 之间的主要请求差异：</span><span class="sxs-lookup"><span data-stu-id="7af57-109">The following table highlights the main request differences between the two APIs:</span></span>

|<span data-ttu-id="7af57-110">请求详细信息</span><span class="sxs-lookup"><span data-stu-id="7af57-110">Request details</span></span>| <span data-ttu-id="7af57-111">Azure AD Graph</span><span class="sxs-lookup"><span data-stu-id="7af57-111">Azure AD Graph</span></span> | <span data-ttu-id="7af57-112">Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="7af57-112">Microsoft Graph</span></span> |
|---|---|---|
|<span data-ttu-id="7af57-113">请求语法</span><span class="sxs-lookup"><span data-stu-id="7af57-113">Request syntax</span></span>| `https://graph.windows.net/{tenant_id}/` <br> `{resource}?{version}&query-parameters` | `https://graph.microsoft.com/`<br>`{version}/{resource}?query-parameters`|
|<span data-ttu-id="7af57-114">服务 &nbsp; 终结点：</span><span class="sxs-lookup"><span data-stu-id="7af57-114">Service&nbsp;endpoints:</span></span>||
|<span data-ttu-id="7af57-115">-&nbsp;全局性</span><span class="sxs-lookup"><span data-stu-id="7af57-115">-&nbsp;Global</span></span>|`https://graph.windows.net`|`https://graph.microsoft.com`|
|<span data-ttu-id="7af57-116">-&nbsp;US &nbsp; .Gov &nbsp; L4</span><span class="sxs-lookup"><span data-stu-id="7af57-116">-&nbsp;US&nbsp;Gov&nbsp;L4</span></span>|`https://graph.microsoftazure.us`|`https://graph.microsoft.us`|
|<span data-ttu-id="7af57-117">-&nbsp;美国 &nbsp; .Gov &nbsp; L5 &nbsp; (DOD) </span><span class="sxs-lookup"><span data-stu-id="7af57-117">-&nbsp;US&nbsp;Gov&nbsp;L5&nbsp;(DOD)</span></span>|`https://graph.microsoftazure.us`|`https://dod-graph.microsoft.us`|
|<span data-ttu-id="7af57-118">-&nbsp;德国</span><span class="sxs-lookup"><span data-stu-id="7af57-118">-&nbsp;Germany</span></span>|`https://graph.cloudapi.de`|`https://graph.microsoft.de`|
|<span data-ttu-id="7af57-119">-&nbsp;中国 &nbsp; (世纪) </span><span class="sxs-lookup"><span data-stu-id="7af57-119">-&nbsp;China&nbsp;(21Vianet)</span></span>| `https://graph.chinacloudapi.cn`|`https://microsoftgraph.chinacloudapi.cn`|
|<span data-ttu-id="7af57-120">{tenant_id}</span><span class="sxs-lookup"><span data-stu-id="7af57-120">{tenant_id}</span></span>|<span data-ttu-id="7af57-121">指定请求中租户的 ID。</span><span class="sxs-lookup"><span data-stu-id="7af57-121">Specify the ID of the tenant in the request.</span></span>|<span data-ttu-id="7af57-122">在请求中指定的租户 ID 是可从访问令牌推断出的可选方法。</span><span class="sxs-lookup"><span data-stu-id="7af57-122">It's optional to specify a tenant ID in the request as it is inferred from the access token.</span></span><br><br><span data-ttu-id="7af57-123">如果您指定租户 ID，它将在 `{version}` `{resource}` 请求 URL 中的和之间。</span><span class="sxs-lookup"><span data-stu-id="7af57-123">If you specify the tenant ID, it goes between the `{version}` and the `{resource}` in the request URL.</span></span>|
|<span data-ttu-id="7af57-124">版本</span><span class="sxs-lookup"><span data-stu-id="7af57-124">{version}</span></span>|<span data-ttu-id="7af57-125">使用所需的查询参数在请求中指定 Azure AD Graph 的发布版本。</span><span class="sxs-lookup"><span data-stu-id="7af57-125">Specify the release version of Azure AD Graph in the request using a required query parameter.</span></span>|<span data-ttu-id="7af57-126">在请求中将 Microsoft Graph 的发布版本指定为服务终结点之后的 URL 路径的一部分。</span><span class="sxs-lookup"><span data-stu-id="7af57-126">Specify the release version of Microsoft Graph in the request as part of the URL path just after the service endpoint.</span></span>|

<span data-ttu-id="7af57-127">您可以继续在 Microsoft Graph 中使用与 Azure AD Graph 相同的查询参数。</span><span class="sxs-lookup"><span data-stu-id="7af57-127">You can continue to use the same query parameters in Microsoft Graph as Azure AD Graph.</span></span>

### <a name="example-request-comparison"></a><span data-ttu-id="7af57-128">示例请求比较</span><span class="sxs-lookup"><span data-stu-id="7af57-128">Example request comparison</span></span>

<span data-ttu-id="7af57-129">假设您需要一个名称以 "Dan" 开头的所有用户的列表。</span><span class="sxs-lookup"><span data-stu-id="7af57-129">Suppose you want a list of all users with names beginning with "Dan".</span></span>

<span data-ttu-id="7af57-130">在 Azure AD Graph 中，可以使用此请求：</span><span class="sxs-lookup"><span data-stu-id="7af57-130">In Azure AD Graph, you might use this request:</span></span>

<span data-ttu-id="7af57-131">`GET https://graph.windows.net/contoso.com/users?$filter=startswith(givenName,'Dan')&api-version=1.6` 和</span><span class="sxs-lookup"><span data-stu-id="7af57-131">`GET https://graph.windows.net/contoso.com/users?$filter=startswith(givenName,'Dan')&api-version=1.6` or</span></span>

`GET https://graph.windows.net/myOrganization/users?$filter=startswith(givenName,'Dan')&api-version=1.6`


<span data-ttu-id="7af57-132">此请求：</span><span class="sxs-lookup"><span data-stu-id="7af57-132">This request:</span></span>

- <span data-ttu-id="7af57-133">面向 Azure AD Graph 的版本1.6。</span><span class="sxs-lookup"><span data-stu-id="7af57-133">Targets version 1.6 of Azure AD Graph.</span></span>
- <span data-ttu-id="7af57-134">指定 `contoso.com` 为租户 ID。</span><span class="sxs-lookup"><span data-stu-id="7af57-134">Specifies `contoso.com` as the tenant ID.</span></span> <span data-ttu-id="7af57-135">替代方法显示了如何 `myOrganization` 根据访问令牌中的租户 ID 使用别名。</span><span class="sxs-lookup"><span data-stu-id="7af57-135">The alternative shows the use of an alias `myOrganization` based on the tenant ID in the access token.</span></span>
- <span data-ttu-id="7af57-136">调用用户资源。</span><span class="sxs-lookup"><span data-stu-id="7af57-136">Calls the users resource.</span></span>
- <span data-ttu-id="7af57-137">使用 `$filter` 查询参数将响应限制为以开头的给定名称 `Dan` 。</span><span class="sxs-lookup"><span data-stu-id="7af57-137">Uses the `$filter` query parameter to limit the response to given names that begin with `Dan`.</span></span>

<span data-ttu-id="7af57-138">结果包括名称如 Daniel、Danforth、Danielle、Danerys 等的用户。</span><span class="sxs-lookup"><span data-stu-id="7af57-138">Results include users with names like Daniel, Danforth, Danielle, Danerys, and so on.</span></span>

<span data-ttu-id="7af57-139">Microsoft Graph 的类似请求如下：</span><span class="sxs-lookup"><span data-stu-id="7af57-139">A similar request for Microsoft Graph would be:</span></span>

`GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName,'Dan')`

<span data-ttu-id="7af57-140">如下</span><span class="sxs-lookup"><span data-stu-id="7af57-140">Here:</span></span>

- <span data-ttu-id="7af57-141">版本为 `v1.0` 。</span><span class="sxs-lookup"><span data-stu-id="7af57-141">The version is `v1.0`.</span></span>
- <span data-ttu-id="7af57-142">租户 ID 是从访问令牌中推断出来 (不会) 显示。</span><span class="sxs-lookup"><span data-stu-id="7af57-142">The tenant ID is inferred from the access token (not shown).</span></span>
- <span data-ttu-id="7af57-143">资源和 `$filter` 查询参数与 AZURE AD 查询相同。</span><span class="sxs-lookup"><span data-stu-id="7af57-143">The resource and `$filter` query parameter are the same as the Azure AD query.</span></span>

> <span data-ttu-id="7af57-144">**注意**：如果使用的是 Azure AD Graph .net 客户端库，请参阅 [.net 客户端库](migrate-azure-ad-graph-client-libraries.md) ，了解更多特定策略和帮助，以移动到 Microsoft Graph .net 客户端库。</span><span class="sxs-lookup"><span data-stu-id="7af57-144">**NOTE**: If you're using the Azure AD Graph .NET client library, see [.NET client libraries](migrate-azure-ad-graph-client-libraries.md) for more specific strategies and assistance to move to the Microsoft Graph .NET client library.</span></span>

### <a name="key-identifiers-objectid-vs-id"></a><span data-ttu-id="7af57-145">键标识符： objectId vs id</span><span class="sxs-lookup"><span data-stu-id="7af57-145">Key identifiers: objectId vs id</span></span>

<span data-ttu-id="7af57-146">在 Azure AD Graph 中，所有实体资源类型都有一个唯一的标识符 (或称为 **objectId**的键) 。</span><span class="sxs-lookup"><span data-stu-id="7af57-146">In Azure AD Graph, all entity resource types have a unique identifier (or key) called **objectId**.</span></span>  <span data-ttu-id="7af57-147">大多数情况 (（除非另有说明）) 此同一标识符在 Microsoft Graph 中称为 **id** 。</span><span class="sxs-lookup"><span data-stu-id="7af57-147">For the most part (unless otherwise stated) this same identifier is called **id** in Microsoft Graph.</span></span>

## <a name="default-properties-and-select"></a><span data-ttu-id="7af57-148">默认属性和 $select</span><span class="sxs-lookup"><span data-stu-id="7af57-148">Default properties and $select</span></span>

<span data-ttu-id="7af57-149">使用 `$select` GET requests 中的查询参数自定义响应，以包含您的应用程序所需的所有属性。</span><span class="sxs-lookup"><span data-stu-id="7af57-149">Use the `$select` query parameter, in GET requests, to customize the response to include all the properties that your app requires.</span></span>

<span data-ttu-id="7af57-150">Microsoft Graph **get** 或 **list** 操作对于用户或组资源，仅返回所有属性（称为 _默认属性_）的子集。</span><span class="sxs-lookup"><span data-stu-id="7af57-150">Microsoft Graph **get** or **list** operations for user or group resources returns only a subset of all properties, known as the _default properties_.</span></span> <span data-ttu-id="7af57-151">默认属性表示资源的最常用属性。</span><span class="sxs-lookup"><span data-stu-id="7af57-151">The default properties represent the most commonly-used properties for a resource.</span></span> <span data-ttu-id="7af57-152">另一方面，Azure AD Graph 将返回相应资源的所有属性的完整集。</span><span class="sxs-lookup"><span data-stu-id="7af57-152">On the other hand, Azure AD Graph returns the full set of all properties for the respective resource.</span></span>

<span data-ttu-id="7af57-153">若要获取 v1.0 中的其他属性，应用需要使用查询参数显式请求这些属性 `$select` 。</span><span class="sxs-lookup"><span data-stu-id="7af57-153">To get other properties in v1.0, your app needs to explicitly request them, using the `$select` query parameter.</span></span> <span data-ttu-id="7af57-154">这包括您的应用程序可能使用的任何目录架构扩展。</span><span class="sxs-lookup"><span data-stu-id="7af57-154">This includes any directory schema extensions your app might be using.</span></span> <span data-ttu-id="7af57-155">最佳做法是仅请求应用程序真正需要的属性。</span><span class="sxs-lookup"><span data-stu-id="7af57-155">It's a best practice to only request the properties your app really needs.</span></span>

<span data-ttu-id="7af57-156">为了说明区别，请使用 Graph 浏览器运行以下请求并比较不同的响应。</span><span class="sxs-lookup"><span data-stu-id="7af57-156">To illustrate the difference, use Graph Explorer to run the following requests and compare the different responses.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/
GET https://graph.microsoft.com/beta/me/
```

<span data-ttu-id="7af57-157">查看每个查询的响应。</span><span class="sxs-lookup"><span data-stu-id="7af57-157">Review the responses from each query.</span></span> <span data-ttu-id="7af57-158">您会注意到，地址信息是由/beta 版本（而不是/v1.0 版本）返回的。</span><span class="sxs-lookup"><span data-stu-id="7af57-158">You'll notice that address information is returned by the /beta version, but not the /v1.0 version.</span></span>  <span data-ttu-id="7af57-159">这是因为地址属性不在默认属性集中。</span><span class="sxs-lookup"><span data-stu-id="7af57-159">That's because the address properties aren't in the default property set.</span></span>

<span data-ttu-id="7af57-160">如果您的应用程序依赖于地址属性，则需要更新您的 v1.0 请求以包含 `$select` 查询参数：</span><span class="sxs-lookup"><span data-stu-id="7af57-160">If your app relies on the address properties, you need to update your v1.0 requests to include the `$select` query parameter:</span></span>

```http
https://graph.microsoft.com/v1.0/me/?$select=displayName,streetAddress,city,state,postalCode
```

<span data-ttu-id="7af57-161">此请求的响应将包括地址属性。</span><span class="sxs-lookup"><span data-stu-id="7af57-161">The response for this request would include the address properties.</span></span>  <span data-ttu-id="7af57-162">它还包括 **displayName** 属性，但仅由于它是由查询参数指定的。</span><span class="sxs-lookup"><span data-stu-id="7af57-162">It also includes the **displayName** property, but only because it was specified by the query parameter.</span></span>

<span data-ttu-id="7af57-163">若要了解详细信息，请参阅：</span><span class="sxs-lookup"><span data-stu-id="7af57-163">To learn more about:</span></span>

- <span data-ttu-id="7af57-164">用户的默认属性，请参阅 [users](/graph/api/resources/users?view=graph-rest-1.0)</span><span class="sxs-lookup"><span data-stu-id="7af57-164">Default properties on user, see [users](/graph/api/resources/users?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="7af57-165">`$select`参数和其他受支持的 ODATA 查询参数，请参阅[使用查询参数自定义响应](./query-parameters.md)。</span><span class="sxs-lookup"><span data-stu-id="7af57-165">The `$select` parameter and other supported ODATA query parameters, see [Use query parameters to customize responses](./query-parameters.md).</span></span>
- <span data-ttu-id="7af57-166">此操作和其他建议的优化，请参阅 [最佳实践](./best-practices-concept.md)。</span><span class="sxs-lookup"><span data-stu-id="7af57-166">This and other recommended optimizations, see [Best practices](./best-practices-concept.md).</span></span>

## <a name="relationships-and-navigation-properties"></a><span data-ttu-id="7af57-167">关系和导航属性</span><span class="sxs-lookup"><span data-stu-id="7af57-167">Relationships and navigation properties</span></span>

<span data-ttu-id="7af57-168">关系 (或导航属性) 是 Azure AD Graph 和 Microsoft Graph 中的关键概念，创建了相关资源的网络。</span><span class="sxs-lookup"><span data-stu-id="7af57-168">Relationships (or navigation properties) are a key concept in Azure AD Graph and Microsoft Graph, creating a network of related resources.</span></span> <span data-ttu-id="7af57-169">例如， **manager** 和 **directReports** 属性扩展了用户资源，以提供组织的层次结构。</span><span class="sxs-lookup"><span data-stu-id="7af57-169">For example, the **manager** and **directReports** properties extend the user resource to provide organizational hierarchy.</span></span>

<span data-ttu-id="7af57-170">关系还定义成员身份，如用户所属的组、属于某个组的成员或目录角色，等等。</span><span class="sxs-lookup"><span data-stu-id="7af57-170">Relationships also define memberships, such as the groups a user belongs to, the members belonging to a group or a directory role, and so on.</span></span>

<span data-ttu-id="7af57-171">Azure AD Graph 请求用于 `$link` 指示资源之间的关系。</span><span class="sxs-lookup"><span data-stu-id="7af57-171">Azure AD Graph requests use `$link` to indicate relationships between resources.</span></span>  <span data-ttu-id="7af57-172">在 Microsoft Graph 中，使用的是 ODATA 4.01 `$ref` 表示法。</span><span class="sxs-lookup"><span data-stu-id="7af57-172">In Microsoft Graph this uses the ODATA 4.01 `$ref` notation instead.</span></span>

<span data-ttu-id="7af57-173">下表显示了几个示例：</span><span class="sxs-lookup"><span data-stu-id="7af57-173">The following table shows several examples:</span></span>

| <span data-ttu-id="7af57-174">任务</span><span class="sxs-lookup"><span data-stu-id="7af57-174">Task</span></span> | <span data-ttu-id="7af57-175">Azure AD Graph</span><span class="sxs-lookup"><span data-stu-id="7af57-175">Azure AD Graph</span></span> | <span data-ttu-id="7af57-176">Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="7af57-176">Microsoft Graph</span></span> |
|------|----------------|-----------------|
| <span data-ttu-id="7af57-177">添加成员</span><span class="sxs-lookup"><span data-stu-id="7af57-177">Add member</span></span>        | ```POST /groups/{id}/$link/members```        | ```POST /groups/{id}/members/$ref```        |
| <span data-ttu-id="7af57-178">列出成员链接</span><span class="sxs-lookup"><span data-stu-id="7af57-178">List member links</span></span> | ```GET /groups/{id}/$link/members```         | ```GET /groups/{id}/members/$ref```         |
| <span data-ttu-id="7af57-179">列出成员</span><span class="sxs-lookup"><span data-stu-id="7af57-179">List members</span></span>      | ```GET /groups/{id}/members```                | ```GET /groups/{id}/members```               |
| <span data-ttu-id="7af57-180">删除成员</span><span class="sxs-lookup"><span data-stu-id="7af57-180">Remove member</span></span>     | ```DELETE /groups/{id}/$link/members/{id}``` | ```DELETE /groups/{id}/members/{id}/$ref``` |

<span data-ttu-id="7af57-181">将应用程序迁移到 Microsoft Graph 时，请查找使用 `$link` 关联资源的请求; 请将这些请求更改为改用 `$ref` 。</span><span class="sxs-lookup"><span data-stu-id="7af57-181">When migrating your apps to Microsoft Graph, look for requests that use `$link` to associate resources; change these to use `$ref` instead.</span></span>

## <a name="next-steps"></a><span data-ttu-id="7af57-182">后续步骤</span><span class="sxs-lookup"><span data-stu-id="7af57-182">Next Steps</span></span>

- <span data-ttu-id="7af57-183">了解 Azure AD Graph 与 Microsoft Graph 之间的 [服务功能差异](migrate-azure-ad-graph-feature-differences.md) 。</span><span class="sxs-lookup"><span data-stu-id="7af57-183">Learn about [service feature differences](migrate-azure-ad-graph-feature-differences.md) between Azure AD Graph and Microsoft Graph.</span></span>
- <span data-ttu-id="7af57-184">再次查看 [检查表](migrate-azure-ad-graph-planning-checklist.md) 。</span><span class="sxs-lookup"><span data-stu-id="7af57-184">Review the [checklist](migrate-azure-ad-graph-planning-checklist.md) again.</span></span>