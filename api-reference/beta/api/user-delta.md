---
title: 'user: delta'
description: 获取新创建、更新或删除的用户, 而无需对整个用户集执行完全读取。 有关详细信息, 请参阅跟踪更改。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6fd8eb71c1b647550219ae6686a0bc814420b2fa
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32536999"
---
# <a name="user-delta"></a><span data-ttu-id="10eb1-104">user: delta</span><span class="sxs-lookup"><span data-stu-id="10eb1-104">user: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10eb1-105">获取新创建、更新或删除的用户, 而无需对整个用户集执行完全读取。</span><span class="sxs-lookup"><span data-stu-id="10eb1-105">Get newly created, updated, or deleted users without having to perform a full read of the entire user collection.</span></span> <span data-ttu-id="10eb1-106">有关详细信息, 请参阅[跟踪更改](/graph/delta-query-overview)。</span><span class="sxs-lookup"><span data-stu-id="10eb1-106">See [Track changes](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="10eb1-107">权限</span><span class="sxs-lookup"><span data-stu-id="10eb1-107">Permissions</span></span>

<span data-ttu-id="10eb1-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="10eb1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="10eb1-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="10eb1-110">Permission type</span></span>      | <span data-ttu-id="10eb1-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="10eb1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="10eb1-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="10eb1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="10eb1-113">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="10eb1-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="10eb1-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="10eb1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10eb1-115">User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="10eb1-115">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="10eb1-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="10eb1-116">Application</span></span> | <span data-ttu-id="10eb1-117">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10eb1-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="10eb1-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="10eb1-118">HTTP request</span></span>

<span data-ttu-id="10eb1-119">为开始跟踪更改，请在用户资源上发出包含 delta 函数的请求。</span><span class="sxs-lookup"><span data-stu-id="10eb1-119">To begin tracking changes, you make a request including the delta function on the users resource.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/delta
```

## <a name="query-parameters"></a><span data-ttu-id="10eb1-120">查询参数</span><span class="sxs-lookup"><span data-stu-id="10eb1-120">Query parameters</span></span>

<span data-ttu-id="10eb1-121">跟踪用户的更改会产生一个或多个**delta**函数调用的往返。</span><span class="sxs-lookup"><span data-stu-id="10eb1-121">Tracking changes in users incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="10eb1-122">如果使用任何查询参数 (而不是`$deltatoken` and `$skiptoken`), 则必须在初始**delta**请求中指定它。</span><span class="sxs-lookup"><span data-stu-id="10eb1-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="10eb1-123">Microsoft Graph 自动将任何指定的参数编码到响应中提供`nextLink`的`deltaLink` or URL 的令牌部分。</span><span class="sxs-lookup"><span data-stu-id="10eb1-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="10eb1-124">只需预先指定所需的任何查询参数一次。</span><span class="sxs-lookup"><span data-stu-id="10eb1-124">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="10eb1-125">在后续请求中，可以复制并应用之前响应中返回的 `nextLink` 或 `deltaLink` URL，因为此 URL 已包含所需的编码参数。</span><span class="sxs-lookup"><span data-stu-id="10eb1-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="10eb1-126">查询参数</span><span class="sxs-lookup"><span data-stu-id="10eb1-126">Query parameter</span></span>      | <span data-ttu-id="10eb1-127">类型</span><span class="sxs-lookup"><span data-stu-id="10eb1-127">Type</span></span>   |<span data-ttu-id="10eb1-128">说明</span><span class="sxs-lookup"><span data-stu-id="10eb1-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="10eb1-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="10eb1-129">$deltatoken</span></span> | <span data-ttu-id="10eb1-130">string</span><span class="sxs-lookup"><span data-stu-id="10eb1-130">string</span></span> | <span data-ttu-id="10eb1-p105">对同一个用户集合之前的 **delta** 函数调用的 `deltaLink` URL 中返回的[状态令牌](/graph/delta-query-overview)，指示该组更改跟踪的完成状态。将此令牌包含在对该集合的下一组更改追踪的首次请求中，并保存和应用整个 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="10eb1-p105">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same user collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="10eb1-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="10eb1-133">$skiptoken</span></span> | <span data-ttu-id="10eb1-134">string</span><span class="sxs-lookup"><span data-stu-id="10eb1-134">string</span></span> | <span data-ttu-id="10eb1-135">对之前的 **delta** 函数调用的 `nextLink` URL 中返回的[状态令牌](/graph/delta-query-overview)，指示同一个用户集合中有进一步的更改需要追踪。</span><span class="sxs-lookup"><span data-stu-id="10eb1-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same user collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="10eb1-136">OData 查询参数</span><span class="sxs-lookup"><span data-stu-id="10eb1-136">OData query parameters</span></span>

<span data-ttu-id="10eb1-137">此方法支持可选的 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="10eb1-137">This method supports optional OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="10eb1-p106">像在任何 GET 请求中一样，你可以使用 `$select` 查询参数以仅指定获取最佳性能所需的属性。始终返回 *id* 属性。</span><span class="sxs-lookup"><span data-stu-id="10eb1-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The *id* property is always returned.</span></span>
- <span data-ttu-id="10eb1-140">对`$filter`以下项的支持有限:</span><span class="sxs-lookup"><span data-stu-id="10eb1-140">There is limited support for `$filter`:</span></span>
  - <span data-ttu-id="10eb1-141">唯一支持的 `$filter` 表达式用于跟踪对特定对象 `$filter=id+eq+{value}` 的更改。</span><span class="sxs-lookup"><span data-stu-id="10eb1-141">The only supported `$filter` expression is for tracking changes on a specific object: `$filter=id+eq+{value}`.</span></span> <span data-ttu-id="10eb1-142">可以筛选多个对象。</span><span class="sxs-lookup"><span data-stu-id="10eb1-142">You can filter multiple objects.</span></span> <span data-ttu-id="10eb1-143">例如，`https://graph.microsoft.com/beta/users/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`。</span><span class="sxs-lookup"><span data-stu-id="10eb1-143">For example, `https://graph.microsoft.com/beta/users/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span></span> <span data-ttu-id="10eb1-144">筛选对象不能超出 50 个。</span><span class="sxs-lookup"><span data-stu-id="10eb1-144">There is a limit of 50 filtered objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="10eb1-145">请求标头</span><span class="sxs-lookup"><span data-stu-id="10eb1-145">Request headers</span></span>
