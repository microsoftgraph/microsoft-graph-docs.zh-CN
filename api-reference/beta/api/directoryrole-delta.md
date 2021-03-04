---
title: directoryRole： delta
description: 获取新创建、更新或删除的目录角色，而无需执行整个资源集合的完全读取。 有关详细信息，请参阅使用 Delta 查询。
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 8ab916a6808422624ba511ad728100b315156be7
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436818"
---
# <a name="directoryrole-delta"></a><span data-ttu-id="0c455-104">directoryRole： delta</span><span class="sxs-lookup"><span data-stu-id="0c455-104">directoryRole: delta</span></span>

<span data-ttu-id="0c455-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c455-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c455-106">获取新创建、更新或删除的目录角色，而无需执行整个资源集合的完全读取。</span><span class="sxs-lookup"><span data-stu-id="0c455-106">Get newly created, updated, or deleted directory roles without having to perform a full read of the entire resource collection.</span></span> <span data-ttu-id="0c455-107">有关详细信息 [，请参阅](/graph/delta-query-overview) 使用 Delta 查询。</span><span class="sxs-lookup"><span data-stu-id="0c455-107">See [Using Delta Query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="0c455-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="0c455-108">Permissions</span></span>

<span data-ttu-id="0c455-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0c455-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c455-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0c455-111">Permission type</span></span>      | <span data-ttu-id="0c455-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0c455-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0c455-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0c455-113">Delegated (work or school account)</span></span> | <span data-ttu-id="0c455-114">RoleManagement.Read.Directory、Directory.Read.All、RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0c455-114">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0c455-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0c455-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c455-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0c455-116">Not supported.</span></span>    |
|<span data-ttu-id="0c455-117">Application</span><span class="sxs-lookup"><span data-stu-id="0c455-117">Application</span></span> | <span data-ttu-id="0c455-118">RoleManagement.Read.Directory、Directory.Read.All、RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c455-118">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0c455-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0c455-119">HTTP request</span></span>

<span data-ttu-id="0c455-120">若要开始跟踪更改，请对 directoryRole 资源提出包含 delta 函数的请求。</span><span class="sxs-lookup"><span data-stu-id="0c455-120">To begin tracking changes, you make a request including the delta function on the directoryRole resource.</span></span>

<!-- { "blockType": "ignored" } -->
```http

GET /directoryRoles/delta

```

### <a name="query-parameters"></a><span data-ttu-id="0c455-121">查询参数</span><span class="sxs-lookup"><span data-stu-id="0c455-121">Query parameters</span></span>

<span data-ttu-id="0c455-122">跟踪更改将引发一轮或多次 **delta** 函数调用。</span><span class="sxs-lookup"><span data-stu-id="0c455-122">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="0c455-123">如果要使用任意查询参数（`$deltatoken` 和 `$skiptoken` 除外），则必须在最初的 **delta** 请求中指定它。</span><span class="sxs-lookup"><span data-stu-id="0c455-123">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="0c455-124">Microsoft Graph 自动将指定的任意参数编码为响应中提供的 `nextLink` 或 `deltaLink` URL 的令牌部分。</span><span class="sxs-lookup"><span data-stu-id="0c455-124">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="0c455-125">只需预先指定所需的任何查询参数一次。</span><span class="sxs-lookup"><span data-stu-id="0c455-125">You only need to specify any desired query parameters once upfront.</span></span> <span data-ttu-id="0c455-126">在后续请求中，可以复制并应用之前响应中返回的 `nextLink` 或 `deltaLink` URL，因为此 URL 已包含所需的编码参数。</span><span class="sxs-lookup"><span data-stu-id="0c455-126">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="0c455-127">查询参数</span><span class="sxs-lookup"><span data-stu-id="0c455-127">Query parameter</span></span>      | <span data-ttu-id="0c455-128">类型</span><span class="sxs-lookup"><span data-stu-id="0c455-128">Type</span></span>   |<span data-ttu-id="0c455-129">说明</span><span class="sxs-lookup"><span data-stu-id="0c455-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0c455-130">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="0c455-130">$deltatoken</span></span> | <span data-ttu-id="0c455-131">string</span><span class="sxs-lookup"><span data-stu-id="0c455-131">string</span></span> | <span data-ttu-id="0c455-132">同[一资源](/graph/delta-query-overview)集合的上一个 delta 函数调用的 URL 中返回的状态令牌，指示完成这一轮 `deltaLink` 更改跟踪。 </span><span class="sxs-lookup"><span data-stu-id="0c455-132">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="0c455-133">将此令牌包含在对该集合的下一组更改追踪的首次请求中，并保存和应用整个 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="0c455-133">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="0c455-134">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="0c455-134">$skiptoken</span></span> | <span data-ttu-id="0c455-135">string</span><span class="sxs-lookup"><span data-stu-id="0c455-135">string</span></span> | <span data-ttu-id="0c455-136">在[上一](/graph/delta-query-overview)个 delta 函数调用的 URL 中返回的状态令牌，指示同一资源集合中还有要跟踪的进一 `nextLink` 步更改。 </span><span class="sxs-lookup"><span data-stu-id="0c455-136">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same resource collection.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="0c455-137">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0c455-137">Optional query parameters</span></span>

<span data-ttu-id="0c455-138">此方法支持 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0c455-138">This method supports OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="0c455-p106">像在任何 GET 请求中一样，你可以使用 `$select` 查询参数以仅指定获取最佳性能所需的属性。始终返回 _id_ 属性。</span><span class="sxs-lookup"><span data-stu-id="0c455-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 

- <span data-ttu-id="0c455-141">提供对 `$filter` 的有限支持：</span><span class="sxs-lookup"><span data-stu-id="0c455-141">There is limited support for `$filter`:</span></span>
  * <span data-ttu-id="0c455-142">唯一受支持的表达式用于按 id： 或 跟踪特定 `$filter` 资源的  `$filter=id+eq+{value}` 更改 `$filter=id+eq+{value1}+or+id+eq+{value2}` 。</span><span class="sxs-lookup"><span data-stu-id="0c455-142">The only supported `$filter` expression is for tracking changes for specific resources, by their id:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="0c455-143">可以指定的 ID 数受最大 URL 长度限制。</span><span class="sxs-lookup"><span data-stu-id="0c455-143">The number of ids you can specify is limited by the maximum URL length.</span></span>


## <a name="request-headers"></a><span data-ttu-id="0c455-144">请求标头</span><span class="sxs-lookup"><span data-stu-id="0c455-144">Request headers</span></span>
| <span data-ttu-id="0c455-145">名称</span><span class="sxs-lookup"><span data-stu-id="0c455-145">Name</span></span>       | <span data-ttu-id="0c455-146">说明</span><span class="sxs-lookup"><span data-stu-id="0c455-146">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0c455-147">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c455-147">Authorization</span></span>  | <span data-ttu-id="0c455-148">持有者&lt;令牌&gt;</span><span class="sxs-lookup"><span data-stu-id="0c455-148">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="0c455-149">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0c455-149">Content-Type</span></span>  | <span data-ttu-id="0c455-150">application/json</span><span class="sxs-lookup"><span data-stu-id="0c455-150">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="0c455-151">请求正文</span><span class="sxs-lookup"><span data-stu-id="0c455-151">Request body</span></span>
<span data-ttu-id="0c455-152">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0c455-152">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="0c455-153">响应</span><span class="sxs-lookup"><span data-stu-id="0c455-153">Response</span></span>

<span data-ttu-id="0c455-154">如果成功，此方法在响应正文中返回响应代码 `200 OK` 和 [directoryRole](../resources/directoryrole.md) 集合对象。</span><span class="sxs-lookup"><span data-stu-id="0c455-154">If successful, this method returns `200 OK` response code and [directoryRole](../resources/directoryrole.md) collection object in the response body.</span></span> <span data-ttu-id="0c455-155">该响应还包括 nextLink URL 或 deltaLink URL。</span><span class="sxs-lookup"><span data-stu-id="0c455-155">The response also includes a nextLink URL or a deltaLink URL.</span></span> 

- <span data-ttu-id="0c455-156">如果 `nextLink` 返回 URL，则会话中将检索其他数据页。</span><span class="sxs-lookup"><span data-stu-id="0c455-156">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="0c455-157">应用程序继续使用 `nextLink` URL 发出请求，直到响应中包含 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="0c455-157">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>

- <span data-ttu-id="0c455-158">如果返回 URL，则不再返回有关资源现有状态 `deltaLink` 的数据。</span><span class="sxs-lookup"><span data-stu-id="0c455-158">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="0c455-159">保留并使用 `deltaLink` URL 了解将来对资源的更改。</span><span class="sxs-lookup"><span data-stu-id="0c455-159">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="0c455-160">请参阅：</span><span class="sxs-lookup"><span data-stu-id="0c455-160">See:</span></span></br>
- <span data-ttu-id="0c455-161">[使用增量查询](/graph/delta-query-overview)了解更多详细信息</span><span class="sxs-lookup"><span data-stu-id="0c455-161">[Using Delta Query](/graph/delta-query-overview) for more details</span></span></br>
- <span data-ttu-id="0c455-162">[获取用户的增量更改](/graph/delta-query-users)获取示例请求。</span><span class="sxs-lookup"><span data-stu-id="0c455-162">[Get incremental changes for users](/graph/delta-query-users) for an example requests.</span></span></br>

### <a name="example"></a><span data-ttu-id="0c455-163">示例</span><span class="sxs-lookup"><span data-stu-id="0c455-163">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0c455-164">请求</span><span class="sxs-lookup"><span data-stu-id="0c455-164">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="0c455-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="0c455-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryRole_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoles/delta
```
# <a name="c"></a>[<span data-ttu-id="0c455-166">C#</span><span class="sxs-lookup"><span data-stu-id="0c455-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryrole-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0c455-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0c455-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryrole-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0c455-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0c455-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryrole-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0c455-169">Java</span><span class="sxs-lookup"><span data-stu-id="0c455-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryrole-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0c455-170">响应</span><span class="sxs-lookup"><span data-stu-id="0c455-170">Response</span></span>
<span data-ttu-id="0c455-p111">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0c455-p111">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- { 
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole",
  "isCollection": true 
} --> 
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryRoles",
  "@odata.nextLink":"https://graph.microsoft.com/beta/directoryRoles/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
      {
      "description": "description-value",
      "displayName": "displayName-value",
      "roleTemplateId": "roleTemplateId-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryRole: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


