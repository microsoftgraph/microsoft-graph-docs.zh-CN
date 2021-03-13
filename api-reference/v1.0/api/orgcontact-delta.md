---
title: orgContact： delta
description: 获取新建、更新或删除的组织联系人，而无需执行整个集合的完全读取。
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: c941e1704d41159050ee573ebb1acc8e9eed432b
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761351"
---
# <a name="orgcontact-delta"></a><span data-ttu-id="66d32-103">orgContact： delta</span><span class="sxs-lookup"><span data-stu-id="66d32-103">orgContact: delta</span></span>

<span data-ttu-id="66d32-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66d32-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="66d32-105">获取新建、更新或删除的组织联系人，而无需执行整个集合的完全读取。</span><span class="sxs-lookup"><span data-stu-id="66d32-105">Get newly created, updated, or deleted organizational contacts without having to perform a full read of the entire collection.</span></span> <span data-ttu-id="66d32-106">有关详细信息，请参阅[更改跟踪](/graph/delta-query-overview)。</span><span class="sxs-lookup"><span data-stu-id="66d32-106">See [change tracking](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="66d32-107">权限</span><span class="sxs-lookup"><span data-stu-id="66d32-107">Permissions</span></span>

<span data-ttu-id="66d32-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="66d32-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="66d32-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="66d32-110">Permission type</span></span>      | <span data-ttu-id="66d32-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="66d32-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="66d32-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="66d32-112">Delegated (work or school account)</span></span> | <span data-ttu-id="66d32-113">OrgContact.Read.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="66d32-113">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="66d32-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="66d32-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66d32-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="66d32-115">Not supported.</span></span>  |
|<span data-ttu-id="66d32-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="66d32-116">Application</span></span> | <span data-ttu-id="66d32-117">OrgContact.Read.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66d32-117">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="66d32-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="66d32-118">HTTP request</span></span>

