---
title: oauth2permissiongrant： delta
description: 在不执行整个资源集合的完全读取的情况下，获取新创建、更新或删除的 oauth2permissiongrants。
localization_priority: Normal
author: psignoret
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 64ac1a599051b08922a8f0a7c7b5b21a8553d265
ms.sourcegitcommit: d14e2abb24d9fbab519458b1c9fec890a5e51d70
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2020
ms.locfileid: "43543456"
---
# <a name="oauth2permissiongrant-delta"></a><span data-ttu-id="69fc0-103">oauth2permissiongrant： delta</span><span class="sxs-lookup"><span data-stu-id="69fc0-103">oauth2permissiongrant: delta</span></span>

<span data-ttu-id="69fc0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69fc0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69fc0-105">获取新创建、更新或删除的**oauth2permissiongrant**对象，而不执行整个资源集合的完全读取。</span><span class="sxs-lookup"><span data-stu-id="69fc0-105">Get newly created, updated, or deleted **oauth2permissiongrant** objects without performing a full read of the entire resource collection.</span></span> <span data-ttu-id="69fc0-106">有关详细信息，请参阅[Using delta query](/graph/delta-query-overview)。</span><span class="sxs-lookup"><span data-stu-id="69fc0-106">For details, see [Using delta query](/graph/delta-query-overview).</span></span>

## <a name="permissions"></a><span data-ttu-id="69fc0-107">权限</span><span class="sxs-lookup"><span data-stu-id="69fc0-107">Permissions</span></span>

<span data-ttu-id="69fc0-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="69fc0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="69fc0-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="69fc0-110">Permission type</span></span>      | <span data-ttu-id="69fc0-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="69fc0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="69fc0-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="69fc0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="69fc0-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="69fc0-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="69fc0-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="69fc0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69fc0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="69fc0-115">Not supported.</span></span>    |
|<span data-ttu-id="69fc0-116">oauth2permissiongrant</span><span class="sxs-lookup"><span data-stu-id="69fc0-116">oauth2permissiongrant</span></span> | <span data-ttu-id="69fc0-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69fc0-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="69fc0-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="69fc0-118">HTTP request</span></span>

