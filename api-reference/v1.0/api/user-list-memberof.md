---
title: 列出 memberOf
description: '返回用户是其直接成员的组和目录角色。 '
author: krbain
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: f0d4c3f45cc45700b64b54a87e5043c1356ea660
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905863"
---
# <a name="list-memberof"></a><span data-ttu-id="c010e-103">列出 memberOf</span><span class="sxs-lookup"><span data-stu-id="c010e-103">List memberOf</span></span>

<span data-ttu-id="c010e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c010e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c010e-105">获取用户是其直接成员的[组](../resources/group.md)和[目录角色](../resources/directoryrole.md)。</span><span class="sxs-lookup"><span data-stu-id="c010e-105">Get [groups](../resources/group.md) and [directory roles](../resources/directoryrole.md) that the user is a direct member of.</span></span> 

## <a name="permissions"></a><span data-ttu-id="c010e-106">权限</span><span class="sxs-lookup"><span data-stu-id="c010e-106">Permissions</span></span>
<span data-ttu-id="c010e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c010e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c010e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c010e-109">Permission type</span></span>      | <span data-ttu-id="c010e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c010e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c010e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c010e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c010e-112">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c010e-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c010e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c010e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c010e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c010e-114">Not supported.</span></span>    |
|<span data-ttu-id="c010e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c010e-115">Application</span></span> | <span data-ttu-id="c010e-116">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c010e-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="c010e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c010e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/memberOf
GET /users/{id | userPrincipalName}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c010e-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c010e-118">Optional query parameters</span></span>

<span data-ttu-id="c010e-119">此方法支持[OData query parameters](/graph/query-parameters)以帮助自定义响应，包括 `$search`、`$count`、 和 `$filter`</span><span class="sxs-lookup"><span data-stu-id="c010e-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="c010e-120">还启用了 OData 强制转换，例如，你可以强制转换为仅获取用户所属的 directoryRoles。</span><span class="sxs-lookup"><span data-stu-id="c010e-120">OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of.</span></span> <span data-ttu-id="c010e-121">`$search`可以用在 **displayName** 属性。</span><span class="sxs-lookup"><span data-stu-id="c010e-121">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="c010e-122">为该资源添加或更新项目时，将对它们进行专门索引，以便与 `$count` 和 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="c010e-122">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="c010e-123">在添加或更新项目与在索引中可用之间可能会稍有延迟。</span><span class="sxs-lookup"><span data-stu-id="c010e-123">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="c010e-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="c010e-124">Request headers</span></span>
| <span data-ttu-id="c010e-125">标头</span><span class="sxs-lookup"><span data-stu-id="c010e-125">Header</span></span>       | <span data-ttu-id="c010e-126">值</span><span class="sxs-lookup"><span data-stu-id="c010e-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c010e-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="c010e-127">Authorization</span></span>  | <span data-ttu-id="c010e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c010e-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c010e-130">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="c010e-130">ConsistencyLevel</span></span> | <span data-ttu-id="c010e-131">最终。</span><span class="sxs-lookup"><span data-stu-id="c010e-131">eventual.</span></span> <span data-ttu-id="c010e-132">使用 `$search`、`$filter`、`$orderby` 或 OData 强制转换查询参数时，此标头和 `$count` 是必需的。</span><span class="sxs-lookup"><span data-stu-id="c010e-132">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="c010e-133">它使用的索引可能与对象的最新更改不同步。</span><span class="sxs-lookup"><span data-stu-id="c010e-133">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c010e-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="c010e-134">Request body</span></span>
<span data-ttu-id="c010e-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c010e-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c010e-136">响应</span><span class="sxs-lookup"><span data-stu-id="c010e-136">Response</span></span>

<span data-ttu-id="c010e-137">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c010e-137">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c010e-138">示例</span><span class="sxs-lookup"><span data-stu-id="c010e-138">Examples</span></span>

### <a name="example-1-get-groups-directory-roles-and-administrative-units-that-the-user-is-a-direct-member-of"></a><span data-ttu-id="c010e-139">示例 1：获取用户是其直接成员的组、目录角色和管理单元</span><span class="sxs-lookup"><span data-stu-id="c010e-139">Example 1: Get groups, directory roles, and administrative units that the user is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="c010e-140">请求</span><span class="sxs-lookup"><span data-stu-id="c010e-140">Request</span></span>

<span data-ttu-id="c010e-141">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c010e-141">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c010e-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="c010e-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="c010e-143">C#</span><span class="sxs-lookup"><span data-stu-id="c010e-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c010e-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c010e-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c010e-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c010e-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c010e-146">Java</span><span class="sxs-lookup"><span data-stu-id="c010e-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-get-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c010e-147">响应</span><span class="sxs-lookup"><span data-stu-id="c010e-147">Response</span></span>

