---
title: directoryObject： 增量
description: 获取新创建、 更新或删除以下类型的目录对象： 用户、 组和组织的联系人，请在单个增量查询。 请参阅修订的详细信息。
localization_priority: Normal
ms.openlocfilehash: 823107bce56d77c4e9c29a77405ac014443f5190
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854493"
---
# <a name="directoryobject-delta"></a><span data-ttu-id="7caeb-104">directoryObject： 增量</span><span class="sxs-lookup"><span data-stu-id="7caeb-104">directoryObject: delta</span></span>

> <span data-ttu-id="7caeb-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7caeb-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7caeb-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7caeb-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7caeb-107">获取新创建、 更新或删除以下类型的目录对象：[用户](../resources/user.md)、[组](../resources/group.md)和[组织的联系人](../resources/orgcontact.md)，请在单个增量查询。</span><span class="sxs-lookup"><span data-stu-id="7caeb-107">Get newly created, updated, or deleted directory objects of the following types: [user](../resources/user.md), [group](../resources/group.md) and [organizational contact](../resources/orgcontact.md), in a single delta query.</span></span> <span data-ttu-id="7caeb-108">有关详细信息，请参阅[修订](/graph/delta-query-overview)。</span><span class="sxs-lookup"><span data-stu-id="7caeb-108">See [Track changes](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="7caeb-109">权限</span><span class="sxs-lookup"><span data-stu-id="7caeb-109">Permissions</span></span>

<span data-ttu-id="7caeb-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7caeb-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7caeb-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="7caeb-112">Permission type</span></span>      | <span data-ttu-id="7caeb-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7caeb-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7caeb-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7caeb-114">Delegated (work or school account)</span></span> | <span data-ttu-id="7caeb-115">Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7caeb-115">Directory.Read.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="7caeb-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7caeb-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7caeb-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="7caeb-117">Not supported.</span></span>  |
|<span data-ttu-id="7caeb-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="7caeb-118">Application</span></span> | <span data-ttu-id="7caeb-119">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7caeb-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7caeb-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7caeb-120">HTTP request</span></span>

<span data-ttu-id="7caeb-121">若要开始跟踪的更改，您发出请求包含增量函数对 directoryObjects 资源。</span><span class="sxs-lookup"><span data-stu-id="7caeb-121">To begin tracking changes, you make a request including the delta function on the directoryObjects resource.</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /directoryObjects/delta
```

## <a name="query-parameters"></a><span data-ttu-id="7caeb-122">查询参数</span><span class="sxs-lookup"><span data-stu-id="7caeb-122">Query parameters</span></span>

<span data-ttu-id="7caeb-123">跟踪更改会导致一个或多个**增量**函数调用的往返。</span><span class="sxs-lookup"><span data-stu-id="7caeb-123">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="7caeb-124">如果您使用任何查询参数 (以外的其他`$deltatoken`和`$skiptoken`)，则必须指定该初始**增量**请求中。</span><span class="sxs-lookup"><span data-stu-id="7caeb-124">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="7caeb-125">Microsoft Graph 自动将任何指定的参数编码为的令牌部分`nextLink`或`deltaLink`响应中提供的 URL。</span><span class="sxs-lookup"><span data-stu-id="7caeb-125">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="7caeb-126">只需预先指定所需的任何查询参数一次。</span><span class="sxs-lookup"><span data-stu-id="7caeb-126">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="7caeb-127">在后续请求中，可以复制并应用之前响应中返回的 `nextLink` 或 `deltaLink` URL，因为此 URL 已包含所需的编码参数。</span><span class="sxs-lookup"><span data-stu-id="7caeb-127">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="7caeb-128">查询参数</span><span class="sxs-lookup"><span data-stu-id="7caeb-128">Query parameter</span></span> | <span data-ttu-id="7caeb-129">类型</span><span class="sxs-lookup"><span data-stu-id="7caeb-129">Type</span></span> |<span data-ttu-id="7caeb-130">说明</span><span class="sxs-lookup"><span data-stu-id="7caeb-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7caeb-131">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="7caeb-131">$deltatoken</span></span> | <span data-ttu-id="7caeb-132">string</span><span class="sxs-lookup"><span data-stu-id="7caeb-132">string</span></span> | <span data-ttu-id="7caeb-p106">对同一个用户集合之前的 **delta** 函数调用的 `deltaLink` URL 中返回的[状态令牌](/graph/delta-query-overview)，指示该组更改跟踪的完成状态。将此令牌包含在对该集合的下一组更改追踪的首次请求中，并保存和应用整个 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="7caeb-p106">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same user collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="7caeb-135">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="7caeb-135">$skiptoken</span></span> | <span data-ttu-id="7caeb-136">string</span><span class="sxs-lookup"><span data-stu-id="7caeb-136">string</span></span> | <span data-ttu-id="7caeb-137">对之前的 **delta** 函数调用的 `nextLink` URL 中返回的[状态令牌](/graph/delta-query-overview)，指示同一个用户集合中有进一步的更改需要追踪。</span><span class="sxs-lookup"><span data-stu-id="7caeb-137">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same user collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="7caeb-138">OData 查询参数</span><span class="sxs-lookup"><span data-stu-id="7caeb-138">OData query parameters</span></span>

<span data-ttu-id="7caeb-139">此方法支持可选的 OData 查询参数，以帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7caeb-139">This method supports optional OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="7caeb-140">您可以使用`$filter`与特殊`isOf`派生自 directoryObject 运算符筛选类型的子集。</span><span class="sxs-lookup"><span data-stu-id="7caeb-140">You can use `$filter` with the special `isOf` operator to filter a subset of types derived from directoryObject.</span></span>
  - <span data-ttu-id="7caeb-141">您可以组合使用的多个表达式`or`，这使您能够具有跟踪多个类型的单个增量查询。</span><span class="sxs-lookup"><span data-stu-id="7caeb-141">You can combine multiple expressions using an `or`, which allows you to have a single delta query tracking multiple types.</span></span> <span data-ttu-id="7caeb-142">请参阅[第三个示例](#request-3)的详细信息。</span><span class="sxs-lookup"><span data-stu-id="7caeb-142">See the [third example](#request-3) for details.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7caeb-143">请求标头</span><span class="sxs-lookup"><span data-stu-id="7caeb-143">Request headers</span></span>

| <span data-ttu-id="7caeb-144">名称</span><span class="sxs-lookup"><span data-stu-id="7caeb-144">Name</span></span>       | <span data-ttu-id="7caeb-145">说明</span><span class="sxs-lookup"><span data-stu-id="7caeb-145">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7caeb-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="7caeb-146">Authorization</span></span>  | <span data-ttu-id="7caeb-147">持有者&lt;令牌&gt;</span><span class="sxs-lookup"><span data-stu-id="7caeb-147">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="7caeb-148">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7caeb-148">Content-Type</span></span>  | <span data-ttu-id="7caeb-149">application/json</span><span class="sxs-lookup"><span data-stu-id="7caeb-149">application/json</span></span> |
| <span data-ttu-id="7caeb-150">Prefer</span><span class="sxs-lookup"><span data-stu-id="7caeb-150">Prefer</span></span> | <span data-ttu-id="7caeb-151">返回 = 最少</span><span class="sxs-lookup"><span data-stu-id="7caeb-151">return=minimal</span></span> <br><br><span data-ttu-id="7caeb-152">指定与请求使用此标头`deltaLink`会返回自上次循环后已更改的对象属性。</span><span class="sxs-lookup"><span data-stu-id="7caeb-152">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="7caeb-153">可选。</span><span class="sxs-lookup"><span data-stu-id="7caeb-153">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7caeb-154">请求正文</span><span class="sxs-lookup"><span data-stu-id="7caeb-154">Request body</span></span>

<span data-ttu-id="7caeb-155">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7caeb-155">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="7caeb-156">响应</span><span class="sxs-lookup"><span data-stu-id="7caeb-156">Response</span></span>

<span data-ttu-id="7caeb-157">如果成功，此方法返回`200 OK`响应正文中的响应代码和[用户](../resources/directoryobject.md)集合的对象。</span><span class="sxs-lookup"><span data-stu-id="7caeb-157">If successful, this method returns `200 OK` response code and [user](../resources/directoryobject.md) collection object in the response body.</span></span> <span data-ttu-id="7caeb-158">响应还包括`nextLink`URL 或`deltaLink`URL。</span><span class="sxs-lookup"><span data-stu-id="7caeb-158">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="7caeb-159">如果`nextLink`返回 URL:</span><span class="sxs-lookup"><span data-stu-id="7caeb-159">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="7caeb-160">这指示有会话中检索的数据的其他页面。</span><span class="sxs-lookup"><span data-stu-id="7caeb-160">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="7caeb-161">应用程序将继续进行请求使用`nextLink`直到 URL `deltaLink` URL 包含响应中。</span><span class="sxs-lookup"><span data-stu-id="7caeb-161">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="7caeb-162">响应包含一组相同的属性，如初始增量查询请求中所示。</span><span class="sxs-lookup"><span data-stu-id="7caeb-162">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="7caeb-163">这样，您可以在启动增量周期捕获对象的完整当前状态。</span><span class="sxs-lookup"><span data-stu-id="7caeb-163">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="7caeb-164">如果`deltaLink`返回 URL:</span><span class="sxs-lookup"><span data-stu-id="7caeb-164">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="7caeb-165">这表明没有更多有关要返回的资源的现有状态数据。</span><span class="sxs-lookup"><span data-stu-id="7caeb-165">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="7caeb-166">保存并使用`deltaLink`URL 以了解如何更改为下一轮中的资源。</span><span class="sxs-lookup"><span data-stu-id="7caeb-166">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="7caeb-167">您可以选择指定`Prefer:return=minimal`标头，以响应时间以来已经更改的属性值中包括`deltaLink`颁发。</span><span class="sxs-lookup"><span data-stu-id="7caeb-167">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="7caeb-168">默认值： 返回作为初始增量请求的同一属性</span><span class="sxs-lookup"><span data-stu-id="7caeb-168">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="7caeb-169">默认情况下，请求使用`deltaLink`或`nextLink`与选定初始增量查询中相同的属性返回以下方式：</span><span class="sxs-lookup"><span data-stu-id="7caeb-169">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="7caeb-170">如果已更改的属性，在响应中包含的新值。</span><span class="sxs-lookup"><span data-stu-id="7caeb-170">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="7caeb-171">这包括属性被设置为 null 值。</span><span class="sxs-lookup"><span data-stu-id="7caeb-171">This includes properties being set to null value.</span></span>
- <span data-ttu-id="7caeb-172">如果具有未更改的属性，在响应中包含的旧值。</span><span class="sxs-lookup"><span data-stu-id="7caeb-172">If the property has not changed, the old value is included in the response.</span></span>
- <span data-ttu-id="7caeb-173">如果从未它将不会包含在响应中根本之前设置该属性。</span><span class="sxs-lookup"><span data-stu-id="7caeb-173">If the property has never been set before it will not be included in the response at all.</span></span>


> <span data-ttu-id="7caeb-174">**注意：** 与此行为，通过查看响应它不能以告知属性是否已更改或未。</span><span class="sxs-lookup"><span data-stu-id="7caeb-174">**Note:** With this behavior, by looking at the response it is not possible to tell whether a property is changing or not.</span></span> <span data-ttu-id="7caeb-175">此外，则 delta 响应容易很大，因为它们包含的所有属性值。</span><span class="sxs-lookup"><span data-stu-id="7caeb-175">Also, the delta responses tend to be large because they contain all property values.</span></span>

#### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="7caeb-176">可选： 仅返回已更改的属性</span><span class="sxs-lookup"><span data-stu-id="7caeb-176">Alternative: return only the changed properties</span></span>

<span data-ttu-id="7caeb-177">添加可选请求标头中的`prefer:return=minimal`-导致以下行为：</span><span class="sxs-lookup"><span data-stu-id="7caeb-177">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="7caeb-178">如果已更改的属性，在响应中包含的新值。</span><span class="sxs-lookup"><span data-stu-id="7caeb-178">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="7caeb-179">这包括属性被设置为 null 值。</span><span class="sxs-lookup"><span data-stu-id="7caeb-179">This includes properties being set to null value.</span></span>
- <span data-ttu-id="7caeb-180">如果具有未更改的属性，该属性不包括在响应中根本。</span><span class="sxs-lookup"><span data-stu-id="7caeb-180">If the property has not changed, the property is not included in the response at all.</span></span> <span data-ttu-id="7caeb-181">（不同于默认行为。）</span><span class="sxs-lookup"><span data-stu-id="7caeb-181">(Different from the default behavior.)</span></span>

> <span data-ttu-id="7caeb-182">**注意：** 标头可以添加到`deltaLink`任何时间点的增量周期中的请求。</span><span class="sxs-lookup"><span data-stu-id="7caeb-182">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="7caeb-183">头只影响的响应中包括的属性集，而不会影响如何执行增量查询。</span><span class="sxs-lookup"><span data-stu-id="7caeb-183">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span>

## <a name="example"></a><span data-ttu-id="7caeb-184">示例</span><span class="sxs-lookup"><span data-stu-id="7caeb-184">Example</span></span>

### <a name="request-1"></a><span data-ttu-id="7caeb-185">请求 1</span><span class="sxs-lookup"><span data-stu-id="7caeb-185">Request 1</span></span>

<span data-ttu-id="7caeb-186">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7caeb-186">The following is an example of the request.</span></span> <span data-ttu-id="7caeb-187">没有任何`$select`参数，以便跟踪和返回一组默认属性。</span><span class="sxs-lookup"><span data-stu-id="7caeb-187">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/beta/directoryObjects/delta
```

### <a name="response-1"></a><span data-ttu-id="7caeb-188">响应 1</span><span class="sxs-lookup"><span data-stu-id="7caeb-188">Response 1</span></span>

<span data-ttu-id="7caeb-189">以下是时使用的响应示例`deltaLink`获取从查询初始化。</span><span class="sxs-lookup"><span data-stu-id="7caeb-189">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="7caeb-190">不`isOf`已使用筛选器，以便返回所有派生自 directoryObject 的类型。</span><span class="sxs-lookup"><span data-stu-id="7caeb-190">No `isOf` filter has been used, so all types derived from directoryObject are returned.</span></span>

><span data-ttu-id="7caeb-p120">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7caeb-p120">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "jobTitle": null,
      <...response trimmed for brevity...>
    },
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "cf33844a-b6f8-4d4d-84f4-54e8d45094f0",
      "deletedDateTime": null,
      "classification": null,
      "createdDateTime": "2018-06-20T16:50:09Z",
      "description": null,
      "displayName": "testgp",
      <...response trimmed for brevity...>
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
      "id": "string (identifier)",
      "jobTitle": "string",
      <...response trimmed for brevity...>
    },
    <...response trimmed for brevity...>
  ]
}
```

### <a name="request-2"></a><span data-ttu-id="7caeb-193">请求 2</span><span class="sxs-lookup"><span data-stu-id="7caeb-193">Request 2</span></span>

<span data-ttu-id="7caeb-194">下一个示例演示如何使用备用内容最少响应行为：</span><span class="sxs-lookup"><span data-stu-id="7caeb-194">The next example shows the use of the alternative minimal response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "directoryObject_delta"
}-->

```http
GET https://graph.microsoft.com/beta/directoryObjects/delta
Prefer: return=minimal
```

### <a name="response-2"></a><span data-ttu-id="7caeb-195">响应 2</span><span class="sxs-lookup"><span data-stu-id="7caeb-195">Response 2</span></span>

<span data-ttu-id="7caeb-196">以下是时使用的响应示例`deltaLink`获取从查询初始化。</span><span class="sxs-lookup"><span data-stu-id="7caeb-196">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="7caeb-197">请注意会返回实际发生了更改的属性。</span><span class="sxs-lookup"><span data-stu-id="7caeb-197">Note only the properties that have actually changed are returned.</span></span>

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
    },
    <...response trimmed for brevity...>
  ]
}
```

