---
title: 'directoryRole: delta'
description: 获取新创建、更新或删除的目录角色, 而无需对整个资源集合执行完全读取。 有关详细信息, 请参阅 Using Delta Query。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 46f6eaa2938c44c458159415b1cca1838f549ffa
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/31/2019
ms.locfileid: "34656949"
---
# <a name="directoryrole-delta"></a><span data-ttu-id="d5b69-104">directoryRole: delta</span><span class="sxs-lookup"><span data-stu-id="d5b69-104">directoryRole: delta</span></span>

<span data-ttu-id="d5b69-105">获取新创建、更新或删除的目录角色, 而无需对整个资源集合执行完全读取。</span><span class="sxs-lookup"><span data-stu-id="d5b69-105">Get newly created, updated, or deleted directory roles without having to perform a full read of the entire resource collection.</span></span> <span data-ttu-id="d5b69-106">有关详细信息, 请参阅[Using Delta Query](/graph/delta-query-overview) 。</span><span class="sxs-lookup"><span data-stu-id="d5b69-106">See [Using Delta Query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="d5b69-107">权限</span><span class="sxs-lookup"><span data-stu-id="d5b69-107">Permissions</span></span>

<span data-ttu-id="d5b69-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d5b69-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d5b69-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d5b69-110">Permission type</span></span>      | <span data-ttu-id="d5b69-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d5b69-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d5b69-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d5b69-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d5b69-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d5b69-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d5b69-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d5b69-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5b69-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d5b69-115">Not supported.</span></span>    |
|<span data-ttu-id="d5b69-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d5b69-116">Application</span></span> | <span data-ttu-id="d5b69-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5b69-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d5b69-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d5b69-118">HTTP request</span></span>

<span data-ttu-id="d5b69-119">若要开始跟踪更改, 请在[directoryRole](../resources/directoryrole.md)资源上发出包含**delta**函数的请求。</span><span class="sxs-lookup"><span data-stu-id="d5b69-119">To begin tracking changes, you make a request including the **delta** function on the [directoryRole](../resources/directoryrole.md) resource.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/delta
```

## <a name="query-parameters"></a><span data-ttu-id="d5b69-120">查询参数</span><span class="sxs-lookup"><span data-stu-id="d5b69-120">Query parameters</span></span>

<span data-ttu-id="d5b69-121">跟踪更改会产生一个或多个**delta**函数调用的往返。</span><span class="sxs-lookup"><span data-stu-id="d5b69-121">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="d5b69-122">如果要使用任意查询参数（`$deltatoken` 和 `$skiptoken` 除外），则必须在最初的 **delta** 请求中指定它。</span><span class="sxs-lookup"><span data-stu-id="d5b69-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="d5b69-123">Microsoft Graph 自动将指定的任意参数编码为响应中提供的 `nextLink` 或 `deltaLink` URL 的令牌部分。</span><span class="sxs-lookup"><span data-stu-id="d5b69-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="d5b69-124">只需预先指定所需的任何查询参数一次。</span><span class="sxs-lookup"><span data-stu-id="d5b69-124">You only need to specify any desired query parameters once upfront.</span></span> <span data-ttu-id="d5b69-125">在后续请求中，可以复制并应用之前响应中返回的 `nextLink` 或 `deltaLink` URL，因为此 URL 已包含所需的编码参数。</span><span class="sxs-lookup"><span data-stu-id="d5b69-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="d5b69-126">查询参数</span><span class="sxs-lookup"><span data-stu-id="d5b69-126">Query parameter</span></span>      | <span data-ttu-id="d5b69-127">类型</span><span class="sxs-lookup"><span data-stu-id="d5b69-127">Type</span></span>   |<span data-ttu-id="d5b69-128">说明</span><span class="sxs-lookup"><span data-stu-id="d5b69-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d5b69-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="d5b69-129">$deltatoken</span></span> | <span data-ttu-id="d5b69-130">string</span><span class="sxs-lookup"><span data-stu-id="d5b69-130">string</span></span> | <span data-ttu-id="d5b69-131">为同一资源集合在上`deltaLink`一个**delta**函数调用的 URL 中返回的[状态令牌](/graph/delta-query-overview), 指示该往返一轮的更改。</span><span class="sxs-lookup"><span data-stu-id="d5b69-131">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="d5b69-132">在此集合的下`deltaLink`一轮变更跟踪请求中, 保存并应用整个 URL (包括此令牌)。</span><span class="sxs-lookup"><span data-stu-id="d5b69-132">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="d5b69-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="d5b69-133">$skiptoken</span></span> | <span data-ttu-id="d5b69-134">string</span><span class="sxs-lookup"><span data-stu-id="d5b69-134">string</span></span> | <span data-ttu-id="d5b69-135">在上一个**delta**函数调用`nextLink`的 URL 中返回的[状态令牌](/graph/delta-query-overview), 指示同一个资源集合中有进一步的更改需要跟踪。</span><span class="sxs-lookup"><span data-stu-id="d5b69-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same resource collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="d5b69-136">OData 查询参数</span><span class="sxs-lookup"><span data-stu-id="d5b69-136">OData query parameters</span></span>

<span data-ttu-id="d5b69-137">此方法支持 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d5b69-137">This method supports OData query parameters to help customize the response.</span></span>

- <span data-ttu-id="d5b69-p106">像在任何 GET 请求中一样，你可以使用 `$select` 查询参数以仅指定获取最佳性能所需的属性。始终返回 _id_ 属性。</span><span class="sxs-lookup"><span data-stu-id="d5b69-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span>

- <span data-ttu-id="d5b69-140">提供对 `$filter` 的有限支持：</span><span class="sxs-lookup"><span data-stu-id="d5b69-140">There is limited support for `$filter`:</span></span>

  - <span data-ttu-id="d5b69-141">唯一受支持`$filter`的表达式是跟踪对特定资源所做的更改, 其`$filter=id+eq+{value}` id `$filter=id+eq+{value1}+or+id+eq+{value2}`: 或。</span><span class="sxs-lookup"><span data-stu-id="d5b69-141">The only supported `$filter` expression is for tracking changes for specific resources, by their id:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="d5b69-142">您可以指定的 id 数受最大 URL 长度的限制。</span><span class="sxs-lookup"><span data-stu-id="d5b69-142">The number of ids you can specify is limited by the maximum URL length.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d5b69-143">请求标头</span><span class="sxs-lookup"><span data-stu-id="d5b69-143">Request headers</span></span>

| <span data-ttu-id="d5b69-144">名称</span><span class="sxs-lookup"><span data-stu-id="d5b69-144">Name</span></span>       | <span data-ttu-id="d5b69-145">说明</span><span class="sxs-lookup"><span data-stu-id="d5b69-145">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d5b69-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5b69-146">Authorization</span></span>  | <span data-ttu-id="d5b69-147">持有者&lt;令牌&gt;</span><span class="sxs-lookup"><span data-stu-id="d5b69-147">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="d5b69-148">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d5b69-148">Content-Type</span></span>  | <span data-ttu-id="d5b69-149">application/json</span><span class="sxs-lookup"><span data-stu-id="d5b69-149">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d5b69-150">请求正文</span><span class="sxs-lookup"><span data-stu-id="d5b69-150">Request body</span></span>

<span data-ttu-id="d5b69-151">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d5b69-151">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="d5b69-152">响应</span><span class="sxs-lookup"><span data-stu-id="d5b69-152">Response</span></span>

<span data-ttu-id="d5b69-153">如果成功, 此方法在`200 OK`响应正文中返回响应代码和[directoryRole](../resources/directoryrole.md)集合对象。</span><span class="sxs-lookup"><span data-stu-id="d5b69-153">If successful, this method returns `200 OK` response code and [directoryRole](../resources/directoryrole.md) collection object in the response body.</span></span> <span data-ttu-id="d5b69-154">该响应还包括 `nextLink`URL 或 `deltaLink`URL。</span><span class="sxs-lookup"><span data-stu-id="d5b69-154">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="d5b69-155">如果返回`nextLink` URL, 则会在会话中检索其他数据页。</span><span class="sxs-lookup"><span data-stu-id="d5b69-155">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="d5b69-156">应用程序继续使用 `nextLink` URL 发出请求，直到响应中包含 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="d5b69-156">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>

- <span data-ttu-id="d5b69-157">如果返回`deltaLink` URL, 则没有有关要返回的资源的现有状态的更多数据。</span><span class="sxs-lookup"><span data-stu-id="d5b69-157">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="d5b69-158">保存`deltaLink` URL 并在下一次**增量**调用中应用它, 以了解将来对资源所做的更改。</span><span class="sxs-lookup"><span data-stu-id="d5b69-158">Save `deltaLink` URL and apply it in the next **delta** call to learn about changes to the resource in the future.</span></span>

### <a name="example"></a><span data-ttu-id="d5b69-159">示例</span><span class="sxs-lookup"><span data-stu-id="d5b69-159">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d5b69-160">请求</span><span class="sxs-lookup"><span data-stu-id="d5b69-160">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryRole_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/directoryRoles/delta
```

##### <a name="response"></a><span data-ttu-id="d5b69-161">响应</span><span class="sxs-lookup"><span data-stu-id="d5b69-161">Response</span></span>

<span data-ttu-id="d5b69-p111">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d5b69-p111">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d5b69-164">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="d5b69-164">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d5b69-165">C#</span><span class="sxs-lookup"><span data-stu-id="d5b69-165">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/directoryRole_delta-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d5b69-166">Javascript</span><span class="sxs-lookup"><span data-stu-id="d5b69-166">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/directoryRole_delta-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="see-also"></a><span data-ttu-id="d5b69-167">另请参阅</span><span class="sxs-lookup"><span data-stu-id="d5b69-167">See also</span></span>

- <span data-ttu-id="d5b69-168">[使用 delta 查询跟踪 Microsoft Graph 数据中的更改](/graph/delta-query-overview), 了解更多详细信息</span><span class="sxs-lookup"><span data-stu-id="d5b69-168">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview) for more details</span></span>
- <span data-ttu-id="d5b69-169">[获取用户的增量更改](/graph/delta-query-users)获取示例请求。</span><span class="sxs-lookup"><span data-stu-id="d5b69-169">[Get incremental changes for users](/graph/delta-query-users) for an example requests.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryRole: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/directoryrole-delta.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/directoryrole-delta.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