<span data-ttu-id="c010e-148">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c010e-148">The following is an example of the response.</span></span>

><span data-ttu-id="c010e-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c010e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-all-groups-directory-roles-and-administrative-units-that-the-user-is-a-direct-member-of"></a><span data-ttu-id="c010e-151">示例 2：只获取用户是其直接成员的所有组、目录角色和管理单元的计数</span><span class="sxs-lookup"><span data-stu-id="c010e-151">Example 2: Get only a count of all groups, directory roles, and administrative units that the user is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="c010e-152">请求</span><span class="sxs-lookup"><span data-stu-id="c010e-152">Request</span></span>

<span data-ttu-id="c010e-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c010e-153">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c010e-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="c010e-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user_memberof_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/memberOf/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="c010e-155">C#</span><span class="sxs-lookup"><span data-stu-id="c010e-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-memberof-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c010e-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c010e-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-memberof-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c010e-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c010e-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-memberof-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c010e-158">Java</span><span class="sxs-lookup"><span data-stu-id="c010e-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-memberof-count-only-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c010e-159">响应</span><span class="sxs-lookup"><span data-stu-id="c010e-159">Response</span></span>

<span data-ttu-id="c010e-160">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c010e-160">The following is an example of the response.</span></span>

><span data-ttu-id="c010e-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c010e-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`893`

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-group-membership"></a><span data-ttu-id="c010e-163">示例 3：使用 OData 强制转换以仅获取组成员身份的计数</span><span class="sxs-lookup"><span data-stu-id="c010e-163">Example 3: Use OData cast to get only a count of group membership</span></span>

#### <a name="request"></a><span data-ttu-id="c010e-164">请求</span><span class="sxs-lookup"><span data-stu-id="c010e-164">Request</span></span>

<span data-ttu-id="c010e-165">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c010e-165">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c010e-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="c010e-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/memberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="c010e-167">C#</span><span class="sxs-lookup"><span data-stu-id="c010e-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c010e-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c010e-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c010e-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c010e-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c010e-170">Java</span><span class="sxs-lookup"><span data-stu-id="c010e-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-count-only-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c010e-171">响应</span><span class="sxs-lookup"><span data-stu-id="c010e-171">Response</span></span>

<span data-ttu-id="c010e-172">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c010e-172">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`294`

### <a name="example-4-use-search-and-odata-cast-to-get-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="c010e-173">示例 4：使用 $search 和 OData 强制转换来获取显示名称中包含字母“tier”（包括返回的对象数）的组的成员资格</span><span class="sxs-lookup"><span data-stu-id="c010e-173">Example 4: Use $search and OData cast to get membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="c010e-174">请求</span><span class="sxs-lookup"><span data-stu-id="c010e-174">Request</span></span>

<span data-ttu-id="c010e-175">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c010e-175">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c010e-176">HTTP</span><span class="sxs-lookup"><span data-stu-id="c010e-176">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="c010e-177">C#</span><span class="sxs-lookup"><span data-stu-id="c010e-177">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tier-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c010e-178">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c010e-178">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tier-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c010e-179">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c010e-179">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tier-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c010e-180">Java</span><span class="sxs-lookup"><span data-stu-id="c010e-180">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tier-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c010e-181">响应</span><span class="sxs-lookup"><span data-stu-id="c010e-181">Response</span></span>

<span data-ttu-id="c010e-182">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c010e-182">The following is an example of the response.</span></span>

><span data-ttu-id="c010e-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c010e-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups(displayName,id)",
  "@odata.count":7,
  "value":[
    {
      "displayName":"Contoso-tier Query Notification",
      "id":"11111111-2222-3333-4444-555555555555"
    }
  ]
}
```

### <a name="example-5-use-filter-and-odata-cast-to-get-groups-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="c010e-185">示例 5：使用 $filter 和 OData 强制转换来获取显示名称以“a”开头（包括返回的对象数）的组</span><span class="sxs-lookup"><span data-stu-id="c010e-185">Example 5: Use $filter and OData cast to get groups with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="c010e-186">请求</span><span class="sxs-lookup"><span data-stu-id="c010e-186">Request</span></span>

<span data-ttu-id="c010e-187">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c010e-187">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c010e-188">HTTP</span><span class="sxs-lookup"><span data-stu-id="c010e-188">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'a') 
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="c010e-189">C#</span><span class="sxs-lookup"><span data-stu-id="c010e-189">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c010e-190">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c010e-190">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c010e-191">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c010e-191">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c010e-192">Java</span><span class="sxs-lookup"><span data-stu-id="c010e-192">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-a-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c010e-193">响应</span><span class="sxs-lookup"><span data-stu-id="c010e-193">Response</span></span>

<span data-ttu-id="c010e-194">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c010e-194">The following is an example of the response.</span></span>

><span data-ttu-id="c010e-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c010e-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
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
<!-- {
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
