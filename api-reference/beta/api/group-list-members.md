---
title: List group members
description: 获取组的直接成员列表。
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: a188f5f9ddbad07456235ccbe53ef9d0680867d1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48002156"
---
# <a name="list-group-members"></a><span data-ttu-id="ae2cc-103">List group members</span><span class="sxs-lookup"><span data-stu-id="ae2cc-103">List group members</span></span>

<span data-ttu-id="ae2cc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae2cc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae2cc-105">获取组的直接成员列表。</span><span class="sxs-lookup"><span data-stu-id="ae2cc-105">Get a list of the group's direct members.</span></span> <span data-ttu-id="ae2cc-106">组可以将用户、联系人、设备、服务主体和其他组作为成员。</span><span class="sxs-lookup"><span data-stu-id="ae2cc-106">A group can have users, contacts, devices, service principals, and other groups as members.</span></span> <span data-ttu-id="ae2cc-107">此操作不可传递。</span><span class="sxs-lookup"><span data-stu-id="ae2cc-107">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="ae2cc-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="ae2cc-108">Permissions</span></span>

<span data-ttu-id="ae2cc-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ae2cc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ae2cc-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ae2cc-111">Permission type</span></span> | <span data-ttu-id="ae2cc-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ae2cc-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="ae2cc-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ae2cc-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ae2cc-114">User.ReadBasic.All、User.Read.All、Group.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae2cc-114">User.ReadBasic.All, User.Read.All, Group.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="ae2cc-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ae2cc-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae2cc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ae2cc-116">Not supported.</span></span> |
| <span data-ttu-id="ae2cc-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ae2cc-117">Application</span></span> | <span data-ttu-id="ae2cc-118">Group. all、read. all、Directory。 All</span><span class="sxs-lookup"><span data-stu-id="ae2cc-118">Group.Read.All, User.Read.All, Directory.Read.All</span></span> |

> <span data-ttu-id="ae2cc-119">**注意：** 若要列出隐藏的成员资格组的成员，则需要使用 Read. Hidden 权限是必需的。</span><span class="sxs-lookup"><span data-stu-id="ae2cc-119">**Note:** To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]
 
## <a name="http-request"></a><span data-ttu-id="ae2cc-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ae2cc-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ae2cc-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ae2cc-121">Optional query parameters</span></span>

<span data-ttu-id="ae2cc-122">此方法支持[OData query parameters](/graph/query_parameters)以帮助自定义响应，包括 `$search`、`$count`、 和 `$filter`</span><span class="sxs-lookup"><span data-stu-id="ae2cc-122">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="ae2cc-123">此外，还会启用 OData 强制转换，例如，您可以强制转换以仅获取属于该组成员的用户。</span><span class="sxs-lookup"><span data-stu-id="ae2cc-123">OData cast is also enabled, for example, you can cast to get just the users that are a member of the group.</span></span> <span data-ttu-id="ae2cc-124">`$search`可以用在 **displayName**属性。</span><span class="sxs-lookup"><span data-stu-id="ae2cc-124">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="ae2cc-125">为该资源添加或更新项目时，将对它们进行专门索引，以便与 `$count` 和 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="ae2cc-125">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="ae2cc-126">在添加或更新项目与在索引中可用之间可能会稍有延迟。</span><span class="sxs-lookup"><span data-stu-id="ae2cc-126">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ae2cc-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="ae2cc-127">Request headers</span></span>

