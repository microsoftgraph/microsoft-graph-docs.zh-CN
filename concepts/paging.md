---
title: '在应用中对 Microsoft Graph 数据进行分页 '
description: '响应中的 odata.nextLink` 属性，其中包含下一页结果的 URL。 '
author: davidmu1
localization_priority: Priority
ms.custom: graphiamtop20, scenarios:getting-started
ms.openlocfilehash: be2d927de3cf1f3d419d7daa5747e0cc9e70c28c
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030878"
---
# <a name="paging-microsoft-graph-data-in-your-app"></a><span data-ttu-id="6e989-103">在应用中对 Microsoft Graph 数据进行分页</span><span class="sxs-lookup"><span data-stu-id="6e989-103">Paging Microsoft Graph data in your app</span></span> 

<span data-ttu-id="6e989-p101">由于服务器端分页或由于使用 `$top` 查询参数来明确限制请求中的页面大小，致使针对 Microsoft Graph 的一些查询返回多页数据。当结果集跨多个页面时，Microsoft Graph 将在响应中返回 `@odata.nextLink` 属性，该属性包含指向结果下一页的 URL。</span><span class="sxs-lookup"><span data-stu-id="6e989-p101">Some queries against Microsoft Graph return multiple pages of data either due to server-side paging or due to the use of the `$top` query parameter to specifically limit the page size in a request. When a result set spans multiple pages, Microsoft Graph returns an `@odata.nextLink` property in the response that contains a URL to the next page of results.</span></span> 

<span data-ttu-id="6e989-106">例如，以下 URL 要求对组织中的所有用户使用页面大小 5（使用 `$top` 查询参数指定）：</span><span class="sxs-lookup"><span data-stu-id="6e989-106">For example, the following URL requests all the users in an organization with a page size of 5, specified with the `$top` query parameter:</span></span>

```html
https://graph.microsoft.com/v1.0/users?$top=5
```

<span data-ttu-id="6e989-107">如果结果包含超过 5 个用户，则 Microsoft Graph 将返回一个下列类似的 `@odata.nextLink` 属性以及第一页的用户。</span><span class="sxs-lookup"><span data-stu-id="6e989-107">If the result contains more than five users, Microsoft Graph will return an `@odata.nextLink` property similar to the following along with the first page of users.</span></span>

```json
"@odata.nextLink": "https://graph.microsoft.com/v1.0/users?$top=5&$skiptoken=X%274453707 ... 6633B900000000000000000000%27"
```

<span data-ttu-id="6e989-108">可以通过将 `@odata.nextLink` 属性的 URL 值发送到 Microsoft Graph 来检索结果的下一页。</span><span class="sxs-lookup"><span data-stu-id="6e989-108">You can retrieve the next page of results by sending the URL value of the `@odata.nextLink` property to Microsoft Graph.</span></span> 

```html
https://graph.microsoft.com/v1.0/users?$top=5&$skiptoken=X%274453707 ... 6633B900000000000000000000%27
```

<span data-ttu-id="6e989-109">Microsoft Graph 将继续通过每次响应返回对 `@odata.nextLink` 属性中下一页数据的引用，直到读取结果的所有页面。</span><span class="sxs-lookup"><span data-stu-id="6e989-109">Microsoft Graph will continue to return a reference to the next page of data in the `@odata.nextLink` property with each response until all pages of the result have been read.</span></span>

><span data-ttu-id="6e989-110">**重要说明：** 应该在请求的 `@odata.nextLink` 属性中包括整个 URL，以获取下一页结果。</span><span class="sxs-lookup"><span data-stu-id="6e989-110">**Important:** You should include the entire URL in the `@odata.nextLink` property in your request for the next page of results.</span></span> <span data-ttu-id="6e989-111">根据正在对其执行查询的 API， `@odata.nextLink` URL 值将包含 `$skiptoken` 或 `$skip` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="6e989-111">Depending on the API that the query is being performed against, the `@odata.nextLink` URL value will contain either a `$skiptoken` or a `$skip` query parameter.</span></span> <span data-ttu-id="6e989-112">该 URL 还包含原始请求中存在的所有其他查询参数。</span><span class="sxs-lookup"><span data-stu-id="6e989-112">The URL also contains all the other query parameters present in the original request.</span></span> <span data-ttu-id="6e989-113">请勿尝试提取 `$skiptoken` 或 `$skip` 值，也不要在不同的请求中使用它。</span><span class="sxs-lookup"><span data-stu-id="6e989-113">Do not try to extract the `$skiptoken` or `$skip` value and use it in a different request.</span></span> 

