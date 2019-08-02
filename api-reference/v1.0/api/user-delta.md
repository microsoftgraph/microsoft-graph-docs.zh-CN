---
title: 'user: delta'
description: 获得新建、更新或删除的用户，无需对整个用户集合执行完整读取。
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 161f1951883d05e1e39957e30c64eb56ee99931a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027172"
---
# <a name="user-delta"></a><span data-ttu-id="67f70-103">user: delta</span><span class="sxs-lookup"><span data-stu-id="67f70-103">user: delta</span></span>

<span data-ttu-id="67f70-104">获得新建、更新或删除的用户，无需对整个用户集合执行完整读取。</span><span class="sxs-lookup"><span data-stu-id="67f70-104">Get newly created, updated, or deleted users without having to perform a full read of the entire user collection.</span></span> <span data-ttu-id="67f70-105">有关详细信息，请参阅[跟踪更改](/graph/delta-query-overview)。</span><span class="sxs-lookup"><span data-stu-id="67f70-105">See [Track changes](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="67f70-106">权限</span><span class="sxs-lookup"><span data-stu-id="67f70-106">Permissions</span></span>

<span data-ttu-id="67f70-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="67f70-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="67f70-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="67f70-109">Permission type</span></span>      | <span data-ttu-id="67f70-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="67f70-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="67f70-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="67f70-111">Delegated (work or school account)</span></span> | <span data-ttu-id="67f70-112">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="67f70-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="67f70-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="67f70-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67f70-114">User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="67f70-114">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="67f70-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="67f70-115">Application</span></span> | <span data-ttu-id="67f70-116">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67f70-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="67f70-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="67f70-117">HTTP request</span></span>

<span data-ttu-id="67f70-118">为开始跟踪更改，请在用户资源上发出包含 delta 函数的请求。</span><span class="sxs-lookup"><span data-stu-id="67f70-118">To begin tracking changes, you make a request including the delta function on the users resource.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/delta
```

## <a name="query-parameters"></a><span data-ttu-id="67f70-119">查询参数</span><span class="sxs-lookup"><span data-stu-id="67f70-119">Query parameters</span></span>

<span data-ttu-id="67f70-120">跟踪用户更改会引发一组对 **delta** 函数的一次或多次调用。</span><span class="sxs-lookup"><span data-stu-id="67f70-120">Tracking changes in users incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="67f70-121">如果要使用任意查询参数（`$deltatoken` 和 `$skiptoken` 除外），则必须在最初的 **delta** 请求中指定它。</span><span class="sxs-lookup"><span data-stu-id="67f70-121">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="67f70-122">Microsoft Graph 自动将指定的任意参数编码为响应中提供的 `nextLink` 或 `deltaLink` URL 的令牌部分。</span><span class="sxs-lookup"><span data-stu-id="67f70-122">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="67f70-123">只需预先指定所需的任何查询参数一次。</span><span class="sxs-lookup"><span data-stu-id="67f70-123">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="67f70-124">在后续请求中，可以复制并应用之前响应中返回的 `nextLink` 或 `deltaLink` URL，因为此 URL 已包含所需的编码参数。</span><span class="sxs-lookup"><span data-stu-id="67f70-124">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="67f70-125">查询参数</span><span class="sxs-lookup"><span data-stu-id="67f70-125">Query parameter</span></span>      | <span data-ttu-id="67f70-126">类型</span><span class="sxs-lookup"><span data-stu-id="67f70-126">Type</span></span>   |<span data-ttu-id="67f70-127">说明</span><span class="sxs-lookup"><span data-stu-id="67f70-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="67f70-128">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="67f70-128">$deltatoken</span></span> | <span data-ttu-id="67f70-129">string</span><span class="sxs-lookup"><span data-stu-id="67f70-129">string</span></span> | <span data-ttu-id="67f70-p104">对同一个用户集合之前的 **delta** 函数调用的 `deltaLink` URL 中返回的[状态令牌](/graph/delta-query-overview)，指示该组更改跟踪的完成状态。将此令牌包含在对该集合的下一组更改追踪的首次请求中，并保存和应用整个 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="67f70-p104">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same user collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="67f70-132">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="67f70-132">$skiptoken</span></span> | <span data-ttu-id="67f70-133">string</span><span class="sxs-lookup"><span data-stu-id="67f70-133">string</span></span> | <span data-ttu-id="67f70-134">对之前的 **delta** 函数调用的 `nextLink` URL 中返回的[状态令牌](/graph/delta-query-overview)，指示同一个用户集合中有进一步的更改需要追踪。</span><span class="sxs-lookup"><span data-stu-id="67f70-134">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same user collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="67f70-135">OData 查询参数</span><span class="sxs-lookup"><span data-stu-id="67f70-135">OData query parameters</span></span>

<span data-ttu-id="67f70-136">此方法支持可选 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="67f70-136">This method supports optional OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="67f70-p105">像在任何 GET 请求中一样，你可以使用 `$select` 查询参数以仅指定获取最佳性能所需的属性。始终返回 *id* 属性。</span><span class="sxs-lookup"><span data-stu-id="67f70-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The *id* property is always returned.</span></span>
- <span data-ttu-id="67f70-139">提供对 `$filter` 的有限支持：</span><span class="sxs-lookup"><span data-stu-id="67f70-139">There is limited support for `$filter`:</span></span>
  - <span data-ttu-id="67f70-140">唯一支持的 `$filter` 表达式用于跟踪对特定对象 `$filter=id+eq+{value}` 的更改。</span><span class="sxs-lookup"><span data-stu-id="67f70-140">The only supported `$filter` expression is for tracking changes on a specific object: `$filter=id+eq+{value}`.</span></span> <span data-ttu-id="67f70-141">可以筛选多个对象。</span><span class="sxs-lookup"><span data-stu-id="67f70-141">You can filter multiple objects.</span></span> <span data-ttu-id="67f70-142">例如，`https://graph.microsoft.com/v1.0/users/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`。</span><span class="sxs-lookup"><span data-stu-id="67f70-142">For example, `https://graph.microsoft.com/v1.0/users/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span></span> <span data-ttu-id="67f70-143">筛选对象不能超出 50 个。</span><span class="sxs-lookup"><span data-stu-id="67f70-143">There is a limit of 50 filtered objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="67f70-144">请求标头</span><span class="sxs-lookup"><span data-stu-id="67f70-144">Request headers</span></span>
| <span data-ttu-id="67f70-145">名称</span><span class="sxs-lookup"><span data-stu-id="67f70-145">Name</span></span>       | <span data-ttu-id="67f70-146">说明</span><span class="sxs-lookup"><span data-stu-id="67f70-146">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="67f70-147">Authorization</span><span class="sxs-lookup"><span data-stu-id="67f70-147">Authorization</span></span>  | <span data-ttu-id="67f70-148">持有者&lt;令牌&gt;</span><span class="sxs-lookup"><span data-stu-id="67f70-148">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="67f70-149">Content-Type</span><span class="sxs-lookup"><span data-stu-id="67f70-149">Content-Type</span></span>  | <span data-ttu-id="67f70-150">application/json</span><span class="sxs-lookup"><span data-stu-id="67f70-150">application/json</span></span> |
| <span data-ttu-id="67f70-151">Prefer</span><span class="sxs-lookup"><span data-stu-id="67f70-151">Prefer</span></span> | <span data-ttu-id="67f70-152">return=minimal</span><span class="sxs-lookup"><span data-stu-id="67f70-152">return=minimal</span></span> <br><br><span data-ttu-id="67f70-153">在使用 `deltaLink` 的请求中执行此标头将仅返回自上一轮之后发生更改的对象属性。</span><span class="sxs-lookup"><span data-stu-id="67f70-153">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="67f70-154">可选。</span><span class="sxs-lookup"><span data-stu-id="67f70-154">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="67f70-155">请求正文</span><span class="sxs-lookup"><span data-stu-id="67f70-155">Request body</span></span>
<span data-ttu-id="67f70-156">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="67f70-156">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="67f70-157">响应</span><span class="sxs-lookup"><span data-stu-id="67f70-157">Response</span></span>

<span data-ttu-id="67f70-158">如果成功，此方法的响应正文返回`200 OK`响应代码和[用户](../resources/user.md)集合对象。</span><span class="sxs-lookup"><span data-stu-id="67f70-158">If successful, this method returns `200 OK` response code and [user](../resources/user.md) collection object in the response body.</span></span> <span data-ttu-id="67f70-159">该响应还包括 `nextLink`URL 或 `deltaLink`URL。</span><span class="sxs-lookup"><span data-stu-id="67f70-159">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="67f70-160">如果返回 `nextLink`URL：</span><span class="sxs-lookup"><span data-stu-id="67f70-160">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="67f70-161">这表示绘画中存在要检索的其他数据页面。</span><span class="sxs-lookup"><span data-stu-id="67f70-161">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="67f70-162">应用程序继续使用 `nextLink` URL 发出请求，直到响应中包含 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="67f70-162">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="67f70-163">响应包含与初始 Delta 查询请求相同的属性集。</span><span class="sxs-lookup"><span data-stu-id="67f70-163">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="67f70-164">这使你能够在发起 Delta 循环时捕获对象当前的完整状态。</span><span class="sxs-lookup"><span data-stu-id="67f70-164">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="67f70-165">如果返回 `deltaLink`URL：</span><span class="sxs-lookup"><span data-stu-id="67f70-165">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="67f70-166">这表示未返回关于资源现有状态的更多数据。</span><span class="sxs-lookup"><span data-stu-id="67f70-166">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="67f70-167">保存并使用 `deltaLink` URL 来了解下一轮资源更改。</span><span class="sxs-lookup"><span data-stu-id="67f70-167">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="67f70-168">只有对于在签发 `deltaLink` 之后更改的属性，你才可以选择指定 `Prefer:return=minimal` 标头以包含在响应值中。</span><span class="sxs-lookup"><span data-stu-id="67f70-168">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="67f70-169">默认：返回与初始 Delta 请求相同的属性</span><span class="sxs-lookup"><span data-stu-id="67f70-169">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="67f70-170">默认情况下，使用 `deltaLink` 或 `nextLink` 的请求将通过以下方式返回与初始 Delta 查询中选择的相同属性：</span><span class="sxs-lookup"><span data-stu-id="67f70-170">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="67f70-171">如果属性已更改，则新值将包括在响应中。</span><span class="sxs-lookup"><span data-stu-id="67f70-171">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="67f70-172">这包括设为 Null 值的属性。</span><span class="sxs-lookup"><span data-stu-id="67f70-172">This includes properties being set to null value.</span></span>
- <span data-ttu-id="67f70-173">如果属性未更改，则旧值将包括在响应中。</span><span class="sxs-lookup"><span data-stu-id="67f70-173">If the property has not changed, the old value is included in the response.</span></span>
- <span data-ttu-id="67f70-174">如果之前从未设置属性，则它不会包括在响应中。</span><span class="sxs-lookup"><span data-stu-id="67f70-174">If the property has never been set before it will not be included in the response at all.</span></span>


> <span data-ttu-id="67f70-175">**注意：** 如果出现此行为，那么通过查看响应无法区分属性是否已更改。</span><span class="sxs-lookup"><span data-stu-id="67f70-175">**Note:** With this behavior, by looking at the response it is not possible to tell whether a property is changing or not.</span></span> <span data-ttu-id="67f70-176">此外，Delta 响应往往过大，因为它们包含所有属性值，如[示例 2](#example-2-selecting-three-properties) 所示。</span><span class="sxs-lookup"><span data-stu-id="67f70-176">Also, the delta responses tend to be large because they contain all property values  - as shown in the [second example](#example-2-selecting-three-properties) below.</span></span>

### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="67f70-177">备用：仅返回更改的属性</span><span class="sxs-lookup"><span data-stu-id="67f70-177">Alternative: return only the changed properties</span></span>

<span data-ttu-id="67f70-178">添加可选请求标头 - `prefer:return=minimal` - 将导致出现以下行为：</span><span class="sxs-lookup"><span data-stu-id="67f70-178">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="67f70-179">如果属性已更改，则新值将包括在响应中。</span><span class="sxs-lookup"><span data-stu-id="67f70-179">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="67f70-180">这包括设为 Null 值的属性。</span><span class="sxs-lookup"><span data-stu-id="67f70-180">This includes properties being set to null value.</span></span>
- <span data-ttu-id="67f70-181">如果属性未更改，则该属性不会包括在响应中。</span><span class="sxs-lookup"><span data-stu-id="67f70-181">If the property has not changed, the property is not included in the response at all.</span></span> <span data-ttu-id="67f70-182">（不同于默认行为。）</span><span class="sxs-lookup"><span data-stu-id="67f70-182">(Different from the default behavior.)</span></span>

> <span data-ttu-id="67f70-183">**注意：** 可以在 Delta 循环中的任何时间点将标头添加到 `deltaLink` 请求中。</span><span class="sxs-lookup"><span data-stu-id="67f70-183">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="67f70-184">标头仅影响响应中包含的属性集，它不会影响执行 Delta 查询的方式。</span><span class="sxs-lookup"><span data-stu-id="67f70-184">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span> <span data-ttu-id="67f70-185">请参阅[示例 3](#example-3-alternative-minimal-response-behavior)。</span><span class="sxs-lookup"><span data-stu-id="67f70-185">See Example 3.</span></span>

## <a name="examples"></a><span data-ttu-id="67f70-186">示例</span><span class="sxs-lookup"><span data-stu-id="67f70-186">Examples</span></span>

### <a name="example-1-default-properties"></a><span data-ttu-id="67f70-187">示例 1：默认属性</span><span class="sxs-lookup"><span data-stu-id="67f70-187">Example 1: Default properties</span></span>

#### <a name="request"></a><span data-ttu-id="67f70-188">请求</span><span class="sxs-lookup"><span data-stu-id="67f70-188">Request</span></span>

<span data-ttu-id="67f70-189">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="67f70-189">The following is an example of the request.</span></span> <span data-ttu-id="67f70-190">没有 `$select` 参数，因为将跟踪并返回默认的属性集。</span><span class="sxs-lookup"><span data-stu-id="67f70-190">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="67f70-191">HTTP</span><span class="sxs-lookup"><span data-stu-id="67f70-191">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/users/delta
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="67f70-192">C#</span><span class="sxs-lookup"><span data-stu-id="67f70-192">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="67f70-193">Javascript</span><span class="sxs-lookup"><span data-stu-id="67f70-193">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="67f70-194">Objective-C</span><span class="sxs-lookup"><span data-stu-id="67f70-194">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="67f70-195">Java</span><span class="sxs-lookup"><span data-stu-id="67f70-195">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="67f70-196">响应</span><span class="sxs-lookup"><span data-stu-id="67f70-196">Response</span></span>

<span data-ttu-id="67f70-197">以下示例所示为使用从查询初始化获得的 `deltaLink` 时的响应。</span><span class="sxs-lookup"><span data-stu-id="67f70-197">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span>

><span data-ttu-id="67f70-p118">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="67f70-p118">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
### <a name="example-2-selecting-three-properties"></a><span data-ttu-id="67f70-200">示例 2：选择三个属性</span><span class="sxs-lookup"><span data-stu-id="67f70-200">Example 2: Selecting three properties</span></span>

#### <a name="request"></a><span data-ttu-id="67f70-201">请求</span><span class="sxs-lookup"><span data-stu-id="67f70-201">Request</span></span>

<span data-ttu-id="67f70-202">下一个示例所示为通过默认响应行为选择三种更改跟踪属性时的初始请求。</span><span class="sxs-lookup"><span data-stu-id="67f70-202">The next example shows the initial request selecting 3 properties for change tracking, with default response behavior:</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="67f70-203">HTTP</span><span class="sxs-lookup"><span data-stu-id="67f70-203">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_delta_select"
}-->

```http
GET https://graph.microsoft.com/v1.0/users/delta?$select=displayName,jobTitle,mobilePhone
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="67f70-204">C#</span><span class="sxs-lookup"><span data-stu-id="67f70-204">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-delta-select-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="67f70-205">Javascript</span><span class="sxs-lookup"><span data-stu-id="67f70-205">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-delta-select-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="67f70-206">Objective-C</span><span class="sxs-lookup"><span data-stu-id="67f70-206">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-delta-select-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="67f70-207">Java</span><span class="sxs-lookup"><span data-stu-id="67f70-207">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-delta-select-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="67f70-208">响应</span><span class="sxs-lookup"><span data-stu-id="67f70-208">Response</span></span>

<span data-ttu-id="67f70-209">以下示例所示为使用从查询初始化获得的 `deltaLink` 时的响应。</span><span class="sxs-lookup"><span data-stu-id="67f70-209">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="67f70-210">请注意，所有三种属性将包括在响应中，并且无法知道在获得 `deltaLink` 之后哪些属性发生了更改。</span><span class="sxs-lookup"><span data-stu-id="67f70-210">Note that all 3 properties are included in the response and it is not known which ones have changed since the `deltaLink` was obtained.</span></span>

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

### <a name="example-3-alternative-minimal-response-behavior"></a><span data-ttu-id="67f70-211">示例 3：备用最小响应行为</span><span class="sxs-lookup"><span data-stu-id="67f70-211">Example 3: Alternative minimal response behavior</span></span>

#### <a name="request"></a><span data-ttu-id="67f70-212">请求</span><span class="sxs-lookup"><span data-stu-id="67f70-212">Request</span></span>

<span data-ttu-id="67f70-213">下一个示例所示为通过备用最小响应行为选择三种更改跟踪属性时的初始请求。</span><span class="sxs-lookup"><span data-stu-id="67f70-213">The next example shows the initial request selecting 3 properties for change tracking, with alternative minimal response behavior:</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="67f70-214">HTTP</span><span class="sxs-lookup"><span data-stu-id="67f70-214">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_delta_minimal"
}-->

```http
GET https://graph.microsoft.com/v1.0/users/delta?$select=displayName,jobTitle,mobilePhone
Prefer: return=minimal
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="67f70-215">C#</span><span class="sxs-lookup"><span data-stu-id="67f70-215">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-delta-minimal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="67f70-216">Javascript</span><span class="sxs-lookup"><span data-stu-id="67f70-216">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-delta-minimal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="67f70-217">Objective-C</span><span class="sxs-lookup"><span data-stu-id="67f70-217">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-delta-minimal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="67f70-218">Java</span><span class="sxs-lookup"><span data-stu-id="67f70-218">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-delta-minimal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="67f70-219">响应</span><span class="sxs-lookup"><span data-stu-id="67f70-219">Response</span></span>

<span data-ttu-id="67f70-220">以下示例所示为使用从查询初始化获得的 `deltaLink` 时的响应。</span><span class="sxs-lookup"><span data-stu-id="67f70-220">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="67f70-221">请注意，`mobilePhone` 属性不包括在内，这意味着它在上一轮 Delta 查询之后未发生更改；并且 `displayName` 和 `jobTitle` 将包括在内，这意味着其值已发生更改。</span><span class="sxs-lookup"><span data-stu-id="67f70-221">Note that the `mobilePhone` property is not included, which means it has not changed since the last delta query; `displayName` and `jobTitle` are included which means their values have changed.</span></span>

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
## <a name="see-also"></a><span data-ttu-id="67f70-222">另请参阅</span><span class="sxs-lookup"><span data-stu-id="67f70-222">See also</span></span>

- <span data-ttu-id="67f70-223">[使用 Delta 查询跟踪 Microsoft Graph 数据更改](/graph/delta-query-overview)。</span><span class="sxs-lookup"><span data-stu-id="67f70-223">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>
- <span data-ttu-id="67f70-224">[获取用户的增量更改](/graph/delta-query-users)。</span><span class="sxs-lookup"><span data-stu-id="67f70-224">[Get incremental changes for users](/graph/delta-query-users).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
