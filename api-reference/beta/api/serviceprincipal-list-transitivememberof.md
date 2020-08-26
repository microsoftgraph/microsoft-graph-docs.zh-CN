---
title: List servicePrincipal transitive memberOf
description: 获取此服务主体所属的组和目录角色。
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: e1d263f11eeb74efe7df00ee34cd8222e23d285b
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2020
ms.locfileid: "46872773"
---
# <a name="list-serviceprincipal-transitive-memberof"></a><span data-ttu-id="26b0c-103">List servicePrincipal transitive memberOf</span><span class="sxs-lookup"><span data-stu-id="26b0c-103">List servicePrincipal transitive memberOf</span></span>

<span data-ttu-id="26b0c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26b0c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26b0c-105">获取此 [servicePrincipal](../resources/serviceprincipal.md) 所属的组和目录角色。</span><span class="sxs-lookup"><span data-stu-id="26b0c-105">Get the groups and directory roles that this [servicePrincipal](../resources/serviceprincipal.md) is a member of.</span></span> <span data-ttu-id="26b0c-106">此操作是可传递的，将包括此服务主体以嵌套方式所属的组。</span><span class="sxs-lookup"><span data-stu-id="26b0c-106">This operation is transitive and will include all groups that this service principal is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="26b0c-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="26b0c-107">Permissions</span></span>
<span data-ttu-id="26b0c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="26b0c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26b0c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="26b0c-110">Permission type</span></span>      | <span data-ttu-id="26b0c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="26b0c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="26b0c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="26b0c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="26b0c-113">Application.Read.All、Application.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="26b0c-113">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="26b0c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="26b0c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26b0c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="26b0c-115">Not supported.</span></span>    |
|<span data-ttu-id="26b0c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="26b0c-116">Application</span></span> | <span data-ttu-id="26b0c-117">Application.Read.All、Application.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26b0c-117">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="26b0c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="26b0c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/transitiveMemberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="26b0c-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="26b0c-119">Optional query parameters</span></span>
<span data-ttu-id="26b0c-120">此方法支持[OData query parameters](/graph/query_parameters)以帮助自定义响应，包括 `$search`、`$count`、 和 `$filter`</span><span class="sxs-lookup"><span data-stu-id="26b0c-120">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="26b0c-121">还启用了 OData 强制转换，例如，你可以强制转换为仅获取用户所属的 directoryRoles。</span><span class="sxs-lookup"><span data-stu-id="26b0c-121">OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of.</span></span> <span data-ttu-id="26b0c-122">`$search`可以用在 **displayName**属性。</span><span class="sxs-lookup"><span data-stu-id="26b0c-122">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="26b0c-123">为该资源添加或更新项目时，将对它们进行专门索引，以便与 `$count` 和 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="26b0c-123">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="26b0c-124">在添加或更新项目与在索引中可用之间可能会稍有延迟。</span><span class="sxs-lookup"><span data-stu-id="26b0c-124">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="26b0c-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="26b0c-125">Request headers</span></span>

| <span data-ttu-id="26b0c-126">名称</span><span class="sxs-lookup"><span data-stu-id="26b0c-126">Name</span></span>       | <span data-ttu-id="26b0c-127">类型</span><span class="sxs-lookup"><span data-stu-id="26b0c-127">Type</span></span> | <span data-ttu-id="26b0c-128">说明</span><span class="sxs-lookup"><span data-stu-id="26b0c-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="26b0c-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="26b0c-129">Authorization</span></span>  | <span data-ttu-id="26b0c-130">string</span><span class="sxs-lookup"><span data-stu-id="26b0c-130">string</span></span>  | <span data-ttu-id="26b0c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="26b0c-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="26b0c-133">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="26b0c-133">ConsistencyLevel</span></span> | <span data-ttu-id="26b0c-134">最终。</span><span class="sxs-lookup"><span data-stu-id="26b0c-134">eventual.</span></span> <span data-ttu-id="26b0c-135">使用 `$search`、`$filter`、`$orderby` 或 OData 强制转换查询参数时，此标头和 `$count` 是必需的。</span><span class="sxs-lookup"><span data-stu-id="26b0c-135">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="26b0c-136">它使用的索引可能与对象的最新更改不同步。</span><span class="sxs-lookup"><span data-stu-id="26b0c-136">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="26b0c-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="26b0c-137">Request body</span></span>
<span data-ttu-id="26b0c-138">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="26b0c-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="26b0c-139">响应</span><span class="sxs-lookup"><span data-stu-id="26b0c-139">Response</span></span>

<span data-ttu-id="26b0c-140">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="26b0c-140">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="26b0c-141">示例</span><span class="sxs-lookup"><span data-stu-id="26b0c-141">Examples</span></span>

### <a name="example-1-get-groups-and-directory-roles-that-the-service-principal-is-a-transitive-member-of"></a><span data-ttu-id="26b0c-142">示例 1：获取此服务主体作为可传递成员所属的组和目录角色</span><span class="sxs-lookup"><span data-stu-id="26b0c-142">Example 1: Get groups and directory roles that the service principal is a transitive member of</span></span>

#### <a name="request"></a><span data-ttu-id="26b0c-143">请求</span><span class="sxs-lookup"><span data-stu-id="26b0c-143">Request</span></span>

<span data-ttu-id="26b0c-144">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="26b0c-144">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="26b0c-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="26b0c-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal_tranitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="26b0c-146">C#</span><span class="sxs-lookup"><span data-stu-id="26b0c-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceprincipal-tranitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="26b0c-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="26b0c-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceprincipal-tranitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="26b0c-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="26b0c-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceprincipal-tranitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="26b0c-149">响应</span><span class="sxs-lookup"><span data-stu-id="26b0c-149">Response</span></span>