<span data-ttu-id="66d32-119">若要开始跟踪更改，请对 contacts 资源提出包含 delta 函数的请求。</span><span class="sxs-lookup"><span data-stu-id="66d32-119">To begin tracking changes, you make a request including the delta function on the contacts resource.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /contacts/delta
```

## <a name="query-parameters"></a><span data-ttu-id="66d32-120">查询参数</span><span class="sxs-lookup"><span data-stu-id="66d32-120">Query parameters</span></span>

<span data-ttu-id="66d32-121">跟踪组织联系人的更改将引发一组 delta 函数调用。 </span><span class="sxs-lookup"><span data-stu-id="66d32-121">Tracking changes in organizational contacts incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="66d32-122">如果要使用任意查询参数（`$deltatoken` 和 `$skiptoken` 除外），则必须在最初的 **delta** 请求中指定它。</span><span class="sxs-lookup"><span data-stu-id="66d32-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="66d32-123">Microsoft Graph 自动将指定的任意参数编码为响应中提供的 `nextLink` 或 `deltaLink` URL 的令牌部分。</span><span class="sxs-lookup"><span data-stu-id="66d32-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="66d32-124">只需指定任何查询参数一次。</span><span class="sxs-lookup"><span data-stu-id="66d32-124">You only need to specify any query parameters once up front.</span></span>

<span data-ttu-id="66d32-125">在后续请求中，复制并应用 `nextLink` 上 `deltaLink` 一响应中的 或 URL。</span><span class="sxs-lookup"><span data-stu-id="66d32-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response.</span></span> <span data-ttu-id="66d32-126">该 URL 已包含编码参数。</span><span class="sxs-lookup"><span data-stu-id="66d32-126">That URL already includes the encoded parameters.</span></span>

| <span data-ttu-id="66d32-127">查询参数</span><span class="sxs-lookup"><span data-stu-id="66d32-127">Query parameter</span></span>      | <span data-ttu-id="66d32-128">类型</span><span class="sxs-lookup"><span data-stu-id="66d32-128">Type</span></span>   |<span data-ttu-id="66d32-129">说明</span><span class="sxs-lookup"><span data-stu-id="66d32-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="66d32-130">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="66d32-130">$deltatoken</span></span> | <span data-ttu-id="66d32-131">string</span><span class="sxs-lookup"><span data-stu-id="66d32-131">string</span></span> | <span data-ttu-id="66d32-132">对[同一](/graph/delta-query-overview)个组织联系人集合之前的 delta 函数调用的 URL 中返回的状态令牌，指示完成这一轮 `deltaLink` 更改跟踪。 </span><span class="sxs-lookup"><span data-stu-id="66d32-132">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same organization contact collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="66d32-133">在集合的下一轮更改跟踪的第一个请求中保存和应用整个 `deltaLink` URL（包括此令牌）。</span><span class="sxs-lookup"><span data-stu-id="66d32-133">Save and apply the entire `deltaLink` URL, including this token, in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="66d32-134">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="66d32-134">$skiptoken</span></span> | <span data-ttu-id="66d32-135">string</span><span class="sxs-lookup"><span data-stu-id="66d32-135">string</span></span> | <span data-ttu-id="66d32-136">之前的[delta](/graph/delta-query-overview)函数调用的 URL 中返回的状态令牌，指示同一组织联系人集合中还有进一步 `nextLink` 的更改需要跟踪。 </span><span class="sxs-lookup"><span data-stu-id="66d32-136">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating that there are further changes to be tracked in the same organization contact collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="66d32-137">OData 查询参数</span><span class="sxs-lookup"><span data-stu-id="66d32-137">OData query parameters</span></span>

<span data-ttu-id="66d32-138">此方法支持可选的 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="66d32-138">This method supports optional OData query parameters to help customize the response.</span></span>

- <span data-ttu-id="66d32-p106">像在任何 GET 请求中一样，你可以使用 `$select` 查询参数以仅指定获取最佳性能所需的属性。始终返回 **id** 属性。</span><span class="sxs-lookup"><span data-stu-id="66d32-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The **id** property is always returned.</span></span>
- <span data-ttu-id="66d32-141">提供对 `$filter` 的有限支持：</span><span class="sxs-lookup"><span data-stu-id="66d32-141">There is limited support for `$filter`:</span></span>
  - <span data-ttu-id="66d32-142">唯一支持的 `$filter` 表达式用于跟踪对特定对象 `$filter=id+eq+{value}` 的更改。</span><span class="sxs-lookup"><span data-stu-id="66d32-142">The only supported `$filter` expression is for tracking changes on a specific object: `$filter=id+eq+{value}`.</span></span> <span data-ttu-id="66d32-143">可以筛选多个对象。</span><span class="sxs-lookup"><span data-stu-id="66d32-143">You can filter multiple objects.</span></span> <span data-ttu-id="66d32-144">例如，`https://graph.microsoft.com/v1.0/contacts/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`。</span><span class="sxs-lookup"><span data-stu-id="66d32-144">For example, `https://graph.microsoft.com/v1.0/contacts/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span></span> <span data-ttu-id="66d32-145">筛选对象不能超出 50 个。</span><span class="sxs-lookup"><span data-stu-id="66d32-145">There is a limit of 50 filtered objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="66d32-146">请求标头</span><span class="sxs-lookup"><span data-stu-id="66d32-146">Request headers</span></span>
| <span data-ttu-id="66d32-147">名称</span><span class="sxs-lookup"><span data-stu-id="66d32-147">Name</span></span>       | <span data-ttu-id="66d32-148">说明</span><span class="sxs-lookup"><span data-stu-id="66d32-148">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="66d32-149">Authorization</span><span class="sxs-lookup"><span data-stu-id="66d32-149">Authorization</span></span>  | <span data-ttu-id="66d32-150">持有者 &lt;token&gt;。</span><span class="sxs-lookup"><span data-stu-id="66d32-150">Bearer &lt;token&gt;.</span></span> <span data-ttu-id="66d32-151">必需。</span><span class="sxs-lookup"><span data-stu-id="66d32-151">Required.</span></span>|
| <span data-ttu-id="66d32-152">Prefer</span><span class="sxs-lookup"><span data-stu-id="66d32-152">Prefer</span></span> | <span data-ttu-id="66d32-153">return=minimal</span><span class="sxs-lookup"><span data-stu-id="66d32-153">return=minimal</span></span> <br><br><span data-ttu-id="66d32-154">在使用 `deltaLink` 的请求中执行此标头将仅返回自上一轮之后发生更改的对象属性。</span><span class="sxs-lookup"><span data-stu-id="66d32-154">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="66d32-155">可选。</span><span class="sxs-lookup"><span data-stu-id="66d32-155">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="66d32-156">请求正文</span><span class="sxs-lookup"><span data-stu-id="66d32-156">Request body</span></span>
<span data-ttu-id="66d32-157">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="66d32-157">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66d32-158">响应</span><span class="sxs-lookup"><span data-stu-id="66d32-158">Response</span></span>

