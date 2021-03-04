---
title: oauth2permissiongrant： delta
description: 获取新创建、更新或删除的 oauth2permissiongrants，而无需执行整个资源集合的完全读取。
localization_priority: Normal
author: psignoret
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: e4a4568dc143148597729e5b0981bda606649e27
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442386"
---
# <a name="oauth2permissiongrant-delta"></a><span data-ttu-id="8c496-103">oauth2permissiongrant： delta</span><span class="sxs-lookup"><span data-stu-id="8c496-103">oauth2permissiongrant: delta</span></span>

<span data-ttu-id="8c496-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c496-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c496-105">获取新创建、更新或删除的 **oauth2permissiongrant** 对象，而无需执行整个资源集合的完全读取。</span><span class="sxs-lookup"><span data-stu-id="8c496-105">Get newly created, updated, or deleted **oauth2permissiongrant** objects without performing a full read of the entire resource collection.</span></span> <span data-ttu-id="8c496-106">有关详细信息，请参阅使用 [delta 查询](/graph/delta-query-overview)。</span><span class="sxs-lookup"><span data-stu-id="8c496-106">For details, see [Using delta query](/graph/delta-query-overview).</span></span>

## <a name="permissions"></a><span data-ttu-id="8c496-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="8c496-107">Permissions</span></span>

<span data-ttu-id="8c496-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8c496-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8c496-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8c496-110">Permission type</span></span>      | <span data-ttu-id="8c496-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8c496-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c496-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8c496-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8c496-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8c496-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8c496-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8c496-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c496-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8c496-115">Not supported.</span></span>    |
|<span data-ttu-id="8c496-116">oauth2permissiongrant</span><span class="sxs-lookup"><span data-stu-id="8c496-116">oauth2permissiongrant</span></span> | <span data-ttu-id="8c496-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c496-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c496-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8c496-118">HTTP request</span></span>

