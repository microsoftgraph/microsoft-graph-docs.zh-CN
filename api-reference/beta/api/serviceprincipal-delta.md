---
title: servicePrincipal： delta
description: 获取新创建、更新或删除的服务主体，而无需对整个资源集合执行完全读取。 有关详细信息，请参阅 Using Delta Query。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: beb322602d9f1487a8a285c1d4060d108efa56cc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48010526"
---
# <a name="serviceprincipal-delta"></a><span data-ttu-id="57a01-104">servicePrincipal： delta</span><span class="sxs-lookup"><span data-stu-id="57a01-104">servicePrincipal: delta</span></span>

<span data-ttu-id="57a01-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57a01-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57a01-106">获取新创建、更新或删除的服务主体，而无需对整个资源集合执行完全读取。</span><span class="sxs-lookup"><span data-stu-id="57a01-106">Get newly created, updated, or deleted service principals without having to perform a full read of the entire resource collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="57a01-107">权限</span><span class="sxs-lookup"><span data-stu-id="57a01-107">Permissions</span></span>

<span data-ttu-id="57a01-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="57a01-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="57a01-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="57a01-110">Permission type</span></span>      | <span data-ttu-id="57a01-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="57a01-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="57a01-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="57a01-112">Delegated (work or school account)</span></span> | <span data-ttu-id="57a01-113">Application.Read.All、Directory.Read.All、Application.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="57a01-113">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="57a01-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="57a01-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57a01-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="57a01-115">Not supported.</span></span>    |
|<span data-ttu-id="57a01-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="57a01-116">Application</span></span> | <span data-ttu-id="57a01-117">"Application.readwrite.ownedby"、"所有"、"readwrite"、"全部"、"所有"、"</span><span class="sxs-lookup"><span data-stu-id="57a01-117">Application.Read.All, Directory.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="57a01-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="57a01-118">HTTP request</span></span>

