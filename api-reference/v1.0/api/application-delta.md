---
title: application： delta
description: 无需执行整个资源集合的完整读取，即可创建、更新或删除应用程序。
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 8640221a136d6b19391e146b4d3d24a5a7daa974
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132517"
---
# <a name="application-delta"></a><span data-ttu-id="63e76-103">application： delta</span><span class="sxs-lookup"><span data-stu-id="63e76-103">application: delta</span></span>

<span data-ttu-id="63e76-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63e76-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="63e76-105">获得新建、更新或删除的应用，无需完全读取整个资源集合。</span><span class="sxs-lookup"><span data-stu-id="63e76-105">Get newly created, updated, or deleted applications without performing a full read of the entire resource collection.</span></span> <span data-ttu-id="63e76-106">有关详细信息，请参阅使用 [delta 查询](/graph/delta-query-overview)。</span><span class="sxs-lookup"><span data-stu-id="63e76-106">For details, see [Using delta query](/graph/delta-query-overview).</span></span>

## <a name="permissions"></a><span data-ttu-id="63e76-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="63e76-107">Permissions</span></span>

<span data-ttu-id="63e76-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="63e76-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="63e76-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="63e76-110">Permission type</span></span>      | <span data-ttu-id="63e76-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="63e76-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="63e76-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="63e76-112">Delegated (work or school account)</span></span> | <span data-ttu-id="63e76-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="63e76-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="63e76-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="63e76-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63e76-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="63e76-115">Not supported.</span></span>    |
|<span data-ttu-id="63e76-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="63e76-116">Application</span></span> | <span data-ttu-id="63e76-117">Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="63e76-117">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="63e76-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="63e76-118">HTTP request</span></span>

