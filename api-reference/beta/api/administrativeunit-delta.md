---
title: administrativeUnit： delta
description: 获取新建、更新或删除的管理单元，而无需执行整个资源集合的完全读取。
localization_priority: Normal
author: anandyadavMSFT
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: c5cfa9588897715d12668483b115395668d18141
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048286"
---
# <a name="administrativeunit-delta"></a><span data-ttu-id="a6622-103">administrativeUnit： delta</span><span class="sxs-lookup"><span data-stu-id="a6622-103">administrativeUnit: delta</span></span>

<span data-ttu-id="a6622-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6622-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6622-105">获取新创建、更新或删除 **的管理单元** ，而无需执行整个资源集合的完全读取。</span><span class="sxs-lookup"><span data-stu-id="a6622-105">Get newly created, updated, or deleted **administrativeUnits** without having to perform a full read of the entire resource collection.</span></span> <span data-ttu-id="a6622-106">有关详细信息，请参阅使用 [delta 查询](/graph/delta-query-overview)。</span><span class="sxs-lookup"><span data-stu-id="a6622-106">For details, see [Using delta query](/graph/delta-query-overview).</span></span>

## <a name="permissions"></a><span data-ttu-id="a6622-107">权限</span><span class="sxs-lookup"><span data-stu-id="a6622-107">Permissions</span></span>

<span data-ttu-id="a6622-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a6622-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a6622-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a6622-110">Permission type</span></span>      | <span data-ttu-id="a6622-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a6622-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a6622-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a6622-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a6622-113">AdministrativeUnit.Read.All、Directory.Read.All、AdministrativeUnit.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a6622-113">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a6622-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a6622-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6622-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a6622-115">Not supported.</span></span>    |
|<span data-ttu-id="a6622-116">administrativeunit</span><span class="sxs-lookup"><span data-stu-id="a6622-116">administrativeunit</span></span> | <span data-ttu-id="a6622-117">AdministrativeUnit.Read.All、Directory.Read.All、AdministrativeUnit.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6622-117">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a6622-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a6622-118">HTTP request</span></span>

