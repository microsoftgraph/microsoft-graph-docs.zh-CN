# <a name="group-delta"></a><span data-ttu-id="e2ee6-101">group: delta</span><span class="sxs-lookup"><span data-stu-id="e2ee6-101">group: delta</span></span>
<span data-ttu-id="e2ee6-102">获取新创建、 更新或删除组，而无需执行整个组集合的完全读取包括组成员身份更改。</span><span class="sxs-lookup"><span data-stu-id="e2ee6-102">Get newly created, updated, or deleted groups, including group membership changes, without having to perform a full read of the entire group collection.</span></span> <span data-ttu-id="e2ee6-103">有关详细信息，请参阅[使用增量查询](../../../concepts/delta_query_overview.md)。</span><span class="sxs-lookup"><span data-stu-id="e2ee6-103">See [Using Delta Query](../../../concepts/delta_query_overview.md) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="e2ee6-104">权限</span><span class="sxs-lookup"><span data-stu-id="e2ee6-104">Permissions</span></span>

<span data-ttu-id="e2ee6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="e2ee6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e2ee6-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="e2ee6-107">Permission type</span></span>      | <span data-ttu-id="e2ee6-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e2ee6-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2ee6-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e2ee6-109">Delegated (work or school account)</span></span> | <span data-ttu-id="e2ee6-110">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2ee6-110">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e2ee6-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e2ee6-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2ee6-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="e2ee6-112">Not supported.</span></span>    |
|<span data-ttu-id="e2ee6-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="e2ee6-113">Application</span></span> | <span data-ttu-id="e2ee6-114">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2ee6-114">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2ee6-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e2ee6-115">HTTP request</span></span>

