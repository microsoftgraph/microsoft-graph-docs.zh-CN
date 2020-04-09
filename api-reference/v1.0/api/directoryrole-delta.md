---
title: directoryRole： delta
description: 获取新创建、更新或删除的目录角色，而无需对整个资源集合执行完全读取。 有关详细信息，请参阅 Using Delta Query。
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bfd98c1415381e4daf1e8a551dc9050df122ff49
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181418"
---
# <a name="directoryrole-delta"></a><span data-ttu-id="7c659-104">directoryRole： delta</span><span class="sxs-lookup"><span data-stu-id="7c659-104">directoryRole: delta</span></span>

<span data-ttu-id="7c659-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c659-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7c659-106">获取新创建、更新或删除的目录角色，而无需对整个资源集合执行完全读取。</span><span class="sxs-lookup"><span data-stu-id="7c659-106">Get newly created, updated, or deleted directory roles without having to perform a full read of the entire resource collection.</span></span> <span data-ttu-id="7c659-107">有关详细信息，请参阅[Using Delta Query](/graph/delta-query-overview) 。</span><span class="sxs-lookup"><span data-stu-id="7c659-107">See [Using Delta Query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="7c659-108">权限</span><span class="sxs-lookup"><span data-stu-id="7c659-108">Permissions</span></span>

<span data-ttu-id="7c659-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7c659-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7c659-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7c659-111">Permission type</span></span>      | <span data-ttu-id="7c659-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7c659-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7c659-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7c659-113">Delegated (work or school account)</span></span> | <span data-ttu-id="7c659-114">RoleManagement、RoleManagement、Directory.accessasuser.all、all、、all、all 和的所有子目录。</span><span class="sxs-lookup"><span data-stu-id="7c659-114">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7c659-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7c659-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c659-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7c659-116">Not supported.</span></span>    |
|<span data-ttu-id="7c659-117">Application</span><span class="sxs-lookup"><span data-stu-id="7c659-117">Application</span></span> | <span data-ttu-id="7c659-118">RoleManagement、RoleManagement、目录和所有读写的所有子目录。所有</span><span class="sxs-lookup"><span data-stu-id="7c659-118">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7c659-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7c659-119">HTTP request</span></span>

<span data-ttu-id="7c659-120">若要开始跟踪更改，请在[directoryRole](../resources/directoryrole.md)资源上发出包含**delta**函数的请求。</span><span class="sxs-lookup"><span data-stu-id="7c659-120">To begin tracking changes, you make a request including the **delta** function on the [directoryRole](../resources/directoryrole.md) resource.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/delta
```

## <a name="query-parameters"></a><span data-ttu-id="7c659-121">查询参数</span><span class="sxs-lookup"><span data-stu-id="7c659-121">Query parameters</span></span>

<span data-ttu-id="7c659-122">跟踪更改会产生一个或多个**delta**函数调用的往返。</span><span class="sxs-lookup"><span data-stu-id="7c659-122">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="7c659-123">如果要使用任意查询参数（`$deltatoken` 和 `$skiptoken` 除外），则必须在最初的 **delta** 请求中指定它。</span><span class="sxs-lookup"><span data-stu-id="7c659-123">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="7c659-124">Microsoft Graph 自动将指定的任意参数编码为响应中提供的 `nextLink` 或 `deltaLink` URL 的令牌部分。</span><span class="sxs-lookup"><span data-stu-id="7c659-124">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="7c659-125">只需预先指定所需的任何查询参数一次。</span><span class="sxs-lookup"><span data-stu-id="7c659-125">You only need to specify any desired query parameters once upfront.</span></span> <span data-ttu-id="7c659-126">在后续请求中，可以复制并应用之前响应中返回的 `nextLink` 或 `deltaLink` URL，因为此 URL 已包含所需的编码参数。</span><span class="sxs-lookup"><span data-stu-id="7c659-126">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="7c659-127">查询参数</span><span class="sxs-lookup"><span data-stu-id="7c659-127">Query parameter</span></span>      | <span data-ttu-id="7c659-128">类型</span><span class="sxs-lookup"><span data-stu-id="7c659-128">Type</span></span>   |<span data-ttu-id="7c659-129">说明</span><span class="sxs-lookup"><span data-stu-id="7c659-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7c659-130">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="7c659-130">$deltatoken</span></span> | <span data-ttu-id="7c659-131">string</span><span class="sxs-lookup"><span data-stu-id="7c659-131">string</span></span> | <span data-ttu-id="7c659-132">为同一资源集合在上`deltaLink`一个**delta**函数调用的 URL 中返回的[状态令牌](/graph/delta-query-overview)，指示该往返一轮的更改。</span><span class="sxs-lookup"><span data-stu-id="7c659-132">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="7c659-133">将此令牌包含在对该集合的下一组更改追踪的首次请求中，并保存和应用整个 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="7c659-133">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="7c659-134">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="7c659-134">$skiptoken</span></span> | <span data-ttu-id="7c659-135">string</span><span class="sxs-lookup"><span data-stu-id="7c659-135">string</span></span> | <span data-ttu-id="7c659-136">在上一个**delta**函数调用`nextLink`的 URL 中返回的[状态令牌](/graph/delta-query-overview)，指示同一个资源集合中有进一步的更改需要跟踪。</span><span class="sxs-lookup"><span data-stu-id="7c659-136">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same resource collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="7c659-137">OData 查询参数</span><span class="sxs-lookup"><span data-stu-id="7c659-137">OData query parameters</span></span>

<span data-ttu-id="7c659-138">此方法支持 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7c659-138">This method supports OData query parameters to help customize the response.</span></span>

- <span data-ttu-id="7c659-p106">像在任何 GET 请求中一样，你可以使用 `$select` 查询参数以仅指定获取最佳性能所需的属性。始终返回 _id_ 属性。</span><span class="sxs-lookup"><span data-stu-id="7c659-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span>

- <span data-ttu-id="7c659-141">提供对 `$filter` 的有限支持：</span><span class="sxs-lookup"><span data-stu-id="7c659-141">There is limited support for `$filter`:</span></span>

  - <span data-ttu-id="7c659-142">唯一受支持`$filter`的表达式是跟踪对特定资源所做的更改，其`$filter=id+eq+{value}` id `$filter=id+eq+{value1}+or+id+eq+{value2}`：或。</span><span class="sxs-lookup"><span data-stu-id="7c659-142">The only supported `$filter` expression is for tracking changes for specific resources, by their id:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="7c659-143">您可以指定的 id 数受最大 URL 长度的限制。</span><span class="sxs-lookup"><span data-stu-id="7c659-143">The number of ids you can specify is limited by the maximum URL length.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7c659-144">请求标头</span><span class="sxs-lookup"><span data-stu-id="7c659-144">Request headers</span></span>

| <span data-ttu-id="7c659-145">名称</span><span class="sxs-lookup"><span data-stu-id="7c659-145">Name</span></span>       | <span data-ttu-id="7c659-146">说明</span><span class="sxs-lookup"><span data-stu-id="7c659-146">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7c659-147">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c659-147">Authorization</span></span>  | <span data-ttu-id="7c659-148">持有者&lt;令牌&gt;</span><span class="sxs-lookup"><span data-stu-id="7c659-148">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="7c659-149">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7c659-149">Content-Type</span></span>  | <span data-ttu-id="7c659-150">application/json</span><span class="sxs-lookup"><span data-stu-id="7c659-150">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="7c659-151">请求正文</span><span class="sxs-lookup"><span data-stu-id="7c659-151">Request body</span></span>

<span data-ttu-id="7c659-152">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7c659-152">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="7c659-153">响应</span><span class="sxs-lookup"><span data-stu-id="7c659-153">Response</span></span>

<span data-ttu-id="7c659-154">如果成功，此方法在`200 OK`响应正文中返回响应代码和[directoryRole](../resources/directoryrole.md)集合对象。</span><span class="sxs-lookup"><span data-stu-id="7c659-154">If successful, this method returns `200 OK` response code and [directoryRole](../resources/directoryrole.md) collection object in the response body.</span></span> <span data-ttu-id="7c659-155">该响应还包括 `nextLink`URL 或 `deltaLink`URL。</span><span class="sxs-lookup"><span data-stu-id="7c659-155">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="7c659-156">如果返回`nextLink` URL，则会在会话中检索其他数据页。</span><span class="sxs-lookup"><span data-stu-id="7c659-156">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="7c659-157">应用程序继续使用 `nextLink` URL 发出请求，直到响应中包含 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="7c659-157">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>

- <span data-ttu-id="7c659-158">如果返回`deltaLink` URL，则没有有关要返回的资源的现有状态的更多数据。</span><span class="sxs-lookup"><span data-stu-id="7c659-158">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="7c659-159">保存`deltaLink` URL 并在下一次**增量**调用中应用它，以了解将来对资源所做的更改。</span><span class="sxs-lookup"><span data-stu-id="7c659-159">Save `deltaLink` URL and apply it in the next **delta** call to learn about changes to the resource in the future.</span></span>

### <a name="example"></a><span data-ttu-id="7c659-160">示例</span><span class="sxs-lookup"><span data-stu-id="7c659-160">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7c659-161">请求</span><span class="sxs-lookup"><span data-stu-id="7c659-161">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="7c659-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="7c659-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryRole_delta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directoryRoles/delta
```
# <a name="c"></a>[<span data-ttu-id="7c659-163">C#</span><span class="sxs-lookup"><span data-stu-id="7c659-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryrole-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7c659-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7c659-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryrole-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7c659-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7c659-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryrole-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7c659-166">Java</span><span class="sxs-lookup"><span data-stu-id="7c659-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryrole-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7c659-167">响应</span><span class="sxs-lookup"><span data-stu-id="7c659-167">Response</span></span>

<span data-ttu-id="7c659-p111">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7c659-p111">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#directoryRoles",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/directoryRoles/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
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

### <a name="see-also"></a><span data-ttu-id="7c659-170">另请参阅</span><span class="sxs-lookup"><span data-stu-id="7c659-170">See also</span></span>

- <span data-ttu-id="7c659-171">[使用 delta 查询跟踪 Microsoft Graph 数据中的更改](/graph/delta-query-overview)，了解更多详细信息</span><span class="sxs-lookup"><span data-stu-id="7c659-171">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview) for more details</span></span>
- <span data-ttu-id="7c659-172">[获取用户的增量更改](/graph/delta-query-users)获取示例请求。</span><span class="sxs-lookup"><span data-stu-id="7c659-172">[Get incremental changes for users](/graph/delta-query-users) for an example requests.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryRole: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