<span data-ttu-id="a6622-119">若要开始跟踪更改，请对 **administrativeUnit** 资源提出包含 delta 函数的请求。</span><span class="sxs-lookup"><span data-stu-id="a6622-119">To begin tracking changes, you make a request that includes the delta function on the **administrativeUnit** resource.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits/delta
```

## <a name="query-parameters"></a><span data-ttu-id="a6622-120">查询参数</span><span class="sxs-lookup"><span data-stu-id="a6622-120">Query parameters</span></span>

<span data-ttu-id="a6622-121">跟踪更改将引发一次或多组 **delta** 函数调用。</span><span class="sxs-lookup"><span data-stu-id="a6622-121">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="a6622-122">如果要使用任意查询参数（`$deltatoken` 和 `$skiptoken` 除外），则必须在最初的 **delta** 请求中指定它。</span><span class="sxs-lookup"><span data-stu-id="a6622-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="a6622-123">Microsoft Graph 自动将指定的任意参数编码为响应中提供的 `nextLink` 或 `deltaLink` URL 的令牌部分。</span><span class="sxs-lookup"><span data-stu-id="a6622-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="a6622-124">只需指定任何查询参数一次。</span><span class="sxs-lookup"><span data-stu-id="a6622-124">You only need to specify any query parameters once up front.</span></span> <span data-ttu-id="a6622-125">在后续请求中，复制并应用 `nextLink` 上 `deltaLink` 一响应中的 或 URL。</span><span class="sxs-lookup"><span data-stu-id="a6622-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response.</span></span> <span data-ttu-id="a6622-126">该 URL 已包含编码参数。</span><span class="sxs-lookup"><span data-stu-id="a6622-126">That URL already includes the encoded parameters.</span></span>

| <span data-ttu-id="a6622-127">查询参数</span><span class="sxs-lookup"><span data-stu-id="a6622-127">Query parameter</span></span>      | <span data-ttu-id="a6622-128">类型</span><span class="sxs-lookup"><span data-stu-id="a6622-128">Type</span></span>   |<span data-ttu-id="a6622-129">说明</span><span class="sxs-lookup"><span data-stu-id="a6622-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a6622-130">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="a6622-130">$deltatoken</span></span> | <span data-ttu-id="a6622-131">string</span><span class="sxs-lookup"><span data-stu-id="a6622-131">string</span></span> | <span data-ttu-id="a6622-132">对[同一](/graph/delta-query-overview)资源集合之前的 delta 函数调用的 URL 中返回的状态令牌，指示完成这一轮 `deltaLink` 更改跟踪。 </span><span class="sxs-lookup"><span data-stu-id="a6622-132">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="a6622-133">将此令牌包含在对该集合的下一组更改追踪的首次请求中，并保存和应用整个 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="a6622-133">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="a6622-134">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="a6622-134">$skiptoken</span></span> | <span data-ttu-id="a6622-135">string</span><span class="sxs-lookup"><span data-stu-id="a6622-135">string</span></span> | <span data-ttu-id="a6622-136">之前的[delta](/graph/delta-query-overview)函数调用的 URL 中返回的状态令牌，指示同一资源集合中还有进一 `nextLink` 步的更改需要跟踪。 </span><span class="sxs-lookup"><span data-stu-id="a6622-136">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same resource collection.</span></span> |

### <a name="optional-query-parameters"></a><span data-ttu-id="a6622-137">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a6622-137">Optional query parameters</span></span>

<span data-ttu-id="a6622-138">此方法支持以下 OData 查询参数，它们有助于自定义响应：</span><span class="sxs-lookup"><span data-stu-id="a6622-138">This method supports the following OData query parameters to help customize the response:</span></span>

- <span data-ttu-id="a6622-p105">像在任何 GET 请求中一样，你可以使用 `$select` 查询参数以仅指定获取最佳性能所需的属性。始终返回 **id** 属性。</span><span class="sxs-lookup"><span data-stu-id="a6622-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The **id** property is always returned.</span></span> 

- <span data-ttu-id="a6622-141">提供对 `$filter` 的有限支持：</span><span class="sxs-lookup"><span data-stu-id="a6622-141">There is limited support for `$filter`:</span></span>
  * <span data-ttu-id="a6622-142">唯一 `$filter` 受支持的表达式用于按其 ID 跟踪特定资源的  `$filter=id+eq+{value}` 更改：或 `$filter=id+eq+{value1}+or+id+eq+{value2}` 。</span><span class="sxs-lookup"><span data-stu-id="a6622-142">The only supported `$filter` expression is for tracking changes for specific resources, by their ID:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="a6622-143">可以指定的 ID 数受最大 URL 长度限制。</span><span class="sxs-lookup"><span data-stu-id="a6622-143">The number of IDs you can specify is limited by the maximum URL length.</span></span>


## <a name="request-headers"></a><span data-ttu-id="a6622-144">请求标头</span><span class="sxs-lookup"><span data-stu-id="a6622-144">Request headers</span></span>
| <span data-ttu-id="a6622-145">名称</span><span class="sxs-lookup"><span data-stu-id="a6622-145">Name</span></span>       | <span data-ttu-id="a6622-146">说明</span><span class="sxs-lookup"><span data-stu-id="a6622-146">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a6622-147">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6622-147">Authorization</span></span>  | <span data-ttu-id="a6622-p107">持有者 &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a6622-p107">Bearer &lt;token&gt;. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6622-150">请求正文</span><span class="sxs-lookup"><span data-stu-id="a6622-150">Request body</span></span>
<span data-ttu-id="a6622-151">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a6622-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a6622-152">响应</span><span class="sxs-lookup"><span data-stu-id="a6622-152">Response</span></span>

<span data-ttu-id="a6622-153">如果成功，此方法在 `200 OK` 响应正文中返回 响应代码和 [administrativeUnit](../resources/administrativeunit.md) 集合对象。</span><span class="sxs-lookup"><span data-stu-id="a6622-153">If successful, this method returns `200 OK` response code and an [administrativeUnit](../resources/administrativeunit.md) collection object in the response body.</span></span> <span data-ttu-id="a6622-154">该响应还包括 `nextLink`URL 或 `deltaLink`URL。</span><span class="sxs-lookup"><span data-stu-id="a6622-154">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span> 

- <span data-ttu-id="a6622-155">如果 `nextLink` 返回 URL，则会话中有其他要检索的数据页。</span><span class="sxs-lookup"><span data-stu-id="a6622-155">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="a6622-156">**administrativeUnit** 继续使用 URL 提出 `nextLink` 请求，直到响应中包括 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="a6622-156">The **administrativeUnit** continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>

- <span data-ttu-id="a6622-157">如果 `deltaLink` 返回 URL，则不再返回有关资源现有状态的数据。</span><span class="sxs-lookup"><span data-stu-id="a6622-157">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="a6622-158">保留并使用 `deltaLink` URL 了解将来对资源的更改。</span><span class="sxs-lookup"><span data-stu-id="a6622-158">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="a6622-159">有关详细信息和示例，请参阅使用[delta 查询和](/graph/delta-query-overview)[获取用户的增量更改](/graph/delta-query-users)。</span><span class="sxs-lookup"><span data-stu-id="a6622-159">For details and an example, see [Using delta query](/graph/delta-query-overview) and [Get incremental changes for users](/graph/delta-query-users).</span></span>

## <a name="example"></a><span data-ttu-id="a6622-160">示例</span><span class="sxs-lookup"><span data-stu-id="a6622-160">Example</span></span>
### <a name="request"></a><span data-ttu-id="a6622-161">请求</span><span class="sxs-lookup"><span data-stu-id="a6622-161">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="a6622-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="a6622-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "administrativeunit_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/administrativeUnits/delta
```
# <a name="c"></a>[<span data-ttu-id="a6622-163">C#</span><span class="sxs-lookup"><span data-stu-id="a6622-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/administrativeunit-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a6622-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a6622-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/administrativeunit-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a6622-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a6622-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/administrativeunit-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a6622-166">Java</span><span class="sxs-lookup"><span data-stu-id="a6622-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/administrativeunit-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a6622-167">响应</span><span class="sxs-lookup"><span data-stu-id="a6622-167">Response</span></span>
><span data-ttu-id="a6622-168">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a6622-168">**Note:** The response object shown here might be shortened for readability.</span></span>
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