<span data-ttu-id="66d32-159">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` ab [orgContact](../resources/orgcontact.md) 集合对象。</span><span class="sxs-lookup"><span data-stu-id="66d32-159">If successful, this method returns a `200 OK` response code and ab [orgContact](../resources/orgcontact.md) collection object in the response body.</span></span> <span data-ttu-id="66d32-160">该响应还包括 `nextLink`URL 或 `deltaLink`URL。</span><span class="sxs-lookup"><span data-stu-id="66d32-160">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="66d32-161">如果返回 `nextLink`URL：</span><span class="sxs-lookup"><span data-stu-id="66d32-161">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="66d32-162">这表示会话中有其他要检索的数据页。</span><span class="sxs-lookup"><span data-stu-id="66d32-162">This indicates that there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="66d32-163">应用程序继续使用 `nextLink` URL 发出请求，直到响应中包含 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="66d32-163">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="66d32-164">响应包含与初始 Delta 查询请求相同的属性集。</span><span class="sxs-lookup"><span data-stu-id="66d32-164">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="66d32-165">这使你能够在发起 Delta 循环时捕获对象当前的完整状态。</span><span class="sxs-lookup"><span data-stu-id="66d32-165">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="66d32-166">如果返回 `deltaLink`URL：</span><span class="sxs-lookup"><span data-stu-id="66d32-166">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="66d32-167">这表示不再返回有关资源现有状态的数据。</span><span class="sxs-lookup"><span data-stu-id="66d32-167">This indicates that there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="66d32-168">保存并使用 `deltaLink` URL 来了解下一轮资源更改。</span><span class="sxs-lookup"><span data-stu-id="66d32-168">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="66d32-169">只有对于在签发 `deltaLink` 之后更改的属性，你才可以选择指定 `Prefer:return=minimal` 标头以包含在响应值中。</span><span class="sxs-lookup"><span data-stu-id="66d32-169">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="66d32-170">默认：返回与初始 Delta 请求相同的属性</span><span class="sxs-lookup"><span data-stu-id="66d32-170">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="66d32-171">默认情况下，使用 `deltaLink` 或 `nextLink` 的请求将通过以下方式返回与初始 Delta 查询中选择的相同属性：</span><span class="sxs-lookup"><span data-stu-id="66d32-171">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="66d32-172">如果属性已更改，则新值将包括在响应中。</span><span class="sxs-lookup"><span data-stu-id="66d32-172">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="66d32-173">这包括设为 Null 值的属性。</span><span class="sxs-lookup"><span data-stu-id="66d32-173">This includes properties being set to null value.</span></span>
- <span data-ttu-id="66d32-174">如果属性未更改，则旧值将包括在响应中。</span><span class="sxs-lookup"><span data-stu-id="66d32-174">If the property has not changed, the old value is included in the response.</span></span>
- <span data-ttu-id="66d32-175">如果之前从未设置过该属性，则它完全不会包含在响应中。</span><span class="sxs-lookup"><span data-stu-id="66d32-175">If the property has never been set before, it will not be included in the response at all.</span></span>


> <span data-ttu-id="66d32-176">**注意：** 通过此行为，无法通过查看响应来判断属性是否正在更改。</span><span class="sxs-lookup"><span data-stu-id="66d32-176">**Note:** With this behavior, it is not possible to tell whether a property is changing by looking at the response.</span></span> <span data-ttu-id="66d32-177">此外，增量响应往往很大，因为它们包含所有属性值，如示例 [2 所示](#example-2-selecting-three-properties)。</span><span class="sxs-lookup"><span data-stu-id="66d32-177">Also, the delta responses tend to be large because they contain all property values,as shown in [Example 2](#example-2-selecting-three-properties).</span></span>

### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="66d32-178">备用：仅返回更改的属性</span><span class="sxs-lookup"><span data-stu-id="66d32-178">Alternative: return only the changed properties</span></span>

<span data-ttu-id="66d32-179">添加可选请求标头 - `prefer:return=minimal` - 将导致出现以下行为：</span><span class="sxs-lookup"><span data-stu-id="66d32-179">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="66d32-180">如果属性已更改，则新值将包括在响应中。</span><span class="sxs-lookup"><span data-stu-id="66d32-180">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="66d32-181">这包括设为 Null 值的属性。</span><span class="sxs-lookup"><span data-stu-id="66d32-181">This includes properties being set to null value.</span></span>
- <span data-ttu-id="66d32-182">如果属性未更改，则该属性不会包括在响应中。</span><span class="sxs-lookup"><span data-stu-id="66d32-182">If the property has not changed, the property is not included in the response at all.</span></span> <span data-ttu-id="66d32-183">（不同于默认行为。）</span><span class="sxs-lookup"><span data-stu-id="66d32-183">(Different from the default behavior.)</span></span>

> <span data-ttu-id="66d32-184">**注意：** 可以在 Delta 循环中的任何时间点将标头添加到 `deltaLink` 请求中。</span><span class="sxs-lookup"><span data-stu-id="66d32-184">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="66d32-185">标头仅影响响应中包含的属性集，而不会影响增量查询的运行。</span><span class="sxs-lookup"><span data-stu-id="66d32-185">The header only affects the set of properties included in the response and it does not affect how the delta query is run.</span></span> <span data-ttu-id="66d32-186">请参阅[示例 3](#example-3-alternative-minimal-response-behavior)。</span><span class="sxs-lookup"><span data-stu-id="66d32-186">See [Example 3](#example-3-alternative-minimal-response-behavior).</span></span>

## <a name="examples"></a><span data-ttu-id="66d32-187">示例</span><span class="sxs-lookup"><span data-stu-id="66d32-187">Examples</span></span>

### <a name="example-1-default-properties"></a><span data-ttu-id="66d32-188">示例 1：默认属性</span><span class="sxs-lookup"><span data-stu-id="66d32-188">Example 1: Default properties</span></span>

#### <a name="request"></a><span data-ttu-id="66d32-189">请求</span><span class="sxs-lookup"><span data-stu-id="66d32-189">Request</span></span>

<span data-ttu-id="66d32-190">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="66d32-190">The following is an example of the request.</span></span> <span data-ttu-id="66d32-191">没有 `$select` 参数，因为将跟踪并返回默认的属性集。</span><span class="sxs-lookup"><span data-stu-id="66d32-191">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>


# <a name="http"></a>[<span data-ttu-id="66d32-192">HTTP</span><span class="sxs-lookup"><span data-stu-id="66d32-192">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "orgContact_delta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts/delta
```
# <a name="c"></a>[<span data-ttu-id="66d32-193">C#</span><span class="sxs-lookup"><span data-stu-id="66d32-193">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="66d32-194">JavaScript</span><span class="sxs-lookup"><span data-stu-id="66d32-194">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="66d32-195">Objective-C</span><span class="sxs-lookup"><span data-stu-id="66d32-195">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="66d32-196">Java</span><span class="sxs-lookup"><span data-stu-id="66d32-196">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="66d32-197">响应</span><span class="sxs-lookup"><span data-stu-id="66d32-197">Response</span></span>

