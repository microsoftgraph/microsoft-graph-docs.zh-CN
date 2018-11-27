# <a name="user-delta"></a><span data-ttu-id="55d33-101">user: delta</span><span class="sxs-lookup"><span data-stu-id="55d33-101">user: delta</span></span>

<span data-ttu-id="55d33-102">获取新创建、 更新或删除用户，而无需执行的整个用户集的完全读取。</span><span class="sxs-lookup"><span data-stu-id="55d33-102">Get newly created, updated, or deleted users without having to perform a full read of the entire user collection.</span></span> <span data-ttu-id="55d33-103">有关详细信息，请参阅[修订](../../../concepts/delta_query_overview.md)。</span><span class="sxs-lookup"><span data-stu-id="55d33-103">See [Track changes](../../../concepts/delta_query_overview.md) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="55d33-104">权限</span><span class="sxs-lookup"><span data-stu-id="55d33-104">Permissions</span></span>

<span data-ttu-id="55d33-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="55d33-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="55d33-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="55d33-107">Permission type</span></span>      | <span data-ttu-id="55d33-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="55d33-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="55d33-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="55d33-109">Delegated (work or school account)</span></span> | <span data-ttu-id="55d33-110">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="55d33-110">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="55d33-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="55d33-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55d33-112">User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="55d33-112">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="55d33-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="55d33-113">Application</span></span> | <span data-ttu-id="55d33-114">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55d33-114">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="55d33-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="55d33-115">HTTP request</span></span>

<span data-ttu-id="55d33-116">为开始跟踪更改，请在用户资源上发出包含 delta 函数的请求。</span><span class="sxs-lookup"><span data-stu-id="55d33-116">To begin tracking changes, you make a request including the delta function on the users resource.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/delta
```

## <a name="query-parameters"></a><span data-ttu-id="55d33-117">查询参数</span><span class="sxs-lookup"><span data-stu-id="55d33-117">Query parameters</span></span>

<span data-ttu-id="55d33-118">跟踪中用户的更改会导致一个或多个**增量**函数调用的往返。</span><span class="sxs-lookup"><span data-stu-id="55d33-118">Tracking changes in users incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="55d33-119">如果您使用任何查询参数 (以外的其他`$deltatoken`和`$skiptoken`)，则必须指定该初始**增量**请求中。</span><span class="sxs-lookup"><span data-stu-id="55d33-119">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="55d33-120">Microsoft Graph 自动将任何指定的参数编码为的令牌部分`nextLink`或`deltaLink`响应中提供的 URL。</span><span class="sxs-lookup"><span data-stu-id="55d33-120">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="55d33-121">只需预先指定所需的任何查询参数一次。</span><span class="sxs-lookup"><span data-stu-id="55d33-121">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="55d33-122">在后续请求中，可以复制并应用之前响应中返回的 `nextLink` 或 `deltaLink` URL，因为此 URL 已包含所需的编码参数。</span><span class="sxs-lookup"><span data-stu-id="55d33-122">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="55d33-123">查询参数</span><span class="sxs-lookup"><span data-stu-id="55d33-123">Query parameter</span></span>      | <span data-ttu-id="55d33-124">类型</span><span class="sxs-lookup"><span data-stu-id="55d33-124">Type</span></span>   |<span data-ttu-id="55d33-125">说明</span><span class="sxs-lookup"><span data-stu-id="55d33-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="55d33-126">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="55d33-126">$deltatoken</span></span> | <span data-ttu-id="55d33-127">string</span><span class="sxs-lookup"><span data-stu-id="55d33-127">string</span></span> | <span data-ttu-id="55d33-p104">对同一个用户集合之前的 **delta** 函数调用的 `deltaLink` URL 中返回的[状态令牌](../../../concepts/delta_query_overview.md)，指示该组更改跟踪的完成状态。将此令牌包含在对该集合的下一组更改追踪的首次请求中，并保存和应用整个 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="55d33-p104">A [state token](../../../concepts/delta_query_overview.md) returned in the `deltaLink` URL of the previous **delta** function call for the same user collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="55d33-130">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="55d33-130">$skiptoken</span></span> | <span data-ttu-id="55d33-131">string</span><span class="sxs-lookup"><span data-stu-id="55d33-131">string</span></span> | <span data-ttu-id="55d33-132">对之前的 **delta** 函数调用的 `nextLink` URL 中返回的[状态令牌](../../../concepts/delta_query_overview.md)，指示同一个用户集合中有进一步的更改需要追踪。</span><span class="sxs-lookup"><span data-stu-id="55d33-132">A [state token](../../../concepts/delta_query_overview.md) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same user collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="55d33-133">OData 查询参数</span><span class="sxs-lookup"><span data-stu-id="55d33-133">OData query parameters</span></span>

<span data-ttu-id="55d33-134">此方法支持可选的 OData 查询参数，以帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="55d33-134">This method supports optional OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="55d33-p105">像在任何 GET 请求中一样，你可以使用 `$select` 查询参数以仅指定获取最佳性能所需的属性。始终返回 *id* 属性。</span><span class="sxs-lookup"><span data-stu-id="55d33-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The *id* property is always returned.</span></span>
- <span data-ttu-id="55d33-137">支持是有限的`$filter`:</span><span class="sxs-lookup"><span data-stu-id="55d33-137">There is limited support for `$filter`:</span></span>
  - <span data-ttu-id="55d33-138">唯一支持的 `$filter` 表达式用于跟踪对特定对象 `$filter=id+eq+{value}` 的更改。</span><span class="sxs-lookup"><span data-stu-id="55d33-138">The only supported `$filter` expression is for tracking changes on a specific object: `$filter=id+eq+{value}`.</span></span> <span data-ttu-id="55d33-139">可以筛选多个对象。</span><span class="sxs-lookup"><span data-stu-id="55d33-139">You can filter multiple objects.</span></span> <span data-ttu-id="55d33-140">例如，`https://graph.microsoft.com/v1.0/users/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`。</span><span class="sxs-lookup"><span data-stu-id="55d33-140">For example, `https://graph.microsoft.com/v1.0/users/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span></span> <span data-ttu-id="55d33-141">筛选对象不能超出 50 个。</span><span class="sxs-lookup"><span data-stu-id="55d33-141">There is a limit of 50 filtered objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="55d33-142">请求标头</span><span class="sxs-lookup"><span data-stu-id="55d33-142">Request headers</span></span>