| <span data-ttu-id="ae2cc-128">名称</span><span class="sxs-lookup"><span data-stu-id="ae2cc-128">Name</span></span> | <span data-ttu-id="ae2cc-129">说明</span><span class="sxs-lookup"><span data-stu-id="ae2cc-129">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="ae2cc-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae2cc-130">Authorization</span></span> | <span data-ttu-id="ae2cc-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ae2cc-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ae2cc-133">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="ae2cc-133">ConsistencyLevel</span></span> | <span data-ttu-id="ae2cc-134">最终。</span><span class="sxs-lookup"><span data-stu-id="ae2cc-134">eventual.</span></span> <span data-ttu-id="ae2cc-135">使用 `$search`、`$filter`、`$orderby` 或 OData 强制转换查询参数时，此标头和 `$count` 是必需的。</span><span class="sxs-lookup"><span data-stu-id="ae2cc-135">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="ae2cc-136">它使用的索引可能与对象的最新更改不同步。</span><span class="sxs-lookup"><span data-stu-id="ae2cc-136">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ae2cc-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="ae2cc-137">Request body</span></span>

<span data-ttu-id="ae2cc-138">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ae2cc-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae2cc-139">响应</span><span class="sxs-lookup"><span data-stu-id="ae2cc-139">Response</span></span>

<span data-ttu-id="ae2cc-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ae2cc-140">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ae2cc-141">示例</span><span class="sxs-lookup"><span data-stu-id="ae2cc-141">Examples</span></span>

### <a name="example-1-get-the-direct-membership-in-a-group"></a><span data-ttu-id="ae2cc-142">示例1：获取组中的直接成员身份</span><span class="sxs-lookup"><span data-stu-id="ae2cc-142">Example 1: Get the direct membership in a group</span></span>

#### <a name="request"></a><span data-ttu-id="ae2cc-143">请求</span><span class="sxs-lookup"><span data-stu-id="ae2cc-143">Request</span></span>

