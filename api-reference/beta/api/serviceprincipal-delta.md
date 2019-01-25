---
title: servicePrincipal： 增量
description: 获取新创建、 更新或删除的服务主体，而无需执行的整个资源集的完全读取。 有关详细信息，请参阅使用增量查询。
localization_priority: Normal
ms.openlocfilehash: ed0cf279d1d076e324d24e1774734e9aa14a6b34
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520072"
---
# <a name="serviceprincipal-delta"></a><span data-ttu-id="39855-104">servicePrincipal： 增量</span><span class="sxs-lookup"><span data-stu-id="39855-104">servicePrincipal: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39855-105">获取新创建、 更新或删除的服务主体，而无需执行的整个资源集的完全读取。</span><span class="sxs-lookup"><span data-stu-id="39855-105">Get newly created, updated, or deleted service principals without having to perform a full read of the entire resource collection.</span></span> <span data-ttu-id="39855-106">有关详细信息，请参阅[使用增量查询](/graph/delta-query-overview)。</span><span class="sxs-lookup"><span data-stu-id="39855-106">See [Using Delta Query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="39855-107">权限</span><span class="sxs-lookup"><span data-stu-id="39855-107">Permissions</span></span>

<span data-ttu-id="39855-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="39855-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="39855-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="39855-110">Permission type</span></span>      | <span data-ttu-id="39855-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="39855-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="39855-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="39855-112">Delegated (work or school account)</span></span> | <span data-ttu-id="39855-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="39855-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="39855-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="39855-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39855-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="39855-115">Not supported.</span></span>    |
|<span data-ttu-id="39855-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="39855-116">Application</span></span> | <span data-ttu-id="39855-117">Application.ReadWrite.All Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="39855-117">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="39855-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="39855-118">HTTP request</span></span>