| <span data-ttu-id="55d33-143">名称</span><span class="sxs-lookup"><span data-stu-id="55d33-143">Name</span></span>       | <span data-ttu-id="55d33-144">说明</span><span class="sxs-lookup"><span data-stu-id="55d33-144">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="55d33-145">Authorization</span><span class="sxs-lookup"><span data-stu-id="55d33-145">Authorization</span></span>  | <span data-ttu-id="55d33-146">持有者&lt;令牌&gt;</span><span class="sxs-lookup"><span data-stu-id="55d33-146">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="55d33-147">Content-Type</span><span class="sxs-lookup"><span data-stu-id="55d33-147">Content-Type</span></span>  | <span data-ttu-id="55d33-148">application/json</span><span class="sxs-lookup"><span data-stu-id="55d33-148">application/json</span></span> |
| <span data-ttu-id="55d33-149">Prefer</span><span class="sxs-lookup"><span data-stu-id="55d33-149">Prefer</span></span> | <span data-ttu-id="55d33-150">返回 = 最少</span><span class="sxs-lookup"><span data-stu-id="55d33-150">return=minimal</span></span> <br><br><span data-ttu-id="55d33-151">指定与请求使用此标头`deltaLink`会返回自上次循环后已更改的对象属性。</span><span class="sxs-lookup"><span data-stu-id="55d33-151">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="55d33-152">可选。</span><span class="sxs-lookup"><span data-stu-id="55d33-152">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="55d33-153">请求正文</span><span class="sxs-lookup"><span data-stu-id="55d33-153">Request body</span></span>
<span data-ttu-id="55d33-154">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="55d33-154">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="55d33-155">响应</span><span class="sxs-lookup"><span data-stu-id="55d33-155">Response</span></span>