### <a name="request-3"></a><span data-ttu-id="7caeb-198">请求 3</span><span class="sxs-lookup"><span data-stu-id="7caeb-198">Request 3</span></span>

<span data-ttu-id="7caeb-199">下面的示例演示初始请求使用`isOf`运算符筛选出只有用户和组的实体：</span><span class="sxs-lookup"><span data-stu-id="7caeb-199">The next example shows the initial request using the `isOf` operator to filter out only user and group entities:</span></span>
<!-- {
  "blockType": "request",
  "name": "directoryobject_delta"
}-->

```http
GET https://graph.microsoft.com/beta/directoryObjects/delta?$filter=isOf('Microsoft.Graph.User')+or+isOf('Microsoft.Graph.Group')
```

### <a name="response-3"></a><span data-ttu-id="7caeb-200">响应 3</span><span class="sxs-lookup"><span data-stu-id="7caeb-200">Response 3</span></span>

<span data-ttu-id="7caeb-201">以下是时使用的响应示例`deltaLink`获取从查询初始化。</span><span class="sxs-lookup"><span data-stu-id="7caeb-201">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="7caeb-202">请注意返回的唯一用户和组对象：</span><span class="sxs-lookup"><span data-stu-id="7caeb-202">Note that only user and group objects are returned:</span></span>

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
      "jobTitle": null,
      <...response trimmed for brevity...>
    },
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "cf33844a-b6f8-4d4d-84f4-54e8d45094f0",
      "deletedDateTime": null,
      "classification": null,
      "createdDateTime": "2018-06-20T16:50:09Z",
      "description": null,
      "displayName": "testgp",
      <...response trimmed for brevity...>
    },
    <...response trimmed for brevity...>
  ]
}
```

- <span data-ttu-id="7caeb-203">[使用增量查询来跟踪 Microsoft Graph 数据中的更改](/graph/delta-query-overview)。</span><span class="sxs-lookup"><span data-stu-id="7caeb-203">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>
- <span data-ttu-id="7caeb-204">[获取用户的增量更改](/graph/delta-query-users)。</span><span class="sxs-lookup"><span data-stu-id="7caeb-204">[Get incremental changes for users](/graph/delta-query-users).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