<span data-ttu-id="ae2cc-144">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ae2cc-144">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ae2cc-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="ae2cc-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/members
```
# <a name="c"></a>[<span data-ttu-id="ae2cc-146">C#</span><span class="sxs-lookup"><span data-stu-id="ae2cc-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ae2cc-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ae2cc-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ae2cc-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ae2cc-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="ae2cc-149">响应</span><span class="sxs-lookup"><span data-stu-id="ae2cc-149">Response</span></span>

<span data-ttu-id="ae2cc-150">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ae2cc-150">The following is an example of the response.</span></span>
><span data-ttu-id="ae2cc-151">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ae2cc-151">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ae2cc-152">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ae2cc-152">All the properties will be returned from an actual call.</span></span>

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
      "id": "11111111-2222-3333-4444-555555555555",
      "mail": "group1@contoso.com",
      "mailEnabled": true,
      "mailNickname": "Contoso1",
      "securityEnabled": true
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-all-membership"></a><span data-ttu-id="ae2cc-153">示例2：仅获取所有成员身份的计数</span><span class="sxs-lookup"><span data-stu-id="ae2cc-153">Example 2: Get only a count of all membership</span></span>

#### <a name="request"></a><span data-ttu-id="ae2cc-154">请求</span><span class="sxs-lookup"><span data-stu-id="ae2cc-154">Request</span></span>

<span data-ttu-id="ae2cc-155">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ae2cc-155">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ae2cc-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="ae2cc-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/members/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="ae2cc-157">C#</span><span class="sxs-lookup"><span data-stu-id="ae2cc-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ae2cc-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ae2cc-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ae2cc-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ae2cc-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ae2cc-160">响应</span><span class="sxs-lookup"><span data-stu-id="ae2cc-160">Response</span></span>

<span data-ttu-id="ae2cc-161">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ae2cc-161">The following is an example of the response.</span></span>

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

<span data-ttu-id="ae2cc-162">893</span><span class="sxs-lookup"><span data-stu-id="ae2cc-162">893</span></span>

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-user-membership"></a><span data-ttu-id="ae2cc-163">示例3：使用 OData 强制转换仅获取用户成员身份的计数</span><span class="sxs-lookup"><span data-stu-id="ae2cc-163">Example 3: Use OData cast to get only a count of user membership</span></span>

#### <a name="request"></a><span data-ttu-id="ae2cc-164">请求</span><span class="sxs-lookup"><span data-stu-id="ae2cc-164">Request</span></span>

<span data-ttu-id="ae2cc-165">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ae2cc-165">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ae2cc-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="ae2cc-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_user_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/members/microsoft.graph.user/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="ae2cc-167">C#</span><span class="sxs-lookup"><span data-stu-id="ae2cc-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-user-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ae2cc-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ae2cc-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-user-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ae2cc-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ae2cc-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-user-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ae2cc-170">响应</span><span class="sxs-lookup"><span data-stu-id="ae2cc-170">Response</span></span>

<span data-ttu-id="ae2cc-171">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ae2cc-171">The following is an example of the response.</span></span>

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

<span data-ttu-id="ae2cc-172">893</span><span class="sxs-lookup"><span data-stu-id="ae2cc-172">893</span></span>

### <a name="example-4-use-search-and-odata-cast-to-get-user-membership-in-groups-with-display-names-that-contain-the-letters-pr-including-a-count-of-returned-objects"></a><span data-ttu-id="ae2cc-173">示例4：使用 $search 和 OData cast 以使用包含字母 "Pr" 的显示名称获取组中的用户成员身份，包括返回对象的计数</span><span class="sxs-lookup"><span data-stu-id="ae2cc-173">Example 4: Use $search and OData cast to get user membership in groups with display names that contain the letters 'Pr' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="ae2cc-174">请求</span><span class="sxs-lookup"><span data-stu-id="ae2cc-174">Request</span></span>

<span data-ttu-id="ae2cc-175">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ae2cc-175">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ae2cc-176">HTTP</span><span class="sxs-lookup"><span data-stu-id="ae2cc-176">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_pr_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/members/microsoft.graph.user?$count=true&$orderby=displayName&$search="displayName:Pr"&$select=displayName,id
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="ae2cc-177">C#</span><span class="sxs-lookup"><span data-stu-id="ae2cc-177">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-pr-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ae2cc-178">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ae2cc-178">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-pr-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ae2cc-179">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ae2cc-179">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-pr-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ae2cc-180">响应</span><span class="sxs-lookup"><span data-stu-id="ae2cc-180">Response</span></span>

<span data-ttu-id="ae2cc-181">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ae2cc-181">The following is an example of the response.</span></span>
><span data-ttu-id="ae2cc-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ae2cc-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users(displayName,id)",
  "@odata.count":7,
  "value":[
    {
      "displayName":"Joseph Price",
      "id":"11111111-2222-3333-4444-555555555555"
    },
    {
      "displayName":"Preston Morales",
      "id":"11111111-2222-3333-4444-555555555555"
    }
  ]
}
```

### <a name="example-5-use-filter-to-get-group-membership-with-a-display-name-that-starts-with-the-letter-a-including-a-count-of-returned-objects"></a><span data-ttu-id="ae2cc-184">示例5：使用 $filter 获取带有以字母 "A" 开头的显示名称的组成员身份，包括返回对象的计数</span><span class="sxs-lookup"><span data-stu-id="ae2cc-184">Example 5: Use $filter to get group membership with a display name that starts with the letter 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="ae2cc-185">请求</span><span class="sxs-lookup"><span data-stu-id="ae2cc-185">Request</span></span>

<span data-ttu-id="ae2cc-186">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ae2cc-186">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ae2cc-187">HTTP</span><span class="sxs-lookup"><span data-stu-id="ae2cc-187">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/members?$count=true&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="ae2cc-188">C#</span><span class="sxs-lookup"><span data-stu-id="ae2cc-188">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ae2cc-189">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ae2cc-189">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ae2cc-190">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ae2cc-190">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ae2cc-191">响应</span><span class="sxs-lookup"><span data-stu-id="ae2cc-191">Response</span></span>

<span data-ttu-id="ae2cc-192">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ae2cc-192">The following is an example of the response.</span></span>
><span data-ttu-id="ae2cc-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ae2cc-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "List group members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


