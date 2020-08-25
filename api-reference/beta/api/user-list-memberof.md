---
title: List user memberOf
description: 获取用户是其直接成员的组、目录角色和管理单元。 此操作不可传递。
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 0c5b1e89bcc234894c83abee9ac52ab2ff0fa0b3
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873291"
---
# <a name="list-user-memberof"></a><span data-ttu-id="03017-104">List user memberOf</span><span class="sxs-lookup"><span data-stu-id="03017-104">List user memberOf</span></span>

<span data-ttu-id="03017-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03017-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03017-106">获取用户是其直接成员的组、目录角色和管理单元。</span><span class="sxs-lookup"><span data-stu-id="03017-106">Get groups, directory roles and administrative units that the user is a direct member of.</span></span> <span data-ttu-id="03017-107">此操作不可传递。</span><span class="sxs-lookup"><span data-stu-id="03017-107">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="03017-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="03017-108">Permissions</span></span>

<span data-ttu-id="03017-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="03017-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="03017-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="03017-111">Permission type</span></span> | <span data-ttu-id="03017-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="03017-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="03017-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="03017-113">Delegated (work or school account)</span></span> | <span data-ttu-id="03017-114">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="03017-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="03017-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="03017-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03017-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="03017-116">Not supported.</span></span> |
| <span data-ttu-id="03017-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="03017-117">Application</span></span> | <span data-ttu-id="03017-118">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03017-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="03017-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="03017-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/memberOf
or
GET /users/{id | userPrincipalName}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="03017-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="03017-120">Optional query parameters</span></span>

<span data-ttu-id="03017-121">此方法支持[OData query parameters](/graph/query_parameters)以帮助自定义响应，包括 `$search`、`$count`、 和 `$filter`</span><span class="sxs-lookup"><span data-stu-id="03017-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="03017-122">此外，还会启用 OData 强制转换，例如，您可以强制转换为仅获取用户所属的 directoryRoles。</span><span class="sxs-lookup"><span data-stu-id="03017-122">OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of.</span></span> <span data-ttu-id="03017-123">`$search`可以用在 **displayName**属性。</span><span class="sxs-lookup"><span data-stu-id="03017-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="03017-124">为该资源添加或更新项目时，将对它们进行专门索引，以便与 `$count` 和 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="03017-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="03017-125">在添加或更新项目与在索引中可用之间可能会稍有延迟。</span><span class="sxs-lookup"><span data-stu-id="03017-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="03017-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="03017-126">Request headers</span></span>

| <span data-ttu-id="03017-127">标头</span><span class="sxs-lookup"><span data-stu-id="03017-127">Header</span></span> | <span data-ttu-id="03017-128">值</span><span class="sxs-lookup"><span data-stu-id="03017-128">Value</span></span> |
|:------ |:----- |
| <span data-ttu-id="03017-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="03017-129">Authorization</span></span>  | <span data-ttu-id="03017-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="03017-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="03017-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="03017-132">ConsistencyLevel</span></span> | <span data-ttu-id="03017-133">最终。</span><span class="sxs-lookup"><span data-stu-id="03017-133">eventual.</span></span> <span data-ttu-id="03017-134">在 `$count` 使用 `$search` 、 `$filter` 、 `$orderby` 或 OData 转换查询参数时，此标头和是必需的。</span><span class="sxs-lookup"><span data-stu-id="03017-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="03017-135">它使用的索引可能不是最新的，并包含对对象的最新更改。</span><span class="sxs-lookup"><span data-stu-id="03017-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="03017-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="03017-136">Request body</span></span>

<span data-ttu-id="03017-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="03017-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="03017-138">响应</span><span class="sxs-lookup"><span data-stu-id="03017-138">Response</span></span>

<span data-ttu-id="03017-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="03017-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="03017-140">示例</span><span class="sxs-lookup"><span data-stu-id="03017-140">Examples</span></span>

### <a name="example-1-get-groups-directory-roles-and-administrative-units-that-the-user-is-a-direct-member-of"></a><span data-ttu-id="03017-141">示例1：获取用户是其直接成员的组、目录角色和管理单元</span><span class="sxs-lookup"><span data-stu-id="03017-141">Example 1: Get groups, directory roles, and administrative units that the user is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="03017-142">请求</span><span class="sxs-lookup"><span data-stu-id="03017-142">Request</span></span>

<span data-ttu-id="03017-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="03017-143">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="03017-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="03017-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="03017-145">C#</span><span class="sxs-lookup"><span data-stu-id="03017-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="03017-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="03017-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="03017-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="03017-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="03017-148">响应</span><span class="sxs-lookup"><span data-stu-id="03017-148">Response</span></span>

