# <a name="group-delta"></a><span data-ttu-id="0ff3e-101">group: delta</span><span class="sxs-lookup"><span data-stu-id="0ff3e-101">group: delta</span></span>
<span data-ttu-id="0ff3e-p101">[分区查询](../../../concepts/delta_query_overview.md)使应用程序能够发现新创建、更新或删除的实体，无需使用每个请求对目标资源执行完全读取。若要发现组更改，请使用 *delta* 函数执行请求。请参阅[使用增量查询](../../../concepts/delta_query_overview.md)了解详细信息。</span><span class="sxs-lookup"><span data-stu-id="0ff3e-p101">[Delta query](../../../concepts/delta_query_overview.md) enables applications to discover newly created, updated, or deleted entities without performing a full read of the target resource with every request. To discover changes to groups, perform a request using the *delta* function. See [Using Delta Query](../../../concepts/delta_query_overview.md) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ff3e-105">权限</span><span class="sxs-lookup"><span data-stu-id="0ff3e-105">Permissions</span></span>
<span data-ttu-id="0ff3e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="0ff3e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0ff3e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="0ff3e-108">Permission type</span></span>      | <span data-ttu-id="0ff3e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0ff3e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ff3e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0ff3e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0ff3e-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ff3e-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0ff3e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0ff3e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ff3e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="0ff3e-113">Not supported.</span></span>    |
|<span data-ttu-id="0ff3e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="0ff3e-114">Application</span></span> | <span data-ttu-id="0ff3e-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ff3e-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ff3e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0ff3e-116">HTTP request</span></span>
<span data-ttu-id="0ff3e-117">为开始跟踪更改，请在组资源上发出包含 delta 函数的请求。</span><span class="sxs-lookup"><span data-stu-id="0ff3e-117">To begin tracking changes, you make a request including the delta function on the groups resource.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /groups/delta
```

### <a name="query-parameters"></a><span data-ttu-id="0ff3e-118">查询参数</span><span class="sxs-lookup"><span data-stu-id="0ff3e-118">Query parameters</span></span>
<span data-ttu-id="0ff3e-p103">跟踪组中的更改会触发一个或多个 **delta** 函数调用。如果使用任何查询参数（而不是 `$deltatoken` 和 `$skiptoken`），必须在初始 **delta** 请求中指定它。Microsoft Graph 会自动将任何指定参数编码为响应中返回的 `nextLink` 或 `deltaLink` URL 的令牌部分。</span><span class="sxs-lookup"><span data-stu-id="0ff3e-p103">Tracking changes in groups incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="0ff3e-122">只需预先指定所需的任何查询参数一次。</span><span class="sxs-lookup"><span data-stu-id="0ff3e-122">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="0ff3e-123">在后续请求中，可以复制并应用之前响应中返回的 `nextLink` 或 `deltaLink` URL，因为此 URL 已包含所需的编码参数。</span><span class="sxs-lookup"><span data-stu-id="0ff3e-123">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="0ff3e-124">查询参数</span><span class="sxs-lookup"><span data-stu-id="0ff3e-124">Query parameter</span></span>      | <span data-ttu-id="0ff3e-125">类型</span><span class="sxs-lookup"><span data-stu-id="0ff3e-125">Type</span></span>   |<span data-ttu-id="0ff3e-126">说明</span><span class="sxs-lookup"><span data-stu-id="0ff3e-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0ff3e-127">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="0ff3e-127">$deltatoken</span></span> | <span data-ttu-id="0ff3e-128">string</span><span class="sxs-lookup"><span data-stu-id="0ff3e-128">string</span></span> | <span data-ttu-id="0ff3e-p104">对同一个组集合之前的 **delta** 函数调用的 `deltaLink` URL 中返回的[状态令牌](../../../concepts/delta_query_overview.md)，指示该组更改跟踪的完成状态。将此令牌包含在对该集合的下一组更改追踪的首次请求中，并保存和应用整个 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="0ff3e-p104">A [state token](../../../concepts/delta_query_overview.md) returned in the `deltaLink` URL of the previous **delta** function call for the same group collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="0ff3e-131">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="0ff3e-131">$skiptoken</span></span> | <span data-ttu-id="0ff3e-132">string</span><span class="sxs-lookup"><span data-stu-id="0ff3e-132">string</span></span> | <span data-ttu-id="0ff3e-133">对之前的 **delta** 函数调用的 `nextLink` URL 中返回的[状态令牌](../../../concepts/delta_query_overview.md)，指示同一个组集合中有进一步的更改需要追踪。</span><span class="sxs-lookup"><span data-stu-id="0ff3e-133">A [state token](../../../concepts/delta_query_overview.md) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same group collection.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="0ff3e-134">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0ff3e-134">Optional query parameters</span></span>
<span data-ttu-id="0ff3e-135">此方法支持 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0ff3e-135">This method supports OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="0ff3e-p105">像在任何 GET 请求中一样，你可以使用 `$select` 查询参数以仅指定获取最佳性能所需的属性。始终返回 _id_ 属性。</span><span class="sxs-lookup"><span data-stu-id="0ff3e-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 
- <span data-ttu-id="0ff3e-138">对于组，Delta 查询支持 `$select`、`$top` 和 `$expand`。</span><span class="sxs-lookup"><span data-stu-id="0ff3e-138">Delta query support `$select`, `$top`, and `$expand` for groups.</span></span> 
- <span data-ttu-id="0ff3e-139">提供对 `$filter` 和 `$orderby` 的有限支持：</span><span class="sxs-lookup"><span data-stu-id="0ff3e-139">There is limited support for `$filter` and `$orderby`:</span></span>
  * <span data-ttu-id="0ff3e-140">唯一支持的 `$filter` 表达式用于跟踪对特定对象 `$filter=id+eq+{value}` 的更改。</span><span class="sxs-lookup"><span data-stu-id="0ff3e-140">The only supported `$filter` expression is for tracking changes on a specific object: `$filter=id+eq+{value}`.</span></span> <span data-ttu-id="0ff3e-141">可以筛选多个对象。</span><span class="sxs-lookup"><span data-stu-id="0ff3e-141">You can filter multiple objects.</span></span> <span data-ttu-id="0ff3e-142">例如，`https://graph.microsoft.com/v1.0/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff`。</span><span class="sxs-lookup"><span data-stu-id="0ff3e-142">For example: `https://graph.microsoft.com/v1.0/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff`.</span></span> <span data-ttu-id="0ff3e-143">筛选对象不能超出 50 个。</span><span class="sxs-lookup"><span data-stu-id="0ff3e-143">There is a limit of 50 filtered objects.</span></span>
