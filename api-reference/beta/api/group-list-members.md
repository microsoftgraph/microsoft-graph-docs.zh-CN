---
title: List group members
description: 获取组的直接成员列表。
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 2a1c50dfbee4a4846f40d6372a29b1561a1071f5
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48954028"
---
# <a name="list-group-members"></a><span data-ttu-id="532d7-103">List group members</span><span class="sxs-lookup"><span data-stu-id="532d7-103">List group members</span></span>

<span data-ttu-id="532d7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="532d7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="532d7-105">获取组的直接成员列表。</span><span class="sxs-lookup"><span data-stu-id="532d7-105">Get a list of the group's direct members.</span></span> <span data-ttu-id="532d7-106">组可以将用户、联系人、设备、服务主体和其他组作为成员。</span><span class="sxs-lookup"><span data-stu-id="532d7-106">A group can have users, contacts, devices, service principals, and other groups as members.</span></span> <span data-ttu-id="532d7-107">此操作不可传递。</span><span class="sxs-lookup"><span data-stu-id="532d7-107">This operation is not transitive.</span></span>

<span data-ttu-id="532d7-108">当组包含超过 100 个成员时，Microsoft Graph 将在响应中返回 `@odata.nextLink` 属性，其中包含指向下一页结果的 URL。</span><span class="sxs-lookup"><span data-stu-id="532d7-108">When a group contains more than 100 members, Microsoft Graph returns a `@odata.nextLink` property in the response that contains a URL to the next page of results.</span></span> <span data-ttu-id="532d7-109">如果该属性存在，请继续使用每次响应中的 `@odata.nextLink` URL 来创建额外请求，直至返回所有结果，如[在应用中对 Microsoft Graph 数据进行分页](/graph/paging)一文中所述。</span><span class="sxs-lookup"><span data-stu-id="532d7-109">If that property is present, continue making additional requests with the `@odata.nextLink` URL in each response, until all the results are returned, as described in [paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="532d7-110">权限</span><span class="sxs-lookup"><span data-stu-id="532d7-110">Permissions</span></span>

<span data-ttu-id="532d7-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="532d7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="532d7-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="532d7-113">Permission type</span></span> | <span data-ttu-id="532d7-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="532d7-114">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="532d7-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="532d7-115">Delegated (work or school account)</span></span> | <span data-ttu-id="532d7-116">Group.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="532d7-116">Group.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="532d7-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="532d7-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="532d7-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="532d7-118">Not supported.</span></span> |
| <span data-ttu-id="532d7-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="532d7-119">Application</span></span> | <span data-ttu-id="532d7-120">Group.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="532d7-120">Group.Read.All, Directory.Read.All</span></span> |

> <span data-ttu-id="532d7-121">**注意：** 若要列出隐藏的成员资格组的成员，则需要使用 Read. Hidden 权限是必需的。</span><span class="sxs-lookup"><span data-stu-id="532d7-121">**Note:** To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]
 
## <a name="http-request"></a><span data-ttu-id="532d7-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="532d7-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="532d7-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="532d7-123">Optional query parameters</span></span>

<span data-ttu-id="532d7-124">此方法支持[OData query parameters](/graph/query_parameters)以帮助自定义响应，包括 `$search`、`$count`、 和 `$filter`</span><span class="sxs-lookup"><span data-stu-id="532d7-124">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="532d7-125">还启用了 OData 强制转换，例如，你可以通过强制转换来获取仅是组成员的用户。</span><span class="sxs-lookup"><span data-stu-id="532d7-125">OData cast is also enabled, for example, you can cast to get just the users that are a member of the group.</span></span> <span data-ttu-id="532d7-126">`$search`可以用在 **displayName** 属性。</span><span class="sxs-lookup"><span data-stu-id="532d7-126">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="532d7-127">为该资源添加或更新项目时，将对它们进行专门索引，以便与 `$count` 和 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="532d7-127">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="532d7-128">在添加或更新项目与在索引中可用之间可能会稍有延迟。</span><span class="sxs-lookup"><span data-stu-id="532d7-128">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="532d7-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="532d7-129">Request headers</span></span>

