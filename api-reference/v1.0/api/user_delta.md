# <a name="user-delta"></a><span data-ttu-id="111a6-101">user: delta</span><span class="sxs-lookup"><span data-stu-id="111a6-101">user: delta</span></span>

<span data-ttu-id="111a6-p101">[分区查询](../../../concepts/delta_query_overview.md)使应用程序能够发现新创建、更新或删除的实体，无需使用每个请求对目标资源执行完全读取。若要发现用户更改，请使用 *delta* 函数执行请求。请参阅[使用增量查询](../../../concepts/delta_query_overview.md)了解详细信息。</span><span class="sxs-lookup"><span data-stu-id="111a6-p101">[Delta query](../../../concepts/delta_query_overview.md) enables applications to discover newly created, updated, or deleted entities without performing a full read of the target resource with every request. To discover changes to users, perform a request using the *delta* function. See [Using Delta Query](../../../concepts/delta_query_overview.md) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="111a6-105">权限</span><span class="sxs-lookup"><span data-stu-id="111a6-105">Permissions</span></span>

<span data-ttu-id="111a6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="111a6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="111a6-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="111a6-108">Permission type</span></span>      | <span data-ttu-id="111a6-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="111a6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="111a6-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="111a6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="111a6-111">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="111a6-111">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="111a6-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="111a6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="111a6-113">User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="111a6-113">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="111a6-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="111a6-114">Application</span></span> | <span data-ttu-id="111a6-115">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="111a6-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="111a6-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="111a6-116">HTTP request</span></span>

<span data-ttu-id="111a6-117">为开始跟踪更改，请在用户资源上发出包含 delta 函数的请求。</span><span class="sxs-lookup"><span data-stu-id="111a6-117">To begin tracking changes, you make a request including the delta function on the users resource.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /users/delta
```

## <a name="query-parameters"></a><span data-ttu-id="111a6-118">查询参数</span><span class="sxs-lookup"><span data-stu-id="111a6-118">Query parameters</span></span>

<span data-ttu-id="111a6-p103">跟踪用户更改会引发一组对 **delta** 函数的一次或多次调用。如果要使用任意查询参数（`$deltatoken` 和 `$skiptoken` 除外），则必须在最初的 **delta** 请求中指定它。Microsoft Graph 自动将指定的任意参数编码为响应中提供的 `nextLink` 或 `deltaLink` URL 的令牌部分。你只需预先指定任意所需查询参数一次。在后续的请求中，只需复制并应用以前响应中的 `nextLink` 或 `deltaLink` URL，因为该 URL 已包含所需的编码参数。</span><span class="sxs-lookup"><span data-stu-id="111a6-p103">Tracking changes in users incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response. You only need to specify any desired query parameters once upfront. In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="111a6-124">查询参数</span><span class="sxs-lookup"><span data-stu-id="111a6-124">Query parameter</span></span>      | <span data-ttu-id="111a6-125">类型</span><span class="sxs-lookup"><span data-stu-id="111a6-125">Type</span></span>   |<span data-ttu-id="111a6-126">说明</span><span class="sxs-lookup"><span data-stu-id="111a6-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="111a6-127">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="111a6-127">$deltatoken</span></span> | <span data-ttu-id="111a6-128">string</span><span class="sxs-lookup"><span data-stu-id="111a6-128">string</span></span> | <span data-ttu-id="111a6-p104">对同一个用户集合之前的 **delta** 函数调用的 `deltaLink` URL 中返回的[状态令牌](../../../concepts/delta_query_overview.md)，指示该组更改跟踪的完成状态。将此令牌包含在对该集合的下一组更改追踪的首次请求中，并保存和应用整个 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="111a6-p104">A [state token](../../../concepts/delta_query_overview.md) returned in the `deltaLink` URL of the previous **delta** function call for the same user collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="111a6-131">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="111a6-131">$skiptoken</span></span> | <span data-ttu-id="111a6-132">string</span><span class="sxs-lookup"><span data-stu-id="111a6-132">string</span></span> | <span data-ttu-id="111a6-133">对之前的 **delta** 函数调用的 `nextLink` URL 中返回的[状态令牌](../../../concepts/delta_query_overview.md)，指示同一个用户集合中有进一步的更改需要追踪。</span><span class="sxs-lookup"><span data-stu-id="111a6-133">A [state token](../../../concepts/delta_query_overview.md) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same user collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="111a6-134">OData 查询参数</span><span class="sxs-lookup"><span data-stu-id="111a6-134">OData query parameters</span></span>

<span data-ttu-id="111a6-135">此方法支持可选的 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="111a6-135">This method supports the OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="111a6-p105">像在任何 GET 请求中一样，你可以使用 `$select` 查询参数以仅指定获取最佳性能所需的属性。始终返回 _id_ 属性。</span><span class="sxs-lookup"><span data-stu-id="111a6-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 
- <span data-ttu-id="111a6-138">对于邮件，Delta 查询支持 `$select`、`$top` 和 `$expand`。</span><span class="sxs-lookup"><span data-stu-id="111a6-138">Delta query support `$select`, `$top`, and `$expand` for messages.</span></span> 
- <span data-ttu-id="111a6-139">提供对 `$filter` 和 `$orderby` 的有限支持：</span><span class="sxs-lookup"><span data-stu-id="111a6-139">There is limited support for `$filter` and `$orderby`:</span></span>
  * <span data-ttu-id="111a6-140">唯一支持的 `$filter` 表达式用于跟踪对一个或两个特定用户 `$filter=id+eq+{value}` 或 `$filter=id+eq+{value1}+or+id+eq+{value2}` 的更改 `$filter=id+eq+{value1}+or+id+eq+{value2}`</span><span class="sxs-lookup"><span data-stu-id="111a6-140">The only supported `$filter` expression is for tracking changes on one or two specific users:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`</span></span> 
  * <span data-ttu-id="111a6-141">唯一支持的 `$orderby` 表达式是 `$orderby=receivedDateTime+desc`。</span><span class="sxs-lookup"><span data-stu-id="111a6-141">The only supported `$orderby` expression is `$orderby=receivedDateTime+desc`.</span></span> <span data-ttu-id="111a6-142">如果不包含 `$orderby` 表达式，则不能保证返回顺序。</span><span class="sxs-lookup"><span data-stu-id="111a6-142">If you do not include  an `$orderby` expression, the return order is not guaranteed.</span></span> 
