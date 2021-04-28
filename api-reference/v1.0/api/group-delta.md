---
title: 'group: delta'
description: 获取新创建、更新或删除的组，包括组成员身份更改，而无需执行整个组集合的完整读取。
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: e094aaae32d8fe4ccbadd534b3d75ece56f8176e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050484"
---
# <a name="group-delta"></a><span data-ttu-id="a735f-103">group: delta</span><span class="sxs-lookup"><span data-stu-id="a735f-103">group: delta</span></span>

<span data-ttu-id="a735f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a735f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a735f-105">获取新创建、更新或删除的组，包括组成员身份更改，而无需执行整个组集合的完整读取。</span><span class="sxs-lookup"><span data-stu-id="a735f-105">Get newly created, updated, or deleted groups, including group membership changes, without having to perform a full read of the entire group collection.</span></span> <span data-ttu-id="a735f-106">有关详细信息 [，请参阅使用增量](/graph/delta-query-overview) 查询。</span><span class="sxs-lookup"><span data-stu-id="a735f-106">See [Using Delta Query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="a735f-107">权限</span><span class="sxs-lookup"><span data-stu-id="a735f-107">Permissions</span></span>

<span data-ttu-id="a735f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a735f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a735f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a735f-110">Permission type</span></span>      | <span data-ttu-id="a735f-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a735f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a735f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a735f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a735f-113">GroupMember.Read.All、Group.Read.All、Directory.Read.All、Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a735f-113">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="a735f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a735f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a735f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a735f-115">Not supported.</span></span>    |
|<span data-ttu-id="a735f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a735f-116">Application</span></span> | <span data-ttu-id="a735f-117">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a735f-117">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a735f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a735f-118">HTTP request</span></span>

<span data-ttu-id="a735f-119">为开始跟踪更改，请在组资源上发出包含 delta 函数的请求。</span><span class="sxs-lookup"><span data-stu-id="a735f-119">To begin tracking changes, you make a request including the delta function on the groups resource.</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/delta
```

## <a name="query-parameters"></a><span data-ttu-id="a735f-120">查询参数</span><span class="sxs-lookup"><span data-stu-id="a735f-120">Query parameters</span></span>

<span data-ttu-id="a735f-p103">跟踪组中的更改会触发一个或多个 **delta** 函数调用。如果使用任何查询参数（而不是 `$deltatoken` 和 `$skiptoken`），必须在初始 **delta** 请求中指定它。Microsoft Graph 会自动将任何指定参数编码为响应中返回的 `nextLink` 或 `deltaLink` URL 的令牌部分。</span><span class="sxs-lookup"><span data-stu-id="a735f-p103">Tracking changes in groups incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="a735f-124">只需预先指定所需的任何查询参数一次。</span><span class="sxs-lookup"><span data-stu-id="a735f-124">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="a735f-125">在后续请求中，可以复制并应用之前响应中返回的 `nextLink` 或 `deltaLink` URL，因为此 URL 已包含所需的编码参数。</span><span class="sxs-lookup"><span data-stu-id="a735f-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="a735f-126">查询参数</span><span class="sxs-lookup"><span data-stu-id="a735f-126">Query parameter</span></span> | <span data-ttu-id="a735f-127">类型</span><span class="sxs-lookup"><span data-stu-id="a735f-127">Type</span></span>  |<span data-ttu-id="a735f-128">说明</span><span class="sxs-lookup"><span data-stu-id="a735f-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a735f-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="a735f-129">$deltatoken</span></span> | <span data-ttu-id="a735f-130">string</span><span class="sxs-lookup"><span data-stu-id="a735f-130">string</span></span> | <span data-ttu-id="a735f-p104">对同一个组集合之前的 **delta** 函数调用的 `deltaLink` URL 中返回的 [状态令牌](/graph/delta-query-overview)，指示该组更改跟踪的完成状态。将此令牌包含在对该集合的下一组更改追踪的首次请求中，并保存和应用整个 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="a735f-p104">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same group collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="a735f-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="a735f-133">$skiptoken</span></span> | <span data-ttu-id="a735f-134">string</span><span class="sxs-lookup"><span data-stu-id="a735f-134">string</span></span> | <span data-ttu-id="a735f-135">对之前的 **delta** 函数调用的 `nextLink` URL 中返回的 [状态令牌](/graph/delta-query-overview)，指示同一个组集合中有进一步的更改需要追踪。</span><span class="sxs-lookup"><span data-stu-id="a735f-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same group collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="a735f-136">OData 查询参数</span><span class="sxs-lookup"><span data-stu-id="a735f-136">OData query parameters</span></span>

<span data-ttu-id="a735f-137">此方法支持可选的 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a735f-137">This method supports optional OData query parameters to help customize the response.</span></span>

- <span data-ttu-id="a735f-p105">像在任何 GET 请求中一样，你可以使用 `$select` 查询参数以仅指定获取最佳性能所需的属性。始终返回 *id* 属性。</span><span class="sxs-lookup"><span data-stu-id="a735f-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The *id* property is always returned.</span></span>
- <span data-ttu-id="a735f-140">可以使用 获取 `$select=members` 成员身份更改。</span><span class="sxs-lookup"><span data-stu-id="a735f-140">You can use `$select=members` to get membership changes.</span></span> <span data-ttu-id="a735f-141">您还可以通过选择 **directoryObject** 集合类型的任何 [](../resources/group.md#relationships)组关系来跟踪其他更改（如所有权等）。</span><span class="sxs-lookup"><span data-stu-id="a735f-141">You can additionally track other changes like ownership and more by selecting any [group relationship](../resources/group.md#relationships) of type **directoryObject collection**.</span></span>
- <span data-ttu-id="a735f-142">提供对 `$filter` 的有限支持：</span><span class="sxs-lookup"><span data-stu-id="a735f-142">There is limited support for `$filter`:</span></span>
  - <span data-ttu-id="a735f-143">唯一支持的 `$filter` 表达式用于跟踪对特定对象 `$filter=id+eq+{value}` 的更改。</span><span class="sxs-lookup"><span data-stu-id="a735f-143">The only supported `$filter` expression is for tracking changes on a specific object: `$filter=id+eq+{value}`.</span></span> <span data-ttu-id="a735f-144">可以筛选多个对象。</span><span class="sxs-lookup"><span data-stu-id="a735f-144">You can filter multiple objects.</span></span> <span data-ttu-id="a735f-145">例如，`https://graph.microsoft.com/v1.0/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`。</span><span class="sxs-lookup"><span data-stu-id="a735f-145">For example, `https://graph.microsoft.com/v1.0/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span></span> <span data-ttu-id="a735f-146">筛选对象不能超出 50 个。</span><span class="sxs-lookup"><span data-stu-id="a735f-146">There is a limit of 50 filtered objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a735f-147">请求标头</span><span class="sxs-lookup"><span data-stu-id="a735f-147">Request headers</span></span>

| <span data-ttu-id="a735f-148">名称</span><span class="sxs-lookup"><span data-stu-id="a735f-148">Name</span></span>       | <span data-ttu-id="a735f-149">说明</span><span class="sxs-lookup"><span data-stu-id="a735f-149">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a735f-150">Authorization</span><span class="sxs-lookup"><span data-stu-id="a735f-150">Authorization</span></span>  | <span data-ttu-id="a735f-151">持有者&lt;令牌&gt;</span><span class="sxs-lookup"><span data-stu-id="a735f-151">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="a735f-152">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a735f-152">Content-Type</span></span>  | <span data-ttu-id="a735f-153">application/json</span><span class="sxs-lookup"><span data-stu-id="a735f-153">application/json</span></span> |
| <span data-ttu-id="a735f-154">Prefer</span><span class="sxs-lookup"><span data-stu-id="a735f-154">Prefer</span></span> | <span data-ttu-id="a735f-155">return=minimal</span><span class="sxs-lookup"><span data-stu-id="a735f-155">return=minimal</span></span> <br><br><span data-ttu-id="a735f-156">在使用 `deltaLink` 的请求中执行此标头将仅返回自上一轮之后发生更改的对象属性。</span><span class="sxs-lookup"><span data-stu-id="a735f-156">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="a735f-157">可选。</span><span class="sxs-lookup"><span data-stu-id="a735f-157">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a735f-158">请求正文</span><span class="sxs-lookup"><span data-stu-id="a735f-158">Request body</span></span>

<span data-ttu-id="a735f-159">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a735f-159">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="a735f-160">响应</span><span class="sxs-lookup"><span data-stu-id="a735f-160">Response</span></span>

<span data-ttu-id="a735f-161">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和[组](../resources/group.md)集合对象。</span><span class="sxs-lookup"><span data-stu-id="a735f-161">If successful, this method returns `200 OK` response code and [group](../resources/group.md) collection object in the response body.</span></span> <span data-ttu-id="a735f-162">该响应还包括一个状态令牌，即 `nextLink` URL 或 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="a735f-162">The response also includes a state token which is either a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="a735f-163">如果返回 `nextLink`URL：</span><span class="sxs-lookup"><span data-stu-id="a735f-163">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="a735f-164">这表示绘画中存在要检索的其他数据页面。</span><span class="sxs-lookup"><span data-stu-id="a735f-164">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="a735f-165">应用程序继续使用 `nextLink` URL 发出请求，直到响应中包含 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="a735f-165">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="a735f-166">响应包含与初始 Delta 查询请求相同的属性集。</span><span class="sxs-lookup"><span data-stu-id="a735f-166">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="a735f-167">这使你能够在发起 Delta 循环时捕获对象当前的完整状态。</span><span class="sxs-lookup"><span data-stu-id="a735f-167">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="a735f-168">如果返回 `deltaLink`URL：</span><span class="sxs-lookup"><span data-stu-id="a735f-168">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="a735f-169">这表示未返回关于资源现有状态的更多数据。</span><span class="sxs-lookup"><span data-stu-id="a735f-169">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="a735f-170">保存并使用 `deltaLink` URL 来了解下一轮资源更改。</span><span class="sxs-lookup"><span data-stu-id="a735f-170">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="a735f-171">只有对于在签发 `deltaLink` 之后更改的属性，你才可以选择指定 `Prefer:return=minimal` 标头以包含在响应值中。</span><span class="sxs-lookup"><span data-stu-id="a735f-171">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="a735f-172">默认：返回与初始 Delta 请求相同的属性</span><span class="sxs-lookup"><span data-stu-id="a735f-172">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="a735f-173">默认情况下，使用 `deltaLink` 或 `nextLink` 的请求将通过以下方式返回与初始 Delta 查询中选择的相同属性：</span><span class="sxs-lookup"><span data-stu-id="a735f-173">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="a735f-174">如果属性已更改，则新值将包括在响应中。</span><span class="sxs-lookup"><span data-stu-id="a735f-174">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="a735f-175">这包括设为 Null 值的属性。</span><span class="sxs-lookup"><span data-stu-id="a735f-175">This includes properties being set to null value.</span></span>
- <span data-ttu-id="a735f-176">如果属性未更改，则旧值将包括在响应中。</span><span class="sxs-lookup"><span data-stu-id="a735f-176">If the property has not changed, the old value is included in the response.</span></span>
- <span data-ttu-id="a735f-177">如果之前从未设置属性，则它不会包括在响应中。</span><span class="sxs-lookup"><span data-stu-id="a735f-177">If the property has never been set before it will not be included in the response at all.</span></span>


> <span data-ttu-id="a735f-178">**注意：** 如果出现此行为，那么通过查看响应无法区分属性是否已更改。</span><span class="sxs-lookup"><span data-stu-id="a735f-178">**Note:** With this behavior, by looking at the response it is not possible to tell whether a property is changing or not.</span></span> <span data-ttu-id="a735f-179">此外，Delta 响应往往过大，因为它们包含所有属性值，如下面的[第二个示例](#request-2)所示。</span><span class="sxs-lookup"><span data-stu-id="a735f-179">Also, the delta responses tend to be large because they contain all property values  - as shown in the [second example](#request-2) below.</span></span>

#### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="a735f-180">备用：仅返回更改的属性</span><span class="sxs-lookup"><span data-stu-id="a735f-180">Alternative: return only the changed properties</span></span>

<span data-ttu-id="a735f-181">添加可选请求标头 - `prefer:return=minimal` - 将导致出现以下行为：</span><span class="sxs-lookup"><span data-stu-id="a735f-181">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="a735f-182">如果属性已更改，则新值将包括在响应中。</span><span class="sxs-lookup"><span data-stu-id="a735f-182">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="a735f-183">这包括设为 Null 值的属性。</span><span class="sxs-lookup"><span data-stu-id="a735f-183">This includes properties being set to null value.</span></span>
- <span data-ttu-id="a735f-184">如果属性未更改，则该属性不会包括在响应中。</span><span class="sxs-lookup"><span data-stu-id="a735f-184">If the property has not changed, the property is not included in the response at all.</span></span> <span data-ttu-id="a735f-185">（不同于默认行为。）</span><span class="sxs-lookup"><span data-stu-id="a735f-185">(Different from the default behavior.)</span></span>

> <span data-ttu-id="a735f-186">**注意：** 可以在 Delta 循环中的任何时间点将标头添加到 `deltaLink` 请求中。</span><span class="sxs-lookup"><span data-stu-id="a735f-186">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="a735f-187">标头仅影响响应中包含的属性集，它不会影响执行 Delta 查询的方式。</span><span class="sxs-lookup"><span data-stu-id="a735f-187">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span> <span data-ttu-id="a735f-188">请参阅下面的[第三个示例](#request-3)。</span><span class="sxs-lookup"><span data-stu-id="a735f-188">See the [third example](#request-3) below.</span></span>

### <a name="example"></a><span data-ttu-id="a735f-189">示例</span><span class="sxs-lookup"><span data-stu-id="a735f-189">Example</span></span>

#### <a name="request-1"></a><span data-ttu-id="a735f-190">请求 1</span><span class="sxs-lookup"><span data-stu-id="a735f-190">Request 1</span></span>

<span data-ttu-id="a735f-191">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a735f-191">The following is an example of the request.</span></span> <span data-ttu-id="a735f-192">没有 `$select` 参数，因为将跟踪并返回默认的属性集。</span><span class="sxs-lookup"><span data-stu-id="a735f-192">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>

# <a name="http"></a>[<span data-ttu-id="a735f-193">HTTP</span><span class="sxs-lookup"><span data-stu-id="a735f-193">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/delta
```
# <a name="c"></a>[<span data-ttu-id="a735f-194">C#</span><span class="sxs-lookup"><span data-stu-id="a735f-194">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a735f-195">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a735f-195">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a735f-196">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a735f-196">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a735f-197">Java</span><span class="sxs-lookup"><span data-stu-id="a735f-197">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response-1"></a><span data-ttu-id="a735f-198">响应 1</span><span class="sxs-lookup"><span data-stu-id="a735f-198">Response 1</span></span>

<span data-ttu-id="a735f-199">以下示例所示为使用从查询初始化获得的 `deltaLink` 时的响应。</span><span class="sxs-lookup"><span data-stu-id="a735f-199">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span>

><span data-ttu-id="a735f-200">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a735f-200">**Note:** The response object shown here might be shortened for readability.</span></span>
>
> <span data-ttu-id="a735f-201">请注意存在包含 *members@delta* 成员对象的 ID 的 members@delta 属性。</span><span class="sxs-lookup"><span data-stu-id="a735f-201">Note the presence of the *members@delta* property which includes the ids of member objects in the group.</span></span>

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

#### <a name="request-2"></a><span data-ttu-id="a735f-202">请求 2</span><span class="sxs-lookup"><span data-stu-id="a735f-202">Request 2</span></span>

<span data-ttu-id="a735f-203">下一个示例所示为通过默认响应行为选择 3 种更改跟踪属性时的初始请求：</span><span class="sxs-lookup"><span data-stu-id="a735f-203">The next example shows the initial request selecting 3 properties for change tracking, with default response behavior:</span></span>

# <a name="http"></a>[<span data-ttu-id="a735f-204">HTTP</span><span class="sxs-lookup"><span data-stu-id="a735f-204">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_delta_with_select"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description,mailNickname
```
# <a name="c"></a>[<span data-ttu-id="a735f-205">C#</span><span class="sxs-lookup"><span data-stu-id="a735f-205">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-delta-with-select-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a735f-206">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a735f-206">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-delta-with-select-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a735f-207">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a735f-207">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-delta-with-select-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a735f-208">Java</span><span class="sxs-lookup"><span data-stu-id="a735f-208">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-delta-with-select-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response-2"></a><span data-ttu-id="a735f-209">响应 2</span><span class="sxs-lookup"><span data-stu-id="a735f-209">Response 2</span></span>

<span data-ttu-id="a735f-210">以下示例所示为使用从查询初始化获得的 `deltaLink` 时的响应。</span><span class="sxs-lookup"><span data-stu-id="a735f-210">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="a735f-211">请注意，所有 3 种属性将包括在响应中，并且无法知道在获得 `deltaLink` 之后发生更改的属性。</span><span class="sxs-lookup"><span data-stu-id="a735f-211">Note that all 3 properties are included in the response and it is not known which ones have changed since the `deltaLink` was obtained.</span></span>

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

#### <a name="request-3"></a><span data-ttu-id="a735f-212">请求 3</span><span class="sxs-lookup"><span data-stu-id="a735f-212">Request 3</span></span>

<span data-ttu-id="a735f-213">下一个示例所示为通过备用最小响应行为选择 3 种更改跟踪属性时的初始请求：</span><span class="sxs-lookup"><span data-stu-id="a735f-213">The next example shows the initial request selecting 3 properties for change tracking, with alternative minimal response behavior:</span></span>

# <a name="http"></a>[<span data-ttu-id="a735f-214">HTTP</span><span class="sxs-lookup"><span data-stu-id="a735f-214">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_delta_minimal"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description,mailNickname
Prefer: return=minimal
```
# <a name="c"></a>[<span data-ttu-id="a735f-215">C#</span><span class="sxs-lookup"><span data-stu-id="a735f-215">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-delta-minimal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a735f-216">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a735f-216">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-delta-minimal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a735f-217">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a735f-217">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-delta-minimal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a735f-218">Java</span><span class="sxs-lookup"><span data-stu-id="a735f-218">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-delta-minimal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response-3"></a><span data-ttu-id="a735f-219">响应 3</span><span class="sxs-lookup"><span data-stu-id="a735f-219">Response 3</span></span>

<span data-ttu-id="a735f-220">以下示例所示为使用从查询初始化获得的 `deltaLink` 时的响应。</span><span class="sxs-lookup"><span data-stu-id="a735f-220">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="a735f-221">请注意，`mailNickname` 属性不包括在内，这意味着它在上一轮 Delta 查询之后未发生更改；并且 `displayName` 和 `description` 将包括在内，这意味着其值已发生更改。</span><span class="sxs-lookup"><span data-stu-id="a735f-221">Note that the `mailNickname` property is not included, which means it has not changed since the last delta query; `displayName` and `description` are included which means their values have changed.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="a735f-222">另请参阅</span><span class="sxs-lookup"><span data-stu-id="a735f-222">See also</span></span>

- <span data-ttu-id="a735f-223">[使用 Delta 查询跟踪 Microsoft Graph 数据更改](/graph/delta-query-overview)。</span><span class="sxs-lookup"><span data-stu-id="a735f-223">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>
- <span data-ttu-id="a735f-224">[获取组的增量更改](/graph/delta-query-groups)。</span><span class="sxs-lookup"><span data-stu-id="a735f-224">[Get incremental changes for groups](/graph/delta-query-groups).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

