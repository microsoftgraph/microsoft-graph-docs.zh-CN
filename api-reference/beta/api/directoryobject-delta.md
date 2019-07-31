---
title: 'directoryObject: delta'
description: '在单个增量查询中获取以下类型的新创建、更新或删除的目录对象: 用户、组和组织联系人。 有关详细信息，请参阅“跟踪更改”。'
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d9a02cd054c7cb7c47de27d227bb100303b8ca84
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35951181"
---
# <a name="directoryobject-delta"></a><span data-ttu-id="f65ca-104">directoryObject: delta</span><span class="sxs-lookup"><span data-stu-id="f65ca-104">directoryObject: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f65ca-105">在单个增量查询中获取以下类型的新创建、更新或删除的目录对象:[用户](../resources/user.md)、[组](../resources/group.md)和[组织联系人](../resources/orgcontact.md)。</span><span class="sxs-lookup"><span data-stu-id="f65ca-105">Get newly created, updated, or deleted directory objects of the following types: [user](../resources/user.md), [group](../resources/group.md) and [organizational contact](../resources/orgcontact.md), in a single delta query.</span></span> <span data-ttu-id="f65ca-106">有关详细信息，请参阅[跟踪更改](/graph/delta-query-overview)。</span><span class="sxs-lookup"><span data-stu-id="f65ca-106">See [Track changes](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="f65ca-107">权限</span><span class="sxs-lookup"><span data-stu-id="f65ca-107">Permissions</span></span>

<span data-ttu-id="f65ca-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f65ca-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f65ca-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f65ca-110">Permission type</span></span>      | <span data-ttu-id="f65ca-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f65ca-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f65ca-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f65ca-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f65ca-113">Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f65ca-113">Directory.Read.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="f65ca-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f65ca-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f65ca-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f65ca-115">Not supported.</span></span>  |
|<span data-ttu-id="f65ca-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f65ca-116">Application</span></span> | <span data-ttu-id="f65ca-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f65ca-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f65ca-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f65ca-118">HTTP request</span></span>

