---
title: servicePrincipal： delta
description: 获取新创建、更新或删除的服务主体，而无需对整个资源集合执行完全读取。 有关详细信息，请参阅 Using Delta Query。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 19d7e364c5a3c8a6ea7aa9839ec53320b8c4c434
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2020
ms.locfileid: "44383558"
---
# <a name="serviceprincipal-delta"></a><span data-ttu-id="2156d-104">servicePrincipal： delta</span><span class="sxs-lookup"><span data-stu-id="2156d-104">servicePrincipal: delta</span></span>

<span data-ttu-id="2156d-105">获取新创建、更新或删除的服务主体，而无需对整个资源集合执行完全读取。</span><span class="sxs-lookup"><span data-stu-id="2156d-105">Get newly created, updated, or deleted service principals without having to perform a full read of the entire resource collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="2156d-106">权限</span><span class="sxs-lookup"><span data-stu-id="2156d-106">Permissions</span></span>

<span data-ttu-id="2156d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2156d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2156d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2156d-109">Permission type</span></span>      | <span data-ttu-id="2156d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2156d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2156d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2156d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2156d-112">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2156d-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2156d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2156d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2156d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2156d-114">Not supported.</span></span>    |
|<span data-ttu-id="2156d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2156d-115">Application</span></span> | <span data-ttu-id="2156d-116">Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="2156d-116">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2156d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2156d-117">HTTP request</span></span>

