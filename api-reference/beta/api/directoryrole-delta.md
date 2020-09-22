---
title: directoryRole： delta
description: 获取新创建、更新或删除的目录角色，而无需对整个资源集合执行完全读取。 有关详细信息，请参阅 Using Delta Query。
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e740556f8d6b52bf8cdb8b4bc32d53dacbd3b7aa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48008783"
---
# <a name="directoryrole-delta"></a><span data-ttu-id="d9038-104">directoryRole： delta</span><span class="sxs-lookup"><span data-stu-id="d9038-104">directoryRole: delta</span></span>

<span data-ttu-id="d9038-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9038-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9038-106">获取新创建、更新或删除的目录角色，而无需对整个资源集合执行完全读取。</span><span class="sxs-lookup"><span data-stu-id="d9038-106">Get newly created, updated, or deleted directory roles without having to perform a full read of the entire resource collection.</span></span> <span data-ttu-id="d9038-107">有关详细信息，请参阅 [Using Delta Query](/graph/delta-query-overview) 。</span><span class="sxs-lookup"><span data-stu-id="d9038-107">See [Using Delta Query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="d9038-108">权限</span><span class="sxs-lookup"><span data-stu-id="d9038-108">Permissions</span></span>

<span data-ttu-id="d9038-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d9038-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9038-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d9038-111">Permission type</span></span>      | <span data-ttu-id="d9038-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d9038-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9038-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d9038-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d9038-114">RoleManagement、RoleManagement、Directory.accessasuser.all、all、、all、all 和的所有子目录。</span><span class="sxs-lookup"><span data-stu-id="d9038-114">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d9038-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d9038-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9038-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d9038-116">Not supported.</span></span>    |
|<span data-ttu-id="d9038-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d9038-117">Application</span></span> | <span data-ttu-id="d9038-118">RoleManagement、RoleManagement、目录和所有读写的所有子目录。所有</span><span class="sxs-lookup"><span data-stu-id="d9038-118">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d9038-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d9038-119">HTTP request</span></span>

<span data-ttu-id="d9038-120">若要开始跟踪更改，请在 directoryRole 资源上发出包含 delta 函数的请求。</span><span class="sxs-lookup"><span data-stu-id="d9038-120">To begin tracking changes, you make a request including the delta function on the directoryRole resource.</span></span>

<!-- { "blockType": "ignored" } -->
```http

GET /directoryRoles/delta

```

### <a name="query-parameters"></a><span data-ttu-id="d9038-121">查询参数</span><span class="sxs-lookup"><span data-stu-id="d9038-121">Query parameters</span></span>

<span data-ttu-id="d9038-122">跟踪更改会产生一个或多个 **delta** 函数调用的往返。</span><span class="sxs-lookup"><span data-stu-id="d9038-122">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="d9038-123">如果要使用任意查询参数（`$deltatoken` 和 `$skiptoken` 除外），则必须在最初的 **delta** 请求中指定它。</span><span class="sxs-lookup"><span data-stu-id="d9038-123">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="d9038-124">Microsoft Graph 自动将指定的任意参数编码为响应中提供的 `nextLink` 或 `deltaLink` URL 的令牌部分。</span><span class="sxs-lookup"><span data-stu-id="d9038-124">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="d9038-125">只需预先指定所需的任何查询参数一次。</span><span class="sxs-lookup"><span data-stu-id="d9038-125">You only need to specify any desired query parameters once upfront.</span></span> <span data-ttu-id="d9038-126">在后续请求中，可以复制并应用之前响应中返回的 `nextLink` 或 `deltaLink` URL，因为此 URL 已包含所需的编码参数。</span><span class="sxs-lookup"><span data-stu-id="d9038-126">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="d9038-127">查询参数</span><span class="sxs-lookup"><span data-stu-id="d9038-127">Query parameter</span></span>      | <span data-ttu-id="d9038-128">类型</span><span class="sxs-lookup"><span data-stu-id="d9038-128">Type</span></span>   |<span data-ttu-id="d9038-129">说明</span><span class="sxs-lookup"><span data-stu-id="d9038-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d9038-130">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="d9038-130">$deltatoken</span></span> | <span data-ttu-id="d9038-131">string</span><span class="sxs-lookup"><span data-stu-id="d9038-131">string</span></span> | <span data-ttu-id="d9038-132">[state token](/graph/delta-query-overview) `deltaLink` 为同一资源集合在上一个**delta**函数调用的 URL 中返回的状态令牌，指示该往返一轮的更改。</span><span class="sxs-lookup"><span data-stu-id="d9038-132">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="d9038-133">将此令牌包含在对该集合的下一组更改追踪的首次请求中，并保存和应用整个 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="d9038-133">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="d9038-134">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="d9038-134">$skiptoken</span></span> | <span data-ttu-id="d9038-135">string</span><span class="sxs-lookup"><span data-stu-id="d9038-135">string</span></span> | <span data-ttu-id="d9038-136">在上一个 delta 函数调用的 URL 中返回的[状态令牌](/graph/delta-query-overview) `nextLink` ，指示同一个资源集合中有进一步的更改需要跟踪。 **delta**</span><span class="sxs-lookup"><span data-stu-id="d9038-136">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same resource collection.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="d9038-137">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d9038-137">Optional query parameters</span></span>

<span data-ttu-id="d9038-138">此方法支持 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d9038-138">This method supports OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="d9038-p106">像在任何 GET 请求中一样，你可以使用 `$select` 查询参数以仅指定获取最佳性能所需的属性。始终返回 _id_ 属性。</span><span class="sxs-lookup"><span data-stu-id="d9038-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 

- <span data-ttu-id="d9038-141">提供对 `$filter` 的有限支持：</span><span class="sxs-lookup"><span data-stu-id="d9038-141">There is limited support for `$filter`:</span></span>
  * <span data-ttu-id="d9038-142">唯一受支持的 `$filter` 表达式是跟踪对特定资源所做的更改，其 id：  `$filter=id+eq+{value}` 或 `$filter=id+eq+{value1}+or+id+eq+{value2}` 。</span><span class="sxs-lookup"><span data-stu-id="d9038-142">The only supported `$filter` expression is for tracking changes for specific resources, by their id:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="d9038-143">您可以指定的 id 数受最大 URL 长度的限制。</span><span class="sxs-lookup"><span data-stu-id="d9038-143">The number of ids you can specify is limited by the maximum URL length.</span></span>


## <a name="request-headers"></a><span data-ttu-id="d9038-144">请求标头</span><span class="sxs-lookup"><span data-stu-id="d9038-144">Request headers</span></span>
| <span data-ttu-id="d9038-145">名称</span><span class="sxs-lookup"><span data-stu-id="d9038-145">Name</span></span>       | <span data-ttu-id="d9038-146">说明</span><span class="sxs-lookup"><span data-stu-id="d9038-146">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d9038-147">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9038-147">Authorization</span></span>  | <span data-ttu-id="d9038-148">持有者&lt;令牌&gt;</span><span class="sxs-lookup"><span data-stu-id="d9038-148">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="d9038-149">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d9038-149">Content-Type</span></span>  | <span data-ttu-id="d9038-150">application/json</span><span class="sxs-lookup"><span data-stu-id="d9038-150">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d9038-151">请求正文</span><span class="sxs-lookup"><span data-stu-id="d9038-151">Request body</span></span>
<span data-ttu-id="d9038-152">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d9038-152">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="d9038-153">响应</span><span class="sxs-lookup"><span data-stu-id="d9038-153">Response</span></span>

<span data-ttu-id="d9038-154">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [directoryRole](../resources/directoryrole.md) 集合对象。</span><span class="sxs-lookup"><span data-stu-id="d9038-154">If successful, this method returns `200 OK` response code and [directoryRole](../resources/directoryrole.md) collection object in the response body.</span></span> <span data-ttu-id="d9038-155">该响应还包括一个 nextLink URL 或 deltaLink URL。</span><span class="sxs-lookup"><span data-stu-id="d9038-155">The response also includes a nextLink URL or a deltaLink URL.</span></span> 

- <span data-ttu-id="d9038-156">如果 `nextLink` 返回 URL，则会在会话中检索其他数据页。</span><span class="sxs-lookup"><span data-stu-id="d9038-156">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="d9038-157">应用程序继续使用 `nextLink` URL 发出请求，直到响应中包含 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="d9038-157">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>

- <span data-ttu-id="d9038-158">如果 `deltaLink` 返回 URL，则没有有关要返回的资源的现有状态的更多数据。</span><span class="sxs-lookup"><span data-stu-id="d9038-158">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="d9038-159">保留并使用 `deltaLink` URL 了解将来对资源所做的更改。</span><span class="sxs-lookup"><span data-stu-id="d9038-159">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="d9038-160">请参阅：</span><span class="sxs-lookup"><span data-stu-id="d9038-160">See:</span></span></br>
- <span data-ttu-id="d9038-161">[使用增量查询](/graph/delta-query-overview)了解更多详细信息</span><span class="sxs-lookup"><span data-stu-id="d9038-161">[Using Delta Query](/graph/delta-query-overview) for more details</span></span></br>
- <span data-ttu-id="d9038-162">[获取用户的增量更改](/graph/delta-query-users)获取示例请求。</span><span class="sxs-lookup"><span data-stu-id="d9038-162">[Get incremental changes for users](/graph/delta-query-users) for an example requests.</span></span></br>

### <a name="example"></a><span data-ttu-id="d9038-163">示例</span><span class="sxs-lookup"><span data-stu-id="d9038-163">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d9038-164">请求</span><span class="sxs-lookup"><span data-stu-id="d9038-164">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d9038-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="d9038-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryRole_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoles/delta
```
# <a name="c"></a>[<span data-ttu-id="d9038-166">C#</span><span class="sxs-lookup"><span data-stu-id="d9038-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryrole-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d9038-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d9038-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryrole-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d9038-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d9038-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryrole-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d9038-169">响应</span><span class="sxs-lookup"><span data-stu-id="d9038-169">Response</span></span>
<span data-ttu-id="d9038-p111">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d9038-p111">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