<span data-ttu-id="26b0c-150">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="26b0c-150">The following is an example of the response.</span></span> 
> <span data-ttu-id="26b0c-151">**注意：** 为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="26b0c-151">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="26b0c-152">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="26b0c-152">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-all-transitive-membership"></a><span data-ttu-id="26b0c-153">示例 2：仅获取所有可传递成员身份的计数</span><span class="sxs-lookup"><span data-stu-id="26b0c-153">Example 2: Get only a count of all transitive membership</span></span>

#### <a name="request"></a><span data-ttu-id="26b0c-154">请求</span><span class="sxs-lookup"><span data-stu-id="26b0c-154">Request</span></span>

<span data-ttu-id="26b0c-155">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="26b0c-155">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="26b0c-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="26b0c-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/transitiveMemberOf/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="26b0c-157">C#</span><span class="sxs-lookup"><span data-stu-id="26b0c-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="26b0c-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="26b0c-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="26b0c-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="26b0c-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="26b0c-160">响应</span><span class="sxs-lookup"><span data-stu-id="26b0c-160">Response</span></span>

<span data-ttu-id="26b0c-161">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="26b0c-161">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

<span data-ttu-id="26b0c-162">294</span><span class="sxs-lookup"><span data-stu-id="26b0c-162">294</span></span>

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-transitive-membership-in-groups"></a><span data-ttu-id="26b0c-163">示例 3：使用 OData 强制转换以仅获取组中可传递成员身份的计数</span><span class="sxs-lookup"><span data-stu-id="26b0c-163">Example 3: Use OData cast to get only a count of transitive membership in groups</span></span>

#### <a name="request"></a><span data-ttu-id="26b0c-164">请求</span><span class="sxs-lookup"><span data-stu-id="26b0c-164">Request</span></span>

<span data-ttu-id="26b0c-165">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="26b0c-165">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="26b0c-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="26b0c-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/transitiveMemberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="26b0c-167">C#</span><span class="sxs-lookup"><span data-stu-id="26b0c-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="26b0c-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="26b0c-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="26b0c-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="26b0c-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="26b0c-170">响应</span><span class="sxs-lookup"><span data-stu-id="26b0c-170">Response</span></span>

<span data-ttu-id="26b0c-171">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="26b0c-171">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

<span data-ttu-id="26b0c-172">294</span><span class="sxs-lookup"><span data-stu-id="26b0c-172">294</span></span>

### <a name="example-4-use-search-and-odata-cast-to-get-group-membership-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="26b0c-173">示例 4：使用 $search 和 OData 强制转换获取显示名称中包含字母“Video”（包括返回的对象数）的组成员身份</span><span class="sxs-lookup"><span data-stu-id="26b0c-173">Example 4: Use $search and OData cast to get group membership with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="26b0c-174">请求</span><span class="sxs-lookup"><span data-stu-id="26b0c-174">Request</span></span>

<span data-ttu-id="26b0c-175">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="26b0c-175">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="26b0c-176">HTTP</span><span class="sxs-lookup"><span data-stu-id="26b0c-176">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:Video"&$select=displayName,id
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="26b0c-177">C#</span><span class="sxs-lookup"><span data-stu-id="26b0c-177">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tier-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="26b0c-178">JavaScript</span><span class="sxs-lookup"><span data-stu-id="26b0c-178">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tier-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="26b0c-179">Objective-C</span><span class="sxs-lookup"><span data-stu-id="26b0c-179">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tier-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="26b0c-180">响应</span><span class="sxs-lookup"><span data-stu-id="26b0c-180">Response</span></span>

<span data-ttu-id="26b0c-181">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="26b0c-181">The following is an example of the response.</span></span>
><span data-ttu-id="26b0c-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="26b0c-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups(displayName,id)",
  "@odata.count":7,
  "value":[
    {
      "displayName":"Contoso Videos",
      "id":"11111111-2222-3333-4444-555555555555"
    }
  ]
}
```

### <a name="example-5-use-filter-and-odata-cast-to-get-group-membership-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="26b0c-184">示例 5：使用 $filter 和 OData 强制转换获取显示名称以“A”开头（包括返回的对象数）的组成员身份</span><span class="sxs-lookup"><span data-stu-id="26b0c-184">Example 5: Use $filter and OData cast to get group membership with a display name that starts with 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="26b0c-185">请求</span><span class="sxs-lookup"><span data-stu-id="26b0c-185">Request</span></span>

<span data-ttu-id="26b0c-186">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="26b0c-186">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="26b0c-187">HTTP</span><span class="sxs-lookup"><span data-stu-id="26b0c-187">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="26b0c-188">C#</span><span class="sxs-lookup"><span data-stu-id="26b0c-188">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="26b0c-189">JavaScript</span><span class="sxs-lookup"><span data-stu-id="26b0c-189">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="26b0c-190">Objective-C</span><span class="sxs-lookup"><span data-stu-id="26b0c-190">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="26b0c-191">响应</span><span class="sxs-lookup"><span data-stu-id="26b0c-191">Response</span></span>

<span data-ttu-id="26b0c-192">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="26b0c-192">The following is an example of the response.</span></span>
><span data-ttu-id="26b0c-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="26b0c-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
  "@odata.count":76,
  "value":[
    {
      "displayName":"AAD Contoso Users",
      "mail":"AADContoso_Users@contoso.com",
      "mailEnabled":true,
      "mailNickname":"AADContoso_Users",
      "securityEnabled":true
    }
  ]
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List servicePrincipal transitiveMemberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