<span data-ttu-id="2156d-118">若要开始跟踪更改，请在 servicePrincipal 资源上发出包含 delta 函数的请求。</span><span class="sxs-lookup"><span data-stu-id="2156d-118">To begin tracking changes, you make a request including the delta function on the servicePrincipal resource.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/delta
```

### <a name="query-parameters"></a><span data-ttu-id="2156d-119">查询参数</span><span class="sxs-lookup"><span data-stu-id="2156d-119">Query parameters</span></span>

<span data-ttu-id="2156d-120">跟踪更改会产生一个或多个**delta**函数调用的往返。</span><span class="sxs-lookup"><span data-stu-id="2156d-120">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="2156d-121">如果要使用任意查询参数（`$deltatoken` 和 `$skiptoken` 除外），则必须在最初的 **delta** 请求中指定它。</span><span class="sxs-lookup"><span data-stu-id="2156d-121">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="2156d-122">Microsoft Graph 自动将指定的任意参数编码为响应中提供的 `nextLink` 或 `deltaLink` URL 的令牌部分。</span><span class="sxs-lookup"><span data-stu-id="2156d-122">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="2156d-123">只需预先指定所需的任何查询参数一次。</span><span class="sxs-lookup"><span data-stu-id="2156d-123">You only need to specify any desired query parameters once upfront.</span></span> <span data-ttu-id="2156d-124">在后续请求中，可以复制并应用之前响应中返回的 `nextLink` 或 `deltaLink` URL，因为此 URL 已包含所需的编码参数。</span><span class="sxs-lookup"><span data-stu-id="2156d-124">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="2156d-125">查询参数</span><span class="sxs-lookup"><span data-stu-id="2156d-125">Query parameter</span></span>      | <span data-ttu-id="2156d-126">类型</span><span class="sxs-lookup"><span data-stu-id="2156d-126">Type</span></span>   |<span data-ttu-id="2156d-127">Description</span><span class="sxs-lookup"><span data-stu-id="2156d-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2156d-128">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="2156d-128">$deltatoken</span></span> | <span data-ttu-id="2156d-129">string</span><span class="sxs-lookup"><span data-stu-id="2156d-129">string</span></span> | <span data-ttu-id="2156d-130">[state token](/graph/delta-query-overview) `deltaLink` 为同一资源集合在上一个**delta**函数调用的 URL 中返回的状态令牌，指示该往返一轮的更改。</span><span class="sxs-lookup"><span data-stu-id="2156d-130">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="2156d-131">将此令牌包含在对该集合的下一组更改追踪的首次请求中，并保存和应用整个 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="2156d-131">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="2156d-132">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="2156d-132">$skiptoken</span></span> | <span data-ttu-id="2156d-133">string</span><span class="sxs-lookup"><span data-stu-id="2156d-133">string</span></span> | <span data-ttu-id="2156d-134">在上一个 delta 函数调用的 URL 中返回的[状态令牌](/graph/delta-query-overview) `nextLink` ，指示同一个资源集合中有进一步的更改需要跟踪。 **delta**</span><span class="sxs-lookup"><span data-stu-id="2156d-134">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same resource collection.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="2156d-135">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2156d-135">Optional query parameters</span></span>

<span data-ttu-id="2156d-136">此方法支持 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2156d-136">This method supports OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="2156d-p105">像在任何 GET 请求中一样，你可以使用 `$select` 查询参数以仅指定获取最佳性能所需的属性。始终返回 _id_ 属性。</span><span class="sxs-lookup"><span data-stu-id="2156d-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 

- <span data-ttu-id="2156d-139">提供对 `$filter` 的有限支持：</span><span class="sxs-lookup"><span data-stu-id="2156d-139">There is limited support for `$filter`:</span></span>
  * <span data-ttu-id="2156d-140">唯一受支持的 `$filter` 表达式是跟踪对特定资源所做的更改，其 id： `$filter=id+eq+{value}` 或 `$filter=id+eq+{value1}+or+id+eq+{value2}` 。</span><span class="sxs-lookup"><span data-stu-id="2156d-140">The only supported `$filter` expression is for tracking changes for specific resources, by their id:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="2156d-141">您可以指定的 id 数受最大 URL 长度的限制。</span><span class="sxs-lookup"><span data-stu-id="2156d-141">The number of ids you can specify is limited by the maximum URL length.</span></span>


## <a name="request-headers"></a><span data-ttu-id="2156d-142">请求头</span><span class="sxs-lookup"><span data-stu-id="2156d-142">Request headers</span></span>
| <span data-ttu-id="2156d-143">名称</span><span class="sxs-lookup"><span data-stu-id="2156d-143">Name</span></span>       | <span data-ttu-id="2156d-144">说明</span><span class="sxs-lookup"><span data-stu-id="2156d-144">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2156d-145">Authorization</span><span class="sxs-lookup"><span data-stu-id="2156d-145">Authorization</span></span>  | <span data-ttu-id="2156d-146">持有者&lt;令牌&gt;</span><span class="sxs-lookup"><span data-stu-id="2156d-146">Bearer &lt;token&gt;</span></span>|

## <a name="request-body"></a><span data-ttu-id="2156d-147">请求正文</span><span class="sxs-lookup"><span data-stu-id="2156d-147">Request body</span></span>
<span data-ttu-id="2156d-148">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2156d-148">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="2156d-149">响应</span><span class="sxs-lookup"><span data-stu-id="2156d-149">Response</span></span>

<span data-ttu-id="2156d-150">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[servicePrincipal](../resources/serviceprincipal.md)集合对象。</span><span class="sxs-lookup"><span data-stu-id="2156d-150">If successful, this method returns a `200 OK` response code and [servicePrincipal](../resources/serviceprincipal.md) collection object in the response body.</span></span> <span data-ttu-id="2156d-151">该响应还包括一个 nextLink URL 或 deltaLink URL。</span><span class="sxs-lookup"><span data-stu-id="2156d-151">The response also includes a nextLink URL or a deltaLink URL.</span></span> 

- <span data-ttu-id="2156d-152">如果 `nextLink` 返回 URL，则会在会话中检索其他数据页。</span><span class="sxs-lookup"><span data-stu-id="2156d-152">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="2156d-153">应用程序继续使用 `nextLink` URL 发出请求，直到响应中包含 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="2156d-153">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>

- <span data-ttu-id="2156d-154">如果 `deltaLink` 返回 URL，则没有有关要返回的资源的现有状态的更多数据。</span><span class="sxs-lookup"><span data-stu-id="2156d-154">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="2156d-155">保留并使用 `deltaLink` URL 了解将来对资源所做的更改。</span><span class="sxs-lookup"><span data-stu-id="2156d-155">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="2156d-156">请参阅：</span><span class="sxs-lookup"><span data-stu-id="2156d-156">See:</span></span></br>
- <span data-ttu-id="2156d-157">[使用增量查询](/graph/delta-query-overview)了解更多详细信息</span><span class="sxs-lookup"><span data-stu-id="2156d-157">[Using Delta Query](/graph/delta-query-overview) for more details</span></span></br>
- <span data-ttu-id="2156d-158">[获取用户的增量更改](/graph/delta-query-users)获取示例请求。</span><span class="sxs-lookup"><span data-stu-id="2156d-158">[Get incremental changes for users](/graph/delta-query-users) for an example requests.</span></span></br>

## <a name="example"></a><span data-ttu-id="2156d-159">示例</span><span class="sxs-lookup"><span data-stu-id="2156d-159">Example</span></span>
#### <a name="request"></a><span data-ttu-id="2156d-160">请求</span><span class="sxs-lookup"><span data-stu-id="2156d-160">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="2156d-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="2156d-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "servicePrincipal_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/delta
```
# <a name="c"></a>[<span data-ttu-id="2156d-162">C#</span><span class="sxs-lookup"><span data-stu-id="2156d-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2156d-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2156d-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2156d-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2156d-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2156d-165">Java</span><span class="sxs-lookup"><span data-stu-id="2156d-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2156d-166">响应</span><span class="sxs-lookup"><span data-stu-id="2156d-166">Response</span></span>
><span data-ttu-id="2156d-167">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2156d-167">Note: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2156d-168">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="2156d-168">All the properties will be returned from an actual call.</span></span>
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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#servicePrincipals",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/servicePrincipals/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
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