<span data-ttu-id="f65ca-119">若要开始跟踪更改, 请在 directoryObjects 资源上发出包含 delta 函数的请求。</span><span class="sxs-lookup"><span data-stu-id="f65ca-119">To begin tracking changes, you make a request including the delta function on the directoryObjects resource.</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /directoryObjects/delta
```

## <a name="query-parameters"></a><span data-ttu-id="f65ca-120">查询参数</span><span class="sxs-lookup"><span data-stu-id="f65ca-120">Query parameters</span></span>

<span data-ttu-id="f65ca-121">跟踪更改会产生一个或多个**delta**函数调用的往返。</span><span class="sxs-lookup"><span data-stu-id="f65ca-121">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="f65ca-122">如果要使用任意查询参数（`$deltatoken` 和 `$skiptoken` 除外），则必须在最初的 **delta** 请求中指定它。</span><span class="sxs-lookup"><span data-stu-id="f65ca-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="f65ca-123">Microsoft Graph 自动将指定的任意参数编码为响应中提供的 `nextLink` 或 `deltaLink` URL 的令牌部分。</span><span class="sxs-lookup"><span data-stu-id="f65ca-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="f65ca-124">只需预先指定所需的任何查询参数一次。</span><span class="sxs-lookup"><span data-stu-id="f65ca-124">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="f65ca-125">在后续请求中，可以复制并应用之前响应中返回的 `nextLink` 或 `deltaLink` URL，因为此 URL 已包含所需的编码参数。</span><span class="sxs-lookup"><span data-stu-id="f65ca-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="f65ca-126">查询参数</span><span class="sxs-lookup"><span data-stu-id="f65ca-126">Query parameter</span></span> | <span data-ttu-id="f65ca-127">类型</span><span class="sxs-lookup"><span data-stu-id="f65ca-127">Type</span></span> |<span data-ttu-id="f65ca-128">说明</span><span class="sxs-lookup"><span data-stu-id="f65ca-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f65ca-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="f65ca-129">$deltatoken</span></span> | <span data-ttu-id="f65ca-130">string</span><span class="sxs-lookup"><span data-stu-id="f65ca-130">string</span></span> | <span data-ttu-id="f65ca-p105">对同一个用户集合之前的 **delta** 函数调用的 `deltaLink` URL 中返回的[状态令牌](/graph/delta-query-overview)，指示该组更改跟踪的完成状态。将此令牌包含在对该集合的下一组更改追踪的首次请求中，并保存和应用整个 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="f65ca-p105">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same user collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="f65ca-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="f65ca-133">$skiptoken</span></span> | <span data-ttu-id="f65ca-134">string</span><span class="sxs-lookup"><span data-stu-id="f65ca-134">string</span></span> | <span data-ttu-id="f65ca-135">对之前的 **delta** 函数调用的 `nextLink` URL 中返回的[状态令牌](/graph/delta-query-overview)，指示同一个用户集合中有进一步的更改需要追踪。</span><span class="sxs-lookup"><span data-stu-id="f65ca-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same user collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="f65ca-136">OData 查询参数</span><span class="sxs-lookup"><span data-stu-id="f65ca-136">OData query parameters</span></span>

<span data-ttu-id="f65ca-137">此方法支持可选 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f65ca-137">This method supports optional OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="f65ca-138">您可以与`$filter`特殊`isOf`运算符一起使用, 以筛选从 directoryObject 派生的类型的子集。</span><span class="sxs-lookup"><span data-stu-id="f65ca-138">You can use `$filter` with the special `isOf` operator to filter a subset of types derived from directoryObject.</span></span>
  - <span data-ttu-id="f65ca-139">您可以将多个表达式与`or`结合使用, 这样您就可以让单个增量查询跟踪多个类型。</span><span class="sxs-lookup"><span data-stu-id="f65ca-139">You can combine multiple expressions using an `or`, which allows you to have a single delta query tracking multiple types.</span></span> <span data-ttu-id="f65ca-140">有关详细信息, 请参阅[第三个示例](#request-3)。</span><span class="sxs-lookup"><span data-stu-id="f65ca-140">See the [third example](#request-3) for details.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f65ca-141">请求标头</span><span class="sxs-lookup"><span data-stu-id="f65ca-141">Request headers</span></span>

| <span data-ttu-id="f65ca-142">名称</span><span class="sxs-lookup"><span data-stu-id="f65ca-142">Name</span></span>       | <span data-ttu-id="f65ca-143">说明</span><span class="sxs-lookup"><span data-stu-id="f65ca-143">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f65ca-144">Authorization</span><span class="sxs-lookup"><span data-stu-id="f65ca-144">Authorization</span></span>  | <span data-ttu-id="f65ca-145">持有者&lt;令牌&gt;</span><span class="sxs-lookup"><span data-stu-id="f65ca-145">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="f65ca-146">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f65ca-146">Content-Type</span></span>  | <span data-ttu-id="f65ca-147">application/json</span><span class="sxs-lookup"><span data-stu-id="f65ca-147">application/json</span></span> |
| <span data-ttu-id="f65ca-148">Prefer</span><span class="sxs-lookup"><span data-stu-id="f65ca-148">Prefer</span></span> | <span data-ttu-id="f65ca-149">return=minimal</span><span class="sxs-lookup"><span data-stu-id="f65ca-149">return=minimal</span></span> <br><br><span data-ttu-id="f65ca-150">在使用 `deltaLink` 的请求中执行此标头将仅返回自上一轮之后发生更改的对象属性。</span><span class="sxs-lookup"><span data-stu-id="f65ca-150">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="f65ca-151">可选。</span><span class="sxs-lookup"><span data-stu-id="f65ca-151">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f65ca-152">请求正文</span><span class="sxs-lookup"><span data-stu-id="f65ca-152">Request body</span></span>

<span data-ttu-id="f65ca-153">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f65ca-153">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="f65ca-154">响应</span><span class="sxs-lookup"><span data-stu-id="f65ca-154">Response</span></span>

<span data-ttu-id="f65ca-155">如果成功，此方法的响应正文返回`200 OK`响应代码和[用户](../resources/directoryobject.md)集合对象。</span><span class="sxs-lookup"><span data-stu-id="f65ca-155">If successful, this method returns `200 OK` response code and [user](../resources/directoryobject.md) collection object in the response body.</span></span> <span data-ttu-id="f65ca-156">该响应还包括 `nextLink`URL 或 `deltaLink`URL。</span><span class="sxs-lookup"><span data-stu-id="f65ca-156">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="f65ca-157">如果返回 `nextLink`URL：</span><span class="sxs-lookup"><span data-stu-id="f65ca-157">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="f65ca-158">这表示绘画中存在要检索的其他数据页面。</span><span class="sxs-lookup"><span data-stu-id="f65ca-158">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="f65ca-159">应用程序继续使用 `nextLink` URL 发出请求，直到响应中包含 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="f65ca-159">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="f65ca-160">响应包含与初始 Delta 查询请求相同的属性集。</span><span class="sxs-lookup"><span data-stu-id="f65ca-160">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="f65ca-161">这使你能够在发起 Delta 循环时捕获对象当前的完整状态。</span><span class="sxs-lookup"><span data-stu-id="f65ca-161">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="f65ca-162">如果返回 `deltaLink`URL：</span><span class="sxs-lookup"><span data-stu-id="f65ca-162">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="f65ca-163">这表示未返回关于资源现有状态的更多数据。</span><span class="sxs-lookup"><span data-stu-id="f65ca-163">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="f65ca-164">保存并使用 `deltaLink` URL 来了解下一轮资源更改。</span><span class="sxs-lookup"><span data-stu-id="f65ca-164">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="f65ca-165">只有对于在签发 `deltaLink` 之后更改的属性，你才可以选择指定 `Prefer:return=minimal` 标头以包含在响应值中。</span><span class="sxs-lookup"><span data-stu-id="f65ca-165">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="f65ca-166">默认：返回与初始 Delta 请求相同的属性</span><span class="sxs-lookup"><span data-stu-id="f65ca-166">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="f65ca-167">默认情况下，使用 `deltaLink` 或 `nextLink` 的请求将通过以下方式返回与初始 Delta 查询中选择的相同属性：</span><span class="sxs-lookup"><span data-stu-id="f65ca-167">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="f65ca-168">如果属性已更改，则新值将包括在响应中。</span><span class="sxs-lookup"><span data-stu-id="f65ca-168">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="f65ca-169">这包括设为 Null 值的属性。</span><span class="sxs-lookup"><span data-stu-id="f65ca-169">This includes properties being set to null value.</span></span>
- <span data-ttu-id="f65ca-170">如果属性未更改，则旧值将包括在响应中。</span><span class="sxs-lookup"><span data-stu-id="f65ca-170">If the property has not changed, the old value is included in the response.</span></span>
- <span data-ttu-id="f65ca-171">如果之前从未设置属性，则它不会包括在响应中。</span><span class="sxs-lookup"><span data-stu-id="f65ca-171">If the property has never been set before it will not be included in the response at all.</span></span>


> <span data-ttu-id="f65ca-172">**注意：** 如果出现此行为，那么通过查看响应无法区分属性是否已更改。</span><span class="sxs-lookup"><span data-stu-id="f65ca-172">**Note:** With this behavior, by looking at the response it is not possible to tell whether a property is changing or not.</span></span> <span data-ttu-id="f65ca-173">此外, 增量响应往往很大, 因为它们包含所有属性值。</span><span class="sxs-lookup"><span data-stu-id="f65ca-173">Also, the delta responses tend to be large because they contain all property values.</span></span>

#### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="f65ca-174">备用：仅返回更改的属性</span><span class="sxs-lookup"><span data-stu-id="f65ca-174">Alternative: return only the changed properties</span></span>

<span data-ttu-id="f65ca-175">添加可选请求标头 - `prefer:return=minimal` - 将导致出现以下行为：</span><span class="sxs-lookup"><span data-stu-id="f65ca-175">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="f65ca-176">如果属性已更改，则新值将包括在响应中。</span><span class="sxs-lookup"><span data-stu-id="f65ca-176">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="f65ca-177">这包括设为 Null 值的属性。</span><span class="sxs-lookup"><span data-stu-id="f65ca-177">This includes properties being set to null value.</span></span>
- <span data-ttu-id="f65ca-178">如果属性未更改，则该属性不会包括在响应中。</span><span class="sxs-lookup"><span data-stu-id="f65ca-178">If the property has not changed, the property is not included in the response at all.</span></span> <span data-ttu-id="f65ca-179">（不同于默认行为。）</span><span class="sxs-lookup"><span data-stu-id="f65ca-179">(Different from the default behavior.)</span></span>

> <span data-ttu-id="f65ca-180">**注意：** 可以在 Delta 循环中的任何时间点将标头添加到 `deltaLink` 请求中。</span><span class="sxs-lookup"><span data-stu-id="f65ca-180">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="f65ca-181">标头仅影响响应中包含的属性集，它不会影响执行 Delta 查询的方式。</span><span class="sxs-lookup"><span data-stu-id="f65ca-181">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span>

## <a name="example"></a><span data-ttu-id="f65ca-182">示例</span><span class="sxs-lookup"><span data-stu-id="f65ca-182">Example</span></span>

### <a name="request-1"></a><span data-ttu-id="f65ca-183">请求 1</span><span class="sxs-lookup"><span data-stu-id="f65ca-183">Request 1</span></span>

<span data-ttu-id="f65ca-184">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f65ca-184">The following is an example of the request.</span></span> <span data-ttu-id="f65ca-185">没有 `$select` 参数，因为将跟踪并返回默认的属性集。</span><span class="sxs-lookup"><span data-stu-id="f65ca-185">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f65ca-186">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="f65ca-186">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directory_object_delta"
}-->

```http
GET https://graph.microsoft.com/beta/directoryObjects/delta
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f65ca-187">C#</span><span class="sxs-lookup"><span data-stu-id="f65ca-187">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directory-object-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f65ca-188">Javascript</span><span class="sxs-lookup"><span data-stu-id="f65ca-188">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directory-object-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f65ca-189">目标-C</span><span class="sxs-lookup"><span data-stu-id="f65ca-189">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directory-object-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f65ca-190">Java</span><span class="sxs-lookup"><span data-stu-id="f65ca-190">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directory-object-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-1"></a><span data-ttu-id="f65ca-191">响应 1</span><span class="sxs-lookup"><span data-stu-id="f65ca-191">Response 1</span></span>