<span data-ttu-id="e2ee6-116">为开始跟踪更改，请在组资源上发出包含 delta 函数的请求。</span><span class="sxs-lookup"><span data-stu-id="e2ee6-116">To begin tracking changes, you make a request including the delta function on the groups resource.</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/delta
```

## <a name="query-parameters"></a><span data-ttu-id="e2ee6-117">查询参数</span><span class="sxs-lookup"><span data-stu-id="e2ee6-117">Query parameters</span></span>

<span data-ttu-id="e2ee6-p103">跟踪组中的更改会触发一个或多个 **delta** 函数调用。如果使用任何查询参数（而不是 `$deltatoken` 和 `$skiptoken`），必须在初始 **delta** 请求中指定它。Microsoft Graph 会自动将任何指定参数编码为响应中返回的 `nextLink` 或 `deltaLink` URL 的令牌部分。</span><span class="sxs-lookup"><span data-stu-id="e2ee6-p103">Tracking changes in groups incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="e2ee6-121">只需预先指定所需的任何查询参数一次。</span><span class="sxs-lookup"><span data-stu-id="e2ee6-121">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="e2ee6-122">在后续请求中，可以复制并应用之前响应中返回的 `nextLink` 或 `deltaLink` URL，因为此 URL 已包含所需的编码参数。</span><span class="sxs-lookup"><span data-stu-id="e2ee6-122">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="e2ee6-123">查询参数</span><span class="sxs-lookup"><span data-stu-id="e2ee6-123">Query parameter</span></span> | <span data-ttu-id="e2ee6-124">类型</span><span class="sxs-lookup"><span data-stu-id="e2ee6-124">Type</span></span>  |<span data-ttu-id="e2ee6-125">说明</span><span class="sxs-lookup"><span data-stu-id="e2ee6-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e2ee6-126">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="e2ee6-126">$deltatoken</span></span> | <span data-ttu-id="e2ee6-127">string</span><span class="sxs-lookup"><span data-stu-id="e2ee6-127">string</span></span> | <span data-ttu-id="e2ee6-p104">对同一个组集合之前的 **delta** 函数调用的 `deltaLink` URL 中返回的[状态令牌](../../../concepts/delta_query_overview.md)，指示该组更改跟踪的完成状态。将此令牌包含在对该集合的下一组更改追踪的首次请求中，并保存和应用整个 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="e2ee6-p104">A [state token](../../../concepts/delta_query_overview.md) returned in the `deltaLink` URL of the previous **delta** function call for the same group collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="e2ee6-130">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="e2ee6-130">$skiptoken</span></span> | <span data-ttu-id="e2ee6-131">string</span><span class="sxs-lookup"><span data-stu-id="e2ee6-131">string</span></span> | <span data-ttu-id="e2ee6-132">对之前的 **delta** 函数调用的 `nextLink` URL 中返回的[状态令牌](../../../concepts/delta_query_overview.md)，指示同一个组集合中有进一步的更改需要追踪。</span><span class="sxs-lookup"><span data-stu-id="e2ee6-132">A [state token](../../../concepts/delta_query_overview.md) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same group collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="e2ee6-133">OData 查询参数</span><span class="sxs-lookup"><span data-stu-id="e2ee6-133">OData query parameters</span></span>

<span data-ttu-id="e2ee6-134">此方法支持可选的 OData 查询参数，以帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e2ee6-134">This method supports optional OData query parameters to help customize the response.</span></span>

- <span data-ttu-id="e2ee6-p105">像在任何 GET 请求中一样，你可以使用 `$select` 查询参数以仅指定获取最佳性能所需的属性。始终返回 *id* 属性。</span><span class="sxs-lookup"><span data-stu-id="e2ee6-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The *id* property is always returned.</span></span>
- <span data-ttu-id="e2ee6-137">您可以使用`$expand=members`获取成员身份更改。</span><span class="sxs-lookup"><span data-stu-id="e2ee6-137">You can use `$expand=members` to get membership changes.</span></span>
- <span data-ttu-id="e2ee6-138">支持是有限的`$filter`:</span><span class="sxs-lookup"><span data-stu-id="e2ee6-138">There is limited support for `$filter`:</span></span>
  - <span data-ttu-id="e2ee6-139">唯一支持的 `$filter` 表达式用于跟踪对特定对象 `$filter=id+eq+{value}` 的更改。</span><span class="sxs-lookup"><span data-stu-id="e2ee6-139">The only supported `$filter` expression is for tracking changes on a specific object: `$filter=id+eq+{value}`.</span></span> <span data-ttu-id="e2ee6-140">可以筛选多个对象。</span><span class="sxs-lookup"><span data-stu-id="e2ee6-140">You can filter multiple objects.</span></span> <span data-ttu-id="e2ee6-141">例如，`https://graph.microsoft.com/v1.0/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`。</span><span class="sxs-lookup"><span data-stu-id="e2ee6-141">For example, `https://graph.microsoft.com/v1.0/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span></span> <span data-ttu-id="e2ee6-142">筛选对象不能超出 50 个。</span><span class="sxs-lookup"><span data-stu-id="e2ee6-142">There is a limit of 50 filtered objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e2ee6-143">请求标头</span><span class="sxs-lookup"><span data-stu-id="e2ee6-143">Request headers</span></span>

| <span data-ttu-id="e2ee6-144">名称</span><span class="sxs-lookup"><span data-stu-id="e2ee6-144">Name</span></span>       | <span data-ttu-id="e2ee6-145">说明</span><span class="sxs-lookup"><span data-stu-id="e2ee6-145">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e2ee6-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2ee6-146">Authorization</span></span>  | <span data-ttu-id="e2ee6-147">持有者&lt;令牌&gt;</span><span class="sxs-lookup"><span data-stu-id="e2ee6-147">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="e2ee6-148">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e2ee6-148">Content-Type</span></span>  | <span data-ttu-id="e2ee6-149">application/json</span><span class="sxs-lookup"><span data-stu-id="e2ee6-149">application/json</span></span> |
| <span data-ttu-id="e2ee6-150">Prefer</span><span class="sxs-lookup"><span data-stu-id="e2ee6-150">Prefer</span></span> | <span data-ttu-id="e2ee6-151">返回 = 最少</span><span class="sxs-lookup"><span data-stu-id="e2ee6-151">return=minimal</span></span> <br><br><span data-ttu-id="e2ee6-152">指定与请求使用此标头`deltaLink`会返回自上次循环后已更改的对象属性。</span><span class="sxs-lookup"><span data-stu-id="e2ee6-152">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="e2ee6-153">可选。</span><span class="sxs-lookup"><span data-stu-id="e2ee6-153">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e2ee6-154">请求正文</span><span class="sxs-lookup"><span data-stu-id="e2ee6-154">Request body</span></span>