<span data-ttu-id="39855-119">若要开始跟踪的更改，您发出请求包含增量函数对 servicePrincipal 资源。</span><span class="sxs-lookup"><span data-stu-id="39855-119">To begin tracking changes, you make a request including the delta function on the servicePrincipal resource.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/delta
```

### <a name="query-parameters"></a><span data-ttu-id="39855-120">查询参数</span><span class="sxs-lookup"><span data-stu-id="39855-120">Query parameters</span></span>

<span data-ttu-id="39855-121">跟踪更改会导致一个或多个**增量**函数调用的往返。</span><span class="sxs-lookup"><span data-stu-id="39855-121">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="39855-122">如果您使用任何查询参数 (以外的其他`$deltatoken`和`$skiptoken`)，则必须指定该初始**增量**请求中。</span><span class="sxs-lookup"><span data-stu-id="39855-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="39855-123">Microsoft Graph 自动将任何指定的参数编码为的令牌部分`nextLink`或`deltaLink`响应中提供的 URL。</span><span class="sxs-lookup"><span data-stu-id="39855-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="39855-124">只需预先指定所需的任何查询参数一次。</span><span class="sxs-lookup"><span data-stu-id="39855-124">You only need to specify any desired query parameters once upfront.</span></span> <span data-ttu-id="39855-125">在后续请求中，可以复制并应用之前响应中返回的 `nextLink` 或 `deltaLink` URL，因为此 URL 已包含所需的编码参数。</span><span class="sxs-lookup"><span data-stu-id="39855-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="39855-126">查询参数</span><span class="sxs-lookup"><span data-stu-id="39855-126">Query parameter</span></span>      | <span data-ttu-id="39855-127">类型</span><span class="sxs-lookup"><span data-stu-id="39855-127">Type</span></span>   |<span data-ttu-id="39855-128">说明</span><span class="sxs-lookup"><span data-stu-id="39855-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="39855-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="39855-129">$deltatoken</span></span> | <span data-ttu-id="39855-130">string</span><span class="sxs-lookup"><span data-stu-id="39855-130">string</span></span> | <span data-ttu-id="39855-131">返回一个[状态标记](/graph/delta-query-overview)`deltaLink`指示完成的修订的往返相同的资源集合，以前**增量**函数调用的 URL。</span><span class="sxs-lookup"><span data-stu-id="39855-131">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="39855-132">保存并应用整个`deltaLink`下一轮更改跟踪集合的第一个请求中包括此令牌的 URL。</span><span class="sxs-lookup"><span data-stu-id="39855-132">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="39855-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="39855-133">$skiptoken</span></span> | <span data-ttu-id="39855-134">string</span><span class="sxs-lookup"><span data-stu-id="39855-134">string</span></span> | <span data-ttu-id="39855-135">返回一个[状态标记](/graph/delta-query-overview)`nextLink`的以前的**增量**函数调用，指示有进一步的更改跟踪相同的资源集合中的 URL。</span><span class="sxs-lookup"><span data-stu-id="39855-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same resource collection.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="39855-136">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="39855-136">Optional query parameters</span></span>

<span data-ttu-id="39855-137">此方法支持 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="39855-137">This method supports OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="39855-p106">像在任何 GET 请求中一样，你可以使用 `$select` 查询参数以仅指定获取最佳性能所需的属性。始终返回 _id_ 属性。</span><span class="sxs-lookup"><span data-stu-id="39855-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 

- <span data-ttu-id="39855-140">支持是有限的`$filter`:</span><span class="sxs-lookup"><span data-stu-id="39855-140">There is limited support for `$filter`:</span></span>
  * <span data-ttu-id="39855-141">仅支持`$filter`按其 id 跟踪的特定资源，更改为表达式：`$filter=id+eq+{value}`或`$filter=id+eq+{value1}+or+id+eq+{value2}`。</span><span class="sxs-lookup"><span data-stu-id="39855-141">The only supported `$filter` expression is for tracking changes for specific resources, by their id:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="39855-142">您可以指定的 id 数受最大 URL 长度限制。</span><span class="sxs-lookup"><span data-stu-id="39855-142">The number of ids you can specify is limited by the maximum URL length.</span></span>


## <a name="request-headers"></a><span data-ttu-id="39855-143">请求标头</span><span class="sxs-lookup"><span data-stu-id="39855-143">Request headers</span></span>
| <span data-ttu-id="39855-144">名称</span><span class="sxs-lookup"><span data-stu-id="39855-144">Name</span></span>       | <span data-ttu-id="39855-145">说明</span><span class="sxs-lookup"><span data-stu-id="39855-145">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="39855-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="39855-146">Authorization</span></span>  | <span data-ttu-id="39855-147">持有者&lt;令牌&gt;</span><span class="sxs-lookup"><span data-stu-id="39855-147">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="39855-148">Content-Type</span><span class="sxs-lookup"><span data-stu-id="39855-148">Content-Type</span></span>  | <span data-ttu-id="39855-149">application/json</span><span class="sxs-lookup"><span data-stu-id="39855-149">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="39855-150">请求正文</span><span class="sxs-lookup"><span data-stu-id="39855-150">Request body</span></span>
<span data-ttu-id="39855-151">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="39855-151">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="39855-152">响应</span><span class="sxs-lookup"><span data-stu-id="39855-152">Response</span></span>

<span data-ttu-id="39855-153">如果成功，此方法返回`200 OK`响应正文中的响应代码和[servicePrincipal](../resources/serviceprincipal.md)集合的对象。</span><span class="sxs-lookup"><span data-stu-id="39855-153">If successful, this method returns `200 OK` response code and [servicePrincipal](../resources/serviceprincipal.md) collection object in the response body.</span></span> <span data-ttu-id="39855-154">响应还包括 nextLink 或 deltaLink URL。</span><span class="sxs-lookup"><span data-stu-id="39855-154">The response also includes a nextLink URL or a deltaLink URL.</span></span> 

- <span data-ttu-id="39855-155">如果`nextLink`返回 URL、 有会话中检索的数据的其他页。</span><span class="sxs-lookup"><span data-stu-id="39855-155">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="39855-156">应用程序将继续进行请求使用`nextLink`直到 URL `deltaLink` URL 包含响应中。</span><span class="sxs-lookup"><span data-stu-id="39855-156">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>

- <span data-ttu-id="39855-157">如果`deltaLink`返回 URL、 没有更多有关要返回的资源的现有状态数据。</span><span class="sxs-lookup"><span data-stu-id="39855-157">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="39855-158">保留和使用`deltaLink`URL 将来了解到的资源的更改。</span><span class="sxs-lookup"><span data-stu-id="39855-158">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="39855-159">请参阅：</span><span class="sxs-lookup"><span data-stu-id="39855-159">See:</span></span></br>
- <span data-ttu-id="39855-160">[使用增量查询](/graph/delta-query-overview)了解更多详细信息</span><span class="sxs-lookup"><span data-stu-id="39855-160">[Using Delta Query](/graph/delta-query-overview) for more details</span></span></br>
- <span data-ttu-id="39855-161">[获取用户的增量更改](/graph/delta-query-users)获取示例请求。</span><span class="sxs-lookup"><span data-stu-id="39855-161">[Get incremental changes for users](/graph/delta-query-users) for an example requests.</span></span></br>

### <a name="example"></a><span data-ttu-id="39855-162">示例</span><span class="sxs-lookup"><span data-stu-id="39855-162">Example</span></span>
##### <a name="request"></a><span data-ttu-id="39855-163">请求</span><span class="sxs-lookup"><span data-stu-id="39855-163">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "servicePrincipal_delta"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/delta
```

##### <a name="response"></a><span data-ttu-id="39855-164">响应</span><span class="sxs-lookup"><span data-stu-id="39855-164">Response</span></span>
<span data-ttu-id="39855-p111">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="39855-p111">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/serviceprincipal-delta.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