<span data-ttu-id="69fc0-119">若要开始跟踪更改，请在**oauth2permissiongrant**资源上发出包含 delta 函数的请求。</span><span class="sxs-lookup"><span data-stu-id="69fc0-119">To begin tracking changes, you make a request including the delta function on the **oauth2permissiongrant** resource.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /oauth2permissiongrants/delta
```

## <a name="query-parameters"></a><span data-ttu-id="69fc0-120">查询参数</span><span class="sxs-lookup"><span data-stu-id="69fc0-120">Query parameters</span></span>

<span data-ttu-id="69fc0-121">跟踪更改会产生一个或多个**delta**函数调用的往返。</span><span class="sxs-lookup"><span data-stu-id="69fc0-121">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="69fc0-122">如果要使用任意查询参数（`$deltatoken` 和 `$skiptoken` 除外），则必须在最初的 **delta** 请求中指定它。</span><span class="sxs-lookup"><span data-stu-id="69fc0-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="69fc0-123">Microsoft Graph 自动将指定的任意参数编码为响应中提供的 `nextLink` 或 `deltaLink` URL 的令牌部分。</span><span class="sxs-lookup"><span data-stu-id="69fc0-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="69fc0-124">您只需提前指定任何查询参数。</span><span class="sxs-lookup"><span data-stu-id="69fc0-124">You only need to specify any query parameters once up front.</span></span> <span data-ttu-id="69fc0-125">在后续请求中，复制并应用`nextLink`上`deltaLink`一个响应中的或 URL。</span><span class="sxs-lookup"><span data-stu-id="69fc0-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response.</span></span> <span data-ttu-id="69fc0-126">该 URL 已包含已编码的参数。</span><span class="sxs-lookup"><span data-stu-id="69fc0-126">That URL already includes the encoded parameters.</span></span>

| <span data-ttu-id="69fc0-127">查询参数</span><span class="sxs-lookup"><span data-stu-id="69fc0-127">Query parameter</span></span>      | <span data-ttu-id="69fc0-128">类型</span><span class="sxs-lookup"><span data-stu-id="69fc0-128">Type</span></span>   |<span data-ttu-id="69fc0-129">说明</span><span class="sxs-lookup"><span data-stu-id="69fc0-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="69fc0-130">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="69fc0-130">$deltatoken</span></span> | <span data-ttu-id="69fc0-131">string</span><span class="sxs-lookup"><span data-stu-id="69fc0-131">string</span></span> | <span data-ttu-id="69fc0-132">为同一资源集合在上`deltaLink`一个**delta**函数调用的 URL 中返回的[状态令牌](/graph/delta-query-overview)，指示该往返一轮的更改。</span><span class="sxs-lookup"><span data-stu-id="69fc0-132">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="69fc0-133">在对该集合的`deltaLink`下一轮变更跟踪的第一个请求中，保存并应用整个 URL （包括此令牌）。</span><span class="sxs-lookup"><span data-stu-id="69fc0-133">Save and apply the entire `deltaLink` URL, including this token, in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="69fc0-134">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="69fc0-134">$skiptoken</span></span> | <span data-ttu-id="69fc0-135">string</span><span class="sxs-lookup"><span data-stu-id="69fc0-135">string</span></span> | <span data-ttu-id="69fc0-136">在上一个**delta**函数调用`nextLink`的 URL 中返回的[状态令牌](/graph/delta-query-overview)，指示在同一资源集合中有进一步的更改需要跟踪。</span><span class="sxs-lookup"><span data-stu-id="69fc0-136">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating that there are further changes to be tracked in the same resource collection.</span></span> |

### <a name="optional-query-parameters"></a><span data-ttu-id="69fc0-137">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="69fc0-137">Optional query parameters</span></span>

<span data-ttu-id="69fc0-138">此方法支持 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="69fc0-138">This method supports OData query parameters to help customize the response.</span></span>

- <span data-ttu-id="69fc0-p105">像在任何 GET 请求中一样，你可以使用 `$select` 查询参数以仅指定获取最佳性能所需的属性。始终返回 **id** 属性。</span><span class="sxs-lookup"><span data-stu-id="69fc0-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The **id** property is always returned.</span></span>
- <span data-ttu-id="69fc0-141">提供对 `$filter` 的有限支持：</span><span class="sxs-lookup"><span data-stu-id="69fc0-141">There is limited support for `$filter`:</span></span>
  * <span data-ttu-id="69fc0-142">唯一受支持`$filter`的表达式是跟踪对特定资源所做的更改，其`$filter=id+eq+{value}` ID `$filter=id+eq+{value1}+or+id+eq+{value2}`：或。</span><span class="sxs-lookup"><span data-stu-id="69fc0-142">The only supported `$filter` expression is for tracking changes for specific resources, by their ID:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="69fc0-143">您可以指定的 Id 数受最大 URL 长度的限制。</span><span class="sxs-lookup"><span data-stu-id="69fc0-143">The number of IDs you can specify is limited by the maximum URL length.</span></span>


## <a name="request-headers"></a><span data-ttu-id="69fc0-144">请求标头</span><span class="sxs-lookup"><span data-stu-id="69fc0-144">Request headers</span></span>
| <span data-ttu-id="69fc0-145">名称</span><span class="sxs-lookup"><span data-stu-id="69fc0-145">Name</span></span>       | <span data-ttu-id="69fc0-146">说明</span><span class="sxs-lookup"><span data-stu-id="69fc0-146">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="69fc0-147">Authorization</span><span class="sxs-lookup"><span data-stu-id="69fc0-147">Authorization</span></span>  | <span data-ttu-id="69fc0-148">持有者 &lt;token&gt;。</span><span class="sxs-lookup"><span data-stu-id="69fc0-148">Bearer &lt;token&gt;.</span></span> <span data-ttu-id="69fc0-149">必需。</span><span class="sxs-lookup"><span data-stu-id="69fc0-149">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="69fc0-150">请求正文</span><span class="sxs-lookup"><span data-stu-id="69fc0-150">Request body</span></span>
<span data-ttu-id="69fc0-151">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="69fc0-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="69fc0-152">响应</span><span class="sxs-lookup"><span data-stu-id="69fc0-152">Response</span></span>

<span data-ttu-id="69fc0-153">如果成功，此方法在响应`200 OK`正文中返回响应代码和[oauth2permissiongrant](../resources/oauth2permissiongrant.md)集合对象。</span><span class="sxs-lookup"><span data-stu-id="69fc0-153">If successful, this method returns a `200 OK` response code and an [oauth2permissiongrant](../resources/oauth2permissiongrant.md) collection object in the response body.</span></span> <span data-ttu-id="69fc0-154">该响应还包括 `nextLink`URL 或 `deltaLink`URL。</span><span class="sxs-lookup"><span data-stu-id="69fc0-154">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="69fc0-155">如果返回`nextLink` URL，则会在会话中检索其他数据页。</span><span class="sxs-lookup"><span data-stu-id="69fc0-155">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="69fc0-156">**Oauth2permissiongrant**继续使用`nextLink` URL 发出请求，直到响应中`deltaLink`包含 url 为止。</span><span class="sxs-lookup"><span data-stu-id="69fc0-156">The **oauth2permissiongrant** continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
- <span data-ttu-id="69fc0-157">如果返回`deltaLink` URL，则没有有关要返回的资源的现有状态的更多数据。</span><span class="sxs-lookup"><span data-stu-id="69fc0-157">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="69fc0-158">保留并使用`deltaLink` URL 了解将来对资源所做的更改。</span><span class="sxs-lookup"><span data-stu-id="69fc0-158">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="69fc0-159">有关详细信息，请参阅[Using delta query](/graph/delta-query-overview)。</span><span class="sxs-lookup"><span data-stu-id="69fc0-159">For details, see [Using delta query](/graph/delta-query-overview).</span></span> <span data-ttu-id="69fc0-160">有关示例请求，请参阅[获取用户的增量更改](/graph/delta-query-users)。</span><span class="sxs-lookup"><span data-stu-id="69fc0-160">For example requests, see [Get incremental changes for users](/graph/delta-query-users).</span></span>

## <a name="example"></a><span data-ttu-id="69fc0-161">示例</span><span class="sxs-lookup"><span data-stu-id="69fc0-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="69fc0-162">请求</span><span class="sxs-lookup"><span data-stu-id="69fc0-162">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="69fc0-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="69fc0-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "oauth2permissiongrant_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/oauth2permissiongrants/delta
```

### <a name="response"></a><span data-ttu-id="69fc0-164">响应</span><span class="sxs-lookup"><span data-stu-id="69fc0-164">Response</span></span>
><span data-ttu-id="69fc0-p112">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="69fc0-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
