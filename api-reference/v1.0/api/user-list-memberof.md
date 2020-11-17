---
title: 列出 memberOf
description: '返回用户是其直接成员的组和目录角色。 '
author: krbain
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 79793e48f30d6c94e7d05924f9bec5b0c14c627b
ms.sourcegitcommit: eafb1629e52450dab0da6a1fb6d1ddfa878777c6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2020
ms.locfileid: "49082298"
---
# <a name="list-memberof"></a><span data-ttu-id="6e6cf-103">列出 memberOf</span><span class="sxs-lookup"><span data-stu-id="6e6cf-103">List memberOf</span></span>

<span data-ttu-id="6e6cf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e6cf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6e6cf-105">获取用户是其直接成员的[组](../resources/group.md)和[目录角色](../resources/directoryrole.md)。</span><span class="sxs-lookup"><span data-stu-id="6e6cf-105">Get [groups](../resources/group.md) and [directory roles](../resources/directoryrole.md) that the user is a direct member of.</span></span> 

## <a name="permissions"></a><span data-ttu-id="6e6cf-106">权限</span><span class="sxs-lookup"><span data-stu-id="6e6cf-106">Permissions</span></span>
<span data-ttu-id="6e6cf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6e6cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e6cf-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6e6cf-109">Permission type</span></span>      | <span data-ttu-id="6e6cf-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6e6cf-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6e6cf-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6e6cf-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6e6cf-112">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6e6cf-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6e6cf-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6e6cf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e6cf-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6e6cf-114">Not supported.</span></span>    |
|<span data-ttu-id="6e6cf-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6e6cf-115">Application</span></span> | <span data-ttu-id="6e6cf-116">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e6cf-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="6e6cf-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6e6cf-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/memberOf
GET /users/{id | userPrincipalName}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6e6cf-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6e6cf-118">Optional query parameters</span></span>