<span data-ttu-id="f65ca-192">以下示例所示为使用从查询初始化获得的 `deltaLink` 时的响应。</span><span class="sxs-lookup"><span data-stu-id="f65ca-192">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="f65ca-193">未`isOf`使用任何筛选器, 因此将返回从 directoryObject 派生的所有类型。</span><span class="sxs-lookup"><span data-stu-id="f65ca-193">No `isOf` filter has been used, so all types derived from directoryObject are returned.</span></span>

><span data-ttu-id="f65ca-194">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f65ca-194">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f65ca-195">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f65ca-195">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects",
  "@odata.nextLink":"https://graph.microsoft.com/beta/directoryObjects/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "01754bb5-89de-4003-be72-9106a9fb16f2",
      "deletedDateTime": null,
      "accountEnabled": true,
      "ageGroup": null,
      "city": null,
      "companyName": null,
      "consentProvidedForMinor": null,
      "country": null,
      "createdDateTime": null,
      "department": null,
      "displayName": "John Smith",
      "givenName": null,
      "jobTitle": null
    },
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "cf33844a-b6f8-4d4d-84f4-54e8d45094f0",
      "deletedDateTime": null,
      "classification": null,
      "createdDateTime": "2018-06-20T16:50:09Z",
      "description": null,
      "displayName": "testgp"
    },
    {
      "@odata.type": "#microsoft.graph.orgContact",
      "id": "8f301319-4b4e-493f-8067-bce1dec76e7a",
      "businessPhones": ["string"],
      "city": "string",
      "companyName": "string",
      "country": "string",
      "department": "string",
      "displayName": "string",
      "givenName": "string",      
      "jobTitle": "string"
    }
  ]
}
```

### <a name="request-2"></a><span data-ttu-id="f65ca-196">请求 2</span><span class="sxs-lookup"><span data-stu-id="f65ca-196">Request 2</span></span>

<span data-ttu-id="f65ca-197">下面的示例展示了如何使用替代的最小响应行为:</span><span class="sxs-lookup"><span data-stu-id="f65ca-197">The next example shows the use of the alternative minimal response behavior:</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f65ca-198">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="f65ca-198">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryObject_delta"
}-->

```http
GET https://graph.microsoft.com/beta/directoryObjects/delta
Prefer: return=minimal
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f65ca-199">C#</span><span class="sxs-lookup"><span data-stu-id="f65ca-199">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f65ca-200">Javascript</span><span class="sxs-lookup"><span data-stu-id="f65ca-200">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f65ca-201">目标-C</span><span class="sxs-lookup"><span data-stu-id="f65ca-201">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f65ca-202">Java</span><span class="sxs-lookup"><span data-stu-id="f65ca-202">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-2"></a><span data-ttu-id="f65ca-203">响应 2</span><span class="sxs-lookup"><span data-stu-id="f65ca-203">Response 2</span></span>

