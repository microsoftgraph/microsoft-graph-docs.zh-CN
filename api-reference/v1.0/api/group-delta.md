---
title: 'group: delta'
description: 获取新创建、 更新或删除组，而无需执行整个组集合的完全读取包括组成员身份更改。 有关详细信息，请参阅使用增量查询。
localization_priority: Normal
ms.openlocfilehash: d9032b6066184ddf993f7fa4645cae00ed1d48b9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815139"
---
# <a name="group-delta"></a><span data-ttu-id="e5cca-104">group: delta</span><span class="sxs-lookup"><span data-stu-id="e5cca-104">group: delta</span></span>
<span data-ttu-id="e5cca-105">获取新创建、 更新或删除组，而无需执行整个组集合的完全读取包括组成员身份更改。</span><span class="sxs-lookup"><span data-stu-id="e5cca-105">Get newly created, updated, or deleted groups, including group membership changes, without having to perform a full read of the entire group collection.</span></span> <span data-ttu-id="e5cca-106">有关详细信息，请参阅[使用增量查询](/graph/delta-query-overview)。</span><span class="sxs-lookup"><span data-stu-id="e5cca-106">See [Using Delta Query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="e5cca-107">权限</span><span class="sxs-lookup"><span data-stu-id="e5cca-107">Permissions</span></span>

<span data-ttu-id="e5cca-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e5cca-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5cca-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e5cca-110">Permission type</span></span>      | <span data-ttu-id="e5cca-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e5cca-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5cca-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e5cca-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e5cca-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5cca-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e5cca-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e5cca-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5cca-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e5cca-115">Not supported.</span></span>    |
|<span data-ttu-id="e5cca-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e5cca-116">Application</span></span> | <span data-ttu-id="e5cca-117">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5cca-117">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e5cca-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e5cca-118">HTTP request</span></span>

<span data-ttu-id="e5cca-119">为开始跟踪更改，请在组资源上发出包含 delta 函数的请求。</span><span class="sxs-lookup"><span data-stu-id="e5cca-119">To begin tracking changes, you make a request including the delta function on the groups resource.</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/delta
```

## <a name="query-parameters"></a><span data-ttu-id="e5cca-120">查询参数</span><span class="sxs-lookup"><span data-stu-id="e5cca-120">Query parameters</span></span>

<span data-ttu-id="e5cca-p104">跟踪组中的更改会触发一个或多个 **delta** 函数调用。如果使用任何查询参数（而不是 `$deltatoken` 和 `$skiptoken`），必须在初始 **delta** 请求中指定它。Microsoft Graph 会自动将任何指定参数编码为响应中返回的 `nextLink` 或 `deltaLink` URL 的令牌部分。</span><span class="sxs-lookup"><span data-stu-id="e5cca-p104">Tracking changes in groups incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="e5cca-124">只需预先指定所需的任何查询参数一次。</span><span class="sxs-lookup"><span data-stu-id="e5cca-124">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="e5cca-125">在后续请求中，可以复制并应用之前响应中返回的 `nextLink` 或 `deltaLink` URL，因为此 URL 已包含所需的编码参数。</span><span class="sxs-lookup"><span data-stu-id="e5cca-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="e5cca-126">查询参数</span><span class="sxs-lookup"><span data-stu-id="e5cca-126">Query parameter</span></span> | <span data-ttu-id="e5cca-127">类型</span><span class="sxs-lookup"><span data-stu-id="e5cca-127">Type</span></span>  |<span data-ttu-id="e5cca-128">说明</span><span class="sxs-lookup"><span data-stu-id="e5cca-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e5cca-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="e5cca-129">$deltatoken</span></span> | <span data-ttu-id="e5cca-130">string</span><span class="sxs-lookup"><span data-stu-id="e5cca-130">string</span></span> | <span data-ttu-id="e5cca-p105">对同一个组集合之前的 **delta** 函数调用的 `deltaLink` URL 中返回的[状态令牌](/graph/delta-query-overview)，指示该组更改跟踪的完成状态。将此令牌包含在对该集合的下一组更改追踪的首次请求中，并保存和应用整个 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="e5cca-p105">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same group collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="e5cca-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="e5cca-133">$skiptoken</span></span> | <span data-ttu-id="e5cca-134">string</span><span class="sxs-lookup"><span data-stu-id="e5cca-134">string</span></span> | <span data-ttu-id="e5cca-135">对之前的 **delta** 函数调用的 `nextLink` URL 中返回的[状态令牌](/graph/delta-query-overview)，指示同一个组集合中有进一步的更改需要追踪。</span><span class="sxs-lookup"><span data-stu-id="e5cca-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same group collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="e5cca-136">OData 查询参数</span><span class="sxs-lookup"><span data-stu-id="e5cca-136">OData query parameters</span></span>

<span data-ttu-id="e5cca-137">此方法支持可选的 OData 查询参数，以帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e5cca-137">This method supports optional OData query parameters to help customize the response.</span></span>

- <span data-ttu-id="e5cca-p106">像在任何 GET 请求中一样，你可以使用 `$select` 查询参数以仅指定获取最佳性能所需的属性。始终返回 *id* 属性。</span><span class="sxs-lookup"><span data-stu-id="e5cca-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The *id* property is always returned.</span></span>
- <span data-ttu-id="e5cca-140">您可以使用`$expand=members`获取成员身份更改。</span><span class="sxs-lookup"><span data-stu-id="e5cca-140">You can use `$expand=members` to get membership changes.</span></span>
- <span data-ttu-id="e5cca-141">支持是有限的`$filter`:</span><span class="sxs-lookup"><span data-stu-id="e5cca-141">There is limited support for `$filter`:</span></span>
  - <span data-ttu-id="e5cca-142">唯一支持的 `$filter` 表达式用于跟踪对特定对象 `$filter=id+eq+{value}` 的更改。</span><span class="sxs-lookup"><span data-stu-id="e5cca-142">The only supported `$filter` expression is for tracking changes on a specific object: `$filter=id+eq+{value}`.</span></span> <span data-ttu-id="e5cca-143">可以筛选多个对象。</span><span class="sxs-lookup"><span data-stu-id="e5cca-143">You can filter multiple objects.</span></span> <span data-ttu-id="e5cca-144">例如，`https://graph.microsoft.com/v1.0/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`。</span><span class="sxs-lookup"><span data-stu-id="e5cca-144">For example, `https://graph.microsoft.com/v1.0/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span></span> <span data-ttu-id="e5cca-145">筛选对象不能超出 50 个。</span><span class="sxs-lookup"><span data-stu-id="e5cca-145">There is a limit of 50 filtered objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e5cca-146">请求标头</span><span class="sxs-lookup"><span data-stu-id="e5cca-146">Request headers</span></span>

| <span data-ttu-id="e5cca-147">名称</span><span class="sxs-lookup"><span data-stu-id="e5cca-147">Name</span></span>       | <span data-ttu-id="e5cca-148">说明</span><span class="sxs-lookup"><span data-stu-id="e5cca-148">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e5cca-149">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5cca-149">Authorization</span></span>  | <span data-ttu-id="e5cca-150">持有者&lt;令牌&gt;</span><span class="sxs-lookup"><span data-stu-id="e5cca-150">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="e5cca-151">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e5cca-151">Content-Type</span></span>  | <span data-ttu-id="e5cca-152">application/json</span><span class="sxs-lookup"><span data-stu-id="e5cca-152">application/json</span></span> |
| <span data-ttu-id="e5cca-153">Prefer</span><span class="sxs-lookup"><span data-stu-id="e5cca-153">Prefer</span></span> | <span data-ttu-id="e5cca-154">返回 = 最少</span><span class="sxs-lookup"><span data-stu-id="e5cca-154">return=minimal</span></span> <br><br><span data-ttu-id="e5cca-155">指定与请求使用此标头`deltaLink`会返回自上次循环后已更改的对象属性。</span><span class="sxs-lookup"><span data-stu-id="e5cca-155">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="e5cca-156">可选。</span><span class="sxs-lookup"><span data-stu-id="e5cca-156">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e5cca-157">请求正文</span><span class="sxs-lookup"><span data-stu-id="e5cca-157">Request body</span></span>

<span data-ttu-id="e5cca-158">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e5cca-158">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="e5cca-159">响应</span><span class="sxs-lookup"><span data-stu-id="e5cca-159">Response</span></span>

<span data-ttu-id="e5cca-160">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和[组](../resources/group.md)集合对象。</span><span class="sxs-lookup"><span data-stu-id="e5cca-160">If successful, this method returns `200 OK` response code and [group](../resources/group.md) collection object in the response body.</span></span> <span data-ttu-id="e5cca-161">响应还包括一个状态标记为`nextLink`URL 或`deltaLink`URL。</span><span class="sxs-lookup"><span data-stu-id="e5cca-161">The response also includes a state token which is either a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="e5cca-162">如果`nextLink`返回 URL:</span><span class="sxs-lookup"><span data-stu-id="e5cca-162">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="e5cca-163">这指示有会话中检索的数据的其他页面。</span><span class="sxs-lookup"><span data-stu-id="e5cca-163">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="e5cca-164">应用程序将继续进行请求使用`nextLink`直到 URL `deltaLink` URL 包含响应中。</span><span class="sxs-lookup"><span data-stu-id="e5cca-164">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="e5cca-165">响应包含一组相同的属性，如初始增量查询请求中所示。</span><span class="sxs-lookup"><span data-stu-id="e5cca-165">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="e5cca-166">这样，您可以在启动增量周期捕获对象的完整当前状态。</span><span class="sxs-lookup"><span data-stu-id="e5cca-166">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="e5cca-167">如果`deltaLink`返回 URL:</span><span class="sxs-lookup"><span data-stu-id="e5cca-167">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="e5cca-168">这表明没有更多有关要返回的资源的现有状态数据。</span><span class="sxs-lookup"><span data-stu-id="e5cca-168">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="e5cca-169">保存并使用`deltaLink`URL 以了解如何更改为下一轮中的资源。</span><span class="sxs-lookup"><span data-stu-id="e5cca-169">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="e5cca-170">您可以选择指定`Prefer:return=minimal`标头，以响应时间以来已经更改的属性值中包括`deltaLink`颁发。</span><span class="sxs-lookup"><span data-stu-id="e5cca-170">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="e5cca-171">默认值： 返回作为初始增量请求的同一属性</span><span class="sxs-lookup"><span data-stu-id="e5cca-171">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="e5cca-172">默认情况下，请求使用`deltaLink`或`nextLink`与选定初始增量查询中相同的属性返回以下方式：</span><span class="sxs-lookup"><span data-stu-id="e5cca-172">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="e5cca-173">如果已更改的属性，在响应中包含的新值。</span><span class="sxs-lookup"><span data-stu-id="e5cca-173">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="e5cca-174">这包括属性被设置为 null 值。</span><span class="sxs-lookup"><span data-stu-id="e5cca-174">This includes properties being set to null value.</span></span>
- <span data-ttu-id="e5cca-175">如果具有未更改的属性，在响应中包含的旧值。</span><span class="sxs-lookup"><span data-stu-id="e5cca-175">If the property has not changed, the old value is included in the response.</span></span>
- <span data-ttu-id="e5cca-176">如果从未它将不会包含在响应中根本之前设置该属性。</span><span class="sxs-lookup"><span data-stu-id="e5cca-176">If the property has never been set before it will not be included in the response at all.</span></span>


> <span data-ttu-id="e5cca-177">**注意：** 与此行为，通过查看响应它不能以告知属性是否已更改或未。</span><span class="sxs-lookup"><span data-stu-id="e5cca-177">**Note:** With this behavior, by looking at the response it is not possible to tell whether a property is changing or not.</span></span> <span data-ttu-id="e5cca-178">此外，增量响应倾向于大型因为它们包含的所有属性值-下面的[第二个示例](#request-2)中所示。</span><span class="sxs-lookup"><span data-stu-id="e5cca-178">Also, the delta responses tend to be large because they contain all property values  - as shown in the [second example](#request-2) below.</span></span>

#### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="e5cca-179">可选： 仅返回已更改的属性</span><span class="sxs-lookup"><span data-stu-id="e5cca-179">Alternative: return only the changed properties</span></span>

<span data-ttu-id="e5cca-180">添加可选请求标头中的`prefer:return=minimal`-导致以下行为：</span><span class="sxs-lookup"><span data-stu-id="e5cca-180">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="e5cca-181">如果已更改的属性，在响应中包含的新值。</span><span class="sxs-lookup"><span data-stu-id="e5cca-181">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="e5cca-182">这包括属性被设置为 null 值。</span><span class="sxs-lookup"><span data-stu-id="e5cca-182">This includes properties being set to null value.</span></span>
- <span data-ttu-id="e5cca-183">如果具有未更改的属性，该属性不包括在响应中根本。</span><span class="sxs-lookup"><span data-stu-id="e5cca-183">If the property has not changed, the property is not included in the response at all.</span></span> <span data-ttu-id="e5cca-184">（不同于默认行为。）</span><span class="sxs-lookup"><span data-stu-id="e5cca-184">(Different from the default behavior.)</span></span>

> <span data-ttu-id="e5cca-185">**注意：** 标头可以添加到`deltaLink`任何时间点的增量周期中的请求。</span><span class="sxs-lookup"><span data-stu-id="e5cca-185">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="e5cca-186">头只影响的响应中包括的属性集，而不会影响如何执行增量查询。</span><span class="sxs-lookup"><span data-stu-id="e5cca-186">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span> <span data-ttu-id="e5cca-187">请参阅下面的[第三个示例](#request-3)。</span><span class="sxs-lookup"><span data-stu-id="e5cca-187">See the [third example](#request-3) below.</span></span>

### <a name="example"></a><span data-ttu-id="e5cca-188">示例</span><span class="sxs-lookup"><span data-stu-id="e5cca-188">Example</span></span>

#### <a name="request-1"></a><span data-ttu-id="e5cca-189">请求 1</span><span class="sxs-lookup"><span data-stu-id="e5cca-189">Request 1</span></span>

<span data-ttu-id="e5cca-190">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e5cca-190">The following is an example of the request.</span></span> <span data-ttu-id="e5cca-191">没有任何`$select`参数，以便跟踪和返回一组默认属性。</span><span class="sxs-lookup"><span data-stu-id="e5cca-191">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/groups/delta
```

#### <a name="response-1"></a><span data-ttu-id="e5cca-192">响应 1</span><span class="sxs-lookup"><span data-stu-id="e5cca-192">Response 1</span></span>

<span data-ttu-id="e5cca-193">以下是时使用的响应示例`deltaLink`获取从查询初始化。</span><span class="sxs-lookup"><span data-stu-id="e5cca-193">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span>

><span data-ttu-id="e5cca-194">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e5cca-194">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e5cca-195">所有属性都是从实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e5cca-195">All the properties will be returned from an actual call.</span></span>
>
> <span data-ttu-id="e5cca-196">请注意*members@delta*属性的组中包括的 member 对象的 id 的状态。</span><span class="sxs-lookup"><span data-stu-id="e5cca-196">Note the presence of the *members@delta* property which includes the ids of member objects in the group.</span></span>

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

#### <a name="request-2"></a><span data-ttu-id="e5cca-197">请求 2</span><span class="sxs-lookup"><span data-stu-id="e5cca-197">Request 2</span></span>

<span data-ttu-id="e5cca-198">下面的示例演示选择 3 属性更改跟踪具有默认响应行为的初始请求：</span><span class="sxs-lookup"><span data-stu-id="e5cca-198">The next example shows the initial request selecting 3 properties for change tracking, with default response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description,mailNickname
```

#### <a name="response-2"></a><span data-ttu-id="e5cca-199">响应 2</span><span class="sxs-lookup"><span data-stu-id="e5cca-199">Response 2</span></span>

<span data-ttu-id="e5cca-200">以下是时使用的响应示例`deltaLink`获取从查询初始化。</span><span class="sxs-lookup"><span data-stu-id="e5cca-200">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="e5cca-201">请注意，在响应中包含所有 3 属性并不知道哪些以来已更改`deltaLink`获得。</span><span class="sxs-lookup"><span data-stu-id="e5cca-201">Note that all 3 properties are included in the response and it is not known which ones have changed since the `deltaLink` was obtained.</span></span>

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
      "mailNickname": "mailNickname-value"
    }
  ]
}
```

#### <a name="request-3"></a><span data-ttu-id="e5cca-202">请求 3</span><span class="sxs-lookup"><span data-stu-id="e5cca-202">Request 3</span></span>

<span data-ttu-id="e5cca-203">下面的示例演示选择 3 属性更改跟踪具有最少的替代响应行为的初始请求：</span><span class="sxs-lookup"><span data-stu-id="e5cca-203">The next example shows the initial request selecting 3 properties for change tracking, with alternative minimal response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description,mailNickname
Prefer: return=minimal
```

