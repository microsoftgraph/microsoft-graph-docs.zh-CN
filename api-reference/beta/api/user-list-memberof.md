---
title: List user memberOf
description: 获取用户是其直接成员的组、目录角色和管理单元。 此操作不可传递。
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: cd6b8c9f1cc9fb051e88c4a47542c046a5d163fe
ms.sourcegitcommit: 186d738f04e5a558da423f2429165fb4fbe780aa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086786"
---
# <a name="list-user-memberof"></a><span data-ttu-id="f727f-104">List user memberOf</span><span class="sxs-lookup"><span data-stu-id="f727f-104">List user memberOf</span></span>

<span data-ttu-id="f727f-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f727f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f727f-106">获取用户是其直接成员的组、目录角色和管理单元。</span><span class="sxs-lookup"><span data-stu-id="f727f-106">Get groups, directory roles and administrative units that the user is a direct member of.</span></span> <span data-ttu-id="f727f-107">此操作不可传递。</span><span class="sxs-lookup"><span data-stu-id="f727f-107">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="f727f-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="f727f-108">Permissions</span></span>

<span data-ttu-id="f727f-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f727f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f727f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f727f-111">Permission type</span></span> | <span data-ttu-id="f727f-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f727f-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="f727f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f727f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f727f-114">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f727f-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="f727f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f727f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f727f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f727f-116">Not supported.</span></span> |
| <span data-ttu-id="f727f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f727f-117">Application</span></span> | <span data-ttu-id="f727f-118">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f727f-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f727f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f727f-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/memberOf
or
GET /users/{id | userPrincipalName}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f727f-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f727f-120">Optional query parameters</span></span>