<span data-ttu-id="57a01-119">若要开始跟踪更改，请在 servicePrincipal 资源上发出包含 delta 函数的请求。</span><span class="sxs-lookup"><span data-stu-id="57a01-119">To begin tracking changes, you make a request including the delta function on the servicePrincipal resource.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/delta
```

### <a name="query-parameters"></a><span data-ttu-id="57a01-120">查询参数</span><span class="sxs-lookup"><span data-stu-id="57a01-120">Query parameters</span></span>

<span data-ttu-id="57a01-121">跟踪更改会产生一个或多个 **delta** 函数调用的往返。</span><span class="sxs-lookup"><span data-stu-id="57a01-121">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="57a01-122">如果要使用任意查询参数（`$deltatoken` 和 `$skiptoken` 除外），则必须在最初的 **delta** 请求中指定它。</span><span class="sxs-lookup"><span data-stu-id="57a01-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="57a01-123">Microsoft Graph 自动将指定的任意参数编码为响应中提供的 `nextLink` 或 `deltaLink` URL 的令牌部分。</span><span class="sxs-lookup"><span data-stu-id="57a01-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="57a01-124">只需预先指定所需的任何查询参数一次。</span><span class="sxs-lookup"><span data-stu-id="57a01-124">You only need to specify any desired query parameters once upfront.</span></span> <span data-ttu-id="57a01-125">在后续请求中，可以复制并应用之前响应中返回的 `nextLink` 或 `deltaLink` URL，因为此 URL 已包含所需的编码参数。</span><span class="sxs-lookup"><span data-stu-id="57a01-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="57a01-126">查询参数</span><span class="sxs-lookup"><span data-stu-id="57a01-126">Query parameter</span></span>      | <span data-ttu-id="57a01-127">类型</span><span class="sxs-lookup"><span data-stu-id="57a01-127">Type</span></span>   |<span data-ttu-id="57a01-128">说明</span><span class="sxs-lookup"><span data-stu-id="57a01-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="57a01-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="57a01-129">$deltatoken</span></span> | <span data-ttu-id="57a01-130">string</span><span class="sxs-lookup"><span data-stu-id="57a01-130">string</span></span> | <span data-ttu-id="57a01-131">[state token](/graph/delta-query-overview) `deltaLink` 为同一资源集合在上一个**delta**函数调用的 URL 中返回的状态令牌，指示该往返一轮的更改。</span><span class="sxs-lookup"><span data-stu-id="57a01-131">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="57a01-132">将此令牌包含在对该集合的下一组更改追踪的首次请求中，并保存和应用整个 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="57a01-132">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="57a01-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="57a01-133">$skiptoken</span></span> | <span data-ttu-id="57a01-134">string</span><span class="sxs-lookup"><span data-stu-id="57a01-134">string</span></span> | <span data-ttu-id="57a01-135">在上一个 delta 函数调用的 URL 中返回的[状态令牌](/graph/delta-query-overview) `nextLink` ，指示同一个资源集合中有进一步的更改需要跟踪。 **delta**</span><span class="sxs-lookup"><span data-stu-id="57a01-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same resource collection.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="57a01-136">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="57a01-136">Optional query parameters</span></span>

<span data-ttu-id="57a01-137">此方法支持 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="57a01-137">This method supports OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="57a01-p105">像在任何 GET 请求中一样，你可以使用 `$select` 查询参数以仅指定获取最佳性能所需的属性。始终返回 _id_ 属性。</span><span class="sxs-lookup"><span data-stu-id="57a01-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 

- <span data-ttu-id="57a01-140">提供对 `$filter` 的有限支持：</span><span class="sxs-lookup"><span data-stu-id="57a01-140">There is limited support for `$filter`:</span></span>
  * <span data-ttu-id="57a01-141">唯一受支持的 `$filter` 表达式是跟踪对特定资源所做的更改，其 id：  `$filter=id+eq+{value}` 或 `$filter=id+eq+{value1}+or+id+eq+{value2}` 。</span><span class="sxs-lookup"><span data-stu-id="57a01-141">The only supported `$filter` expression is for tracking changes for specific resources, by their id:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="57a01-142">您可以指定的 id 数受最大 URL 长度的限制。</span><span class="sxs-lookup"><span data-stu-id="57a01-142">The number of ids you can specify is limited by the maximum URL length.</span></span>


## <a name="request-headers"></a><span data-ttu-id="57a01-143">请求标头</span><span class="sxs-lookup"><span data-stu-id="57a01-143">Request headers</span></span>
| <span data-ttu-id="57a01-144">名称</span><span class="sxs-lookup"><span data-stu-id="57a01-144">Name</span></span>       | <span data-ttu-id="57a01-145">说明</span><span class="sxs-lookup"><span data-stu-id="57a01-145">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="57a01-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="57a01-146">Authorization</span></span>  | <span data-ttu-id="57a01-147">持有者&lt;令牌&gt;</span><span class="sxs-lookup"><span data-stu-id="57a01-147">Bearer &lt;token&gt;</span></span>|

## <a name="request-body"></a><span data-ttu-id="57a01-148">请求正文</span><span class="sxs-lookup"><span data-stu-id="57a01-148">Request body</span></span>
<span data-ttu-id="57a01-149">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="57a01-149">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="57a01-150">响应</span><span class="sxs-lookup"><span data-stu-id="57a01-150">Response</span></span>

<span data-ttu-id="57a01-151">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [servicePrincipal](../resources/serviceprincipal.md) 集合对象。</span><span class="sxs-lookup"><span data-stu-id="57a01-151">If successful, this method returns a `200 OK` response code and [servicePrincipal](../resources/serviceprincipal.md) collection object in the response body.</span></span> <span data-ttu-id="57a01-152">该响应还包括一个 nextLink URL 或 deltaLink URL。</span><span class="sxs-lookup"><span data-stu-id="57a01-152">The response also includes a nextLink URL or a deltaLink URL.</span></span> 

- <span data-ttu-id="57a01-153">如果 `nextLink` 返回 URL，则会在会话中检索其他数据页。</span><span class="sxs-lookup"><span data-stu-id="57a01-153">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="57a01-154">应用程序继续使用 `nextLink` URL 发出请求，直到响应中包含 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="57a01-154">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>

- <span data-ttu-id="57a01-155">如果 `deltaLink` 返回 URL，则没有有关要返回的资源的现有状态的更多数据。</span><span class="sxs-lookup"><span data-stu-id="57a01-155">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="57a01-156">保留并使用 `deltaLink` URL 了解将来对资源所做的更改。</span><span class="sxs-lookup"><span data-stu-id="57a01-156">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="57a01-157">请参阅：</span><span class="sxs-lookup"><span data-stu-id="57a01-157">See:</span></span></br>
- <span data-ttu-id="57a01-158">[使用增量查询](/graph/delta-query-overview)了解更多详细信息</span><span class="sxs-lookup"><span data-stu-id="57a01-158">[Using Delta Query](/graph/delta-query-overview) for more details</span></span></br>
- <span data-ttu-id="57a01-159">[获取用户的增量更改](/graph/delta-query-users)获取示例请求。</span><span class="sxs-lookup"><span data-stu-id="57a01-159">[Get incremental changes for users](/graph/delta-query-users) for an example requests.</span></span></br>

## <a name="example"></a><span data-ttu-id="57a01-160">示例</span><span class="sxs-lookup"><span data-stu-id="57a01-160">Example</span></span>
### <a name="request"></a><span data-ttu-id="57a01-161">请求</span><span class="sxs-lookup"><span data-stu-id="57a01-161">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="57a01-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="57a01-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "servicePrincipal_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/delta
```
# <a name="c"></a>[<span data-ttu-id="57a01-163">C#</span><span class="sxs-lookup"><span data-stu-id="57a01-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="57a01-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="57a01-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="57a01-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="57a01-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="57a01-166">响应</span><span class="sxs-lookup"><span data-stu-id="57a01-166">Response</span></span>
><span data-ttu-id="57a01-167">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="57a01-167">Note: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="57a01-168">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="57a01-168">All the properties will be returned from an actual call.</span></span>
<!-- { 
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal",
  "isCollection": true 
} --> 
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#servicePrincipals",
  "@odata.nextLink":"https://graph.microsoft.com/beta/servicePrincipals/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
     {
      "accountEnabled": true,
      "addIns": [
        {
          "id": "id-value",
          "type": "type-value",
          "properties": [
            {
              "key": "key-value",
              "value": "value-value"
            }
          ]
        }
      ],
      "appDisplayName": "appDisplayName-value",
      "appId": "appId-value",
      "appOwnerOrganizationId": "appOwnerOrganizationId-value",
      "appRoleAssignmentRequired": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "servicePrincipal: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


