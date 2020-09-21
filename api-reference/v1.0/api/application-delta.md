---
title: 应用程序： delta
description: 获取已创建、更新或删除的应用程序，而不执行整个资源集合的完全读取。
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ec119e193cbfc2cb7ea1c0294bc7d40ecb9900f8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47966511"
---
# <a name="application-delta"></a><span data-ttu-id="db90c-103">应用程序： delta</span><span class="sxs-lookup"><span data-stu-id="db90c-103">application: delta</span></span>

<span data-ttu-id="db90c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db90c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="db90c-105">获得新建、更新或删除的应用，无需完全读取整个资源集合。</span><span class="sxs-lookup"><span data-stu-id="db90c-105">Get newly created, updated, or deleted applications without performing a full read of the entire resource collection.</span></span> <span data-ttu-id="db90c-106">有关详细信息，请参阅 [Using delta query](/graph/delta-query-overview)。</span><span class="sxs-lookup"><span data-stu-id="db90c-106">For details, see [Using delta query](/graph/delta-query-overview).</span></span>

## <a name="permissions"></a><span data-ttu-id="db90c-107">权限</span><span class="sxs-lookup"><span data-stu-id="db90c-107">Permissions</span></span>

<span data-ttu-id="db90c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="db90c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="db90c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="db90c-110">Permission type</span></span>      | <span data-ttu-id="db90c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="db90c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db90c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="db90c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="db90c-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="db90c-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="db90c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="db90c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db90c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="db90c-115">Not supported.</span></span>    |
|<span data-ttu-id="db90c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="db90c-116">Application</span></span> | <span data-ttu-id="db90c-117">Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="db90c-117">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="db90c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="db90c-118">HTTP request</span></span>

