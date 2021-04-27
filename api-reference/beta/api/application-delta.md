---
title: application： delta
description: 获取新建、更新或删除的应用程序，而无需执行整个资源集合的完整读取。 有关详细信息，请参阅使用增量查询。
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: c3bfedbfdd8aa13e27b3daa1aaf6da3c67c645b5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048125"
---
# <a name="application-delta"></a><span data-ttu-id="d3071-104">application： delta</span><span class="sxs-lookup"><span data-stu-id="d3071-104">application: delta</span></span>

<span data-ttu-id="d3071-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3071-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3071-106">获取新建、更新或删除的应用程序，而无需执行整个资源集合的完整读取。</span><span class="sxs-lookup"><span data-stu-id="d3071-106">Get newly created, updated, or deleted applications without having to perform a full read of the entire resource collection.</span></span> <span data-ttu-id="d3071-107">有关详细信息 [，请参阅使用增量](/graph/delta-query-overview) 查询。</span><span class="sxs-lookup"><span data-stu-id="d3071-107">See [Using Delta Query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="d3071-108">权限</span><span class="sxs-lookup"><span data-stu-id="d3071-108">Permissions</span></span>

<span data-ttu-id="d3071-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d3071-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d3071-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d3071-111">Permission type</span></span>      | <span data-ttu-id="d3071-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d3071-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d3071-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d3071-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d3071-114">Application.Read.All、Directory.Read.All、Application.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d3071-114">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="d3071-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d3071-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3071-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d3071-116">Not supported.</span></span>    |
|<span data-ttu-id="d3071-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d3071-117">Application</span></span> | <span data-ttu-id="d3071-118">Application.Read.All、 Directory.Read.All、 Application.ReadWrite.OwnedBy、 Application.ReadWrite.All、 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3071-118">Application.Read.All, Directory.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d3071-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d3071-119">HTTP request</span></span>

<span data-ttu-id="d3071-120">若要开始跟踪更改，请对应用程序资源提出包含 delta 函数的请求。</span><span class="sxs-lookup"><span data-stu-id="d3071-120">To begin tracking changes, you make a request including the delta function on the application resource.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /applications/delta
```

### <a name="query-parameters"></a><span data-ttu-id="d3071-121">查询参数</span><span class="sxs-lookup"><span data-stu-id="d3071-121">Query parameters</span></span>

<span data-ttu-id="d3071-122">跟踪更改将引发一次或多组 **delta** 函数调用。</span><span class="sxs-lookup"><span data-stu-id="d3071-122">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="d3071-123">如果要使用任意查询参数（`$deltatoken` 和 `$skiptoken` 除外），则必须在最初的 **delta** 请求中指定它。</span><span class="sxs-lookup"><span data-stu-id="d3071-123">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="d3071-124">Microsoft Graph 自动将指定的任意参数编码为响应中提供的 `nextLink` 或 `deltaLink` URL 的令牌部分。</span><span class="sxs-lookup"><span data-stu-id="d3071-124">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="d3071-125">只需预先指定所需的任何查询参数一次。</span><span class="sxs-lookup"><span data-stu-id="d3071-125">You only need to specify any desired query parameters once upfront.</span></span> <span data-ttu-id="d3071-126">在后续请求中，可以复制并应用之前响应中返回的 `nextLink` 或 `deltaLink` URL，因为此 URL 已包含所需的编码参数。</span><span class="sxs-lookup"><span data-stu-id="d3071-126">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="d3071-127">查询参数</span><span class="sxs-lookup"><span data-stu-id="d3071-127">Query parameter</span></span>      | <span data-ttu-id="d3071-128">类型</span><span class="sxs-lookup"><span data-stu-id="d3071-128">Type</span></span>   |<span data-ttu-id="d3071-129">说明</span><span class="sxs-lookup"><span data-stu-id="d3071-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d3071-130">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="d3071-130">$deltatoken</span></span> | <span data-ttu-id="d3071-131">string</span><span class="sxs-lookup"><span data-stu-id="d3071-131">string</span></span> | <span data-ttu-id="d3071-132">对[同一](/graph/delta-query-overview)资源集合之前的 delta 函数调用的 URL 中返回的状态令牌，指示完成这一轮 `deltaLink` 更改跟踪。 </span><span class="sxs-lookup"><span data-stu-id="d3071-132">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="d3071-133">将此令牌包含在对该集合的下一组更改追踪的首次请求中，并保存和应用整个 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="d3071-133">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="d3071-134">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="d3071-134">$skiptoken</span></span> | <span data-ttu-id="d3071-135">string</span><span class="sxs-lookup"><span data-stu-id="d3071-135">string</span></span> | <span data-ttu-id="d3071-136">之前的[delta](/graph/delta-query-overview)函数调用的 URL 中返回的状态令牌，指示同一资源集合中还有进一 `nextLink` 步的更改需要跟踪。 </span><span class="sxs-lookup"><span data-stu-id="d3071-136">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same resource collection.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="d3071-137">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d3071-137">Optional query parameters</span></span>

<span data-ttu-id="d3071-138">此方法支持 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d3071-138">This method supports OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="d3071-p106">像在任何 GET 请求中一样，你可以使用 `$select` 查询参数以仅指定获取最佳性能所需的属性。始终返回 _id_ 属性。</span><span class="sxs-lookup"><span data-stu-id="d3071-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 

- <span data-ttu-id="d3071-141">提供对 `$filter` 的有限支持：</span><span class="sxs-lookup"><span data-stu-id="d3071-141">There is limited support for `$filter`:</span></span>
  * <span data-ttu-id="d3071-142">唯一 `$filter` 受支持的表达式用于按 id： 或 跟踪特定资源的  `$filter=id+eq+{value}` 更改 `$filter=id+eq+{value1}+or+id+eq+{value2}` 。</span><span class="sxs-lookup"><span data-stu-id="d3071-142">The only supported `$filter` expression is for tracking changes for specific resources, by their id:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="d3071-143">可以指定的 ID 数受最大 URL 长度限制。</span><span class="sxs-lookup"><span data-stu-id="d3071-143">The number of ids you can specify is limited by the maximum URL length.</span></span>


## <a name="request-headers"></a><span data-ttu-id="d3071-144">请求标头</span><span class="sxs-lookup"><span data-stu-id="d3071-144">Request headers</span></span>
| <span data-ttu-id="d3071-145">名称</span><span class="sxs-lookup"><span data-stu-id="d3071-145">Name</span></span>       | <span data-ttu-id="d3071-146">说明</span><span class="sxs-lookup"><span data-stu-id="d3071-146">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d3071-147">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3071-147">Authorization</span></span>  | <span data-ttu-id="d3071-148">持有者&lt;令牌&gt;</span><span class="sxs-lookup"><span data-stu-id="d3071-148">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="d3071-149">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d3071-149">Content-Type</span></span>  | <span data-ttu-id="d3071-150">application/json</span><span class="sxs-lookup"><span data-stu-id="d3071-150">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d3071-151">请求正文</span><span class="sxs-lookup"><span data-stu-id="d3071-151">Request body</span></span>
<span data-ttu-id="d3071-152">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d3071-152">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="d3071-153">响应</span><span class="sxs-lookup"><span data-stu-id="d3071-153">Response</span></span>

<span data-ttu-id="d3071-154">如果成功，此方法在 `200 OK` 响应正文中返回 [响应](../resources/application.md) 代码和应用程序集合对象。</span><span class="sxs-lookup"><span data-stu-id="d3071-154">If successful, this method returns `200 OK` response code and [application](../resources/application.md) collection object in the response body.</span></span> <span data-ttu-id="d3071-155">该响应还包括 nextLink URL 或 deltaLink URL。</span><span class="sxs-lookup"><span data-stu-id="d3071-155">The response also includes a nextLink URL or a deltaLink URL.</span></span> 

- <span data-ttu-id="d3071-156">如果 `nextLink` 返回 URL，则会话中有其他要检索的数据页。</span><span class="sxs-lookup"><span data-stu-id="d3071-156">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="d3071-157">应用程序继续使用 `nextLink` URL 发出请求，直到响应中包含 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="d3071-157">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>

- <span data-ttu-id="d3071-158">如果 `deltaLink` 返回 URL，则不再返回有关资源现有状态的数据。</span><span class="sxs-lookup"><span data-stu-id="d3071-158">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="d3071-159">保留并使用 `deltaLink` URL 了解将来对资源的更改。</span><span class="sxs-lookup"><span data-stu-id="d3071-159">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="d3071-160">请参阅：</span><span class="sxs-lookup"><span data-stu-id="d3071-160">See:</span></span></br>
- <span data-ttu-id="d3071-161">[使用增量查询](/graph/delta-query-overview)了解更多详细信息</span><span class="sxs-lookup"><span data-stu-id="d3071-161">[Using Delta Query](/graph/delta-query-overview) for more details</span></span></br>
- <span data-ttu-id="d3071-162">[获取用户的增量更改](/graph/delta-query-users)获取示例请求。</span><span class="sxs-lookup"><span data-stu-id="d3071-162">[Get incremental changes for users](/graph/delta-query-users) for an example requests.</span></span></br>

### <a name="example"></a><span data-ttu-id="d3071-163">示例</span><span class="sxs-lookup"><span data-stu-id="d3071-163">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d3071-164">请求</span><span class="sxs-lookup"><span data-stu-id="d3071-164">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d3071-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="d3071-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/applications/delta
```
# <a name="c"></a>[<span data-ttu-id="d3071-166">C#</span><span class="sxs-lookup"><span data-stu-id="d3071-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d3071-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d3071-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d3071-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d3071-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d3071-169">Java</span><span class="sxs-lookup"><span data-stu-id="d3071-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d3071-170">响应</span><span class="sxs-lookup"><span data-stu-id="d3071-170">Response</span></span>
<span data-ttu-id="d3071-171">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d3071-171">Note: The response object shown here might be shortened for readability.</span></span>
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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#applications",
  "@odata.nextLink":"https://graph.microsoft.com/beta/applications/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
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



