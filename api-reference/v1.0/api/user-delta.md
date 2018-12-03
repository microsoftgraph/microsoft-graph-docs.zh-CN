---
title: 'user: delta'
description: 获取新创建、 更新或删除用户，而无需执行的整个用户集的完全读取。 请参阅修订的详细信息。
ms.openlocfilehash: c460a15a63405a5f913096744b5eb150493c715d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011762"
---
# <a name="user-delta"></a><span data-ttu-id="46517-104">user: delta</span><span class="sxs-lookup"><span data-stu-id="46517-104">user: delta</span></span>

<span data-ttu-id="46517-105">获取新创建、 更新或删除用户，而无需执行的整个用户集的完全读取。</span><span class="sxs-lookup"><span data-stu-id="46517-105">Get newly created, updated, or deleted users without having to perform a full read of the entire user collection.</span></span> <span data-ttu-id="46517-106">有关详细信息，请参阅[修订](/graph/delta-query-overview)。</span><span class="sxs-lookup"><span data-stu-id="46517-106">See [Track changes](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="46517-107">权限</span><span class="sxs-lookup"><span data-stu-id="46517-107">Permissions</span></span>

<span data-ttu-id="46517-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="46517-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="46517-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="46517-110">Permission type</span></span>      | <span data-ttu-id="46517-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="46517-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="46517-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="46517-112">Delegated (work or school account)</span></span> | <span data-ttu-id="46517-113">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="46517-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="46517-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="46517-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46517-115">User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="46517-115">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="46517-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="46517-116">Application</span></span> | <span data-ttu-id="46517-117">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46517-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="46517-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="46517-118">HTTP request</span></span>

<span data-ttu-id="46517-119">为开始跟踪更改，请在用户资源上发出包含 delta 函数的请求。</span><span class="sxs-lookup"><span data-stu-id="46517-119">To begin tracking changes, you make a request including the delta function on the users resource.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/delta
```

## <a name="query-parameters"></a><span data-ttu-id="46517-120">查询参数</span><span class="sxs-lookup"><span data-stu-id="46517-120">Query parameters</span></span>

<span data-ttu-id="46517-121">跟踪中用户的更改会导致一个或多个**增量**函数调用的往返。</span><span class="sxs-lookup"><span data-stu-id="46517-121">Tracking changes in users incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="46517-122">如果您使用任何查询参数 (以外的其他`$deltatoken`和`$skiptoken`)，则必须指定该初始**增量**请求中。</span><span class="sxs-lookup"><span data-stu-id="46517-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="46517-123">Microsoft Graph 自动将任何指定的参数编码为的令牌部分`nextLink`或`deltaLink`响应中提供的 URL。</span><span class="sxs-lookup"><span data-stu-id="46517-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="46517-124">只需预先指定所需的任何查询参数一次。</span><span class="sxs-lookup"><span data-stu-id="46517-124">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="46517-125">在后续请求中，可以复制并应用之前响应中返回的 `nextLink` 或 `deltaLink` URL，因为此 URL 已包含所需的编码参数。</span><span class="sxs-lookup"><span data-stu-id="46517-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="46517-126">查询参数</span><span class="sxs-lookup"><span data-stu-id="46517-126">Query parameter</span></span>      | <span data-ttu-id="46517-127">类型</span><span class="sxs-lookup"><span data-stu-id="46517-127">Type</span></span>   |<span data-ttu-id="46517-128">说明</span><span class="sxs-lookup"><span data-stu-id="46517-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="46517-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="46517-129">$deltatoken</span></span> | <span data-ttu-id="46517-130">string</span><span class="sxs-lookup"><span data-stu-id="46517-130">string</span></span> | <span data-ttu-id="46517-p105">对同一个用户集合之前的 **delta** 函数调用的 `deltaLink` URL 中返回的[状态令牌](/graph/delta-query-overview)，指示该组更改跟踪的完成状态。将此令牌包含在对该集合的下一组更改追踪的首次请求中，并保存和应用整个 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="46517-p105">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same user collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="46517-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="46517-133">$skiptoken</span></span> | <span data-ttu-id="46517-134">string</span><span class="sxs-lookup"><span data-stu-id="46517-134">string</span></span> | <span data-ttu-id="46517-135">对之前的 **delta** 函数调用的 `nextLink` URL 中返回的[状态令牌](/graph/delta-query-overview)，指示同一个用户集合中有进一步的更改需要追踪。</span><span class="sxs-lookup"><span data-stu-id="46517-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same user collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="46517-136">OData 查询参数</span><span class="sxs-lookup"><span data-stu-id="46517-136">OData query parameters</span></span>

<span data-ttu-id="46517-137">此方法支持可选的 OData 查询参数，以帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="46517-137">This method supports optional OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="46517-p106">像在任何 GET 请求中一样，你可以使用 `$select` 查询参数以仅指定获取最佳性能所需的属性。始终返回 *id* 属性。</span><span class="sxs-lookup"><span data-stu-id="46517-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The *id* property is always returned.</span></span>
- <span data-ttu-id="46517-140">支持是有限的`$filter`:</span><span class="sxs-lookup"><span data-stu-id="46517-140">There is limited support for `$filter`:</span></span>
  - <span data-ttu-id="46517-141">唯一支持的 `$filter` 表达式用于跟踪对特定对象 `$filter=id+eq+{value}` 的更改。</span><span class="sxs-lookup"><span data-stu-id="46517-141">The only supported `$filter` expression is for tracking changes on a specific object: `$filter=id+eq+{value}`.</span></span> <span data-ttu-id="46517-142">可以筛选多个对象。</span><span class="sxs-lookup"><span data-stu-id="46517-142">You can filter multiple objects.</span></span> <span data-ttu-id="46517-143">例如，`https://graph.microsoft.com/v1.0/users/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`。</span><span class="sxs-lookup"><span data-stu-id="46517-143">For example, `https://graph.microsoft.com/v1.0/users/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span></span> <span data-ttu-id="46517-144">筛选对象不能超出 50 个。</span><span class="sxs-lookup"><span data-stu-id="46517-144">There is a limit of 50 filtered objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="46517-145">请求标头</span><span class="sxs-lookup"><span data-stu-id="46517-145">Request headers</span></span>
| <span data-ttu-id="46517-146">名称</span><span class="sxs-lookup"><span data-stu-id="46517-146">Name</span></span>       | <span data-ttu-id="46517-147">说明</span><span class="sxs-lookup"><span data-stu-id="46517-147">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="46517-148">Authorization</span><span class="sxs-lookup"><span data-stu-id="46517-148">Authorization</span></span>  | <span data-ttu-id="46517-149">持有者&lt;令牌&gt;</span><span class="sxs-lookup"><span data-stu-id="46517-149">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="46517-150">Content-Type</span><span class="sxs-lookup"><span data-stu-id="46517-150">Content-Type</span></span>  | <span data-ttu-id="46517-151">application/json</span><span class="sxs-lookup"><span data-stu-id="46517-151">application/json</span></span> |
| <span data-ttu-id="46517-152">Prefer</span><span class="sxs-lookup"><span data-stu-id="46517-152">Prefer</span></span> | <span data-ttu-id="46517-153">返回 = 最少</span><span class="sxs-lookup"><span data-stu-id="46517-153">return=minimal</span></span> <br><br><span data-ttu-id="46517-154">指定与请求使用此标头`deltaLink`会返回自上次循环后已更改的对象属性。</span><span class="sxs-lookup"><span data-stu-id="46517-154">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="46517-155">可选。</span><span class="sxs-lookup"><span data-stu-id="46517-155">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="46517-156">请求正文</span><span class="sxs-lookup"><span data-stu-id="46517-156">Request body</span></span>
<span data-ttu-id="46517-157">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="46517-157">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="46517-158">响应</span><span class="sxs-lookup"><span data-stu-id="46517-158">Response</span></span>

<span data-ttu-id="46517-159">如果成功，此方法返回`200 OK`响应正文中的响应代码和[用户](../resources/user.md)集合的对象。</span><span class="sxs-lookup"><span data-stu-id="46517-159">If successful, this method returns `200 OK` response code and [user](../resources/user.md) collection object in the response body.</span></span> <span data-ttu-id="46517-160">响应还包括`nextLink`URL 或`deltaLink`URL。</span><span class="sxs-lookup"><span data-stu-id="46517-160">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="46517-161">如果`nextLink`返回 URL:</span><span class="sxs-lookup"><span data-stu-id="46517-161">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="46517-162">这指示有会话中检索的数据的其他页面。</span><span class="sxs-lookup"><span data-stu-id="46517-162">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="46517-163">应用程序将继续进行请求使用`nextLink`直到 URL `deltaLink` URL 包含响应中。</span><span class="sxs-lookup"><span data-stu-id="46517-163">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="46517-164">响应包含一组相同的属性，如初始增量查询请求中所示。</span><span class="sxs-lookup"><span data-stu-id="46517-164">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="46517-165">这样，您可以在启动增量周期捕获对象的完整当前状态。</span><span class="sxs-lookup"><span data-stu-id="46517-165">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="46517-166">如果`deltaLink`返回 URL:</span><span class="sxs-lookup"><span data-stu-id="46517-166">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="46517-167">这表明没有更多有关要返回的资源的现有状态数据。</span><span class="sxs-lookup"><span data-stu-id="46517-167">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="46517-168">保存并使用`deltaLink`URL 以了解如何更改为下一轮中的资源。</span><span class="sxs-lookup"><span data-stu-id="46517-168">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="46517-169">您可以选择指定`Prefer:return=minimal`标头，以响应时间以来已经更改的属性值中包括`deltaLink`颁发。</span><span class="sxs-lookup"><span data-stu-id="46517-169">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="46517-170">默认值： 返回作为初始增量请求的同一属性</span><span class="sxs-lookup"><span data-stu-id="46517-170">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="46517-171">默认情况下，请求使用`deltaLink`或`nextLink`与选定初始增量查询中相同的属性返回以下方式：</span><span class="sxs-lookup"><span data-stu-id="46517-171">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="46517-172">如果已更改的属性，在响应中包含的新值。</span><span class="sxs-lookup"><span data-stu-id="46517-172">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="46517-173">这包括属性被设置为 null 值。</span><span class="sxs-lookup"><span data-stu-id="46517-173">This includes properties being set to null value.</span></span>
- <span data-ttu-id="46517-174">如果具有未更改的属性，在响应中包含的旧值。</span><span class="sxs-lookup"><span data-stu-id="46517-174">If the property has not changed, the old value is included in the response.</span></span>
- <span data-ttu-id="46517-175">如果从未它将不会包含在响应中根本之前设置该属性。</span><span class="sxs-lookup"><span data-stu-id="46517-175">If the property has never been set before it will not be included in the response at all.</span></span>


> <span data-ttu-id="46517-176">**注意：** 与此行为，通过查看响应它不能以告知属性是否已更改或未。</span><span class="sxs-lookup"><span data-stu-id="46517-176">**Note:** With this behavior, by looking at the response it is not possible to tell whether a property is changing or not.</span></span> <span data-ttu-id="46517-177">此外，增量响应倾向于大型因为它们包含的所有属性值-下面的[第二个示例](#request-2)中所示。</span><span class="sxs-lookup"><span data-stu-id="46517-177">Also, the delta responses tend to be large because they contain all property values  - as shown in the [second example](#request-2) below.</span></span>

#### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="46517-178">可选： 仅返回已更改的属性</span><span class="sxs-lookup"><span data-stu-id="46517-178">Alternative: return only the changed properties</span></span>

<span data-ttu-id="46517-179">添加可选请求标头中的`prefer:return=minimal`-导致以下行为：</span><span class="sxs-lookup"><span data-stu-id="46517-179">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="46517-180">如果已更改的属性，在响应中包含的新值。</span><span class="sxs-lookup"><span data-stu-id="46517-180">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="46517-181">这包括属性被设置为 null 值。</span><span class="sxs-lookup"><span data-stu-id="46517-181">This includes properties being set to null value.</span></span>
- <span data-ttu-id="46517-182">如果具有未更改的属性，该属性不包括在响应中根本。</span><span class="sxs-lookup"><span data-stu-id="46517-182">If the property has not changed, the property is not included in the response at all.</span></span> <span data-ttu-id="46517-183">（不同于默认行为。）</span><span class="sxs-lookup"><span data-stu-id="46517-183">(Different from the default behavior.)</span></span>

> <span data-ttu-id="46517-184">**注意：** 标头可以添加到`deltaLink`任何时间点的增量周期中的请求。</span><span class="sxs-lookup"><span data-stu-id="46517-184">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="46517-185">头只影响的响应中包括的属性集，而不会影响如何执行增量查询。</span><span class="sxs-lookup"><span data-stu-id="46517-185">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span> <span data-ttu-id="46517-186">请参阅下面的[第三个示例](#request-3)。</span><span class="sxs-lookup"><span data-stu-id="46517-186">See the [third example](#request-3) below.</span></span>

### <a name="example"></a><span data-ttu-id="46517-187">示例</span><span class="sxs-lookup"><span data-stu-id="46517-187">Example</span></span>

#### <a name="request-1"></a><span data-ttu-id="46517-188">请求 1</span><span class="sxs-lookup"><span data-stu-id="46517-188">Request 1</span></span>

<span data-ttu-id="46517-189">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="46517-189">The following is an example of the request.</span></span> <span data-ttu-id="46517-190">没有任何`$select`参数，以便跟踪和返回一组默认属性。</span><span class="sxs-lookup"><span data-stu-id="46517-190">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/users/delta
```

#### <a name="response-1"></a><span data-ttu-id="46517-191">响应 1</span><span class="sxs-lookup"><span data-stu-id="46517-191">Response 1</span></span>

<span data-ttu-id="46517-192">以下是时使用的响应示例`deltaLink`获取从查询初始化。</span><span class="sxs-lookup"><span data-stu-id="46517-192">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span>

><span data-ttu-id="46517-p119">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="46517-p119">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

#### <a name="request-2"></a><span data-ttu-id="46517-195">请求 2</span><span class="sxs-lookup"><span data-stu-id="46517-195">Request 2</span></span>

<span data-ttu-id="46517-196">下面的示例演示选择 3 属性更改跟踪具有默认响应行为的初始请求：</span><span class="sxs-lookup"><span data-stu-id="46517-196">The next example shows the initial request selecting 3 properties for change tracking, with default response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/users/delta?$select=displayName,jobTitle,mobilePhone
```

#### <a name="response-2"></a><span data-ttu-id="46517-197">响应 2</span><span class="sxs-lookup"><span data-stu-id="46517-197">Response 2</span></span>

<span data-ttu-id="46517-198">以下是时使用的响应示例`deltaLink`获取从查询初始化。</span><span class="sxs-lookup"><span data-stu-id="46517-198">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="46517-199">请注意，在响应中包含所有 3 属性并不知道哪些以来已更改`deltaLink`获得。</span><span class="sxs-lookup"><span data-stu-id="46517-199">Note that all 3 properties are included in the response and it is not known which ones have changed since the `deltaLink` was obtained.</span></span>

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
      "jobTitle": "jobTitle-value",
      "mobilePhone": null
    }
  ]
}
```

#### <a name="request-3"></a><span data-ttu-id="46517-200">请求 3</span><span class="sxs-lookup"><span data-stu-id="46517-200">Request 3</span></span>

<span data-ttu-id="46517-201">下面的示例演示选择 3 属性更改跟踪具有最少的替代响应行为的初始请求：</span><span class="sxs-lookup"><span data-stu-id="46517-201">The next example shows the initial request selecting 3 properties for change tracking, with alternative minimal response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/users/delta?$select=displayName,jobTitle,mobilePhone
Prefer: return=minimal
```

#### <a name="response-3"></a><span data-ttu-id="46517-202">响应 3</span><span class="sxs-lookup"><span data-stu-id="46517-202">Response 3</span></span>

<span data-ttu-id="46517-203">以下是时使用的响应示例`deltaLink`获取从查询初始化。</span><span class="sxs-lookup"><span data-stu-id="46517-203">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="46517-204">请注意，`mobilePhone`属性不包括在内，这意味着它未更改以来上一次增量查询;`displayName`和`jobTitle`是包含已更改其值的方法。</span><span class="sxs-lookup"><span data-stu-id="46517-204">Note that the `mobilePhone` property is not included, which means it has not changed since the last delta query; `displayName` and `jobTitle` are included which means their values have changed.</span></span>

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

- <span data-ttu-id="46517-205">[使用增量查询来跟踪 Microsoft Graph 数据中的更改](/graph/delta-query-overview)。</span><span class="sxs-lookup"><span data-stu-id="46517-205">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>
- <span data-ttu-id="46517-206">[获取用户的增量更改](/graph/delta-query-users)。</span><span class="sxs-lookup"><span data-stu-id="46517-206">[Get incremental changes for users](/graph/delta-query-users).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->