<span data-ttu-id="55d33-156">如果成功，此方法返回`200 OK`响应正文中的响应代码和[用户](../resources/user.md)集合的对象。</span><span class="sxs-lookup"><span data-stu-id="55d33-156">If successful, this method returns `200 OK` response code and [user](../resources/user.md) collection object in the response body.</span></span> <span data-ttu-id="55d33-157">响应还包括`nextLink`URL 或`deltaLink`URL。</span><span class="sxs-lookup"><span data-stu-id="55d33-157">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="55d33-158">如果`nextLink`返回 URL:</span><span class="sxs-lookup"><span data-stu-id="55d33-158">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="55d33-159">这指示有会话中检索的数据的其他页面。</span><span class="sxs-lookup"><span data-stu-id="55d33-159">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="55d33-160">应用程序将继续进行请求使用`nextLink`直到 URL `deltaLink` URL 包含响应中。</span><span class="sxs-lookup"><span data-stu-id="55d33-160">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="55d33-161">响应包含一组相同的属性，如初始增量查询请求中所示。</span><span class="sxs-lookup"><span data-stu-id="55d33-161">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="55d33-162">这样，您可以在启动增量周期捕获对象的完整当前状态。</span><span class="sxs-lookup"><span data-stu-id="55d33-162">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="55d33-163">如果`deltaLink`返回 URL:</span><span class="sxs-lookup"><span data-stu-id="55d33-163">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="55d33-164">这表明没有更多有关要返回的资源的现有状态数据。</span><span class="sxs-lookup"><span data-stu-id="55d33-164">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="55d33-165">保存并使用`deltaLink`URL 以了解如何更改为下一轮中的资源。</span><span class="sxs-lookup"><span data-stu-id="55d33-165">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="55d33-166">您可以选择指定`Prefer:return=minimal`标头，以响应时间以来已经更改的属性值中包括`deltaLink`颁发。</span><span class="sxs-lookup"><span data-stu-id="55d33-166">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="55d33-167">默认值： 返回作为初始增量请求的同一属性</span><span class="sxs-lookup"><span data-stu-id="55d33-167">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="55d33-168">默认情况下，请求使用`deltaLink`或`nextLink`与选定初始增量查询中相同的属性返回以下方式：</span><span class="sxs-lookup"><span data-stu-id="55d33-168">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="55d33-169">如果该属性已更改的 JSON 响应中返回的属性。</span><span class="sxs-lookup"><span data-stu-id="55d33-169">If the property has changed, return the property in the JSON response.</span></span>
- <span data-ttu-id="55d33-170">如果设置了为空值的属性，返回属性值为 null。</span><span class="sxs-lookup"><span data-stu-id="55d33-170">If the property has been set to an empty value, return the property value as null.</span></span>
- <span data-ttu-id="55d33-171">如果具有未更改的属性，返回的值为 null。</span><span class="sxs-lookup"><span data-stu-id="55d33-171">If the property has not changed, return the value as null.</span></span>

