---
title: servicePrincipal： delta
description: 获取新建、更新或删除的服务主体，而无需执行整个资源集合的完整读取。 有关详细信息，请参阅使用增量查询。
localization_priority: Normal
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: a878e82a591f287712231c68022874b5967cbd1b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051940"
---
# <a name="serviceprincipal-delta"></a><span data-ttu-id="460ae-104">servicePrincipal： delta</span><span class="sxs-lookup"><span data-stu-id="460ae-104">servicePrincipal: delta</span></span>

<span data-ttu-id="460ae-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="460ae-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="460ae-106">获取新建、更新或删除的服务主体，而无需执行整个资源集合的完整读取。</span><span class="sxs-lookup"><span data-stu-id="460ae-106">Get newly created, updated, or deleted service principals without having to perform a full read of the entire resource collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="460ae-107">权限</span><span class="sxs-lookup"><span data-stu-id="460ae-107">Permissions</span></span>

<span data-ttu-id="460ae-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="460ae-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="460ae-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="460ae-110">Permission type</span></span>      | <span data-ttu-id="460ae-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="460ae-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="460ae-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="460ae-112">Delegated (work or school account)</span></span> | <span data-ttu-id="460ae-113">Application.Read.All、Directory.Read.All、Application.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="460ae-113">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="460ae-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="460ae-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="460ae-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="460ae-115">Not supported.</span></span>    |
|<span data-ttu-id="460ae-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="460ae-116">Application</span></span> | <span data-ttu-id="460ae-117">Application.Read.All、 Directory.Read.All、 Application.ReadWrite.OwnedBy、 Application.ReadWrite.All、 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="460ae-117">Application.Read.All, Directory.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="460ae-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="460ae-118">HTTP request</span></span>