<span data-ttu-id="03017-149">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="03017-149">The following is an example of the response.</span></span>
><span data-ttu-id="03017-150">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="03017-150">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="03017-151">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="03017-151">All the properties will be returned from an actual call.</span></span>

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
      "displayName": "All Users",
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-all-groups-directory-roles-and-administrative-units-that-the-user-is-a-direct-member-of"></a><span data-ttu-id="03017-152">示例2：仅获取用户是其直接成员的所有组、目录角色和管理单元的计数</span><span class="sxs-lookup"><span data-stu-id="03017-152">Example 2: Get only a count of all groups, directory roles, and administrative units that the user is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="03017-153">请求</span><span class="sxs-lookup"><span data-stu-id="03017-153">Request</span></span>

<span data-ttu-id="03017-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="03017-154">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="03017-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="03017-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user_memberof_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/memberOf/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="03017-156">C#</span><span class="sxs-lookup"><span data-stu-id="03017-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-memberof-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="03017-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="03017-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-memberof-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="03017-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="03017-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-memberof-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="03017-159">响应</span><span class="sxs-lookup"><span data-stu-id="03017-159">Response</span></span>

<span data-ttu-id="03017-160">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="03017-160">The following is an example of the response.</span></span>
><span data-ttu-id="03017-161">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="03017-161">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="03017-162">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="03017-162">All the properties will be returned from an actual call.</span></span>

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

<span data-ttu-id="03017-163">893</span><span class="sxs-lookup"><span data-stu-id="03017-163">893</span></span>

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-group-membership"></a><span data-ttu-id="03017-164">示例3：使用 OData 强制转换仅获取组成员身份的计数</span><span class="sxs-lookup"><span data-stu-id="03017-164">Example 3: Use OData cast to get only a count of group membership</span></span>

#### <a name="request"></a><span data-ttu-id="03017-165">请求</span><span class="sxs-lookup"><span data-stu-id="03017-165">Request</span></span>

<span data-ttu-id="03017-166">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="03017-166">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="03017-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="03017-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/memberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="03017-168">C#</span><span class="sxs-lookup"><span data-stu-id="03017-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="03017-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="03017-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="03017-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="03017-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="03017-171">响应</span><span class="sxs-lookup"><span data-stu-id="03017-171">Response</span></span>

<span data-ttu-id="03017-172">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="03017-172">The following is an example of the response.</span></span>

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

<span data-ttu-id="03017-173">294</span><span class="sxs-lookup"><span data-stu-id="03017-173">294</span></span>

### <a name="example-4-use-search-and-odata-cast-to-get-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="03017-174">示例4：使用 $search 和 OData cast 获取包含包含字母 "层" 的组的组成员身份，其中包含返回对象的计数</span><span class="sxs-lookup"><span data-stu-id="03017-174">Example 4: Use $search and OData cast to get membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="03017-175">请求</span><span class="sxs-lookup"><span data-stu-id="03017-175">Request</span></span>

<span data-ttu-id="03017-176">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="03017-176">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="03017-177">HTTP</span><span class="sxs-lookup"><span data-stu-id="03017-177">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="03017-178">C#</span><span class="sxs-lookup"><span data-stu-id="03017-178">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tier-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="03017-179">JavaScript</span><span class="sxs-lookup"><span data-stu-id="03017-179">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tier-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="03017-180">Objective-C</span><span class="sxs-lookup"><span data-stu-id="03017-180">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tier-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="03017-181">响应</span><span class="sxs-lookup"><span data-stu-id="03017-181">Response</span></span>

<span data-ttu-id="03017-182">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="03017-182">The following is an example of the response.</span></span>
><span data-ttu-id="03017-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="03017-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "displayName":"Contoso-tier Query Notification",
      "id":"11111111-2222-3333-4444-555555555555"
    }
  ]
}
```

### <a name="example-5-use-filter-and-odata-cast-to-get-groups-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="03017-185">示例5：使用 $filter 和 OData cast 获取显示名称以 ' a ' 开头的组，其中包含返回对象的计数</span><span class="sxs-lookup"><span data-stu-id="03017-185">Example 5: Use $filter and OData cast to get groups with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="03017-186">请求</span><span class="sxs-lookup"><span data-stu-id="03017-186">Request</span></span>

<span data-ttu-id="03017-187">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="03017-187">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="03017-188">HTTP</span><span class="sxs-lookup"><span data-stu-id="03017-188">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'a') 
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="03017-189">C#</span><span class="sxs-lookup"><span data-stu-id="03017-189">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="03017-190">JavaScript</span><span class="sxs-lookup"><span data-stu-id="03017-190">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="03017-191">Objective-C</span><span class="sxs-lookup"><span data-stu-id="03017-191">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="03017-192">响应</span><span class="sxs-lookup"><span data-stu-id="03017-192">Response</span></span>

<span data-ttu-id="03017-193">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="03017-193">The following is an example of the response.</span></span>
><span data-ttu-id="03017-p110">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="03017-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
