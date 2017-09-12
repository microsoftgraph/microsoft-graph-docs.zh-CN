
# <a name="paging-microsoft-graph-data-in-your-app"></a><span data-ttu-id="d2790-101">在应用中对 Microsoft Graph 数据进行分页</span><span class="sxs-lookup"><span data-stu-id="d2790-101">Paging Microsoft Graph data in your app</span></span> 

<span data-ttu-id="d2790-p101">由于服务器端分页或由于使用 `$top` 查询参数来明确限制请求中的页面大小，致使针对 Microsoft Graph 的一些查询返回多页数据。当结果集跨多个页面时，Microsoft Graph 将在响应中返回 `@odata.nextLink` 属性，该属性包含指向结果下一页的 URL。</span><span class="sxs-lookup"><span data-stu-id="d2790-p101">Some queries against Microsoft Graph return multiple pages of data either due to server-side paging or due to the use of the `$top` query parameter to specifically limit the page size in a request. When a result set spans multiple pages, Microsoft Graph returns an `@odata.nextLink` property in the response that contains a URL to the next page of results.</span></span> 

<span data-ttu-id="d2790-104">例如，以下 URL 请求组织中使用 `$top` 查询参数指定的页面大小为 5 的所有用户：</span><span class="sxs-lookup"><span data-stu-id="d2790-104">For example, the following URL requests all of the users in an organization with a page size of 5 specified with the `$top` query parameter:</span></span>

```html
https://graph.microsoft.com/v1.0/users?$top=5
```

<span data-ttu-id="d2790-105">如果结果包含超过 5 个用户，则 Microsoft Graph 将返回类似于以下以及用户第一页的 `odata:nextLink` 属性。</span><span class="sxs-lookup"><span data-stu-id="d2790-105">If the result contains more than 5 users, Microsoft Graph will return an `odata:nextLink` property similar to the following along with the first page of users.</span></span>

```json
"@odata.nextLink": "https://graph.microsoft.com/v1.0/users?$top=5&$skiptoken=X%274453707 ... 6633B900000000000000000000%27"
```

<span data-ttu-id="d2790-106">可以通过将 `@odata:nextLink` 属性的 URL 值发送到 Microsoft Graph 来检索结果的下一页。</span><span class="sxs-lookup"><span data-stu-id="d2790-106">You can retrieve the next page of results by sending the URL value of the `@odata:nextLink` property to Microsoft Graph.</span></span> 

```html
https://graph.microsoft.com/v1.0/users?$top=5&$skiptoken=X%274453707 ... 6633B900000000000000000000%27
```

<span data-ttu-id="d2790-107">Microsoft Graph 将继续通过每次响应返回对 `@odata:nextLink` 属性中下一页数据的引用，直到读取结果的所有页面。</span><span class="sxs-lookup"><span data-stu-id="d2790-107">Microsoft Graph will continue to return a reference to the next page of data in the `@odata:nextLink` property with each response until all pages of the result have been read.</span></span>

><span data-ttu-id="d2790-p102">**重要说明：**应该在请求的 `@odata:nextLink` 属性中包括整个 URL，以获取下一页结果。根据正在对其执行查询的 API，`@odata:nextLink` URL 值将包含 `$skiptoken` 或 `$skip` 查询参数。该 URL 还包含原始请求中存在的所有其他查询参数。请勿尝试提取 `$skiptoken` 或 `$skip` 值，也不要在不同的请求中使用它。</span><span class="sxs-lookup"><span data-stu-id="d2790-p102">**Important:** You should include the entire URL in the `@odata:nextLink` property in your request for the next page of results. Depending on the API that the query is being performed against, the `@odata:nextLink` URL value will contain either a `$skiptoken` or a `$skip` query parameter. The URL also contains all of the other query parameters present in the original request. Do not try to extract the `$skiptoken` or `$skip` value and use it in a different request.</span></span> 

<span data-ttu-id="d2790-p103">分页行为因 Microsoft Graph API 不同而异。处理分页数据时，应考虑以下几点：</span><span class="sxs-lookup"><span data-stu-id="d2790-p103">Paging behavior varies across different Microsoft Graph APIs. You should consider the following when working with paged data:</span></span>

- <span data-ttu-id="d2790-114">不同的 API 可能具有不同的默认页面大小和最大页面大小。</span><span class="sxs-lookup"><span data-stu-id="d2790-114">Different APIs may have different default and maximum page sizes.</span></span>
- <span data-ttu-id="d2790-p104">如果指定超过相应 API 最大页面大小的页面大小（通过 `$top` 查询参数），则不同 API 的行为会有所不同。具体取决于 API，所请求的页面大小可能会被忽略，它默认选择相应 API 的最大页面大小，否则 Microsoft Graph 会返回错误。</span><span class="sxs-lookup"><span data-stu-id="d2790-p104">Different APIs may behave differently if you specify a page size (via the `$top` query parameter) that exceeds the maximum page size for that API. Depending on the API, the requested page size may be ignored, it may default to the maximum page size for that API, or Microsoft Graph may return an error.</span></span> 
- <span data-ttu-id="d2790-p105">并不是所有的资源和关系都支持分页。例如，针对 [directoryRoles](../api-reference/v1.0/resources/directoryrole.md) 的查询不支持分页。这包括读取角色对象本身以及角色成员。</span><span class="sxs-lookup"><span data-stu-id="d2790-p105">Not all resources or relationships support paging. For example, queries against [directoryRoles](../api-reference/v1.0/resources/directoryrole.md) do not support paging. This includes reading role objects themselves as well as role members.</span></span>
- <span data-ttu-id="d2790-p106">一些 Microsoft Graph API 通过将 `previous-page` 查询参数 (`&previous-page=true`) 追加到 `@odata:nextLink` 属性的 URL 值来支持向后分页。将此参数追加到请求后，后续响应中的 `@odata:nextLink` URL 值会将其包括在内。可以继续向后分页，直到返回具有空结果的响应。继续分页将返回错误。或者，可以在发送下一页结果的请求时，通过删除 `previous-page` 参数从当前响应中继续向前分页。</span><span class="sxs-lookup"><span data-stu-id="d2790-p106">Some Microsoft Graph APIs support backward paging by appending the `previous-page` query parameter (`&previous-page=true`) to the URL value of the `@odata:nextLink` property. Once you append this parameter to a request, the `@odata:nextLink` URL value in subsequent responses will include it. You can continue to page backward until a response with an empty result is returned. Paging further will return an error. Alternatively, you can resume paging forward from the current response by removing the `previous-page` parameter when you send the request for the next page of results.</span></span> 