| <span data-ttu-id="532d7-130">名称</span><span class="sxs-lookup"><span data-stu-id="532d7-130">Name</span></span> | <span data-ttu-id="532d7-131">说明</span><span class="sxs-lookup"><span data-stu-id="532d7-131">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="532d7-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="532d7-132">Authorization</span></span> | <span data-ttu-id="532d7-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="532d7-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="532d7-135">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="532d7-135">ConsistencyLevel</span></span> | <span data-ttu-id="532d7-136">最终。</span><span class="sxs-lookup"><span data-stu-id="532d7-136">eventual.</span></span> <span data-ttu-id="532d7-137">使用 `$search`、`$filter`、`$orderby` 或 OData 强制转换查询参数时，此标头和 `$count` 是必需的。</span><span class="sxs-lookup"><span data-stu-id="532d7-137">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="532d7-138">它使用的索引可能与对象的最新更改不同步。</span><span class="sxs-lookup"><span data-stu-id="532d7-138">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="532d7-139">请求正文</span><span class="sxs-lookup"><span data-stu-id="532d7-139">Request body</span></span>

<span data-ttu-id="532d7-140">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="532d7-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="532d7-141">响应</span><span class="sxs-lookup"><span data-stu-id="532d7-141">Response</span></span>

<span data-ttu-id="532d7-142">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="532d7-142">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="532d7-143">示例</span><span class="sxs-lookup"><span data-stu-id="532d7-143">Examples</span></span>

### <a name="example-1-get-the-direct-membership-in-a-group"></a><span data-ttu-id="532d7-144">示例1：获取组中的直接成员身份</span><span class="sxs-lookup"><span data-stu-id="532d7-144">Example 1: Get the direct membership in a group</span></span>

#### <a name="request"></a><span data-ttu-id="532d7-145">请求</span><span class="sxs-lookup"><span data-stu-id="532d7-145">Request</span></span>