<span data-ttu-id="f65ca-204">以下示例所示为使用从查询初始化获得的 `deltaLink` 时的响应。</span><span class="sxs-lookup"><span data-stu-id="f65ca-204">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="f65ca-205">注释仅返回实际已更改的属性。</span><span class="sxs-lookup"><span data-stu-id="f65ca-205">Note only the properties that have actually changed are returned.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects",
  "@odata.nextLink":"https://graph.microsoft.com/beta/directoryObjects/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "01754bb5-89de-4003-be72-9106a9fb16f2",
      "displayName": "John Smith"
    },
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "cf33844a-b6f8-4d4d-84f4-54e8d45094f0",
      "description": null,
      "displayName": "testgp"
    },
    {
      "@odata.type": "#microsoft.graph.orgContact",
      "id": "8f301319-4b4e-493f-8067-bce1dec76e7a",
      "businessPhones": "12345"
    }
  ]
}
```

### <a name="request-3"></a><span data-ttu-id="f65ca-206">请求 3</span><span class="sxs-lookup"><span data-stu-id="f65ca-206">Request 3</span></span>

<span data-ttu-id="f65ca-207">下一个示例显示使用`isOf`运算符筛选出仅用户和组实体的初始请求:</span><span class="sxs-lookup"><span data-stu-id="f65ca-207">The next example shows the initial request using the `isOf` operator to filter out only user and group entities:</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f65ca-208">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="f65ca-208">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_delta"
}-->

```http
GET https://graph.microsoft.com/beta/directoryObjects/delta?$filter=isOf('Microsoft.Graph.User')+or+isOf('Microsoft.Graph.Group')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f65ca-209">C#</span><span class="sxs-lookup"><span data-stu-id="f65ca-209">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f65ca-210">Javascript</span><span class="sxs-lookup"><span data-stu-id="f65ca-210">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f65ca-211">目标-C</span><span class="sxs-lookup"><span data-stu-id="f65ca-211">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f65ca-212">Java</span><span class="sxs-lookup"><span data-stu-id="f65ca-212">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-3"></a><span data-ttu-id="f65ca-213">响应 3</span><span class="sxs-lookup"><span data-stu-id="f65ca-213">Response 3</span></span>