- <span data-ttu-id="111a6-143">不支持 `$search`。</span><span class="sxs-lookup"><span data-stu-id="111a6-143">There is no support for `$search`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="111a6-144">请求标头</span><span class="sxs-lookup"><span data-stu-id="111a6-144">Request headers</span></span>
| <span data-ttu-id="111a6-145">名称</span><span class="sxs-lookup"><span data-stu-id="111a6-145">Name</span></span>       | <span data-ttu-id="111a6-146">说明</span><span class="sxs-lookup"><span data-stu-id="111a6-146">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="111a6-147">Authorization</span><span class="sxs-lookup"><span data-stu-id="111a6-147">Authorization</span></span>  | <span data-ttu-id="111a6-148">持有者&lt;令牌&gt;</span><span class="sxs-lookup"><span data-stu-id="111a6-148">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="111a6-149">Content-Type</span><span class="sxs-lookup"><span data-stu-id="111a6-149">Content-Type</span></span>  | <span data-ttu-id="111a6-150">application/json</span><span class="sxs-lookup"><span data-stu-id="111a6-150">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="111a6-151">请求正文</span><span class="sxs-lookup"><span data-stu-id="111a6-151">Request body</span></span>
<span data-ttu-id="111a6-152">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="111a6-152">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="111a6-153">响应</span><span class="sxs-lookup"><span data-stu-id="111a6-153">Response</span></span>

<span data-ttu-id="111a6-p107">如果成功，此方法的响应正文返回`200 OK`响应代码和[用户](../resources/user.md)集合对象。响应还包括 nextLink URL 或 deltaLink URL。</span><span class="sxs-lookup"><span data-stu-id="111a6-p107">If successful, this method returns `200 OK` response code and [user](../resources/user.md) collection object in the response body. The response also includes a nextLink URL or a deltaLink URL.</span></span> 

- <span data-ttu-id="111a6-p108">如果返回了 nextLink URL，则会话中存在要检索的其他数据页面。应用程序继续使用 nextLink URL 发出请求，直到响应中包含 deltaLink URL。</span><span class="sxs-lookup"><span data-stu-id="111a6-p108">If a nextLink URL is returned, there are additional pages of data to be retrieved in the session. The application continues making requests using the nextLink URL until a deltaLink URL is included in the response.</span></span>

- <span data-ttu-id="111a6-p109">如果返回了 deltaLink URL，则未返回关于资源现有状态的更多数据。为了执行以后的请求，应用程序使用 deltaLink URL 了解资源更改。</span><span class="sxs-lookup"><span data-stu-id="111a6-p109">If a deltaLink URL is returned, there is no more data about the existing state of the resource to be returned. For future requests, the application uses the deltaLink URL to learn about changes to the resource.</span></span>

<span data-ttu-id="111a6-160">请参阅：</span><span class="sxs-lookup"><span data-stu-id="111a6-160">See:</span></span></br>
- <span data-ttu-id="111a6-161">[使用增量查询](../../../concepts/delta_query_overview.md)了解更多详细信息</span><span class="sxs-lookup"><span data-stu-id="111a6-161">[Using Delta Query](../../../concepts/delta_query_overview.md) for more details</span></span></br>
- <span data-ttu-id="111a6-162">[获取用户的增量更改](../../../concepts/delta_query_users.md)获取示例请求。</span><span class="sxs-lookup"><span data-stu-id="111a6-162">[Get incremental changes for users](../../../concepts/delta_query_users.md) for an example requests.</span></span></br>

## <a name="example"></a><span data-ttu-id="111a6-163">示例</span><span class="sxs-lookup"><span data-stu-id="111a6-163">Example</span></span>
##### <a name="request"></a><span data-ttu-id="111a6-164">请求</span><span class="sxs-lookup"><span data-stu-id="111a6-164">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->
```http
GET https://graph.microsoft.com/v1.0/users/delta
```

##### <a name="response"></a><span data-ttu-id="111a6-165">响应</span><span class="sxs-lookup"><span data-stu-id="111a6-165">Response</span></span>
<span data-ttu-id="111a6-p110">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="111a6-p110">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- { 
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true 
} --> 
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "businessPhones": [
          "businessPhones-value"
      ],
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "jobTitle": "jobTitle-value",
      "mail": "mail-value",
      "mobilePhone": "mobilePhone-value",
      "officeLocation": "officeLocation-value",
      "preferredLanguage": "preferredLanguage-value",
      "surname": "surname-value",
      "userPrincipalName": "userPrincipalName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->