<span data-ttu-id="f727f-p104">此方法支持使用 [OData 查询参数](/graph/query_parameters)来帮助自定义响应，包括 `$search`、`$count` 和 `$filter`。此外还将启用 OData 强制转换，例如，你可以强制转换以获取用户所属的 directoryRoles。你可以在 **displayName** 属性上使用 `$search`。为该资源添加或更新项目时，将为它们专门创建索引，以与 `$count` 和 `$search` 查询参数一起使用。添加或更新项目与项目在索引中可用之间可能会稍有延迟。</span><span class="sxs-lookup"><span data-stu-id="f727f-p104">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`. OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of. You can use `$search` on the **displayName** property. When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters. There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f727f-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="f727f-126">Request headers</span></span>

| <span data-ttu-id="f727f-127">标头</span><span class="sxs-lookup"><span data-stu-id="f727f-127">Header</span></span> | <span data-ttu-id="f727f-128">值</span><span class="sxs-lookup"><span data-stu-id="f727f-128">Value</span></span> |
|:------ |:----- |
| <span data-ttu-id="f727f-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="f727f-129">Authorization</span></span>  | <span data-ttu-id="f727f-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f727f-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f727f-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="f727f-132">ConsistencyLevel</span></span> | <span data-ttu-id="f727f-p106">最终。使用 `$search`、`$filter`、`$orderby` 或 OData 强制转换查询参数时，必须提供此标头和 `$count`。它使用的索引可能未根据该对象的最新更改及时更新。</span><span class="sxs-lookup"><span data-stu-id="f727f-p106">eventual. This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters. It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f727f-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="f727f-136">Request body</span></span>

<span data-ttu-id="f727f-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f727f-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f727f-138">响应</span><span class="sxs-lookup"><span data-stu-id="f727f-138">Response</span></span>

<span data-ttu-id="f727f-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f727f-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f727f-140">示例</span><span class="sxs-lookup"><span data-stu-id="f727f-140">Examples</span></span>

### <a name="example-1-get-groups-directory-roles-and-administrative-units-that-the-user-is-a-direct-member-of"></a><span data-ttu-id="f727f-141">示例 1：获取用户是其直接成员的组、目录角色和管理单元</span><span class="sxs-lookup"><span data-stu-id="f727f-141">Example 1: Get groups, directory roles, and administrative units that the user is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="f727f-142">请求</span><span class="sxs-lookup"><span data-stu-id="f727f-142">Request</span></span>

<span data-ttu-id="f727f-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f727f-143">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f727f-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="f727f-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="f727f-145">C#</span><span class="sxs-lookup"><span data-stu-id="f727f-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f727f-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f727f-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f727f-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f727f-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f727f-148">Java</span><span class="sxs-lookup"><span data-stu-id="f727f-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="f727f-149">响应</span><span class="sxs-lookup"><span data-stu-id="f727f-149">Response</span></span>

<span data-ttu-id="f727f-150">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f727f-150">The following is an example of the response.</span></span>
><span data-ttu-id="f727f-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f727f-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "securityEnabled": true
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-all-groups-directory-roles-and-administrative-units-that-the-user-is-a-direct-member-of"></a><span data-ttu-id="f727f-153">示例 2：只获取用户是其直接成员的所有组、目录角色和管理单元的计数</span><span class="sxs-lookup"><span data-stu-id="f727f-153">Example 2: Get only a count of all groups, directory roles, and administrative units that the user is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="f727f-154">请求</span><span class="sxs-lookup"><span data-stu-id="f727f-154">Request</span></span>

<span data-ttu-id="f727f-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f727f-155">Here is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_user_memberof_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/memberOf/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="f727f-156">响应</span><span class="sxs-lookup"><span data-stu-id="f727f-156">Response</span></span>

<span data-ttu-id="f727f-157">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f727f-157">The following is an example of the response.</span></span>
><span data-ttu-id="f727f-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f727f-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-group-membership"></a><span data-ttu-id="f727f-160">示例 3：使用 OData 强制转换以仅获取组成员身份的计数</span><span class="sxs-lookup"><span data-stu-id="f727f-160">Example 3: Use OData cast to get only a count of group membership</span></span>

#### <a name="request"></a><span data-ttu-id="f727f-161">请求</span><span class="sxs-lookup"><span data-stu-id="f727f-161">Request</span></span>

<span data-ttu-id="f727f-162">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f727f-162">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/memberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="f727f-163">响应</span><span class="sxs-lookup"><span data-stu-id="f727f-163">Response</span></span>

<span data-ttu-id="f727f-164">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f727f-164">The following is an example of the response.</span></span>

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

### <a name="example-4-use-search-and-odata-cast-to-get-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="f727f-165">示例 4：使用 $search 和 OData 强制转换来获取显示名称中包含字母“tier”（包括返回的对象数）的组的成员资格</span><span class="sxs-lookup"><span data-stu-id="f727f-165">Example 4: Use $search and OData cast to get membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="f727f-166">请求</span><span class="sxs-lookup"><span data-stu-id="f727f-166">Request</span></span>

<span data-ttu-id="f727f-167">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f727f-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="f727f-168">响应</span><span class="sxs-lookup"><span data-stu-id="f727f-168">Response</span></span>

<span data-ttu-id="f727f-169">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f727f-169">The following is an example of the response.</span></span>
><span data-ttu-id="f727f-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f727f-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-5-use-filter-and-odata-cast-to-get-groups-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="f727f-172">示例 5：使用 $filter 和 OData 强制转换来获取显示名称以“a”开头（包括返回的对象数）的组</span><span class="sxs-lookup"><span data-stu-id="f727f-172">Example 5: Use $filter and OData cast to get groups with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="f727f-173">请求</span><span class="sxs-lookup"><span data-stu-id="f727f-173">Request</span></span>

<span data-ttu-id="f727f-174">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f727f-174">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'a') 
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="f727f-175">响应</span><span class="sxs-lookup"><span data-stu-id="f727f-175">Response</span></span>

<span data-ttu-id="f727f-176">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f727f-176">The following is an example of the response.</span></span>
><span data-ttu-id="f727f-p110">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f727f-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


