---
title: List group transitive memberOf
description: 获取组所属的组和管理单元。
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: bf4e1365b392736a1856cb8c6284a7a4babc97dc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47990877"
---
# <a name="list-group-transitive-memberof"></a><span data-ttu-id="9f3f9-103">List group transitive memberOf</span><span class="sxs-lookup"><span data-stu-id="9f3f9-103">List group transitive memberOf</span></span>

<span data-ttu-id="9f3f9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f3f9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f3f9-105">获取组所属的组和管理单元。</span><span class="sxs-lookup"><span data-stu-id="9f3f9-105">Get groups and administrative units that the group is a member of.</span></span>  <span data-ttu-id="9f3f9-106">此操作是可传递的，还将包括此组嵌套成员的所有组。</span><span class="sxs-lookup"><span data-stu-id="9f3f9-106">This operation is transitive and will also include all groups that this groups is a nested member of.</span></span> <span data-ttu-id="9f3f9-107">与获取用户的 Microsoft 365 组不同，这将返回所有类型的组，而不仅仅是 Microsoft 365 组。</span><span class="sxs-lookup"><span data-stu-id="9f3f9-107">Unlike getting a user's Microsoft 365 groups, this returns all types of groups, not just Microsoft 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="9f3f9-108">权限</span><span class="sxs-lookup"><span data-stu-id="9f3f9-108">Permissions</span></span>

<span data-ttu-id="9f3f9-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9f3f9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9f3f9-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9f3f9-111">Permission type</span></span> | <span data-ttu-id="9f3f9-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9f3f9-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="9f3f9-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9f3f9-113">Delegated (work or school account)</span></span> | <span data-ttu-id="9f3f9-114">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9f3f9-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
| <span data-ttu-id="9f3f9-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9f3f9-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f3f9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9f3f9-116">Not supported.</span></span> |
| <span data-ttu-id="9f3f9-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9f3f9-117">Application</span></span> | <span data-ttu-id="9f3f9-118">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f3f9-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="9f3f9-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9f3f9-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9f3f9-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9f3f9-120">Optional query parameters</span></span>

<span data-ttu-id="9f3f9-121">此方法支持[OData query parameters](/graph/query_parameters)以帮助自定义响应，包括 `$search`、`$count`、 和 `$filter`</span><span class="sxs-lookup"><span data-stu-id="9f3f9-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="9f3f9-122">此外，还会启用 OData 强制转换，例如，您可以强制转换以仅获取组的可传递组成员。</span><span class="sxs-lookup"><span data-stu-id="9f3f9-122">OData cast is also enabled, for example, you can cast to get just the transitive group members of a group.</span></span> <span data-ttu-id="9f3f9-123">`$search`可以用在 **displayName**属性。</span><span class="sxs-lookup"><span data-stu-id="9f3f9-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="9f3f9-124">为该资源添加或更新项目时，将对它们进行专门索引，以便与 `$count` 和 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="9f3f9-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="9f3f9-125">在添加或更新项目与在索引中可用之间可能会稍有延迟。</span><span class="sxs-lookup"><span data-stu-id="9f3f9-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9f3f9-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="9f3f9-126">Request headers</span></span>

| <span data-ttu-id="9f3f9-127">名称</span><span class="sxs-lookup"><span data-stu-id="9f3f9-127">Name</span></span> | <span data-ttu-id="9f3f9-128">说明</span><span class="sxs-lookup"><span data-stu-id="9f3f9-128">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="9f3f9-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f3f9-129">Authorization</span></span>  | <span data-ttu-id="9f3f9-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9f3f9-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9f3f9-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="9f3f9-132">ConsistencyLevel</span></span> | <span data-ttu-id="9f3f9-133">最终。</span><span class="sxs-lookup"><span data-stu-id="9f3f9-133">eventual.</span></span> <span data-ttu-id="9f3f9-134">使用 `$search`、`$filter`、`$orderby` 或 OData 强制转换查询参数时，此标头和 `$count` 是必需的。</span><span class="sxs-lookup"><span data-stu-id="9f3f9-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="9f3f9-135">它使用的索引可能与对象的最新更改不同步。</span><span class="sxs-lookup"><span data-stu-id="9f3f9-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9f3f9-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="9f3f9-136">Request body</span></span>

<span data-ttu-id="9f3f9-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9f3f9-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f3f9-138">响应</span><span class="sxs-lookup"><span data-stu-id="9f3f9-138">Response</span></span>

<span data-ttu-id="9f3f9-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="9f3f9-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9f3f9-140">示例</span><span class="sxs-lookup"><span data-stu-id="9f3f9-140">Examples</span></span>

### <a name="example-1-get-groups-and-administrative-units-that-the-group-is-a-transitive-member-of"></a><span data-ttu-id="9f3f9-141">示例1：获取组是该组的可传递成员的组和管理单元</span><span class="sxs-lookup"><span data-stu-id="9f3f9-141">Example 1: Get groups and administrative units that the group is a transitive member of</span></span>

#### <a name="request"></a><span data-ttu-id="9f3f9-142">请求</span><span class="sxs-lookup"><span data-stu-id="9f3f9-142">Request</span></span>

