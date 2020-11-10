---
title: List servicePrincipal memberOf
description: 获取此服务主体作为直接成员所属的组和目录角色。此操作不可传递。
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: a9a61cd0ac6eda02e527032af19999272a01461e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48972599"
---
# <a name="list-serviceprincipal-memberof"></a><span data-ttu-id="c1bea-104">List servicePrincipal memberOf</span><span class="sxs-lookup"><span data-stu-id="c1bea-104">List servicePrincipal memberOf</span></span>

<span data-ttu-id="c1bea-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1bea-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1bea-p102">获取此 [servicePrincipal](../resources/serviceprincipal.md) 作为直接成员所属的组和目录角色。</span><span class="sxs-lookup"><span data-stu-id="c1bea-p102">Get the groups and directory roles that this [servicePrincipal](../resources/serviceprincipal.md) is a direct member of. This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="c1bea-108">权限</span><span class="sxs-lookup"><span data-stu-id="c1bea-108">Permissions</span></span>

<span data-ttu-id="c1bea-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c1bea-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1bea-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c1bea-111">Permission type</span></span>      | <span data-ttu-id="c1bea-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c1bea-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c1bea-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c1bea-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c1bea-114">Application.Read.All、Directory.Read.All、Application.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c1bea-114">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c1bea-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c1bea-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1bea-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c1bea-116">Not supported.</span></span>    |
|<span data-ttu-id="c1bea-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c1bea-117">Application</span></span> | <span data-ttu-id="c1bea-118">Application.Read.All、Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1bea-118">Application.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="c1bea-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c1bea-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c1bea-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c1bea-120">Optional query parameters</span></span>

