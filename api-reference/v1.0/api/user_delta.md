# <a name="user-delta"></a><span data-ttu-id="a0e1c-101">user: delta</span><span class="sxs-lookup"><span data-stu-id="a0e1c-101">user: delta</span></span>

<span data-ttu-id="a0e1c-p101">[分区查询](../../../concepts/delta_query_overview.md)使应用程序能够发现新创建、更新或删除的实体，无需使用每个请求对目标资源执行完全读取。若要发现用户更改，请使用 *delta* 函数执行请求。请参阅[使用增量查询](../../../concepts/delta_query_overview.md)了解详细信息。</span><span class="sxs-lookup"><span data-stu-id="a0e1c-p101">[Delta query](../../../concepts/delta_query_overview.md) enables applications to discover newly created, updated, or deleted entities without performing a full read of the target resource with every request. To discover changes to users, perform a request using the *delta* function. See [Using Delta Query](../../../concepts/delta_query_overview.md) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="a0e1c-105">权限</span><span class="sxs-lookup"><span data-stu-id="a0e1c-105">Permissions</span></span>

<span data-ttu-id="a0e1c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a0e1c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="a0e1c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="a0e1c-108">Permission type</span></span>      | <span data-ttu-id="a0e1c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a0e1c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a0e1c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a0e1c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a0e1c-111">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a0e1c-111">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a0e1c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a0e1c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0e1c-113">User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a0e1c-113">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="a0e1c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="a0e1c-114">Application</span></span> | <span data-ttu-id="a0e1c-115">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0e1c-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a0e1c-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a0e1c-116">HTTP request</span></span>