<span data-ttu-id="db90c-119">若要开始跟踪更改，请在 **应用程序** 资源上发出包含 delta 函数的请求。</span><span class="sxs-lookup"><span data-stu-id="db90c-119">To begin tracking changes, you make a request including the delta function on the **application** resource.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /applications/delta
```

## <a name="query-parameters"></a><span data-ttu-id="db90c-120">查询参数</span><span class="sxs-lookup"><span data-stu-id="db90c-120">Query parameters</span></span>

<span data-ttu-id="db90c-121">跟踪更改会产生一个或多个 **delta** 函数调用的往返。</span><span class="sxs-lookup"><span data-stu-id="db90c-121">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="db90c-122">如果要使用任意查询参数（`$deltatoken` 和 `$skiptoken` 除外），则必须在最初的 **delta** 请求中指定它。</span><span class="sxs-lookup"><span data-stu-id="db90c-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="db90c-123">Microsoft Graph 自动将指定的任意参数编码为响应中提供的 `nextLink` 或 `deltaLink` URL 的令牌部分。</span><span class="sxs-lookup"><span data-stu-id="db90c-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="db90c-124">您只需提前指定任何查询参数。</span><span class="sxs-lookup"><span data-stu-id="db90c-124">You only need to specify any query parameters once up front.</span></span> <span data-ttu-id="db90c-125">在后续请求中，复制并应用 `nextLink` `deltaLink` 上一个响应中的或 URL。</span><span class="sxs-lookup"><span data-stu-id="db90c-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response.</span></span> <span data-ttu-id="db90c-126">该 URL 已包含已编码的参数。</span><span class="sxs-lookup"><span data-stu-id="db90c-126">That URL already includes the encoded parameters.</span></span>

| <span data-ttu-id="db90c-127">查询参数</span><span class="sxs-lookup"><span data-stu-id="db90c-127">Query parameter</span></span>      | <span data-ttu-id="db90c-128">类型</span><span class="sxs-lookup"><span data-stu-id="db90c-128">Type</span></span>   |<span data-ttu-id="db90c-129">说明</span><span class="sxs-lookup"><span data-stu-id="db90c-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="db90c-130">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="db90c-130">$deltatoken</span></span> | <span data-ttu-id="db90c-131">string</span><span class="sxs-lookup"><span data-stu-id="db90c-131">string</span></span> | <span data-ttu-id="db90c-132">[state token](/graph/delta-query-overview) `deltaLink` 为同一资源集合在上一个**delta**函数调用的 URL 中返回的状态令牌，指示该往返一轮的更改。</span><span class="sxs-lookup"><span data-stu-id="db90c-132">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="db90c-133">将此令牌包含在对该集合的下一组更改追踪的首次请求中，并保存和应用整个 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="db90c-133">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="db90c-134">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="db90c-134">$skiptoken</span></span> | <span data-ttu-id="db90c-135">string</span><span class="sxs-lookup"><span data-stu-id="db90c-135">string</span></span> | <span data-ttu-id="db90c-136">在上一个 delta 函数调用的 URL 中返回的[状态令牌](/graph/delta-query-overview) `nextLink` ，指示在同一资源集合中有进一步的更改需要跟踪。 **delta**</span><span class="sxs-lookup"><span data-stu-id="db90c-136">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating that there are further changes to be tracked in the same resource collection.</span></span> |

### <a name="optional-query-parameters"></a><span data-ttu-id="db90c-137">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="db90c-137">Optional query parameters</span></span>

<span data-ttu-id="db90c-138">此方法支持 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="db90c-138">This method supports OData query parameters to help customize the response.</span></span>

- <span data-ttu-id="db90c-p105">像在任何 GET 请求中一样，你可以使用 `$select` 查询参数以仅指定获取最佳性能所需的属性。始终返回 **id** 属性。</span><span class="sxs-lookup"><span data-stu-id="db90c-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The **id** property is always returned.</span></span>
- <span data-ttu-id="db90c-141">提供对 `$filter` 的有限支持：</span><span class="sxs-lookup"><span data-stu-id="db90c-141">There is limited support for `$filter`:</span></span>
  * <span data-ttu-id="db90c-142">唯一受支持的 `$filter` 表达式是跟踪对特定资源所做的更改，其 ID：  `$filter=id+eq+{value}` 或 `$filter=id+eq+{value1}+or+id+eq+{value2}` 。</span><span class="sxs-lookup"><span data-stu-id="db90c-142">The only supported `$filter` expression is for tracking changes for specific resources, by their ID:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="db90c-143">您可以指定的 Id 数受最大 URL 长度的限制。</span><span class="sxs-lookup"><span data-stu-id="db90c-143">The number of IDs you can specify is limited by the maximum URL length.</span></span>


## <a name="request-headers"></a><span data-ttu-id="db90c-144">请求标头</span><span class="sxs-lookup"><span data-stu-id="db90c-144">Request headers</span></span>
| <span data-ttu-id="db90c-145">名称</span><span class="sxs-lookup"><span data-stu-id="db90c-145">Name</span></span>       | <span data-ttu-id="db90c-146">说明</span><span class="sxs-lookup"><span data-stu-id="db90c-146">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="db90c-147">Authorization</span><span class="sxs-lookup"><span data-stu-id="db90c-147">Authorization</span></span>  | <span data-ttu-id="db90c-148">持有者 &lt;token&gt;。</span><span class="sxs-lookup"><span data-stu-id="db90c-148">Bearer &lt;token&gt;.</span></span> <span data-ttu-id="db90c-149">必需。</span><span class="sxs-lookup"><span data-stu-id="db90c-149">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="db90c-150">请求正文</span><span class="sxs-lookup"><span data-stu-id="db90c-150">Request body</span></span>
<span data-ttu-id="db90c-151">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="db90c-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db90c-152">响应</span><span class="sxs-lookup"><span data-stu-id="db90c-152">Response</span></span>

<span data-ttu-id="db90c-153">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [application](../resources/application.md) 集合对象。</span><span class="sxs-lookup"><span data-stu-id="db90c-153">If successful, this method returns a `200 OK` response code and an [application](../resources/application.md) collection object in the response body.</span></span> <span data-ttu-id="db90c-154">该响应还包括 `nextLink`URL 或 `deltaLink`URL。</span><span class="sxs-lookup"><span data-stu-id="db90c-154">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="db90c-155">如果 `nextLink` 返回 URL，则会在会话中检索其他数据页。</span><span class="sxs-lookup"><span data-stu-id="db90c-155">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="db90c-156">应用程序继续使用 `nextLink` URL 发出请求，直到响应中包含 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="db90c-156">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
- <span data-ttu-id="db90c-157">如果 `deltaLink` 返回 URL，则没有有关要返回的资源的现有状态的更多数据。</span><span class="sxs-lookup"><span data-stu-id="db90c-157">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="db90c-158">保留并使用 `deltaLink` URL 了解将来对资源所做的更改。</span><span class="sxs-lookup"><span data-stu-id="db90c-158">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="db90c-159">有关详细信息，请参阅 [Using delta query](/graph/delta-query-overview)。</span><span class="sxs-lookup"><span data-stu-id="db90c-159">For details, see [Using delta query](/graph/delta-query-overview).</span></span> <span data-ttu-id="db90c-160">有关示例请求，请参阅 [获取用户的增量更改](/graph/delta-query-users)。</span><span class="sxs-lookup"><span data-stu-id="db90c-160">For example requests, see [Get incremental changes for users](/graph/delta-query-users).</span></span>

## <a name="example"></a><span data-ttu-id="db90c-161">示例</span><span class="sxs-lookup"><span data-stu-id="db90c-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="db90c-162">请求</span><span class="sxs-lookup"><span data-stu-id="db90c-162">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="db90c-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="db90c-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications/delta
```
# <a name="c"></a>[<span data-ttu-id="db90c-164">C#</span><span class="sxs-lookup"><span data-stu-id="db90c-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="db90c-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db90c-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="db90c-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db90c-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="db90c-167">Java</span><span class="sxs-lookup"><span data-stu-id="db90c-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="db90c-168">响应</span><span class="sxs-lookup"><span data-stu-id="db90c-168">Response</span></span>
><span data-ttu-id="db90c-p112">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="db90c-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- { 
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true 
} --> 
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#applications",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/applications/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "api": {
        "acceptedAccessTokenVersion": 1,
        "publishedPermissionScopes": [
          {
            "adminConsentDescription": "adminConsentDescription-value",
            "adminConsentDisplayName": "adminConsentDisplayName-value",
            "id": "id-value",
            "isEnabled": true,
            "type": "type-value",
            "userConsentDescription": "userConsentDescription-value",
            "userConsentDisplayName": "userConsentDisplayName-value",
            "value": "value-value"
          }
        ]
      },
      "allowPublicClient": true,
      "applicationAliases": [
        "applicationAliases-value"
      ],
      "createdDateTime": "datetime-value",
      "installedClients": {
        "redirectUrls": [
          "redirectUrls-value"
        ]
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "application: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