<span data-ttu-id="e2ee6-155">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e2ee6-155">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="e2ee6-156">响应</span><span class="sxs-lookup"><span data-stu-id="e2ee6-156">Response</span></span>

<span data-ttu-id="e2ee6-157">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和[组](../resources/group.md)集合对象。</span><span class="sxs-lookup"><span data-stu-id="e2ee6-157">If successful, this method returns `200 OK` response code and [group](../resources/group.md) collection object in the response body.</span></span> <span data-ttu-id="e2ee6-158">响应还包括一个状态标记为`nextLink`URL 或`deltaLink`URL。</span><span class="sxs-lookup"><span data-stu-id="e2ee6-158">The response also includes a state token which is either a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="e2ee6-159">如果`nextLink`返回 URL:</span><span class="sxs-lookup"><span data-stu-id="e2ee6-159">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="e2ee6-160">这指示有会话中检索的数据的其他页面。</span><span class="sxs-lookup"><span data-stu-id="e2ee6-160">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="e2ee6-161">应用程序将继续进行请求使用`nextLink`直到 URL `deltaLink` URL 包含响应中。</span><span class="sxs-lookup"><span data-stu-id="e2ee6-161">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="e2ee6-162">响应包含一组相同的属性，如初始增量查询请求中所示。</span><span class="sxs-lookup"><span data-stu-id="e2ee6-162">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="e2ee6-163">这样，您可以在启动增量周期捕获对象的完整当前状态。</span><span class="sxs-lookup"><span data-stu-id="e2ee6-163">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="e2ee6-164">如果`deltaLink`返回 URL:</span><span class="sxs-lookup"><span data-stu-id="e2ee6-164">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="e2ee6-165">这表明没有更多有关要返回的资源的现有状态数据。</span><span class="sxs-lookup"><span data-stu-id="e2ee6-165">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="e2ee6-166">保存并使用`deltaLink`URL 以了解如何更改为下一轮中的资源。</span><span class="sxs-lookup"><span data-stu-id="e2ee6-166">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="e2ee6-167">您可以选择指定`Prefer:return=minimal`标头，以响应时间以来已经更改的属性值中包括`deltaLink`颁发。</span><span class="sxs-lookup"><span data-stu-id="e2ee6-167">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="e2ee6-168">默认值： 返回作为初始增量请求的同一属性</span><span class="sxs-lookup"><span data-stu-id="e2ee6-168">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="e2ee6-169">默认情况下，请求使用`deltaLink`或`nextLink`与选定初始增量查询中相同的属性返回以下方式：</span><span class="sxs-lookup"><span data-stu-id="e2ee6-169">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="e2ee6-170">如果该属性已更改的 JSON 响应中返回的属性。</span><span class="sxs-lookup"><span data-stu-id="e2ee6-170">If the property has changed, return the property in the JSON response.</span></span>
- <span data-ttu-id="e2ee6-171">如果设置了为空值的属性，返回属性值为 null。</span><span class="sxs-lookup"><span data-stu-id="e2ee6-171">If the property has been set to an empty value, return the property value as null.</span></span>
- <span data-ttu-id="e2ee6-172">如果具有未更改的属性，返回的值为 null。</span><span class="sxs-lookup"><span data-stu-id="e2ee6-172">If the property has not changed, return the value as null.</span></span>