<span data-ttu-id="a0e1c-117">为开始跟踪更改，请在用户资源上发出包含 delta 函数的请求。</span><span class="sxs-lookup"><span data-stu-id="a0e1c-117">To begin tracking changes, you make a request including the delta function on the users resource.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /users/delta
```

### <a name="query-parameters"></a><span data-ttu-id="a0e1c-118">查询参数</span><span class="sxs-lookup"><span data-stu-id="a0e1c-118">Query parameters</span></span>

<span data-ttu-id="a0e1c-p103">跟踪用户更改会引发一组对 **delta** 函数的一次或多次调用。如果要使用任意查询参数（`$deltatoken` 和 `$skiptoken` 除外），则必须在最初的 **delta** 请求中指定它。Microsoft Graph 自动将指定的任意参数编码为响应中提供的 `nextLink` 或 `deltaLink` URL 的令牌部分。你只需预先指定任意所需查询参数一次。在后续的请求中，只需复制并应用以前响应中的 `nextLink` 或 `deltaLink` URL，因为该 URL 已包含所需的编码参数。</span><span class="sxs-lookup"><span data-stu-id="a0e1c-p103">Tracking changes in users incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response. You only need to specify any desired query parameters once upfront. In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="a0e1c-124">查询参数</span><span class="sxs-lookup"><span data-stu-id="a0e1c-124">Query parameter</span></span>      | <span data-ttu-id="a0e1c-125">类型</span><span class="sxs-lookup"><span data-stu-id="a0e1c-125">Type</span></span>   |<span data-ttu-id="a0e1c-126">说明</span><span class="sxs-lookup"><span data-stu-id="a0e1c-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a0e1c-127">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="a0e1c-127">$deltatoken</span></span> | <span data-ttu-id="a0e1c-128">string</span><span class="sxs-lookup"><span data-stu-id="a0e1c-128">string</span></span> | <span data-ttu-id="a0e1c-p104">对同一个用户集合之前的 **delta** 函数调用的 `deltaLink` URL 中返回的[状态令牌](../../../concepts/delta_query_overview.md)，指示该组更改跟踪的完成状态。将此令牌包含在对该集合的下一组更改追踪的首次请求中，并保存和应用整个 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="a0e1c-p104">A [state token](../../../concepts/delta_query_overview.md) returned in the `deltaLink` URL of the previous **delta** function call for the same user collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="a0e1c-131">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="a0e1c-131">$skiptoken</span></span> | <span data-ttu-id="a0e1c-132">string</span><span class="sxs-lookup"><span data-stu-id="a0e1c-132">string</span></span> | <span data-ttu-id="a0e1c-133">对之前的 **delta** 函数调用的 `nextLink` URL 中返回的[状态令牌](../../../concepts/delta_query_overview.md)，指示同一个用户集合中有进一步的更改需要追踪。</span><span class="sxs-lookup"><span data-stu-id="a0e1c-133">A [state token](../../../concepts/delta_query_overview.md) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same user collection.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="a0e1c-134">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a0e1c-134">Optional query parameters</span></span>

<span data-ttu-id="a0e1c-135">此方法支持 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a0e1c-135">This method supports OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="a0e1c-p105">像在任何 GET 请求中一样，你可以使用 `$select` 查询参数以仅指定获取最佳性能所需的属性。始终返回 _id_ 属性。</span><span class="sxs-lookup"><span data-stu-id="a0e1c-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 
- <span data-ttu-id="a0e1c-138">对于邮件，增量查询支持 `$select`、`$top` 和 `$expand`。</span><span class="sxs-lookup"><span data-stu-id="a0e1c-138">Delta query support `$select`, `$top`, and `$expand` for messages.</span></span> 
- <span data-ttu-id="a0e1c-p106">提供对 `$orderby` 的有限支持：唯一支持的 `$orderby` 表达式是 `$orderby=receivedDateTime+desc`。如果不包含 `$orderby` 表达式，则不能保证返回顺序。</span><span class="sxs-lookup"><span data-stu-id="a0e1c-p106">There is limited support for `$orderby`: The only supported `$orderby` expression is `$orderby=receivedDateTime+desc`. If you do not include  an `$orderby` expression, the return order is not guaranteed.</span></span> 
- <span data-ttu-id="a0e1c-141">不支持 `$search`。</span><span class="sxs-lookup"><span data-stu-id="a0e1c-141">There is no support for `$search`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a0e1c-142">请求标头</span><span class="sxs-lookup"><span data-stu-id="a0e1c-142">Request headers</span></span>
| <span data-ttu-id="a0e1c-143">名称</span><span class="sxs-lookup"><span data-stu-id="a0e1c-143">Name</span></span>       | <span data-ttu-id="a0e1c-144">说明</span><span class="sxs-lookup"><span data-stu-id="a0e1c-144">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a0e1c-145">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0e1c-145">Authorization</span></span>  | <span data-ttu-id="a0e1c-146">持有者&lt;令牌&gt;</span><span class="sxs-lookup"><span data-stu-id="a0e1c-146">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="a0e1c-147">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a0e1c-147">Content-Type</span></span>  | <span data-ttu-id="a0e1c-148">application/json</span><span class="sxs-lookup"><span data-stu-id="a0e1c-148">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="a0e1c-149">请求正文</span><span class="sxs-lookup"><span data-stu-id="a0e1c-149">Request body</span></span>
<span data-ttu-id="a0e1c-150">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a0e1c-150">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0e1c-151">响应</span><span class="sxs-lookup"><span data-stu-id="a0e1c-151">Response</span></span>

<span data-ttu-id="a0e1c-p107">如果成功，此方法的响应正文返回`200 OK`响应代码和[用户](../resources/user.md)集合对象。响应还包括 nextLink URL 或 deltaLink URL。</span><span class="sxs-lookup"><span data-stu-id="a0e1c-p107">If successful, this method returns `200 OK` response code and [user](../resources/user.md) collection object in the response body. The response also includes a nextLink URL or a deltaLink URL.</span></span> 

- <span data-ttu-id="a0e1c-p108">如果返回了 nextLink URL，则会话中存在要检索的其他数据页面。应用程序继续使用 nextLink URL 发出请求，直到响应中包含 deltaLink URL。</span><span class="sxs-lookup"><span data-stu-id="a0e1c-p108">If a nextLink URL is returned, there are additional pages of data to be retrieved in the session. The application continues making requests using the nextLink URL until a deltaLink URL is included in the response.</span></span>

- <span data-ttu-id="a0e1c-p109">如果返回了 deltaLink URL，则未返回关于资源现有状态的更多数据。为了执行以后的请求，应用程序使用 deltaLink URL 了解资源更改。</span><span class="sxs-lookup"><span data-stu-id="a0e1c-p109">If a deltaLink URL is returned, there is no more data about the existing state of the resource to be returned. For future requests, the application uses the deltaLink URL to learn about changes to the resource.</span></span>

<span data-ttu-id="a0e1c-158">请参阅：</span><span class="sxs-lookup"><span data-stu-id="a0e1c-158">See:</span></span></br>
- <span data-ttu-id="a0e1c-159">[使用增量查询](../../../concepts/delta_query_overview.md)了解更多详细信息</span><span class="sxs-lookup"><span data-stu-id="a0e1c-159">[Using Delta Query](../../../concepts/delta_query_overview.md) for more details</span></span></br>
- <span data-ttu-id="a0e1c-160">[获取用户的增量更改](../../../concepts/delta_query_users.md)获取示例请求。</span><span class="sxs-lookup"><span data-stu-id="a0e1c-160">[Get incremental changes for users](../../../concepts/delta_query_users.md) for an example requests.</span></span></br>

## <a name="example"></a><span data-ttu-id="a0e1c-161">示例</span><span class="sxs-lookup"><span data-stu-id="a0e1c-161">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a0e1c-162">请求</span><span class="sxs-lookup"><span data-stu-id="a0e1c-162">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->
```http
GET https://graph.microsoft.com/v1.0/users/delta
```

##### <a name="response"></a><span data-ttu-id="a0e1c-163">响应</span><span class="sxs-lookup"><span data-stu-id="a0e1c-163">Response</span></span>
<span data-ttu-id="a0e1c-p110">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a0e1c-p110">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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