<span data-ttu-id="66d32-198">以下示例所示为使用从查询初始化获得的 `deltaLink` 时的响应。</span><span class="sxs-lookup"><span data-stu-id="66d32-198">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span>

><span data-ttu-id="66d32-p120">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="66d32-p120">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#contacts",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/contacts/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "companyName": "companyName-value",
      "department": "department-value",
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "id": "string (identifier)",
      "jobTitle": "jobTitle-value",
      "mail": "mail-value",
      "mailNickname": "mailNickname-value",
      "surname": "surname-value"
    }
  ]
}
```

### <a name="example-2-selecting-three-properties"></a><span data-ttu-id="66d32-201">示例 2：选择三个属性</span><span class="sxs-lookup"><span data-stu-id="66d32-201">Example 2: Selecting three properties</span></span>

#### <a name="request"></a><span data-ttu-id="66d32-202">请求</span><span class="sxs-lookup"><span data-stu-id="66d32-202">Request</span></span>

<span data-ttu-id="66d32-203">下一个示例所示为通过默认响应行为选择三种更改跟踪属性时的初始请求。</span><span class="sxs-lookup"><span data-stu-id="66d32-203">The next example shows the initial request selecting three properties for change tracking, with default response behavior.</span></span>


# <a name="http"></a>[<span data-ttu-id="66d32-204">HTTP</span><span class="sxs-lookup"><span data-stu-id="66d32-204">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "orgcontact_delta_select"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts/delta?$select=displayName,jobTitle,mail
```
# <a name="c"></a>[<span data-ttu-id="66d32-205">C#</span><span class="sxs-lookup"><span data-stu-id="66d32-205">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-delta-select-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="66d32-206">JavaScript</span><span class="sxs-lookup"><span data-stu-id="66d32-206">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-delta-select-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="66d32-207">Objective-C</span><span class="sxs-lookup"><span data-stu-id="66d32-207">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-delta-select-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="66d32-208">Java</span><span class="sxs-lookup"><span data-stu-id="66d32-208">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-delta-select-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="66d32-209">响应</span><span class="sxs-lookup"><span data-stu-id="66d32-209">Response</span></span>

