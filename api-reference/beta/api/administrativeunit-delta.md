---
title: administrativeUnit： delta
description: 获取新创建、更新或删除的管理单元，而无需执行整个资源集合的完全读取。
localization_priority: Normal
author: anandyadavMSFT
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: b3056615a09a027911fd98c0636c6e313a2cad2c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438895"
---
# <a name="administrativeunit-delta"></a><span data-ttu-id="ed7fa-103">administrativeUnit： delta</span><span class="sxs-lookup"><span data-stu-id="ed7fa-103">administrativeUnit: delta</span></span>

<span data-ttu-id="ed7fa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed7fa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed7fa-105">获取新创建、更新或删除的 **administrativeUnits，** 而无需执行整个资源集合的完全读取。</span><span class="sxs-lookup"><span data-stu-id="ed7fa-105">Get newly created, updated, or deleted **administrativeUnits** without having to perform a full read of the entire resource collection.</span></span> <span data-ttu-id="ed7fa-106">有关详细信息，请参阅使用 [delta 查询](/graph/delta-query-overview)。</span><span class="sxs-lookup"><span data-stu-id="ed7fa-106">For details, see [Using delta query](/graph/delta-query-overview).</span></span>

## <a name="permissions"></a><span data-ttu-id="ed7fa-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="ed7fa-107">Permissions</span></span>

<span data-ttu-id="ed7fa-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ed7fa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ed7fa-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ed7fa-110">Permission type</span></span>      | <span data-ttu-id="ed7fa-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ed7fa-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ed7fa-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ed7fa-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ed7fa-113">AdministrativeUnit.Read.All、Directory.Read.All、AdministrativeUnit.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ed7fa-113">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ed7fa-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ed7fa-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed7fa-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ed7fa-115">Not supported.</span></span>    |
|<span data-ttu-id="ed7fa-116">administrativeunit</span><span class="sxs-lookup"><span data-stu-id="ed7fa-116">administrativeunit</span></span> | <span data-ttu-id="ed7fa-117">AdministrativeUnit.Read.All、Directory.Read.All、AdministrativeUnit.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed7fa-117">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ed7fa-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ed7fa-118">HTTP request</span></span>

