---
title: directoryRole： 增量
description: 获取新创建、 更新或删除目录角色而无需执行的整个资源集的完全读取。 有关详细信息，请参阅使用增量查询。
ms.openlocfilehash: b426dd10ead2d1fc34c1d64aa235c343e8e71c3c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041689"
---
# <a name="directoryrole-delta"></a><span data-ttu-id="2a220-104">directoryRole： 增量</span><span class="sxs-lookup"><span data-stu-id="2a220-104">directoryRole: delta</span></span>

> <span data-ttu-id="2a220-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2a220-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2a220-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2a220-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2a220-107">获取新创建、 更新或删除目录角色而无需执行的整个资源集的完全读取。</span><span class="sxs-lookup"><span data-stu-id="2a220-107">Get newly created, updated, or deleted directory roles without having to perform a full read of the entire resource collection.</span></span> <span data-ttu-id="2a220-108">有关详细信息，请参阅[使用增量查询](/graph/delta-query-overview)。</span><span class="sxs-lookup"><span data-stu-id="2a220-108">See [Using Delta Query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="2a220-109">权限</span><span class="sxs-lookup"><span data-stu-id="2a220-109">Permissions</span></span>

<span data-ttu-id="2a220-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2a220-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2a220-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="2a220-112">Permission type</span></span>      | <span data-ttu-id="2a220-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2a220-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2a220-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2a220-114">Delegated (work or school account)</span></span> | <span data-ttu-id="2a220-115">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2a220-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2a220-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2a220-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a220-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="2a220-117">Not supported.</span></span>    |
|<span data-ttu-id="2a220-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="2a220-118">Application</span></span> | <span data-ttu-id="2a220-119">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a220-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2a220-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2a220-120">HTTP request</span></span>

<span data-ttu-id="2a220-121">若要开始跟踪的更改，您发出请求包含增量函数对 directoryRole 资源。</span><span class="sxs-lookup"><span data-stu-id="2a220-121">To begin tracking changes, you make a request including the delta function on the directoryRole resource.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/delta
```

### <a name="query-parameters"></a><span data-ttu-id="2a220-122">查询参数</span><span class="sxs-lookup"><span data-stu-id="2a220-122">Query parameters</span></span>

<span data-ttu-id="2a220-123">跟踪更改会导致一个或多个**增量**函数调用的往返。</span><span class="sxs-lookup"><span data-stu-id="2a220-123">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="2a220-124">如果您使用任何查询参数 (以外的其他`$deltatoken`和`$skiptoken`)，则必须指定该初始**增量**请求中。</span><span class="sxs-lookup"><span data-stu-id="2a220-124">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="2a220-125">Microsoft Graph 自动将任何指定的参数编码为的令牌部分`nextLink`或`deltaLink`响应中提供的 URL。</span><span class="sxs-lookup"><span data-stu-id="2a220-125">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="2a220-126">只需预先指定所需的任何查询参数一次。</span><span class="sxs-lookup"><span data-stu-id="2a220-126">You only need to specify any desired query parameters once upfront.</span></span> <span data-ttu-id="2a220-127">在后续请求中，可以复制并应用之前响应中返回的 `nextLink` 或 `deltaLink` URL，因为此 URL 已包含所需的编码参数。</span><span class="sxs-lookup"><span data-stu-id="2a220-127">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="2a220-128">查询参数</span><span class="sxs-lookup"><span data-stu-id="2a220-128">Query parameter</span></span>      | <span data-ttu-id="2a220-129">类型</span><span class="sxs-lookup"><span data-stu-id="2a220-129">Type</span></span>   |<span data-ttu-id="2a220-130">说明</span><span class="sxs-lookup"><span data-stu-id="2a220-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2a220-131">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="2a220-131">$deltatoken</span></span> | <span data-ttu-id="2a220-132">string</span><span class="sxs-lookup"><span data-stu-id="2a220-132">string</span></span> | <span data-ttu-id="2a220-133">返回一个[状态标记](/graph/delta-query-overview)`deltaLink`指示完成的修订的往返相同的资源集合，以前**增量**函数调用的 URL。</span><span class="sxs-lookup"><span data-stu-id="2a220-133">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="2a220-134">保存并应用整个`deltaLink`下一轮更改跟踪集合的第一个请求中包括此令牌的 URL。</span><span class="sxs-lookup"><span data-stu-id="2a220-134">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="2a220-135">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="2a220-135">$skiptoken</span></span> | <span data-ttu-id="2a220-136">string</span><span class="sxs-lookup"><span data-stu-id="2a220-136">string</span></span> | <span data-ttu-id="2a220-137">返回一个[状态标记](/graph/delta-query-overview)`nextLink`的以前的**增量**函数调用，指示有进一步的更改跟踪相同的资源集合中的 URL。</span><span class="sxs-lookup"><span data-stu-id="2a220-137">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same resource collection.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="2a220-138">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2a220-138">Optional query parameters</span></span>

<span data-ttu-id="2a220-139">此方法支持 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2a220-139">This method supports OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="2a220-p107">像在任何 GET 请求中一样，你可以使用 `$select` 查询参数以仅指定获取最佳性能所需的属性。始终返回 _id_ 属性。</span><span class="sxs-lookup"><span data-stu-id="2a220-p107">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 

- <span data-ttu-id="2a220-142">支持是有限的`$filter`:</span><span class="sxs-lookup"><span data-stu-id="2a220-142">There is limited support for `$filter`:</span></span>
  * <span data-ttu-id="2a220-143">仅支持`$filter`按其 id 跟踪的特定资源，更改为表达式：`$filter=id+eq+{value}`或`$filter=id+eq+{value1}+or+id+eq+{value2}`。</span><span class="sxs-lookup"><span data-stu-id="2a220-143">The only supported `$filter` expression is for tracking changes for specific resources, by their id:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="2a220-144">您可以指定的 id 数受最大 URL 长度限制。</span><span class="sxs-lookup"><span data-stu-id="2a220-144">The number of ids you can specify is limited by the maximum URL length.</span></span>


## <a name="request-headers"></a><span data-ttu-id="2a220-145">请求标头</span><span class="sxs-lookup"><span data-stu-id="2a220-145">Request headers</span></span>
| <span data-ttu-id="2a220-146">名称</span><span class="sxs-lookup"><span data-stu-id="2a220-146">Name</span></span>       | <span data-ttu-id="2a220-147">说明</span><span class="sxs-lookup"><span data-stu-id="2a220-147">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2a220-148">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a220-148">Authorization</span></span>  | <span data-ttu-id="2a220-149">持有者&lt;令牌&gt;</span><span class="sxs-lookup"><span data-stu-id="2a220-149">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="2a220-150">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2a220-150">Content-Type</span></span>  | <span data-ttu-id="2a220-151">application/json</span><span class="sxs-lookup"><span data-stu-id="2a220-151">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="2a220-152">请求正文</span><span class="sxs-lookup"><span data-stu-id="2a220-152">Request body</span></span>
<span data-ttu-id="2a220-153">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2a220-153">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="2a220-154">响应</span><span class="sxs-lookup"><span data-stu-id="2a220-154">Response</span></span>

<span data-ttu-id="2a220-155">如果成功，此方法返回`200 OK`响应正文中的响应代码和[directoryRole](../resources/directoryrole.md)集合的对象。</span><span class="sxs-lookup"><span data-stu-id="2a220-155">If successful, this method returns `200 OK` response code and [directoryRole](../resources/directoryrole.md) collection object in the response body.</span></span> <span data-ttu-id="2a220-156">响应还包括 nextLink 或 deltaLink URL。</span><span class="sxs-lookup"><span data-stu-id="2a220-156">The response also includes a nextLink URL or a deltaLink URL.</span></span> 

- <span data-ttu-id="2a220-157">如果`nextLink`返回 URL、 有会话中检索的数据的其他页。</span><span class="sxs-lookup"><span data-stu-id="2a220-157">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="2a220-158">应用程序将继续进行请求使用`nextLink`直到 URL `deltaLink` URL 包含响应中。</span><span class="sxs-lookup"><span data-stu-id="2a220-158">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>

- <span data-ttu-id="2a220-159">如果`deltaLink`返回 URL、 没有更多有关要返回的资源的现有状态数据。</span><span class="sxs-lookup"><span data-stu-id="2a220-159">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="2a220-160">保留和使用`deltaLink`URL 将来了解到的资源的更改。</span><span class="sxs-lookup"><span data-stu-id="2a220-160">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="2a220-161">请参阅：</span><span class="sxs-lookup"><span data-stu-id="2a220-161">See:</span></span></br>
- <span data-ttu-id="2a220-162">[使用增量查询](/graph/delta-query-overview)了解更多详细信息</span><span class="sxs-lookup"><span data-stu-id="2a220-162">[Using Delta Query](/graph/delta-query-overview) for more details</span></span></br>
- <span data-ttu-id="2a220-163">[获取用户的增量更改](/graph/delta-query-users)获取示例请求。</span><span class="sxs-lookup"><span data-stu-id="2a220-163">[Get incremental changes for users](/graph/delta-query-users) for an example requests.</span></span></br>

### <a name="example"></a><span data-ttu-id="2a220-164">示例</span><span class="sxs-lookup"><span data-stu-id="2a220-164">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2a220-165">请求</span><span class="sxs-lookup"><span data-stu-id="2a220-165">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "directoryRole_delta"
}-->
```http
GET https://graph.microsoft.com/beta/directoryRoles/delta
```

##### <a name="response"></a><span data-ttu-id="2a220-166">响应</span><span class="sxs-lookup"><span data-stu-id="2a220-166">Response</span></span>
<span data-ttu-id="2a220-p112">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2a220-p112">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "directoryRole: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->