| <span data-ttu-id="10eb1-146">名称</span><span class="sxs-lookup"><span data-stu-id="10eb1-146">Name</span></span>       | <span data-ttu-id="10eb1-147">说明</span><span class="sxs-lookup"><span data-stu-id="10eb1-147">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="10eb1-148">Authorization</span><span class="sxs-lookup"><span data-stu-id="10eb1-148">Authorization</span></span>  | <span data-ttu-id="10eb1-149">持有者&lt;令牌&gt;</span><span class="sxs-lookup"><span data-stu-id="10eb1-149">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="10eb1-150">Content-Type</span><span class="sxs-lookup"><span data-stu-id="10eb1-150">Content-Type</span></span>  | <span data-ttu-id="10eb1-151">application/json</span><span class="sxs-lookup"><span data-stu-id="10eb1-151">application/json</span></span> |
| <span data-ttu-id="10eb1-152">Prefer</span><span class="sxs-lookup"><span data-stu-id="10eb1-152">Prefer</span></span> | <span data-ttu-id="10eb1-153">return = 最小</span><span class="sxs-lookup"><span data-stu-id="10eb1-153">return=minimal</span></span> <br><br><span data-ttu-id="10eb1-154">如果使用使用 a 的`deltaLink`请求指定此标头, 则将仅返回自上一轮后已更改的对象属性。</span><span class="sxs-lookup"><span data-stu-id="10eb1-154">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="10eb1-155">可选。</span><span class="sxs-lookup"><span data-stu-id="10eb1-155">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="10eb1-156">请求正文</span><span class="sxs-lookup"><span data-stu-id="10eb1-156">Request body</span></span>
<span data-ttu-id="10eb1-157">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="10eb1-157">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="10eb1-158">响应</span><span class="sxs-lookup"><span data-stu-id="10eb1-158">Response</span></span>