- <span data-ttu-id="0ff3e-144">不支持 `$search`。</span><span class="sxs-lookup"><span data-stu-id="0ff3e-144">There is no support for `$search`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0ff3e-145">请求标头</span><span class="sxs-lookup"><span data-stu-id="0ff3e-145">Request headers</span></span>
| <span data-ttu-id="0ff3e-146">名称</span><span class="sxs-lookup"><span data-stu-id="0ff3e-146">Name</span></span>       | <span data-ttu-id="0ff3e-147">说明</span><span class="sxs-lookup"><span data-stu-id="0ff3e-147">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0ff3e-148">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ff3e-148">Authorization</span></span>  | <span data-ttu-id="0ff3e-149">持有者&lt;令牌&gt;</span><span class="sxs-lookup"><span data-stu-id="0ff3e-149">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="0ff3e-150">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0ff3e-150">Content-Type</span></span>  | <span data-ttu-id="0ff3e-151">application/json</span><span class="sxs-lookup"><span data-stu-id="0ff3e-151">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="0ff3e-152">请求正文</span><span class="sxs-lookup"><span data-stu-id="0ff3e-152">Request body</span></span>
<span data-ttu-id="0ff3e-153">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0ff3e-153">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ff3e-154">响应</span><span class="sxs-lookup"><span data-stu-id="0ff3e-154">Response</span></span>
<span data-ttu-id="0ff3e-p107">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和[组](../resources/group.md)集合对象。响应还包括作为 nextLink URL 或 deltaLink URL 的状态令牌。</span><span class="sxs-lookup"><span data-stu-id="0ff3e-p107">If successful, this method returns `200 OK` response code and [group](../resources/group.md) collection object in the response body. The response also includes a state token which is either a nextLink URL or a deltaLink URL.</span></span>

- <span data-ttu-id="0ff3e-p108">如果返回了 nextLink URL，则会话中存在要检索的其他数据页面。应用程序继续使用 nextLink URL 发出请求，直到响应中包含 deltaLink URL。</span><span class="sxs-lookup"><span data-stu-id="0ff3e-p108">If a nextLink URL is returned, there are additional pages of data to be retrieved in the session. The application continues making requests using the nextLink URL until a deltaLink URL is included in the response.</span></span>

- <span data-ttu-id="0ff3e-p109">如果返回了 deltaLink URL，则未返回关于资源现有状态的更多数据。为了执行以后的请求，应用程序使用 deltaLink URL 了解资源更改。</span><span class="sxs-lookup"><span data-stu-id="0ff3e-p109">If a deltaLink URL is returned, there is no more data about the existing state of the resource to be returned. For future requests, the application uses the deltaLink URL to learn about changes to the resource.</span></span>

<span data-ttu-id="0ff3e-161">请参阅：</span><span class="sxs-lookup"><span data-stu-id="0ff3e-161">See:</span></span></br>
- <span data-ttu-id="0ff3e-162">[使用增量查询](../../../concepts/delta_query_overview.md)了解更多详细信息</span><span class="sxs-lookup"><span data-stu-id="0ff3e-162">[Using Delta Query](../../../concepts/delta_query_overview.md) for more details</span></span></br>
- <span data-ttu-id="0ff3e-163">[获取组的增量更改](../../../concepts/delta_query_groups.md)获取示例请求。</span><span class="sxs-lookup"><span data-stu-id="0ff3e-163">[Get incremental changes for groups](../../../concepts/delta_query_groups.md) for an example requests.</span></span></br>
    
## <a name="example"></a><span data-ttu-id="0ff3e-164">示例</span><span class="sxs-lookup"><span data-stu-id="0ff3e-164">Example</span></span>
#### <a name="request"></a><span data-ttu-id="0ff3e-165">请求</span><span class="sxs-lookup"><span data-stu-id="0ff3e-165">Request</span></span>
<span data-ttu-id="0ff3e-166">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0ff3e-166">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/delta
```

#### <a name="response"></a><span data-ttu-id="0ff3e-167">响应</span><span class="sxs-lookup"><span data-stu-id="0ff3e-167">Response</span></span>
<span data-ttu-id="0ff3e-168">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0ff3e-168">The following is an example of the response.</span></span>
><span data-ttu-id="0ff3e-p110">**注意：**为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0ff3e-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups","@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvY1FSSc_",
  "value":[
    {
      "classification": "classification-value",
      "createdDateTime":"datetime-value",
      "description":"Test group 1",
      "displayName":"TestGroup1",
      "groupTypes": [
        "groupTypes-value"
      ],
      "mail": "mail-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->