> <span data-ttu-id="e2ee6-173">**注意：** 具有上述行为，它不能区分未更改的属性和一个已更改为`null`值。</span><span class="sxs-lookup"><span data-stu-id="e2ee6-173">**Note:** With the above behavior, it is not possible to differentiate between a property that has not changed and one that has changed to a `null` value.</span></span> <span data-ttu-id="e2ee6-174">请参阅下面的[第二个示例](#request-2)。</span><span class="sxs-lookup"><span data-stu-id="e2ee6-174">See the [second example](#request-2) below.</span></span> <span data-ttu-id="e2ee6-175">如果这是重要，我们建议使用下节所述的替代行为。</span><span class="sxs-lookup"><span data-stu-id="e2ee6-175">If this is important, we recommend using the alternative behavior described in the next section.</span></span>

#### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="e2ee6-176">可选： 仅返回已更改的属性</span><span class="sxs-lookup"><span data-stu-id="e2ee6-176">Alternative: return only the changed properties</span></span>

<span data-ttu-id="e2ee6-177">添加可选请求标头中的`prefer:return=minimal`-导致以下行为：</span><span class="sxs-lookup"><span data-stu-id="e2ee6-177">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="e2ee6-178">如果该属性已更改的 JSON 响应中返回的属性。</span><span class="sxs-lookup"><span data-stu-id="e2ee6-178">If the property has changed, return the property in the JSON response.</span></span>
- <span data-ttu-id="e2ee6-179">如果设置了为空值的属性，返回属性值为 null。</span><span class="sxs-lookup"><span data-stu-id="e2ee6-179">If the property has been set to an empty value, return the property value as null.</span></span>
- <span data-ttu-id="e2ee6-180">如果具有未更改的属性，不包括属性中的 JSON 响应。</span><span class="sxs-lookup"><span data-stu-id="e2ee6-180">If the property has not changed, do not include the property in the JSON response.</span></span> <span data-ttu-id="e2ee6-181">（不同于默认行为。）</span><span class="sxs-lookup"><span data-stu-id="e2ee6-181">(Different from the default behavior.)</span></span>

> <span data-ttu-id="e2ee6-182">**注意：** 标头可以添加到`deltaLink`任何时间点的增量周期中的请求。</span><span class="sxs-lookup"><span data-stu-id="e2ee6-182">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="e2ee6-183">头只影响的响应中包括的属性集，而不会影响如何执行增量查询。</span><span class="sxs-lookup"><span data-stu-id="e2ee6-183">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span> <span data-ttu-id="e2ee6-184">请参阅下面的[第三个示例](#request-3)。</span><span class="sxs-lookup"><span data-stu-id="e2ee6-184">See the [third example](#request-3) below.</span></span>

### <a name="example"></a><span data-ttu-id="e2ee6-185">示例</span><span class="sxs-lookup"><span data-stu-id="e2ee6-185">Example</span></span>

#### <a name="request-1"></a><span data-ttu-id="e2ee6-186">请求 1</span><span class="sxs-lookup"><span data-stu-id="e2ee6-186">Request 1</span></span>

<span data-ttu-id="e2ee6-187">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e2ee6-187">The following is an example of the request.</span></span> <span data-ttu-id="e2ee6-188">没有任何`$select`参数，以便跟踪和返回一组默认属性。</span><span class="sxs-lookup"><span data-stu-id="e2ee6-188">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/groups/delta
```

#### <a name="response-1"></a><span data-ttu-id="e2ee6-189">响应 1</span><span class="sxs-lookup"><span data-stu-id="e2ee6-189">Response 1</span></span>

<span data-ttu-id="e2ee6-190">以下是时使用的响应示例`deltaLink`获取从查询初始化。</span><span class="sxs-lookup"><span data-stu-id="e2ee6-190">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span>

><span data-ttu-id="e2ee6-191">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e2ee6-191">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e2ee6-192">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e2ee6-192">All the properties will be returned from an actual call.</span></span>
>
> <span data-ttu-id="e2ee6-193">请注意*members@delta*属性的组中包括的 member 对象的 id 的状态。</span><span class="sxs-lookup"><span data-stu-id="e2ee6-193">Note the presence of the *members@delta* property which includes the ids of member objects in the group.</span></span>

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
      "mail": "mail-value",
      "members@delta": [
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "693acd06-2877-4339-8ade-b704261fe7a0"
               },
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "49320844-be99-4164-8167-87ff5d047ace"
               }
      ]
    }
  ]
}
```

#### <a name="request-2"></a><span data-ttu-id="e2ee6-194">请求 2</span><span class="sxs-lookup"><span data-stu-id="e2ee6-194">Request 2</span></span>

<span data-ttu-id="e2ee6-195">下面的示例演示选择 3 属性更改跟踪具有默认响应行为的初始请求：</span><span class="sxs-lookup"><span data-stu-id="e2ee6-195">The next example shows the initial request selecting 3 properties for change tracking, with default response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description,mailNickname
```

#### <a name="response-2"></a><span data-ttu-id="e2ee6-196">响应 2</span><span class="sxs-lookup"><span data-stu-id="e2ee6-196">Response 2</span></span>

<span data-ttu-id="e2ee6-197">以下是时使用的响应示例`deltaLink`获取从查询初始化。</span><span class="sxs-lookup"><span data-stu-id="e2ee6-197">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="e2ee6-198">请注意，`description`和`mailNickname`具有的值`null`这意味着它们可能已不发生更改或已设置为空值。</span><span class="sxs-lookup"><span data-stu-id="e2ee6-198">Note that `description` and `mailNickname` have the value of `null` which means that they may have not changed or have been set to an empty value.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "description": null,
      "mailNickname": null
    }
  ]
}
```

#### <a name="request-3"></a><span data-ttu-id="e2ee6-199">请求 3</span><span class="sxs-lookup"><span data-stu-id="e2ee6-199">Request 3</span></span>

<span data-ttu-id="e2ee6-200">下面的示例演示选择 3 属性更改跟踪具有最少的替代响应行为的初始请求：</span><span class="sxs-lookup"><span data-stu-id="e2ee6-200">The next example shows the initial request selecting 3 properties for change tracking, with alternative minimal response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description,mailNickname
Prefer: return=minimal
```

#### <a name="response-3"></a><span data-ttu-id="e2ee6-201">响应 3</span><span class="sxs-lookup"><span data-stu-id="e2ee6-201">Response 3</span></span>

<span data-ttu-id="e2ee6-202">以下是时使用的响应示例`deltaLink`获取从查询初始化。</span><span class="sxs-lookup"><span data-stu-id="e2ee6-202">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="e2ee6-203">请注意，`mailNickname`属性不包括在内，这意味着它未更改以来上一次增量查询;`displayName`和`description`是包含已更改其值的方法。</span><span class="sxs-lookup"><span data-stu-id="e2ee6-203">Note that the `mailNickname` property is not included, which means it has not changed since the last delta query; `displayName` and `description` are included which means their values have changed.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "description": null
    }
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="e2ee6-204">另请参阅</span><span class="sxs-lookup"><span data-stu-id="e2ee6-204">See also</span></span>

- <span data-ttu-id="e2ee6-205">[使用增量查询来跟踪 Microsoft Graph 数据中的更改](../../../concepts/delta_query_overview.md)。</span><span class="sxs-lookup"><span data-stu-id="e2ee6-205">[Use delta query to track changes in Microsoft Graph data](../../../concepts/delta_query_overview.md).</span></span>
- <span data-ttu-id="e2ee6-206">[获取组的增量更改](../../../concepts/delta_query_groups.md)。</span><span class="sxs-lookup"><span data-stu-id="e2ee6-206">[Get incremental changes for groups](../../../concepts/delta_query_groups.md).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