<span data-ttu-id="ed7fa-119">若要开始跟踪更改，请对 **administrativeUnit** 资源提出包含 delta 函数的请求。</span><span class="sxs-lookup"><span data-stu-id="ed7fa-119">To begin tracking changes, you make a request that includes the delta function on the **administrativeUnit** resource.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits/delta
```

## <a name="query-parameters"></a><span data-ttu-id="ed7fa-120">查询参数</span><span class="sxs-lookup"><span data-stu-id="ed7fa-120">Query parameters</span></span>

<span data-ttu-id="ed7fa-121">跟踪更改将引发一轮或多次 **delta** 函数调用。</span><span class="sxs-lookup"><span data-stu-id="ed7fa-121">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="ed7fa-122">如果要使用任意查询参数（`$deltatoken` 和 `$skiptoken` 除外），则必须在最初的 **delta** 请求中指定它。</span><span class="sxs-lookup"><span data-stu-id="ed7fa-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="ed7fa-123">Microsoft Graph 自动将指定的任意参数编码为响应中提供的 `nextLink` 或 `deltaLink` URL 的令牌部分。</span><span class="sxs-lookup"><span data-stu-id="ed7fa-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="ed7fa-124">只需指定任何查询参数一次。</span><span class="sxs-lookup"><span data-stu-id="ed7fa-124">You only need to specify any query parameters once up front.</span></span> <span data-ttu-id="ed7fa-125">在后续请求中，复制并应用 `nextLink` 上一 `deltaLink` 响应中的 OR URL。</span><span class="sxs-lookup"><span data-stu-id="ed7fa-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response.</span></span> <span data-ttu-id="ed7fa-126">该 URL 已包含编码参数。</span><span class="sxs-lookup"><span data-stu-id="ed7fa-126">That URL already includes the encoded parameters.</span></span>

| <span data-ttu-id="ed7fa-127">查询参数</span><span class="sxs-lookup"><span data-stu-id="ed7fa-127">Query parameter</span></span>      | <span data-ttu-id="ed7fa-128">类型</span><span class="sxs-lookup"><span data-stu-id="ed7fa-128">Type</span></span>   |<span data-ttu-id="ed7fa-129">说明</span><span class="sxs-lookup"><span data-stu-id="ed7fa-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ed7fa-130">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="ed7fa-130">$deltatoken</span></span> | <span data-ttu-id="ed7fa-131">string</span><span class="sxs-lookup"><span data-stu-id="ed7fa-131">string</span></span> | <span data-ttu-id="ed7fa-132">同[一资源](/graph/delta-query-overview)集合的上一个 delta 函数调用的 URL 中返回的状态令牌，指示完成这一轮 `deltaLink` 更改跟踪。 </span><span class="sxs-lookup"><span data-stu-id="ed7fa-132">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="ed7fa-133">将此令牌包含在对该集合的下一组更改追踪的首次请求中，并保存和应用整个 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="ed7fa-133">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="ed7fa-134">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="ed7fa-134">$skiptoken</span></span> | <span data-ttu-id="ed7fa-135">string</span><span class="sxs-lookup"><span data-stu-id="ed7fa-135">string</span></span> | <span data-ttu-id="ed7fa-136">在[上一](/graph/delta-query-overview)个 delta 函数调用的 URL 中返回的状态令牌，指示同一资源集合中还有要跟踪的进一 `nextLink` 步更改。 </span><span class="sxs-lookup"><span data-stu-id="ed7fa-136">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same resource collection.</span></span> |

### <a name="optional-query-parameters"></a><span data-ttu-id="ed7fa-137">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ed7fa-137">Optional query parameters</span></span>

<span data-ttu-id="ed7fa-138">此方法支持以下 OData 查询参数，它们有助于自定义响应：</span><span class="sxs-lookup"><span data-stu-id="ed7fa-138">This method supports the following OData query parameters to help customize the response:</span></span>

- <span data-ttu-id="ed7fa-p105">像在任何 GET 请求中一样，你可以使用 `$select` 查询参数以仅指定获取最佳性能所需的属性。始终返回 **id** 属性。</span><span class="sxs-lookup"><span data-stu-id="ed7fa-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The **id** property is always returned.</span></span> 

- <span data-ttu-id="ed7fa-141">提供对 `$filter` 的有限支持：</span><span class="sxs-lookup"><span data-stu-id="ed7fa-141">There is limited support for `$filter`:</span></span>
  * <span data-ttu-id="ed7fa-142">唯一受支持的 `$filter` 表达式用于按其 ID 跟踪特定资源的更改：  `$filter=id+eq+{value}` 或 `$filter=id+eq+{value1}+or+id+eq+{value2}` 。</span><span class="sxs-lookup"><span data-stu-id="ed7fa-142">The only supported `$filter` expression is for tracking changes for specific resources, by their ID:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="ed7fa-143">可以指定的 ID 数受最大 URL 长度限制。</span><span class="sxs-lookup"><span data-stu-id="ed7fa-143">The number of IDs you can specify is limited by the maximum URL length.</span></span>


## <a name="request-headers"></a><span data-ttu-id="ed7fa-144">请求标头</span><span class="sxs-lookup"><span data-stu-id="ed7fa-144">Request headers</span></span>
| <span data-ttu-id="ed7fa-145">名称</span><span class="sxs-lookup"><span data-stu-id="ed7fa-145">Name</span></span>       | <span data-ttu-id="ed7fa-146">说明</span><span class="sxs-lookup"><span data-stu-id="ed7fa-146">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ed7fa-147">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed7fa-147">Authorization</span></span>  | <span data-ttu-id="ed7fa-148">持有者 &lt;token&gt;。</span><span class="sxs-lookup"><span data-stu-id="ed7fa-148">Bearer &lt;token&gt;.</span></span> <span data-ttu-id="ed7fa-149">必需。</span><span class="sxs-lookup"><span data-stu-id="ed7fa-149">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed7fa-150">请求正文</span><span class="sxs-lookup"><span data-stu-id="ed7fa-150">Request body</span></span>
<span data-ttu-id="ed7fa-151">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ed7fa-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed7fa-152">响应</span><span class="sxs-lookup"><span data-stu-id="ed7fa-152">Response</span></span>

<span data-ttu-id="ed7fa-153">如果成功，此方法在 `200 OK` 响应正文中返回响应代码和 [administrativeUnit](../resources/administrativeunit.md) 集合对象。</span><span class="sxs-lookup"><span data-stu-id="ed7fa-153">If successful, this method returns `200 OK` response code and an [administrativeUnit](../resources/administrativeunit.md) collection object in the response body.</span></span> <span data-ttu-id="ed7fa-154">该响应还包括 `nextLink`URL 或 `deltaLink`URL。</span><span class="sxs-lookup"><span data-stu-id="ed7fa-154">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span> 

- <span data-ttu-id="ed7fa-155">如果 `nextLink` 返回 URL，则会话中将检索其他数据页。</span><span class="sxs-lookup"><span data-stu-id="ed7fa-155">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="ed7fa-156">**administrativeUnit** 继续使用 URL 提出 `nextLink` 请求，直到 `deltaLink` 响应中包括 URL。</span><span class="sxs-lookup"><span data-stu-id="ed7fa-156">The **administrativeUnit** continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>

- <span data-ttu-id="ed7fa-157">如果 `deltaLink` 返回 URL，则不再返回有关资源现有状态的数据。</span><span class="sxs-lookup"><span data-stu-id="ed7fa-157">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="ed7fa-158">保留并使用 `deltaLink` URL 了解将来资源更改。</span><span class="sxs-lookup"><span data-stu-id="ed7fa-158">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="ed7fa-159">有关详细信息和示例，请参阅使用 [增量查询](/graph/delta-query-overview) 和 [获取用户的增量更改](/graph/delta-query-users)。</span><span class="sxs-lookup"><span data-stu-id="ed7fa-159">For details and an example, see [Using delta query](/graph/delta-query-overview) and [Get incremental changes for users](/graph/delta-query-users).</span></span>

## <a name="example"></a><span data-ttu-id="ed7fa-160">示例</span><span class="sxs-lookup"><span data-stu-id="ed7fa-160">Example</span></span>
### <a name="request"></a><span data-ttu-id="ed7fa-161">请求</span><span class="sxs-lookup"><span data-stu-id="ed7fa-161">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ed7fa-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="ed7fa-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "administrativeunit_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/administrativeUnits/delta
```
# <a name="c"></a>[<span data-ttu-id="ed7fa-163">C#</span><span class="sxs-lookup"><span data-stu-id="ed7fa-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/administrativeunit-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ed7fa-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ed7fa-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/administrativeunit-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ed7fa-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ed7fa-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/administrativeunit-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ed7fa-166">Java</span><span class="sxs-lookup"><span data-stu-id="ed7fa-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/administrativeunit-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ed7fa-167">响应</span><span class="sxs-lookup"><span data-stu-id="ed7fa-167">Response</span></span>
><span data-ttu-id="ed7fa-p111">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ed7fa-p111">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- { 
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeUnit",
  "isCollection": true 
} --> 
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#administrativeunits",
  "@odata.nextLink":"https://graph.microsoft.com/beta/administrativeunits/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "Management Fast Track",
      "visibility": null,
      "extension_fe2174665583431c953114ff7268b7b3_Education_ObjectType": "School",
      "extension_fe2174665583431c953114ff7268b7b3_Education_StateId": "WA",
      "extension_fe2174665583431c953114ff7268b7b3_Education_Address": "2 Microsoft Way",
      "extension_fe2174665583431c953114ff7268b7b3_Education_City": "Redmond",
      "extension_fe2174665583431c953114ff7268b7b3_Education_State": "WA",
      "extension_fe2174665583431c953114ff7268b7b3_Education_Country": "US",
      "extension_fe2174665583431c953114ff7268b7b3_Education_Zip": "98052",
      "extension_fe2174665583431c953114ff7268b7b3_Education_Phone": "555-123-4567",
      "extension_fe2174665583431c953114ff7268b7b3_Education_SyncSource": "SIS",
      "extension_fe2174665583431c953114ff7268b7b3_Education_SyncSource_SchoolId": "10002",
      "extension_fe2174665583431c953114ff7268b7b3_Education_SchoolPrincipalSyncSourceId": "14008",
      "extension_fe2174665583431c953114ff7268b7b3_Education_SchoolPrincipalName": "Amy Roebuck",
      "extension_fe2174665583431c953114ff7268b7b3_Education_SchoolPrincipalEmail": "aroebuck@principal.edu",
      "extension_fe2174665583431c953114ff7268b7b3_Education_SchoolZone": "1",
      "id": "8a07f5a8-edc9-4847-bbf2-dde106594bf4",
      "members@delta": [
        {
            "@odata.type": "#microsoft.graph.user",
            "id": "b66ecf79-a093-4d51-86e0-efcc4531f37a"
        },
        {
            "@odata.type": "#microsoft.graph.user",
            "id": "5bde3e51-d13b-4db1-9948-fe4b109d11a7"
        },
        {
            "@odata.type": "#microsoft.graph.group",
            "id": "801f2093-de7e-4883-a786-8a5f30874ff4"
        },
        {
            "@odata.type": "#microsoft.graph.group",
            "id": "7e4ec76c-8276-43ef-ba10-9aaa197cb212"
        },
        {
            "@odata.type": "#microsoft.graph.user",
            "id": "f5289423-7233-4d60-831a-fe107a8551cc"
        },
        {
            "@odata.type": "#microsoft.graph.user",
            "id": "48d31887-5fad-4d73-a9f5-3c356e68a038"
        },
        {
            "@odata.type": "#microsoft.graph.user",
            "id": "87d349ed-44d7-43e1-9a83-5f2406dee5bd"
        },
        {
            "@odata.type": "#microsoft.graph.user",
            "id": "c03e6eaa-b6ab-46d7-905b-73ec7ea1f755"
        }
      ]
  }
  ]
}
```

<!-- uuid: 69848a18-6b48-44fd-a398-4521803a0a00
2020-04-09 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "administrativeunit: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