<span data-ttu-id="460ae-119">若要开始跟踪更改，请对 servicePrincipal 资源提出包含 delta 函数的请求。</span><span class="sxs-lookup"><span data-stu-id="460ae-119">To begin tracking changes, you make a request including the delta function on the servicePrincipal resource.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/delta
```

### <a name="query-parameters"></a><span data-ttu-id="460ae-120">查询参数</span><span class="sxs-lookup"><span data-stu-id="460ae-120">Query parameters</span></span>

<span data-ttu-id="460ae-121">跟踪更改将引发一次或多组 **delta** 函数调用。</span><span class="sxs-lookup"><span data-stu-id="460ae-121">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="460ae-122">如果要使用任意查询参数（`$deltatoken` 和 `$skiptoken` 除外），则必须在最初的 **delta** 请求中指定它。</span><span class="sxs-lookup"><span data-stu-id="460ae-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="460ae-123">Microsoft Graph 自动将指定的任意参数编码为响应中提供的 `nextLink` 或 `deltaLink` URL 的令牌部分。</span><span class="sxs-lookup"><span data-stu-id="460ae-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="460ae-124">只需预先指定所需的任何查询参数一次。</span><span class="sxs-lookup"><span data-stu-id="460ae-124">You only need to specify any desired query parameters once upfront.</span></span> <span data-ttu-id="460ae-125">在后续请求中，可以复制并应用之前响应中返回的 `nextLink` 或 `deltaLink` URL，因为此 URL 已包含所需的编码参数。</span><span class="sxs-lookup"><span data-stu-id="460ae-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="460ae-126">查询参数</span><span class="sxs-lookup"><span data-stu-id="460ae-126">Query parameter</span></span>      | <span data-ttu-id="460ae-127">类型</span><span class="sxs-lookup"><span data-stu-id="460ae-127">Type</span></span>   |<span data-ttu-id="460ae-128">说明</span><span class="sxs-lookup"><span data-stu-id="460ae-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="460ae-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="460ae-129">$deltatoken</span></span> | <span data-ttu-id="460ae-130">string</span><span class="sxs-lookup"><span data-stu-id="460ae-130">string</span></span> | <span data-ttu-id="460ae-131">对[同一](/graph/delta-query-overview)资源集合之前的 delta 函数调用的 URL 中返回的状态令牌，指示完成这一轮 `deltaLink` 更改跟踪。 </span><span class="sxs-lookup"><span data-stu-id="460ae-131">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="460ae-132">将此令牌包含在对该集合的下一组更改追踪的首次请求中，并保存和应用整个 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="460ae-132">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="460ae-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="460ae-133">$skiptoken</span></span> | <span data-ttu-id="460ae-134">string</span><span class="sxs-lookup"><span data-stu-id="460ae-134">string</span></span> | <span data-ttu-id="460ae-135">之前的[delta](/graph/delta-query-overview)函数调用的 URL 中返回的状态令牌，指示同一资源集合中还有进一 `nextLink` 步的更改需要跟踪。 </span><span class="sxs-lookup"><span data-stu-id="460ae-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same resource collection.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="460ae-136">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="460ae-136">Optional query parameters</span></span>

<span data-ttu-id="460ae-137">此方法支持 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="460ae-137">This method supports OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="460ae-p105">像在任何 GET 请求中一样，你可以使用 `$select` 查询参数以仅指定获取最佳性能所需的属性。始终返回 _id_ 属性。</span><span class="sxs-lookup"><span data-stu-id="460ae-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 

- <span data-ttu-id="460ae-140">提供对 `$filter` 的有限支持：</span><span class="sxs-lookup"><span data-stu-id="460ae-140">There is limited support for `$filter`:</span></span>
  * <span data-ttu-id="460ae-141">唯一 `$filter` 受支持的表达式用于按 id： 或 跟踪特定资源的  `$filter=id+eq+{value}` 更改 `$filter=id+eq+{value1}+or+id+eq+{value2}` 。</span><span class="sxs-lookup"><span data-stu-id="460ae-141">The only supported `$filter` expression is for tracking changes for specific resources, by their id:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="460ae-142">可以指定的 ID 数受最大 URL 长度限制。</span><span class="sxs-lookup"><span data-stu-id="460ae-142">The number of ids you can specify is limited by the maximum URL length.</span></span>


## <a name="request-headers"></a><span data-ttu-id="460ae-143">请求标头</span><span class="sxs-lookup"><span data-stu-id="460ae-143">Request headers</span></span>
| <span data-ttu-id="460ae-144">名称</span><span class="sxs-lookup"><span data-stu-id="460ae-144">Name</span></span>       | <span data-ttu-id="460ae-145">说明</span><span class="sxs-lookup"><span data-stu-id="460ae-145">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="460ae-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="460ae-146">Authorization</span></span>  | <span data-ttu-id="460ae-147">持有者&lt;令牌&gt;</span><span class="sxs-lookup"><span data-stu-id="460ae-147">Bearer &lt;token&gt;</span></span>|

## <a name="request-body"></a><span data-ttu-id="460ae-148">请求正文</span><span class="sxs-lookup"><span data-stu-id="460ae-148">Request body</span></span>
<span data-ttu-id="460ae-149">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="460ae-149">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="460ae-150">响应</span><span class="sxs-lookup"><span data-stu-id="460ae-150">Response</span></span>

<span data-ttu-id="460ae-151">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [servicePrincipal](../resources/serviceprincipal.md) 集合对象。</span><span class="sxs-lookup"><span data-stu-id="460ae-151">If successful, this method returns a `200 OK` response code and [servicePrincipal](../resources/serviceprincipal.md) collection object in the response body.</span></span> <span data-ttu-id="460ae-152">该响应还包括 nextLink URL 或 deltaLink URL。</span><span class="sxs-lookup"><span data-stu-id="460ae-152">The response also includes a nextLink URL or a deltaLink URL.</span></span> 

- <span data-ttu-id="460ae-153">如果 `nextLink` 返回 URL，则会话中有其他要检索的数据页。</span><span class="sxs-lookup"><span data-stu-id="460ae-153">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="460ae-154">应用程序继续使用 `nextLink` URL 发出请求，直到响应中包含 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="460ae-154">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>

- <span data-ttu-id="460ae-155">如果 `deltaLink` 返回 URL，则不再返回有关资源现有状态的数据。</span><span class="sxs-lookup"><span data-stu-id="460ae-155">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="460ae-156">保留并使用 `deltaLink` URL 了解将来对资源的更改。</span><span class="sxs-lookup"><span data-stu-id="460ae-156">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="460ae-157">请参阅：</span><span class="sxs-lookup"><span data-stu-id="460ae-157">See:</span></span></br>
- <span data-ttu-id="460ae-158">[使用增量查询](/graph/delta-query-overview)了解更多详细信息</span><span class="sxs-lookup"><span data-stu-id="460ae-158">[Using Delta Query](/graph/delta-query-overview) for more details</span></span></br>
- <span data-ttu-id="460ae-159">[获取用户的增量更改](/graph/delta-query-users)获取示例请求。</span><span class="sxs-lookup"><span data-stu-id="460ae-159">[Get incremental changes for users](/graph/delta-query-users) for an example requests.</span></span></br>

## <a name="example"></a><span data-ttu-id="460ae-160">示例</span><span class="sxs-lookup"><span data-stu-id="460ae-160">Example</span></span>
### <a name="request"></a><span data-ttu-id="460ae-161">请求</span><span class="sxs-lookup"><span data-stu-id="460ae-161">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="460ae-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="460ae-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "servicePrincipal_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/delta
```
# <a name="c"></a>[<span data-ttu-id="460ae-163">C#</span><span class="sxs-lookup"><span data-stu-id="460ae-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="460ae-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="460ae-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="460ae-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="460ae-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="460ae-166">Java</span><span class="sxs-lookup"><span data-stu-id="460ae-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="460ae-167">响应</span><span class="sxs-lookup"><span data-stu-id="460ae-167">Response</span></span>
><span data-ttu-id="460ae-168">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="460ae-168">Note: The response object shown here might be shortened for readability.</span></span>
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