<span data-ttu-id="6e989-114">分页行为因 Microsoft Graph API 不同而异。</span><span class="sxs-lookup"><span data-stu-id="6e989-114">Paging behavior varies across different Microsoft Graph APIs.</span></span> <span data-ttu-id="6e989-115">处理分页数据时，应考虑以下几点：</span><span class="sxs-lookup"><span data-stu-id="6e989-115">Consider the following when working with paged data:</span></span>

- <span data-ttu-id="6e989-116">不同的 API 可能具有不同的默认页面大小和最大页面大小。</span><span class="sxs-lookup"><span data-stu-id="6e989-116">Different APIs might have different default and maximum page sizes.</span></span>
- <span data-ttu-id="6e989-117">如果指定超过相应 API 最大页面大小的页面大小（通过 `$top` 查询参数），则不同 API 的行为会有所不同。</span><span class="sxs-lookup"><span data-stu-id="6e989-117">Different APIs might behave differently if you specify a page size (via the `$top` query parameter) that exceeds the maximum page size for that API.</span></span> <span data-ttu-id="6e989-118">具体取决于 API，所请求的页面大小可能会被忽略，它默认选择相应 API 的最大页面大小，否则 Microsoft Graph 会返回错误。</span><span class="sxs-lookup"><span data-stu-id="6e989-118">Depending on the API, the requested page size might be ignored, it might default to the maximum page size for that API, or Microsoft Graph might return an error.</span></span> 
- <span data-ttu-id="6e989-p105">并不是所有的资源和关系都支持分页。例如，针对 [directoryRoles](/graph/api/resources/directoryrole) 的查询不支持分页。这包括读取角色对象本身以及角色成员。</span><span class="sxs-lookup"><span data-stu-id="6e989-p105">Not all resources or relationships support paging. For example, queries against [directoryRoles](/graph/api/resources/directoryrole) do not support paging. This includes reading role objects themselves as well as role members.</span></span>
- <span data-ttu-id="6e989-122">对目录资源进行分页时，默认情况下，后续页面请求中不包含任何其他请求标头(如 **ConsistencyLevel** 标头)。</span><span class="sxs-lookup"><span data-stu-id="6e989-122">When paging against directory resources, any additional request headers such as the **ConsistencyLevel** header are not included by default in subsequent page requests.</span></span> <span data-ttu-id="6e989-123">如果需要在后续请求中发送这些标头，则必须显式设置它们。</span><span class="sxs-lookup"><span data-stu-id="6e989-123">If those headers need to be sent on subsequent requests, you must set them explicitly.</span></span>
- <span data-ttu-id="6e989-124">在针对目录资源进行查询时使用 `$count=true` 查询字符串时， `@odata.count` 属性将仅出现在分页数据的第一页中。</span><span class="sxs-lookup"><span data-stu-id="6e989-124">When using the `$count=true` query string when querying against directory resources, the `@odata.count` property will be present only in the first page of the paged data.</span></span>

## <a name="learn-more-about-paging"></a><span data-ttu-id="6e989-125">详细了解分页</span><span class="sxs-lookup"><span data-stu-id="6e989-125">Learn more about paging</span></span>
<span data-ttu-id="6e989-126">以下视频介绍了 Microsoft Graph 中的分页。</span><span class="sxs-lookup"><span data-stu-id="6e989-126">The following video introduces you to paging in Microsoft Graph.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/DB_NoC9a1JI]