<span data-ttu-id="c1bea-p104">此方法支持使用 [OData 查询参数](/graph/query_parameters)来帮助自定义响应，包括 `$search`、`$count` 和 `$filter`。此外还将启用 OData 强制转换，例如，你可以强制转换以获取用户所属的 directoryRoles。你可以在 **displayName** 属性上使用 `$search`。为该资源添加或更新项目时，将为它们专门创建索引，以与 `$count` 和 `$search` 查询参数一起使用。添加或更新项目与项目在索引中可用之间可能会稍有延迟。</span><span class="sxs-lookup"><span data-stu-id="c1bea-p104">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`. OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of. You can use `$search` on the **displayName** property. When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters. There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c1bea-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="c1bea-126">Request headers</span></span>

| <span data-ttu-id="c1bea-127">名称</span><span class="sxs-lookup"><span data-stu-id="c1bea-127">Name</span></span>       | <span data-ttu-id="c1bea-128">类型</span><span class="sxs-lookup"><span data-stu-id="c1bea-128">Type</span></span> | <span data-ttu-id="c1bea-129">说明</span><span class="sxs-lookup"><span data-stu-id="c1bea-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c1bea-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1bea-130">Authorization</span></span>  | <span data-ttu-id="c1bea-131">string</span><span class="sxs-lookup"><span data-stu-id="c1bea-131">string</span></span>  | <span data-ttu-id="c1bea-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c1bea-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c1bea-134">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="c1bea-134">ConsistencyLevel</span></span> | <span data-ttu-id="c1bea-135">最终。</span><span class="sxs-lookup"><span data-stu-id="c1bea-135">eventual.</span></span> <span data-ttu-id="c1bea-136">使用 `$search`、`$filter`、`$orderby` 或 OData 强制转换查询参数时，此标头和 `$count` 是必需的。</span><span class="sxs-lookup"><span data-stu-id="c1bea-136">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="c1bea-137">它使用的索引可能与对象的最新更改不同步。</span><span class="sxs-lookup"><span data-stu-id="c1bea-137">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c1bea-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="c1bea-138">Request body</span></span>
<span data-ttu-id="c1bea-139">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c1bea-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c1bea-140">响应</span><span class="sxs-lookup"><span data-stu-id="c1bea-140">Response</span></span>

<span data-ttu-id="c1bea-141">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c1bea-141">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c1bea-142">示例</span><span class="sxs-lookup"><span data-stu-id="c1bea-142">Examples</span></span>

### <a name="example-1-get-groups-and-directory-roles-that-the-service-principal-is-a-direct-member-of"></a><span data-ttu-id="c1bea-143">示例 1：获取此服务主体作为直接成员所属的组和目录角色</span><span class="sxs-lookup"><span data-stu-id="c1bea-143">Example 1: Get groups and directory roles that the service principal is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="c1bea-144">请求</span><span class="sxs-lookup"><span data-stu-id="c1bea-144">Request</span></span>

<span data-ttu-id="c1bea-145">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c1bea-145">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c1bea-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="c1bea-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="c1bea-147">C#</span><span class="sxs-lookup"><span data-stu-id="c1bea-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceprincipal-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c1bea-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c1bea-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceprincipal-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c1bea-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c1bea-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceprincipal-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c1bea-150">Java</span><span class="sxs-lookup"><span data-stu-id="c1bea-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-serviceprincipal-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c1bea-151">响应</span><span class="sxs-lookup"><span data-stu-id="c1bea-151">Response</span></span>

<span data-ttu-id="c1bea-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c1bea-152">The following is an example of the response.</span></span> 
> <span data-ttu-id="c1bea-153">**注意：** 为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c1bea-153">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c1bea-154">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c1bea-154">All of the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-all-memberships"></a><span data-ttu-id="c1bea-155">示例 2：仅获取所有可成员身份的计数</span><span class="sxs-lookup"><span data-stu-id="c1bea-155">Example 2: Get only a count of all memberships</span></span>

#### <a name="request"></a><span data-ttu-id="c1bea-156">请求</span><span class="sxs-lookup"><span data-stu-id="c1bea-156">Request</span></span>

<span data-ttu-id="c1bea-157">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c1bea-157">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c1bea-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="c1bea-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="c1bea-159">C#</span><span class="sxs-lookup"><span data-stu-id="c1bea-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c1bea-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c1bea-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c1bea-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c1bea-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c1bea-162">Java</span><span class="sxs-lookup"><span data-stu-id="c1bea-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-count-only-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c1bea-163">响应</span><span class="sxs-lookup"><span data-stu-id="c1bea-163">Response</span></span>

<span data-ttu-id="c1bea-164">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c1bea-164">The following is an example of the response.</span></span>

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

<span data-ttu-id="c1bea-165">394</span><span class="sxs-lookup"><span data-stu-id="c1bea-165">394</span></span>

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-group-membership"></a><span data-ttu-id="c1bea-166">示例 3：使用 OData 强制转换以仅获取组成员身份的计数</span><span class="sxs-lookup"><span data-stu-id="c1bea-166">Example 3: Use OData cast to get only a count of group membership</span></span>

#### <a name="request"></a><span data-ttu-id="c1bea-167">请求</span><span class="sxs-lookup"><span data-stu-id="c1bea-167">Request</span></span>

<span data-ttu-id="c1bea-168">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c1bea-168">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c1bea-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="c1bea-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_group_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="c1bea-170">C#</span><span class="sxs-lookup"><span data-stu-id="c1bea-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-group-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c1bea-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c1bea-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-group-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c1bea-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c1bea-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-group-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c1bea-173">Java</span><span class="sxs-lookup"><span data-stu-id="c1bea-173">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-count-group-only-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c1bea-174">响应</span><span class="sxs-lookup"><span data-stu-id="c1bea-174">Response</span></span>

<span data-ttu-id="c1bea-175">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c1bea-175">The following is an example of the response.</span></span>

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

<span data-ttu-id="c1bea-176">394</span><span class="sxs-lookup"><span data-stu-id="c1bea-176">394</span></span>

### <a name="example-4-use-search-and-odata-cast-to-get-group-membership-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="c1bea-177">示例 4：使用 $search 和 OData 强制转换获取显示名称中包含字母“Video”（包括返回的对象数）的组成员身份</span><span class="sxs-lookup"><span data-stu-id="c1bea-177">Example 4: Use $search and OData cast to get group membership with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="c1bea-178">请求</span><span class="sxs-lookup"><span data-stu-id="c1bea-178">Request</span></span>

<span data-ttu-id="c1bea-179">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c1bea-179">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET iv. https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search=”displayName:Video" 
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="c1bea-180">响应</span><span class="sxs-lookup"><span data-stu-id="c1bea-180">Response</span></span>

<span data-ttu-id="c1bea-181">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c1bea-181">The following is an example of the response.</span></span>
><span data-ttu-id="c1bea-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c1bea-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects",
  "@odata.count":1396,
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All videos for the company",
      "displayName": "All Videos",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true
    }
  ]
}
```

### <a name="example-5-use-filter-and-odata-cast-to-get-group-membership-with-a-display-name-that-starts-with-the-letter-a-including-a-count-of-returned-objects"></a><span data-ttu-id="c1bea-184">示例 5：使用 $filter 和 OData 强制转换获取显示名称以字母“A”开头（包括返回的对象数）的组成员身份</span><span class="sxs-lookup"><span data-stu-id="c1bea-184">Example 5: Use $filter and OData cast to get group membership with a display name that starts with the letter 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="c1bea-185">请求</span><span class="sxs-lookup"><span data-stu-id="c1bea-185">Request</span></span>

<span data-ttu-id="c1bea-186">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c1bea-186">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c1bea-187">HTTP</span><span class="sxs-lookup"><span data-stu-id="c1bea-187">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'A')
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="c1bea-188">C#</span><span class="sxs-lookup"><span data-stu-id="c1bea-188">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c1bea-189">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c1bea-189">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c1bea-190">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c1bea-190">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c1bea-191">Java</span><span class="sxs-lookup"><span data-stu-id="c1bea-191">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-a-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c1bea-192">响应</span><span class="sxs-lookup"><span data-stu-id="c1bea-192">Response</span></span>

<span data-ttu-id="c1bea-193">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c1bea-193">The following is an example of the response.</span></span>
><span data-ttu-id="c1bea-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c1bea-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects",
  "@odata.count":76,
  "value":[
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All videos for the company",
      "displayName": "All Videos",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List servicePrincipal memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