<span data-ttu-id="9f3f9-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9f3f9-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9f3f9-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="9f3f9-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="9f3f9-145">C#</span><span class="sxs-lookup"><span data-stu-id="9f3f9-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9f3f9-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9f3f9-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9f3f9-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9f3f9-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="9f3f9-148">响应</span><span class="sxs-lookup"><span data-stu-id="9f3f9-148">Response</span></span>

<span data-ttu-id="9f3f9-149">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="9f3f9-149">The following is an example of the response.</span></span>
><span data-ttu-id="9f3f9-150">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9f3f9-150">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9f3f9-151">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9f3f9-151">All the properties will be returned from an actual call.</span></span>

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
      "mailNickname": "ContosoGroup1",
      "securityEnabled": true
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-all-transitive-membership"></a><span data-ttu-id="9f3f9-152">示例 2：仅获取所有可传递成员身份的计数</span><span class="sxs-lookup"><span data-stu-id="9f3f9-152">Example 2: Get only a count of all transitive membership</span></span>

#### <a name="request"></a><span data-ttu-id="9f3f9-153">请求</span><span class="sxs-lookup"><span data-stu-id="9f3f9-153">Request</span></span>

<span data-ttu-id="9f3f9-154">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9f3f9-154">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9f3f9-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="9f3f9-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="9f3f9-156">C#</span><span class="sxs-lookup"><span data-stu-id="9f3f9-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9f3f9-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9f3f9-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9f3f9-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9f3f9-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9f3f9-159">响应</span><span class="sxs-lookup"><span data-stu-id="9f3f9-159">Response</span></span>

<span data-ttu-id="9f3f9-160">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9f3f9-160">The following is an example of the response.</span></span>

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

<span data-ttu-id="9f3f9-161">294</span><span class="sxs-lookup"><span data-stu-id="9f3f9-161">294</span></span>

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-transitive-membership-in-groups"></a><span data-ttu-id="9f3f9-162">示例 3：使用 OData 强制转换以仅获取组中可传递成员身份的计数</span><span class="sxs-lookup"><span data-stu-id="9f3f9-162">Example 3: Use OData cast to get only a count of transitive membership in groups</span></span>

#### <a name="request"></a><span data-ttu-id="9f3f9-163">请求</span><span class="sxs-lookup"><span data-stu-id="9f3f9-163">Request</span></span>

<span data-ttu-id="9f3f9-164">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9f3f9-164">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9f3f9-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="9f3f9-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="9f3f9-166">C#</span><span class="sxs-lookup"><span data-stu-id="9f3f9-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9f3f9-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9f3f9-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9f3f9-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9f3f9-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9f3f9-169">响应</span><span class="sxs-lookup"><span data-stu-id="9f3f9-169">Response</span></span>

<span data-ttu-id="9f3f9-170">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9f3f9-170">The following is an example of the response.</span></span>

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

<span data-ttu-id="9f3f9-171">294</span><span class="sxs-lookup"><span data-stu-id="9f3f9-171">294</span></span>


### <a name="example-4-use-odata-cast-and-search-to-get-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="9f3f9-172">示例4：使用 OData 强制转换和 $search 获取包含包含字母 "层" 的组的组成员身份，其中包括返回的对象的计数</span><span class="sxs-lookup"><span data-stu-id="9f3f9-172">Example 4: Use OData cast and $search to get membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="9f3f9-173">请求</span><span class="sxs-lookup"><span data-stu-id="9f3f9-173">Request</span></span>

<span data-ttu-id="9f3f9-174">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9f3f9-174">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9f3f9-175">HTTP</span><span class="sxs-lookup"><span data-stu-id="9f3f9-175">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="9f3f9-176">C#</span><span class="sxs-lookup"><span data-stu-id="9f3f9-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tier-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9f3f9-177">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9f3f9-177">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tier-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9f3f9-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9f3f9-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tier-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9f3f9-179">响应</span><span class="sxs-lookup"><span data-stu-id="9f3f9-179">Response</span></span>

<span data-ttu-id="9f3f9-180">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9f3f9-180">The following is an example of the response.</span></span>
><span data-ttu-id="9f3f9-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9f3f9-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-5-use-odata-cast-and-filter-to-get-membership-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="9f3f9-183">示例5：使用 OData 强制转换和 $filter 获取显示名称以 "A" 开头的成员身份，其中包含返回对象的计数</span><span class="sxs-lookup"><span data-stu-id="9f3f9-183">Example 5: Use OData cast and $filter to get membership with a display name that starts with 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="9f3f9-184">请求</span><span class="sxs-lookup"><span data-stu-id="9f3f9-184">Request</span></span>

<span data-ttu-id="9f3f9-185">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9f3f9-185">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9f3f9-186">HTTP</span><span class="sxs-lookup"><span data-stu-id="9f3f9-186">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="9f3f9-187">C#</span><span class="sxs-lookup"><span data-stu-id="9f3f9-187">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9f3f9-188">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9f3f9-188">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9f3f9-189">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9f3f9-189">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9f3f9-190">响应</span><span class="sxs-lookup"><span data-stu-id="9f3f9-190">Response</span></span>

<span data-ttu-id="9f3f9-191">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9f3f9-191">The following is an example of the response.</span></span>
><span data-ttu-id="9f3f9-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9f3f9-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "List group transitive memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