<span data-ttu-id="6e6cf-p102">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应，包括 `$search`、`$count` 和 `$filter`。此外还将启用 OData 强制转换，例如，你可以强制转换以获取用户所属的 directoryRoles。你可以在 **displayName** 属性上使用 `$search`。为该资源添加或更新项目时，将为它们专门创建索引，以与 `$count` 和 `$search` 查询参数一起使用。添加或更新项目与项目在索引中可用之间可能会稍有延迟。</span><span class="sxs-lookup"><span data-stu-id="6e6cf-p102">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`. OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of. You can use `$search` on the **displayName** property. When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters. There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="6e6cf-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="6e6cf-124">Request headers</span></span>
| <span data-ttu-id="6e6cf-125">标头</span><span class="sxs-lookup"><span data-stu-id="6e6cf-125">Header</span></span>       | <span data-ttu-id="6e6cf-126">值</span><span class="sxs-lookup"><span data-stu-id="6e6cf-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6e6cf-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e6cf-127">Authorization</span></span>  | <span data-ttu-id="6e6cf-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6e6cf-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6e6cf-130">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="6e6cf-130">ConsistencyLevel</span></span> | <span data-ttu-id="6e6cf-p104">最终。使用 `$search`、`$filter`、`$orderby` 或 OData 强制转换查询参数时，必须提供此标头和 `$count`。它使用的索引可能未根据该对象的最新更改及时更新。</span><span class="sxs-lookup"><span data-stu-id="6e6cf-p104">eventual. This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters. It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6e6cf-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="6e6cf-134">Request body</span></span>
<span data-ttu-id="6e6cf-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6e6cf-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e6cf-136">响应</span><span class="sxs-lookup"><span data-stu-id="6e6cf-136">Response</span></span>

<span data-ttu-id="6e6cf-137">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="6e6cf-137">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6e6cf-138">示例</span><span class="sxs-lookup"><span data-stu-id="6e6cf-138">Examples</span></span>

### <a name="example-1-get-groups-directory-roles-and-administrative-units-that-the-user-is-a-direct-member-of"></a><span data-ttu-id="6e6cf-139">示例 1：获取用户是其直接成员的组、目录角色和管理单元</span><span class="sxs-lookup"><span data-stu-id="6e6cf-139">Example 1: Get groups, directory roles, and administrative units that the user is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="6e6cf-140">请求</span><span class="sxs-lookup"><span data-stu-id="6e6cf-140">Request</span></span>

<span data-ttu-id="6e6cf-141">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6e6cf-141">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6e6cf-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="6e6cf-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="6e6cf-143">C#</span><span class="sxs-lookup"><span data-stu-id="6e6cf-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6e6cf-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6e6cf-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6e6cf-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6e6cf-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6e6cf-146">Java</span><span class="sxs-lookup"><span data-stu-id="6e6cf-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-get-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6e6cf-147">响应</span><span class="sxs-lookup"><span data-stu-id="6e6cf-147">Response</span></span>

<span data-ttu-id="6e6cf-148">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6e6cf-148">The following is an example of the response.</span></span>

><span data-ttu-id="6e6cf-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6e6cf-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-all-groups-directory-roles-and-administrative-units-that-the-user-is-a-direct-member-of"></a><span data-ttu-id="6e6cf-151">示例 2：只获取用户是其直接成员的所有组、目录角色和管理单元的计数</span><span class="sxs-lookup"><span data-stu-id="6e6cf-151">Example 2: Get only a count of all groups, directory roles, and administrative units that the user is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="6e6cf-152">请求</span><span class="sxs-lookup"><span data-stu-id="6e6cf-152">Request</span></span>

<span data-ttu-id="6e6cf-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6e6cf-153">Here is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_user_memberof_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/memberOf/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="6e6cf-154">响应</span><span class="sxs-lookup"><span data-stu-id="6e6cf-154">Response</span></span>

<span data-ttu-id="6e6cf-155">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6e6cf-155">The following is an example of the response.</span></span>

><span data-ttu-id="6e6cf-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6e6cf-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`893`

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-group-membership"></a><span data-ttu-id="6e6cf-158">示例 3：使用 OData 强制转换以仅获取组成员身份的计数</span><span class="sxs-lookup"><span data-stu-id="6e6cf-158">Example 3: Use OData cast to get only a count of group membership</span></span>

#### <a name="request"></a><span data-ttu-id="6e6cf-159">请求</span><span class="sxs-lookup"><span data-stu-id="6e6cf-159">Request</span></span>

<span data-ttu-id="6e6cf-160">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6e6cf-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/memberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="6e6cf-161">响应</span><span class="sxs-lookup"><span data-stu-id="6e6cf-161">Response</span></span>

<span data-ttu-id="6e6cf-162">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6e6cf-162">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`294`

### <a name="example-4-use-search-and-odata-cast-to-get-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="6e6cf-163">示例 4：使用 $search 和 OData 强制转换来获取显示名称中包含字母“tier”（包括返回的对象数）的组的成员资格</span><span class="sxs-lookup"><span data-stu-id="6e6cf-163">Example 4: Use $search and OData cast to get membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="6e6cf-164">请求</span><span class="sxs-lookup"><span data-stu-id="6e6cf-164">Request</span></span>

<span data-ttu-id="6e6cf-165">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6e6cf-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="6e6cf-166">响应</span><span class="sxs-lookup"><span data-stu-id="6e6cf-166">Response</span></span>

<span data-ttu-id="6e6cf-167">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6e6cf-167">The following is an example of the response.</span></span>

><span data-ttu-id="6e6cf-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6e6cf-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-5-use-filter-and-odata-cast-to-get-groups-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="6e6cf-170">示例 5：使用 $filter 和 OData 强制转换来获取显示名称以“a”开头（包括返回的对象数）的组</span><span class="sxs-lookup"><span data-stu-id="6e6cf-170">Example 5: Use $filter and OData cast to get groups with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="6e6cf-171">请求</span><span class="sxs-lookup"><span data-stu-id="6e6cf-171">Request</span></span>

<span data-ttu-id="6e6cf-172">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6e6cf-172">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'a') 
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="6e6cf-173">响应</span><span class="sxs-lookup"><span data-stu-id="6e6cf-173">Response</span></span>

<span data-ttu-id="6e6cf-174">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6e6cf-174">The following is an example of the response.</span></span>

><span data-ttu-id="6e6cf-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6e6cf-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