<span data-ttu-id="10eb1-159">如果成功，此方法的响应正文返回`200 OK`响应代码和[用户](../resources/user.md)集合对象。</span><span class="sxs-lookup"><span data-stu-id="10eb1-159">If successful, this method returns `200 OK` response code and [user](../resources/user.md) collection object in the response body.</span></span> <span data-ttu-id="10eb1-160">该响应还包括`nextLink` url 或`deltaLink` url。</span><span class="sxs-lookup"><span data-stu-id="10eb1-160">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="10eb1-161">如果返回`nextLink` URL:</span><span class="sxs-lookup"><span data-stu-id="10eb1-161">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="10eb1-162">这表示在会话中有要检索的其他数据页。</span><span class="sxs-lookup"><span data-stu-id="10eb1-162">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="10eb1-163">应用程序将继续使用`nextLink` URL 发出请求, 直到`deltaLink`响应中包含 url 为止。</span><span class="sxs-lookup"><span data-stu-id="10eb1-163">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="10eb1-164">响应包含与初始 delta 查询请求中相同的属性集。</span><span class="sxs-lookup"><span data-stu-id="10eb1-164">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="10eb1-165">这使您可以在启动增量循环时捕获对象的完整当前状态。</span><span class="sxs-lookup"><span data-stu-id="10eb1-165">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="10eb1-166">如果返回`deltaLink` URL:</span><span class="sxs-lookup"><span data-stu-id="10eb1-166">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="10eb1-167">这表示没有更多有关要返回的资源的现有状态的数据。</span><span class="sxs-lookup"><span data-stu-id="10eb1-167">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="10eb1-168">保存并使用`deltaLink` URL, 了解下一轮中对资源的更改。</span><span class="sxs-lookup"><span data-stu-id="10eb1-168">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="10eb1-169">您可以选择指定`Prefer:return=minimal`标头, 以便仅将自发出以来`deltaLink`发生更改的属性的响应值包括在响应值中。</span><span class="sxs-lookup"><span data-stu-id="10eb1-169">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="10eb1-170">默认值: 返回与初始 delta 请求相同的属性</span><span class="sxs-lookup"><span data-stu-id="10eb1-170">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="10eb1-171">默认情况下, 请求使用`deltaLink`或`nextLink`返回在初始 delta 查询中以下列方式选择的相同属性:</span><span class="sxs-lookup"><span data-stu-id="10eb1-171">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="10eb1-172">如果属性已更改, 则新值将包含在响应中。</span><span class="sxs-lookup"><span data-stu-id="10eb1-172">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="10eb1-173">这包括设置为 null 值的属性。</span><span class="sxs-lookup"><span data-stu-id="10eb1-173">This includes properties being set to null value.</span></span>
- <span data-ttu-id="10eb1-174">如果该属性未更改, 则响应中将包含旧值。</span><span class="sxs-lookup"><span data-stu-id="10eb1-174">If the property has not changed, the old value is included in the response.</span></span>
- <span data-ttu-id="10eb1-175">如果从未设置该属性, 则根本不会将其包含在响应中。</span><span class="sxs-lookup"><span data-stu-id="10eb1-175">If the property has never been set before it will not be included in the response at all.</span></span>