> <span data-ttu-id="55d33-172">**注意：** 具有上述行为，它不能区分未更改的属性和一个已更改为`null`值。</span><span class="sxs-lookup"><span data-stu-id="55d33-172">**Note:** With the above behavior, it is not possible to differentiate between a property that has not changed and one that has changed to a `null` value.</span></span> <span data-ttu-id="55d33-173">请参阅下面的[第二个示例](#request-2)。</span><span class="sxs-lookup"><span data-stu-id="55d33-173">See the [second example](#request-2) below.</span></span> <span data-ttu-id="55d33-174">如果这是重要，我们建议使用下节所述的替代行为。</span><span class="sxs-lookup"><span data-stu-id="55d33-174">If this is important, we recommend using the alternative behavior described in the next section.</span></span>

#### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="55d33-175">可选： 仅返回已更改的属性</span><span class="sxs-lookup"><span data-stu-id="55d33-175">Alternative: return only the changed properties</span></span>

<span data-ttu-id="55d33-176">添加可选请求标头中的`prefer:return=minimal`-导致以下行为：</span><span class="sxs-lookup"><span data-stu-id="55d33-176">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="55d33-177">如果该属性已更改的 JSON 响应中返回的属性。</span><span class="sxs-lookup"><span data-stu-id="55d33-177">If the property has changed, return the property in the JSON response.</span></span>
- <span data-ttu-id="55d33-178">如果设置了为空值的属性，返回属性值为 null。</span><span class="sxs-lookup"><span data-stu-id="55d33-178">If the property has been set to an empty value, return the property value as null.</span></span>
- <span data-ttu-id="55d33-179">如果具有未更改的属性，不包括属性中的 JSON 响应。</span><span class="sxs-lookup"><span data-stu-id="55d33-179">If the property has not changed, do not include the property in the JSON response.</span></span> <span data-ttu-id="55d33-180">（不同于默认行为。）</span><span class="sxs-lookup"><span data-stu-id="55d33-180">(Different from the default behavior.)</span></span>

> <span data-ttu-id="55d33-181">**注意：** 标头可以添加到`deltaLink`任何时间点的增量周期中的请求。</span><span class="sxs-lookup"><span data-stu-id="55d33-181">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="55d33-182">头只影响的响应中包括的属性集，而不会影响如何执行增量查询。</span><span class="sxs-lookup"><span data-stu-id="55d33-182">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span> <span data-ttu-id="55d33-183">请参阅下面的[第三个示例](#request-3)。</span><span class="sxs-lookup"><span data-stu-id="55d33-183">See the [third example](#request-3) below.</span></span>

### <a name="example"></a><span data-ttu-id="55d33-184">示例</span><span class="sxs-lookup"><span data-stu-id="55d33-184">Example</span></span>

#### <a name="request-1"></a><span data-ttu-id="55d33-185">请求 1</span><span class="sxs-lookup"><span data-stu-id="55d33-185">Request 1</span></span>

<span data-ttu-id="55d33-186">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="55d33-186">The following is an example of the request.</span></span> <span data-ttu-id="55d33-187">没有任何`$select`参数，以便跟踪和返回一组默认属性。</span><span class="sxs-lookup"><span data-stu-id="55d33-187">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/users/delta
```

#### <a name="response-1"></a><span data-ttu-id="55d33-188">响应 1</span><span class="sxs-lookup"><span data-stu-id="55d33-188">Response 1</span></span>

<span data-ttu-id="55d33-189">以下是时使用的响应示例`deltaLink`获取从查询初始化。</span><span class="sxs-lookup"><span data-stu-id="55d33-189">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span>

><span data-ttu-id="55d33-p116">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="55d33-p116">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

#### <a name="request-2"></a><span data-ttu-id="55d33-192">请求 2</span><span class="sxs-lookup"><span data-stu-id="55d33-192">Request 2</span></span>

<span data-ttu-id="55d33-193">下面的示例演示选择 3 属性更改跟踪具有默认响应行为的初始请求：</span><span class="sxs-lookup"><span data-stu-id="55d33-193">The next example shows the initial request selecting 3 properties for change tracking, with default response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/users/delta?$select=displayName,jobTitle,mobilePhone
```

#### <a name="response-2"></a><span data-ttu-id="55d33-194">响应 2</span><span class="sxs-lookup"><span data-stu-id="55d33-194">Response 2</span></span>

<span data-ttu-id="55d33-195">以下是时使用的响应示例`deltaLink`获取从查询初始化。</span><span class="sxs-lookup"><span data-stu-id="55d33-195">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="55d33-196">请注意，`jobTitle`和`mobilePhone`具有的值`null`这意味着它们可能已不发生更改或已设置为空值。</span><span class="sxs-lookup"><span data-stu-id="55d33-196">Note that `jobTitle` and `mobilePhone` have the value of `null` which means that they may have not changed or have been set to an empty value.</span></span>

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
      "displayName": "displayName-value",
      "jobTitle": null,
      "mobilePhone": null
    }
  ]
}
```

#### <a name="request-3"></a><span data-ttu-id="55d33-197">请求 3</span><span class="sxs-lookup"><span data-stu-id="55d33-197">Request 3</span></span>

<span data-ttu-id="55d33-198">下面的示例演示选择 3 属性更改跟踪具有最少的替代响应行为的初始请求：</span><span class="sxs-lookup"><span data-stu-id="55d33-198">The next example shows the initial request selecting 3 properties for change tracking, with alternative minimal response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/users/delta?$select=displayName,jobTitle,mobilePhone
Prefer: return=minimal
```

#### <a name="response-3"></a><span data-ttu-id="55d33-199">响应 3</span><span class="sxs-lookup"><span data-stu-id="55d33-199">Response 3</span></span>

<span data-ttu-id="55d33-200">以下是时使用的响应示例`deltaLink`获取从查询初始化。</span><span class="sxs-lookup"><span data-stu-id="55d33-200">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="55d33-201">请注意，`mobilePhone`属性不包括在内，这意味着它未更改以来上一次增量查询;`displayName`和`jobTitle`是包含已更改其值的方法。</span><span class="sxs-lookup"><span data-stu-id="55d33-201">Note that the `mobilePhone` property is not included, which means it has not changed since the last delta query; `displayName` and `jobTitle` are included which means their values have changed.</span></span>

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
      "displayName": "displayName-value",
      "jobTitle": null
    }
  ]
}
```

- <span data-ttu-id="55d33-202">[使用增量查询来跟踪 Microsoft Graph 数据中的更改](../../../concepts/delta_query_overview.md)。</span><span class="sxs-lookup"><span data-stu-id="55d33-202">[Use delta query to track changes in Microsoft Graph data](../../../concepts/delta_query_overview.md).</span></span>
- <span data-ttu-id="55d33-203">[获取用户的增量更改](../../../concepts/delta_query_users.md)。</span><span class="sxs-lookup"><span data-stu-id="55d33-203">[Get incremental changes for users](../../../concepts/delta_query_users.md).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->