<span data-ttu-id="f65ca-214">以下示例所示为使用从查询初始化获得的 `deltaLink` 时的响应。</span><span class="sxs-lookup"><span data-stu-id="f65ca-214">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="f65ca-215">请注意, 仅返回 user 和 group 对象:</span><span class="sxs-lookup"><span data-stu-id="f65ca-215">Note that only user and group objects are returned:</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects",
  "@odata.nextLink":"https://graph.microsoft.com/beta/directoryObjects/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "01754bb5-89de-4003-be72-9106a9fb16f2",
      "deletedDateTime": null,
      "accountEnabled": true,
      "ageGroup": null,
      "city": null,
      "companyName": null,
      "consentProvidedForMinor": null,
      "country": null,
      "createdDateTime": null,
      "department": null,
      "displayName": "John Smith",
      "givenName": null,
      "jobTitle": null
    },
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "cf33844a-b6f8-4d4d-84f4-54e8d45094f0",
      "deletedDateTime": null,
      "classification": null,
      "createdDateTime": "2018-06-20T16:50:09Z",
      "description": null,
      "displayName": "testgp"
    }
  ]
}
```

- <span data-ttu-id="f65ca-216">[使用 Delta 查询跟踪 Microsoft Graph 数据更改](/graph/delta-query-overview)。</span><span class="sxs-lookup"><span data-stu-id="f65ca-216">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>
- <span data-ttu-id="f65ca-217">[获取用户的增量更改](/graph/delta-query-users)。</span><span class="sxs-lookup"><span data-stu-id="f65ca-217">[Get incremental changes for users](/graph/delta-query-users).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