<span data-ttu-id="63e76-119">若要开始跟踪更改，请对应用程序资源提出包含 delta 函数 **的请求** 。</span><span class="sxs-lookup"><span data-stu-id="63e76-119">To begin tracking changes, you make a request including the delta function on the **application** resource.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /applications/delta
```

## <a name="query-parameters"></a><span data-ttu-id="63e76-120">查询参数</span><span class="sxs-lookup"><span data-stu-id="63e76-120">Query parameters</span></span>

<span data-ttu-id="63e76-121">跟踪更改会导致一次或多 **组 delta** 函数调用。</span><span class="sxs-lookup"><span data-stu-id="63e76-121">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="63e76-122">如果要使用任意查询参数（`$deltatoken` 和 `$skiptoken` 除外），则必须在最初的 **delta** 请求中指定它。</span><span class="sxs-lookup"><span data-stu-id="63e76-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="63e76-123">Microsoft Graph 自动将指定的任意参数编码为响应中提供的 `nextLink` 或 `deltaLink` URL 的令牌部分。</span><span class="sxs-lookup"><span data-stu-id="63e76-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="63e76-124">只需指定任何查询参数一次。</span><span class="sxs-lookup"><span data-stu-id="63e76-124">You only need to specify any query parameters once up front.</span></span> <span data-ttu-id="63e76-125">在后续请求中，复制并应用上一响应 `nextLink` `deltaLink` 中的或 URL。</span><span class="sxs-lookup"><span data-stu-id="63e76-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response.</span></span> <span data-ttu-id="63e76-126">该 URL 已包含编码参数。</span><span class="sxs-lookup"><span data-stu-id="63e76-126">That URL already includes the encoded parameters.</span></span>

| <span data-ttu-id="63e76-127">查询参数</span><span class="sxs-lookup"><span data-stu-id="63e76-127">Query parameter</span></span>      | <span data-ttu-id="63e76-128">类型</span><span class="sxs-lookup"><span data-stu-id="63e76-128">Type</span></span>   |<span data-ttu-id="63e76-129">说明</span><span class="sxs-lookup"><span data-stu-id="63e76-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="63e76-130">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="63e76-130">$deltatoken</span></span> | <span data-ttu-id="63e76-131">string</span><span class="sxs-lookup"><span data-stu-id="63e76-131">string</span></span> | <span data-ttu-id="63e76-132">对[同一](/graph/delta-query-overview)资源集合的上一个 delta 函数调用的 URL 中返回的状态令牌，指示完成这一轮 `deltaLink` 更改跟踪。 </span><span class="sxs-lookup"><span data-stu-id="63e76-132">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="63e76-133">将此令牌包含在对该集合的下一组更改追踪的首次请求中，并保存和应用整个 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="63e76-133">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="63e76-134">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="63e76-134">$skiptoken</span></span> | <span data-ttu-id="63e76-135">string</span><span class="sxs-lookup"><span data-stu-id="63e76-135">string</span></span> | <span data-ttu-id="63e76-136">在[上一](/graph/delta-query-overview)个 delta 函数调用的 URL 中返回的状态令牌，指示同一资源集合中还有要跟踪的进一 `nextLink` 步更改。 </span><span class="sxs-lookup"><span data-stu-id="63e76-136">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating that there are further changes to be tracked in the same resource collection.</span></span> |

### <a name="optional-query-parameters"></a><span data-ttu-id="63e76-137">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="63e76-137">Optional query parameters</span></span>

<span data-ttu-id="63e76-138">此方法支持 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="63e76-138">This method supports OData query parameters to help customize the response.</span></span>

- <span data-ttu-id="63e76-p105">像在任何 GET 请求中一样，你可以使用 `$select` 查询参数以仅指定获取最佳性能所需的属性。始终返回 **id** 属性。</span><span class="sxs-lookup"><span data-stu-id="63e76-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The **id** property is always returned.</span></span>
- <span data-ttu-id="63e76-141">提供对 `$filter` 的有限支持：</span><span class="sxs-lookup"><span data-stu-id="63e76-141">There is limited support for `$filter`:</span></span>
  * <span data-ttu-id="63e76-142">唯一 `$filter` 受支持的表达式用于按其 ID 或跟踪特定资源的  `$filter=id+eq+{value}` 更改 `$filter=id+eq+{value1}+or+id+eq+{value2}` 。</span><span class="sxs-lookup"><span data-stu-id="63e76-142">The only supported `$filter` expression is for tracking changes for specific resources, by their ID:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="63e76-143">可以指定的 ID 数受最大 URL 长度限制。</span><span class="sxs-lookup"><span data-stu-id="63e76-143">The number of IDs you can specify is limited by the maximum URL length.</span></span>


## <a name="request-headers"></a><span data-ttu-id="63e76-144">请求标头</span><span class="sxs-lookup"><span data-stu-id="63e76-144">Request headers</span></span>
| <span data-ttu-id="63e76-145">名称</span><span class="sxs-lookup"><span data-stu-id="63e76-145">Name</span></span>       | <span data-ttu-id="63e76-146">说明</span><span class="sxs-lookup"><span data-stu-id="63e76-146">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="63e76-147">Authorization</span><span class="sxs-lookup"><span data-stu-id="63e76-147">Authorization</span></span>  | <span data-ttu-id="63e76-148">持有者 &lt;token&gt;。</span><span class="sxs-lookup"><span data-stu-id="63e76-148">Bearer &lt;token&gt;.</span></span> <span data-ttu-id="63e76-149">必填。</span><span class="sxs-lookup"><span data-stu-id="63e76-149">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="63e76-150">请求正文</span><span class="sxs-lookup"><span data-stu-id="63e76-150">Request body</span></span>
<span data-ttu-id="63e76-151">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="63e76-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63e76-152">响应</span><span class="sxs-lookup"><span data-stu-id="63e76-152">Response</span></span>

<span data-ttu-id="63e76-153">如果成功，此方法在响应正文中返回响应代码 `200 OK` 和应用程序集合对象。 [](../resources/application.md)</span><span class="sxs-lookup"><span data-stu-id="63e76-153">If successful, this method returns a `200 OK` response code and an [application](../resources/application.md) collection object in the response body.</span></span> <span data-ttu-id="63e76-154">该响应还包括 `nextLink`URL 或 `deltaLink`URL。</span><span class="sxs-lookup"><span data-stu-id="63e76-154">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="63e76-155">如果 `nextLink` 返回 URL，则会话中有其他要检索的数据页。</span><span class="sxs-lookup"><span data-stu-id="63e76-155">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="63e76-156">应用程序继续使用 `nextLink` URL 发出请求，直到响应中包含 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="63e76-156">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
- <span data-ttu-id="63e76-157">如果 `deltaLink` 返回 URL，则不再返回有关资源现有状态的数据。</span><span class="sxs-lookup"><span data-stu-id="63e76-157">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="63e76-158">保留并使用 `deltaLink` URL 了解将来对资源的更改。</span><span class="sxs-lookup"><span data-stu-id="63e76-158">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="63e76-159">有关详细信息，请参阅使用 [delta 查询](/graph/delta-query-overview)。</span><span class="sxs-lookup"><span data-stu-id="63e76-159">For details, see [Using delta query](/graph/delta-query-overview).</span></span> <span data-ttu-id="63e76-160">有关示例请求，请参阅"[获取用户的增量更改"。](/graph/delta-query-users)</span><span class="sxs-lookup"><span data-stu-id="63e76-160">For example requests, see [Get incremental changes for users](/graph/delta-query-users).</span></span>

## <a name="example"></a><span data-ttu-id="63e76-161">示例</span><span class="sxs-lookup"><span data-stu-id="63e76-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="63e76-162">请求</span><span class="sxs-lookup"><span data-stu-id="63e76-162">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="63e76-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="63e76-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications/delta
```
# <a name="c"></a>[<span data-ttu-id="63e76-164">C#</span><span class="sxs-lookup"><span data-stu-id="63e76-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="63e76-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="63e76-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="63e76-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="63e76-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="63e76-167">Java</span><span class="sxs-lookup"><span data-stu-id="63e76-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="63e76-168">响应</span><span class="sxs-lookup"><span data-stu-id="63e76-168">Response</span></span>
><span data-ttu-id="63e76-p112">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="63e76-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