<span data-ttu-id="66d32-210">以下示例所示为使用从查询初始化获得的 `deltaLink` 时的响应。</span><span class="sxs-lookup"><span data-stu-id="66d32-210">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="66d32-211">请注意，所有三种属性将包括在响应中，并且无法知道在获得 `deltaLink` 之后哪些属性发生了更改。</span><span class="sxs-lookup"><span data-stu-id="66d32-211">Note that all three properties are included in the response and it is not known which ones have changed since the `deltaLink` was obtained.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#contacts",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/contacts/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "jobTitle": "jobTitle-value",
      "mail": null
    }
  ]
}
```

### <a name="example-3-alternative-minimal-response-behavior"></a><span data-ttu-id="66d32-212">示例 3：备用最小响应行为</span><span class="sxs-lookup"><span data-stu-id="66d32-212">Example 3: Alternative minimal response behavior</span></span>

#### <a name="request"></a><span data-ttu-id="66d32-213">请求</span><span class="sxs-lookup"><span data-stu-id="66d32-213">Request</span></span>

<span data-ttu-id="66d32-214">下一个示例所示为通过备用最小响应行为选择三种更改跟踪属性时的初始请求。</span><span class="sxs-lookup"><span data-stu-id="66d32-214">The next example shows the initial request selecting three properties for change tracking, with alternative minimal response behavior.</span></span>


# <a name="http"></a>[<span data-ttu-id="66d32-215">HTTP</span><span class="sxs-lookup"><span data-stu-id="66d32-215">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "orgcontact_delta_minimal"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts/delta?$select=displayName,jobTitle,mail
Prefer: return=minimal
```
# <a name="c"></a>[<span data-ttu-id="66d32-216">C#</span><span class="sxs-lookup"><span data-stu-id="66d32-216">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-delta-minimal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="66d32-217">JavaScript</span><span class="sxs-lookup"><span data-stu-id="66d32-217">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-delta-minimal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="66d32-218">Objective-C</span><span class="sxs-lookup"><span data-stu-id="66d32-218">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-delta-minimal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="66d32-219">Java</span><span class="sxs-lookup"><span data-stu-id="66d32-219">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-delta-minimal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="66d32-220">响应</span><span class="sxs-lookup"><span data-stu-id="66d32-220">Response</span></span>

<span data-ttu-id="66d32-221">以下示例所示为使用从查询初始化获得的 `deltaLink` 时的响应。</span><span class="sxs-lookup"><span data-stu-id="66d32-221">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="66d32-222">请注意，`mail` 属性不包括在内，这意味着它在上一轮 Delta 查询之后未发生更改；并且 `displayName` 和 `jobTitle` 将包括在内，这意味着其值已发生更改。</span><span class="sxs-lookup"><span data-stu-id="66d32-222">Note that the `mail` property is not included, which means it has not changed since the last delta query; `displayName` and `jobTitle` are included which means their values have changed.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#contacts",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/contacts/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "jobTitle": null
    }
  ]
}
```
## <a name="see-also"></a><span data-ttu-id="66d32-223">另请参阅</span><span class="sxs-lookup"><span data-stu-id="66d32-223">See also</span></span>

- <span data-ttu-id="66d32-224">[使用 Delta 查询跟踪 Microsoft Graph 数据更改](/graph/delta-query-overview)。</span><span class="sxs-lookup"><span data-stu-id="66d32-224">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>

<!-- uuid: 3B5A9A7C-6324-432F-8C66-AC4883DD71EF
2020-03-20 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "contact: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