> <span data-ttu-id="10eb1-176">**注意:** 在这种情况下, 通过查看响应, 无法判断属性是否正在更改。</span><span class="sxs-lookup"><span data-stu-id="10eb1-176">**Note:** With this behavior, by looking at the response it is not possible to tell whether a property is changing or not.</span></span> <span data-ttu-id="10eb1-177">此外, 由于增量响应包含所有属性值 (如下面的[第二个示例](#request-2)所示), 因此它们会变大。</span><span class="sxs-lookup"><span data-stu-id="10eb1-177">Also, the delta responses tend to be large because they contain all property values  - as shown in the [second example](#request-2) below.</span></span>

#### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="10eb1-178">替代方法: 仅返回更改的属性</span><span class="sxs-lookup"><span data-stu-id="10eb1-178">Alternative: return only the changed properties</span></span>

<span data-ttu-id="10eb1-179">添加可选请求标头- `prefer:return=minimal` -导致以下行为:</span><span class="sxs-lookup"><span data-stu-id="10eb1-179">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="10eb1-180">如果属性已更改, 则新值将包含在响应中。</span><span class="sxs-lookup"><span data-stu-id="10eb1-180">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="10eb1-181">这包括设置为 null 值的属性。</span><span class="sxs-lookup"><span data-stu-id="10eb1-181">This includes properties being set to null value.</span></span>
- <span data-ttu-id="10eb1-182">如果该属性未更改, 则该属性根本不包含在响应中。</span><span class="sxs-lookup"><span data-stu-id="10eb1-182">If the property has not changed, the property is not included in the response at all.</span></span> <span data-ttu-id="10eb1-183">(与默认行为不同。)</span><span class="sxs-lookup"><span data-stu-id="10eb1-183">(Different from the default behavior.)</span></span>

> <span data-ttu-id="10eb1-184">**注意:** 可以在增量循环中的任何`deltaLink`时间点将标头添加到请求中。</span><span class="sxs-lookup"><span data-stu-id="10eb1-184">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="10eb1-185">标头只会影响响应中包含的一组属性, 而不会影响增量查询的执行方式。</span><span class="sxs-lookup"><span data-stu-id="10eb1-185">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span> <span data-ttu-id="10eb1-186">请参阅下面的[第三个示例](#request-3)。</span><span class="sxs-lookup"><span data-stu-id="10eb1-186">See the [third example](#request-3) below.</span></span>

### <a name="example"></a><span data-ttu-id="10eb1-187">示例</span><span class="sxs-lookup"><span data-stu-id="10eb1-187">Example</span></span>

#### <a name="request-1"></a><span data-ttu-id="10eb1-188">请求 1</span><span class="sxs-lookup"><span data-stu-id="10eb1-188">Request 1</span></span>

<span data-ttu-id="10eb1-189">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="10eb1-189">The following is an example of the request.</span></span> <span data-ttu-id="10eb1-190">没有`$select`参数, 因此会跟踪并返回默认的属性集。</span><span class="sxs-lookup"><span data-stu-id="10eb1-190">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/beta/users/delta
```

#### <a name="response-1"></a><span data-ttu-id="10eb1-191">响应 1</span><span class="sxs-lookup"><span data-stu-id="10eb1-191">Response 1</span></span>

<span data-ttu-id="10eb1-192">以下是使用`deltaLink`从查询初始化获取的响应的示例。</span><span class="sxs-lookup"><span data-stu-id="10eb1-192">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span>

><span data-ttu-id="10eb1-193">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="10eb1-193">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="10eb1-194">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="10eb1-194">All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/beta/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
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

#### <a name="request-2"></a><span data-ttu-id="10eb1-195">请求 2</span><span class="sxs-lookup"><span data-stu-id="10eb1-195">Request 2</span></span>

<span data-ttu-id="10eb1-196">下一个示例显示了使用默认响应行为选择3个属性进行更改跟踪的初始请求:</span><span class="sxs-lookup"><span data-stu-id="10eb1-196">The next example shows the initial request selecting 3 properties for change tracking, with default response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/beta/users/delta?$select=displayName,jobTitle,mobilePhone
```

#### <a name="response-2"></a><span data-ttu-id="10eb1-197">响应 2</span><span class="sxs-lookup"><span data-stu-id="10eb1-197">Response 2</span></span>

<span data-ttu-id="10eb1-198">以下是使用`deltaLink`从查询初始化获取的响应的示例。</span><span class="sxs-lookup"><span data-stu-id="10eb1-198">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="10eb1-199">请注意, 所有3个属性都包含在响应中, 并且不知道是在获取之后`deltaLink`更改的。</span><span class="sxs-lookup"><span data-stu-id="10eb1-199">Note that all 3 properties are included in the response and it is not known which ones have changed since the `deltaLink` was obtained.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/beta/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "jobTitle": "jobTitle-value",
      "mobilePhone": null
    }
  ]
}
```

#### <a name="request-3"></a><span data-ttu-id="10eb1-200">请求 3</span><span class="sxs-lookup"><span data-stu-id="10eb1-200">Request 3</span></span>

<span data-ttu-id="10eb1-201">下一个示例显示了使用替代最小响应行为选择3个更改跟踪属性的初始请求:</span><span class="sxs-lookup"><span data-stu-id="10eb1-201">The next example shows the initial request selecting 3 properties for change tracking, with alternative minimal response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/beta/users/delta?$select=displayName,jobTitle,mobilePhone
Prefer: return=minimal
```

#### <a name="response-3"></a><span data-ttu-id="10eb1-202">响应 3</span><span class="sxs-lookup"><span data-stu-id="10eb1-202">Response 3</span></span>

<span data-ttu-id="10eb1-203">以下是使用`deltaLink`从查询初始化获取的响应的示例。</span><span class="sxs-lookup"><span data-stu-id="10eb1-203">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="10eb1-204">请注意, `mobilePhone`该属性不包括在内, 这意味着自上次增量查询以来它尚未发生更改;`displayName`并`jobTitle`将其包括在内, 这意味着它们的值已更改。</span><span class="sxs-lookup"><span data-stu-id="10eb1-204">Note that the `mobilePhone` property is not included, which means it has not changed since the last delta query; `displayName` and `jobTitle` are included which means their values have changed.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/beta/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "jobTitle": null
    }
  ]
}
```

- <span data-ttu-id="10eb1-205">[使用 delta 查询跟踪 Microsoft Graph 数据中的更改](/graph/delta-query-overview)。</span><span class="sxs-lookup"><span data-stu-id="10eb1-205">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>
- <span data-ttu-id="10eb1-206">[获取用户的增量更改](/graph/delta-query-users)。</span><span class="sxs-lookup"><span data-stu-id="10eb1-206">[Get incremental changes for users](/graph/delta-query-users).</span></span>

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
    "Error: /api-reference/beta/api/user-delta.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