<span data-ttu-id="8c496-119">若要开始跟踪更改，请对 **oauth2permissiongrant** 资源提出包含 delta 函数的请求。</span><span class="sxs-lookup"><span data-stu-id="8c496-119">To begin tracking changes, you make a request including the delta function on the **oauth2permissiongrant** resource.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /oauth2PermissionGrants/delta
```

## <a name="query-parameters"></a><span data-ttu-id="8c496-120">查询参数</span><span class="sxs-lookup"><span data-stu-id="8c496-120">Query parameters</span></span>

<span data-ttu-id="8c496-121">跟踪更改将引发一轮或多次 **delta** 函数调用。</span><span class="sxs-lookup"><span data-stu-id="8c496-121">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="8c496-122">如果要使用任意查询参数（`$deltatoken` 和 `$skiptoken` 除外），则必须在最初的 **delta** 请求中指定它。</span><span class="sxs-lookup"><span data-stu-id="8c496-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="8c496-123">Microsoft Graph 自动将指定的任意参数编码为响应中提供的 `nextLink` 或 `deltaLink` URL 的令牌部分。</span><span class="sxs-lookup"><span data-stu-id="8c496-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="8c496-124">只需指定任何查询参数一次。</span><span class="sxs-lookup"><span data-stu-id="8c496-124">You only need to specify any query parameters once up front.</span></span> <span data-ttu-id="8c496-125">在后续请求中，复制并应用 `nextLink` 上一 `deltaLink` 响应中的或 URL。</span><span class="sxs-lookup"><span data-stu-id="8c496-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response.</span></span> <span data-ttu-id="8c496-126">该 URL 已包含编码参数。</span><span class="sxs-lookup"><span data-stu-id="8c496-126">That URL already includes the encoded parameters.</span></span>

| <span data-ttu-id="8c496-127">查询参数</span><span class="sxs-lookup"><span data-stu-id="8c496-127">Query parameter</span></span>      | <span data-ttu-id="8c496-128">类型</span><span class="sxs-lookup"><span data-stu-id="8c496-128">Type</span></span>   |<span data-ttu-id="8c496-129">说明</span><span class="sxs-lookup"><span data-stu-id="8c496-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8c496-130">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="8c496-130">$deltatoken</span></span> | <span data-ttu-id="8c496-131">string</span><span class="sxs-lookup"><span data-stu-id="8c496-131">string</span></span> | <span data-ttu-id="8c496-132">同[一资源](/graph/delta-query-overview)集合的上一个 delta 函数调用的 URL 中返回的状态令牌，指示完成这一轮 `deltaLink` 更改跟踪。 </span><span class="sxs-lookup"><span data-stu-id="8c496-132">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="8c496-133">在集合的下一轮更改跟踪的第一个请求中保存和应用整个 `deltaLink` URL（包括此令牌）。</span><span class="sxs-lookup"><span data-stu-id="8c496-133">Save and apply the entire `deltaLink` URL, including this token, in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="8c496-134">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="8c496-134">$skiptoken</span></span> | <span data-ttu-id="8c496-135">string</span><span class="sxs-lookup"><span data-stu-id="8c496-135">string</span></span> | <span data-ttu-id="8c496-136">在[上一](/graph/delta-query-overview)个 delta 函数调用的 URL 中返回的状态令牌，指示同一资源集合中还有要跟踪的进一 `nextLink` 步更改。 </span><span class="sxs-lookup"><span data-stu-id="8c496-136">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating that there are further changes to be tracked in the same resource collection.</span></span> |

### <a name="optional-query-parameters"></a><span data-ttu-id="8c496-137">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8c496-137">Optional query parameters</span></span>

<span data-ttu-id="8c496-138">此方法支持 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8c496-138">This method supports OData query parameters to help customize the response.</span></span>

- <span data-ttu-id="8c496-p105">像在任何 GET 请求中一样，你可以使用 `$select` 查询参数以仅指定获取最佳性能所需的属性。始终返回 **id** 属性。</span><span class="sxs-lookup"><span data-stu-id="8c496-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The **id** property is always returned.</span></span>
- <span data-ttu-id="8c496-141">提供对 `$filter` 的有限支持：</span><span class="sxs-lookup"><span data-stu-id="8c496-141">There is limited support for `$filter`:</span></span>
  * <span data-ttu-id="8c496-142">唯一受支持的 `$filter` 表达式用于按其 ID 跟踪特定资源的更改：  `$filter=id+eq+{value}` 或 `$filter=id+eq+{value1}+or+id+eq+{value2}` 。</span><span class="sxs-lookup"><span data-stu-id="8c496-142">The only supported `$filter` expression is for tracking changes for specific resources, by their ID:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="8c496-143">可以指定的 ID 数受最大 URL 长度限制。</span><span class="sxs-lookup"><span data-stu-id="8c496-143">The number of IDs you can specify is limited by the maximum URL length.</span></span>


## <a name="request-headers"></a><span data-ttu-id="8c496-144">请求标头</span><span class="sxs-lookup"><span data-stu-id="8c496-144">Request headers</span></span>
| <span data-ttu-id="8c496-145">名称</span><span class="sxs-lookup"><span data-stu-id="8c496-145">Name</span></span>       | <span data-ttu-id="8c496-146">说明</span><span class="sxs-lookup"><span data-stu-id="8c496-146">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8c496-147">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c496-147">Authorization</span></span>  | <span data-ttu-id="8c496-148">持有者 &lt;token&gt;。</span><span class="sxs-lookup"><span data-stu-id="8c496-148">Bearer &lt;token&gt;.</span></span> <span data-ttu-id="8c496-149">必需。</span><span class="sxs-lookup"><span data-stu-id="8c496-149">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c496-150">请求正文</span><span class="sxs-lookup"><span data-stu-id="8c496-150">Request body</span></span>
<span data-ttu-id="8c496-151">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8c496-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c496-152">响应</span><span class="sxs-lookup"><span data-stu-id="8c496-152">Response</span></span>

<span data-ttu-id="8c496-153">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [oauth2permissiongrant](../resources/oauth2permissiongrant.md) 集合对象。</span><span class="sxs-lookup"><span data-stu-id="8c496-153">If successful, this method returns a `200 OK` response code and an [oauth2permissiongrant](../resources/oauth2permissiongrant.md) collection object in the response body.</span></span> <span data-ttu-id="8c496-154">该响应还包括 `nextLink`URL 或 `deltaLink`URL。</span><span class="sxs-lookup"><span data-stu-id="8c496-154">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="8c496-155">如果 `nextLink` 返回 URL，则会话中将检索其他数据页。</span><span class="sxs-lookup"><span data-stu-id="8c496-155">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="8c496-156">**oauth2permissiongrant** 继续使用 URL 提出请求，直到 `nextLink` `deltaLink` 响应中包括 URL。</span><span class="sxs-lookup"><span data-stu-id="8c496-156">The **oauth2permissiongrant** continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
- <span data-ttu-id="8c496-157">如果 `deltaLink` 返回 URL，则不再返回有关资源现有状态的数据。</span><span class="sxs-lookup"><span data-stu-id="8c496-157">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="8c496-158">保留并使用 `deltaLink` URL 了解将来对资源的更改。</span><span class="sxs-lookup"><span data-stu-id="8c496-158">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="8c496-159">有关详细信息，请参阅使用 [delta 查询](/graph/delta-query-overview)。</span><span class="sxs-lookup"><span data-stu-id="8c496-159">For details, see [Using delta query](/graph/delta-query-overview).</span></span> <span data-ttu-id="8c496-160">例如，请参阅"获取[用户的增量更改"。](/graph/delta-query-users)</span><span class="sxs-lookup"><span data-stu-id="8c496-160">For example requests, see [Get incremental changes for users](/graph/delta-query-users).</span></span>

## <a name="example"></a><span data-ttu-id="8c496-161">示例</span><span class="sxs-lookup"><span data-stu-id="8c496-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="8c496-162">请求</span><span class="sxs-lookup"><span data-stu-id="8c496-162">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8c496-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="8c496-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "oauth2permissiongrant_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/oauth2PermissionGrants/delta
```
# <a name="c"></a>[<span data-ttu-id="8c496-164">C#</span><span class="sxs-lookup"><span data-stu-id="8c496-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/oauth2permissiongrant-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8c496-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8c496-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/oauth2permissiongrant-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8c496-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8c496-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/oauth2permissiongrant-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8c496-167">Java</span><span class="sxs-lookup"><span data-stu-id="8c496-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/oauth2permissiongrant-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8c496-168">响应</span><span class="sxs-lookup"><span data-stu-id="8c496-168">Response</span></span>
><span data-ttu-id="8c496-p112">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8c496-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- { 
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant",
  "isCollection": true 
} --> 
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#oauth2permissiongrants",
  "@odata.nextLink":"https://graph.microsoft.com/beta/oauth2permissiongrants/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "clientId": "22a3c970-8ad4-4120-8127-300837f87f2c",
      "consentType": "Principal",
      "expiryTime": "2017-08-13T21:41:23.3929007Z",
      "principalId": "c2e8df37-c6a7-4d88-89b1-feb4f1fda7c5",
      "resourceId": "98dc9d95-49b6-405a-b3c0-834e969a708b",
      "scope": "User.Read Directory.AccessAsUser.All",
      "startTime": "0001-01-01T00:00:00Z",
      "id": "cMmjItSKIEGBJzAIN_h_LJWd3Ji2SVpAs8CDTpaacIs33-jCp8aITYmx_rTx_afF"
    }
  ]
}
```

<!-- uuid: ba679d55-d10e-4518-b733-6f3e9576afb1
2020-04-09 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oauth2permissiongrant: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