#### <a name="response-3"></a><span data-ttu-id="e5cca-204">响应 3</span><span class="sxs-lookup"><span data-stu-id="e5cca-204">Response 3</span></span>

<span data-ttu-id="e5cca-205">以下是时使用的响应示例`deltaLink`获取从查询初始化。</span><span class="sxs-lookup"><span data-stu-id="e5cca-205">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="e5cca-206">请注意，`mailNickname`属性不包括在内，这意味着它未更改以来上一次增量查询;`displayName`和`description`是包含已更改其值的方法。</span><span class="sxs-lookup"><span data-stu-id="e5cca-206">Note that the `mailNickname` property is not included, which means it has not changed since the last delta query; `displayName` and `description` are included which means their values have changed.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="e5cca-207">另请参阅</span><span class="sxs-lookup"><span data-stu-id="e5cca-207">See also</span></span>

- <span data-ttu-id="e5cca-208">[使用增量查询来跟踪 Microsoft Graph 数据中的更改](/graph/delta-query-overview)。</span><span class="sxs-lookup"><span data-stu-id="e5cca-208">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>
- <span data-ttu-id="e5cca-209">[获取组的增量更改](/graph/delta-query-groups)。</span><span class="sxs-lookup"><span data-stu-id="e5cca-209">[Get incremental changes for groups](/graph/delta-query-groups).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