<span data-ttu-id="532d7-146">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="532d7-146">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="532d7-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="532d7-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/members
```
# <a name="c"></a>[<span data-ttu-id="532d7-148">C#</span><span class="sxs-lookup"><span data-stu-id="532d7-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="532d7-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="532d7-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="532d7-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="532d7-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="532d7-151">Java</span><span class="sxs-lookup"><span data-stu-id="532d7-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="532d7-152">响应</span><span class="sxs-lookup"><span data-stu-id="532d7-152">Response</span></span>

<span data-ttu-id="532d7-153">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="532d7-153">The following is an example of the response.</span></span>
><span data-ttu-id="532d7-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="532d7-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-all-membership"></a><span data-ttu-id="532d7-156">示例 2：仅获取所有会员资格的计数</span><span class="sxs-lookup"><span data-stu-id="532d7-156">Example 2: Get only a count of all membership</span></span>

#### <a name="request"></a><span data-ttu-id="532d7-157">请求</span><span class="sxs-lookup"><span data-stu-id="532d7-157">Request</span></span>

<span data-ttu-id="532d7-158">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="532d7-158">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="532d7-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="532d7-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/members/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="532d7-160">C#</span><span class="sxs-lookup"><span data-stu-id="532d7-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="532d7-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="532d7-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="532d7-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="532d7-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="532d7-163">Java</span><span class="sxs-lookup"><span data-stu-id="532d7-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-count-only-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="532d7-164">响应</span><span class="sxs-lookup"><span data-stu-id="532d7-164">Response</span></span>

<span data-ttu-id="532d7-165">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="532d7-165">The following is an example of the response.</span></span>

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

<span data-ttu-id="532d7-166">893</span><span class="sxs-lookup"><span data-stu-id="532d7-166">893</span></span>

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-user-membership"></a><span data-ttu-id="532d7-167">示例 3：使用 OData 强制转换获取仅用户会员资格的计数</span><span class="sxs-lookup"><span data-stu-id="532d7-167">Example 3: Use OData cast to get only a count of user membership</span></span>

#### <a name="request"></a><span data-ttu-id="532d7-168">请求</span><span class="sxs-lookup"><span data-stu-id="532d7-168">Request</span></span>

<span data-ttu-id="532d7-169">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="532d7-169">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="532d7-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="532d7-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_user_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/members/microsoft.graph.user/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="532d7-171">C#</span><span class="sxs-lookup"><span data-stu-id="532d7-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-user-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="532d7-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="532d7-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-user-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="532d7-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="532d7-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-user-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="532d7-174">Java</span><span class="sxs-lookup"><span data-stu-id="532d7-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-count-user-only-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="532d7-175">响应</span><span class="sxs-lookup"><span data-stu-id="532d7-175">Response</span></span>

<span data-ttu-id="532d7-176">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="532d7-176">The following is an example of the response.</span></span>

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

<span data-ttu-id="532d7-177">893</span><span class="sxs-lookup"><span data-stu-id="532d7-177">893</span></span>

### <a name="example-4-use-search-and-odata-cast-to-get-user-membership-in-groups-with-display-names-that-contain-the-letters-pr-including-a-count-of-returned-objects"></a><span data-ttu-id="532d7-178">示例4：使用 $search 和 OData cast 以使用包含字母 "Pr" 的显示名称获取组中的用户成员身份，包括返回对象的计数</span><span class="sxs-lookup"><span data-stu-id="532d7-178">Example 4: Use $search and OData cast to get user membership in groups with display names that contain the letters 'Pr' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="532d7-179">请求</span><span class="sxs-lookup"><span data-stu-id="532d7-179">Request</span></span>

<span data-ttu-id="532d7-180">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="532d7-180">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="532d7-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="532d7-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_pr_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/members/microsoft.graph.user?$count=true&$orderby=displayName&$search="displayName:Pr"&$select=displayName,id
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="532d7-182">C#</span><span class="sxs-lookup"><span data-stu-id="532d7-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-pr-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="532d7-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="532d7-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-pr-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="532d7-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="532d7-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-pr-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="532d7-185">Java</span><span class="sxs-lookup"><span data-stu-id="532d7-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-pr-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="532d7-186">响应</span><span class="sxs-lookup"><span data-stu-id="532d7-186">Response</span></span>

<span data-ttu-id="532d7-187">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="532d7-187">The following is an example of the response.</span></span>
><span data-ttu-id="532d7-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="532d7-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-5-use-filter-to-get-group-membership-with-a-display-name-that-starts-with-the-letter-a-including-a-count-of-returned-objects"></a><span data-ttu-id="532d7-190">示例 5：使用 $filter 来获取显示名称以字母 “A” 开头（包括返回的对象数目）的组会员资格</span><span class="sxs-lookup"><span data-stu-id="532d7-190">Example 5: Use $filter to get group membership with a display name that starts with the letter 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="532d7-191">请求</span><span class="sxs-lookup"><span data-stu-id="532d7-191">Request</span></span>

<span data-ttu-id="532d7-192">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="532d7-192">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="532d7-193">HTTP</span><span class="sxs-lookup"><span data-stu-id="532d7-193">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/members?$count=true&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="532d7-194">C#</span><span class="sxs-lookup"><span data-stu-id="532d7-194">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="532d7-195">JavaScript</span><span class="sxs-lookup"><span data-stu-id="532d7-195">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="532d7-196">Objective-C</span><span class="sxs-lookup"><span data-stu-id="532d7-196">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="532d7-197">Java</span><span class="sxs-lookup"><span data-stu-id="532d7-197">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-a-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="532d7-198">响应</span><span class="sxs-lookup"><span data-stu-id="532d7-198">Response</span></span>

<span data-ttu-id="532d7-199">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="532d7-199">The following is an example of the response.</span></span>
><span data-ttu-id="532d7-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="532d7-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


