---
title: directoryRole： 增量
description: 获取新创建、 更新或删除目录角色而无需执行的整个资源集的完全读取。 有关详细信息，请参阅使用增量查询。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6da3e8c4cf92edbf79df1b082675c36d54e81292
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923836"
---
# <a name="directoryrole-delta"></a><span data-ttu-id="46fa0-104">directoryRole： 增量</span><span class="sxs-lookup"><span data-stu-id="46fa0-104">directoryRole: delta</span></span>

<span data-ttu-id="46fa0-105">获取新创建、 更新或删除目录角色而无需执行的整个资源集的完全读取。</span><span class="sxs-lookup"><span data-stu-id="46fa0-105">Get newly created, updated, or deleted directory roles without having to perform a full read of the entire resource collection.</span></span> <span data-ttu-id="46fa0-106">有关详细信息，请参阅[使用增量查询](/graph/delta-query-overview)。</span><span class="sxs-lookup"><span data-stu-id="46fa0-106">See [Using Delta Query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="46fa0-107">权限</span><span class="sxs-lookup"><span data-stu-id="46fa0-107">Permissions</span></span>

<span data-ttu-id="46fa0-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="46fa0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="46fa0-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="46fa0-110">Permission type</span></span>      | <span data-ttu-id="46fa0-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="46fa0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="46fa0-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="46fa0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="46fa0-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="46fa0-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="46fa0-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="46fa0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46fa0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="46fa0-115">Not supported.</span></span>    |
|<span data-ttu-id="46fa0-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="46fa0-116">Application</span></span> | <span data-ttu-id="46fa0-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46fa0-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="46fa0-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="46fa0-118">HTTP request</span></span>

<span data-ttu-id="46fa0-119">若要开始跟踪的更改，您发出请求包含**增量**函数对[directoryRole](../resources/directoryrole.md)资源。</span><span class="sxs-lookup"><span data-stu-id="46fa0-119">To begin tracking changes, you make a request including the **delta** function on the [directoryRole](../resources/directoryrole.md) resource.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/delta
```

## <a name="query-parameters"></a><span data-ttu-id="46fa0-120">查询参数</span><span class="sxs-lookup"><span data-stu-id="46fa0-120">Query parameters</span></span>

<span data-ttu-id="46fa0-121">跟踪更改会导致一个或多个**增量**函数调用的往返。</span><span class="sxs-lookup"><span data-stu-id="46fa0-121">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="46fa0-122">如果您使用任何查询参数 (以外的其他`$deltatoken`和`$skiptoken`)，则必须指定该初始**增量**请求中。</span><span class="sxs-lookup"><span data-stu-id="46fa0-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="46fa0-123">Microsoft Graph 自动将任何指定的参数编码为的令牌部分`nextLink`或`deltaLink`响应中提供的 URL。</span><span class="sxs-lookup"><span data-stu-id="46fa0-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="46fa0-124">只需预先指定所需的任何查询参数一次。</span><span class="sxs-lookup"><span data-stu-id="46fa0-124">You only need to specify any desired query parameters once upfront.</span></span> <span data-ttu-id="46fa0-125">在后续请求中，可以复制并应用之前响应中返回的 `nextLink` 或 `deltaLink` URL，因为此 URL 已包含所需的编码参数。</span><span class="sxs-lookup"><span data-stu-id="46fa0-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="46fa0-126">查询参数</span><span class="sxs-lookup"><span data-stu-id="46fa0-126">Query parameter</span></span>      | <span data-ttu-id="46fa0-127">类型</span><span class="sxs-lookup"><span data-stu-id="46fa0-127">Type</span></span>   |<span data-ttu-id="46fa0-128">说明</span><span class="sxs-lookup"><span data-stu-id="46fa0-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="46fa0-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="46fa0-129">$deltatoken</span></span> | <span data-ttu-id="46fa0-130">string</span><span class="sxs-lookup"><span data-stu-id="46fa0-130">string</span></span> | <span data-ttu-id="46fa0-131">返回一个[状态标记](/graph/delta-query-overview)`deltaLink`指示完成的修订的往返相同的资源集合，以前**增量**函数调用的 URL。</span><span class="sxs-lookup"><span data-stu-id="46fa0-131">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="46fa0-132">保存并应用整个`deltaLink`下一轮更改跟踪集合的第一个请求中包括此令牌的 URL。</span><span class="sxs-lookup"><span data-stu-id="46fa0-132">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="46fa0-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="46fa0-133">$skiptoken</span></span> | <span data-ttu-id="46fa0-134">string</span><span class="sxs-lookup"><span data-stu-id="46fa0-134">string</span></span> | <span data-ttu-id="46fa0-135">返回一个[状态标记](/graph/delta-query-overview)`nextLink`的以前的**增量**函数调用，指示有进一步的更改跟踪相同的资源集合中的 URL。</span><span class="sxs-lookup"><span data-stu-id="46fa0-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same resource collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="46fa0-136">OData 查询参数</span><span class="sxs-lookup"><span data-stu-id="46fa0-136">OData query parameters</span></span>

<span data-ttu-id="46fa0-137">此方法支持 OData 查询参数，以帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="46fa0-137">This method supports OData query parameters to help customize the response.</span></span>

- <span data-ttu-id="46fa0-p106">像在任何 GET 请求中一样，你可以使用 `$select` 查询参数以仅指定获取最佳性能所需的属性。始终返回 _id_ 属性。</span><span class="sxs-lookup"><span data-stu-id="46fa0-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span>

- <span data-ttu-id="46fa0-140">支持是有限的`$filter`:</span><span class="sxs-lookup"><span data-stu-id="46fa0-140">There is limited support for `$filter`:</span></span>

  - <span data-ttu-id="46fa0-141">仅支持`$filter`按其 id 跟踪的特定资源，更改为表达式：`$filter=id+eq+{value}`或`$filter=id+eq+{value1}+or+id+eq+{value2}`。</span><span class="sxs-lookup"><span data-stu-id="46fa0-141">The only supported `$filter` expression is for tracking changes for specific resources, by their id:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="46fa0-142">您可以指定的 id 数受最大 URL 长度限制。</span><span class="sxs-lookup"><span data-stu-id="46fa0-142">The number of ids you can specify is limited by the maximum URL length.</span></span>

## <a name="request-headers"></a><span data-ttu-id="46fa0-143">请求标头</span><span class="sxs-lookup"><span data-stu-id="46fa0-143">Request headers</span></span>

| <span data-ttu-id="46fa0-144">名称</span><span class="sxs-lookup"><span data-stu-id="46fa0-144">Name</span></span>       | <span data-ttu-id="46fa0-145">说明</span><span class="sxs-lookup"><span data-stu-id="46fa0-145">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="46fa0-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="46fa0-146">Authorization</span></span>  | <span data-ttu-id="46fa0-147">持有者&lt;令牌&gt;</span><span class="sxs-lookup"><span data-stu-id="46fa0-147">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="46fa0-148">Content-Type</span><span class="sxs-lookup"><span data-stu-id="46fa0-148">Content-Type</span></span>  | <span data-ttu-id="46fa0-149">application/json</span><span class="sxs-lookup"><span data-stu-id="46fa0-149">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="46fa0-150">请求正文</span><span class="sxs-lookup"><span data-stu-id="46fa0-150">Request body</span></span>

<span data-ttu-id="46fa0-151">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="46fa0-151">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="46fa0-152">响应</span><span class="sxs-lookup"><span data-stu-id="46fa0-152">Response</span></span>

<span data-ttu-id="46fa0-153">如果成功，此方法返回`200 OK`响应正文中的响应代码和[directoryRole](../resources/directoryrole.md)集合的对象。</span><span class="sxs-lookup"><span data-stu-id="46fa0-153">If successful, this method returns `200 OK` response code and [directoryRole](../resources/directoryrole.md) collection object in the response body.</span></span> <span data-ttu-id="46fa0-154">响应还包括`nextLink`URL 或`deltaLink`URL。</span><span class="sxs-lookup"><span data-stu-id="46fa0-154">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="46fa0-155">如果`nextLink`返回 URL、 有会话中检索的数据的其他页。</span><span class="sxs-lookup"><span data-stu-id="46fa0-155">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="46fa0-156">应用程序将继续进行请求使用`nextLink`直到 URL `deltaLink` URL 包含响应中。</span><span class="sxs-lookup"><span data-stu-id="46fa0-156">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>

- <span data-ttu-id="46fa0-157">如果`deltaLink`返回 URL、 没有更多有关要返回的资源的现有状态数据。</span><span class="sxs-lookup"><span data-stu-id="46fa0-157">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="46fa0-158">保存`deltaLink`URL 并将其应用在下一次**增量**呼叫将来了解到的资源的更改。</span><span class="sxs-lookup"><span data-stu-id="46fa0-158">Save `deltaLink` URL and apply it in the next **delta** call to learn about changes to the resource in the future.</span></span>

### <a name="example"></a><span data-ttu-id="46fa0-159">示例</span><span class="sxs-lookup"><span data-stu-id="46fa0-159">Example</span></span>

##### <a name="request"></a><span data-ttu-id="46fa0-160">请求</span><span class="sxs-lookup"><span data-stu-id="46fa0-160">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryRole_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/directoryRoles/delta
```

##### <a name="response"></a><span data-ttu-id="46fa0-161">响应</span><span class="sxs-lookup"><span data-stu-id="46fa0-161">Response</span></span>

<span data-ttu-id="46fa0-p111">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="46fa0-p111">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

### <a name="see-also"></a><span data-ttu-id="46fa0-164">另请参阅</span><span class="sxs-lookup"><span data-stu-id="46fa0-164">See also</span></span>

- <span data-ttu-id="46fa0-165">有关详细信息的[使用增量查询来跟踪 Microsoft Graph 数据中的更改](/graph/delta-query-overview)</span><span class="sxs-lookup"><span data-stu-id="46fa0-165">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview) for more details</span></span>
- <span data-ttu-id="46fa0-166">[获取用户的增量更改](/graph/delta-query-users)获取示例请求。</span><span class="sxs-lookup"><span data-stu-id="46fa0-166">[Get incremental changes for users](/graph/delta-query-users) for an example requests.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryRole: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
