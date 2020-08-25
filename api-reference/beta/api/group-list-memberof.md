---
title: List group memberOf
description: 获取组是其直接成员的组和管理单元。
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 463e35eca28d0f5c52a0d01a9f57a23aa356ff43
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2020
ms.locfileid: "46872616"
---
# <a name="list-group-memberof"></a><span data-ttu-id="6f87a-103">List group memberOf</span><span class="sxs-lookup"><span data-stu-id="6f87a-103">List group memberOf</span></span>

<span data-ttu-id="6f87a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f87a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f87a-105">获取组是其直接成员的组和管理单元。</span><span class="sxs-lookup"><span data-stu-id="6f87a-105">Get groups and administrative units that the group is a direct member of.</span></span>

<span data-ttu-id="6f87a-p101">此操作不可传递。与获取用户的 Microsoft 365 组不同，这将返回所有类型的组，而不仅仅是 Microsoft 365 组。</span><span class="sxs-lookup"><span data-stu-id="6f87a-p101">This operation is not transitive. Unlike getting a user's Microsoft 365 groups, this returns all types of groups, not just Microsoft 365 groups.</span></span> 

## <a name="permissions"></a><span data-ttu-id="6f87a-108">权限</span><span class="sxs-lookup"><span data-stu-id="6f87a-108">Permissions</span></span>

<span data-ttu-id="6f87a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6f87a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6f87a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6f87a-111">Permission type</span></span> | <span data-ttu-id="6f87a-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6f87a-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="6f87a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6f87a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="6f87a-114">GroupMember.Read.All、Group.Read.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6f87a-114">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
| <span data-ttu-id="6f87a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6f87a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f87a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6f87a-116">Not supported.</span></span> |
| <span data-ttu-id="6f87a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6f87a-117">Application</span></span> | <span data-ttu-id="6f87a-118">GroupMember.Read.All、Group.Read.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f87a-118">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6f87a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6f87a-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6f87a-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6f87a-120">Optional query parameters</span></span>

<span data-ttu-id="6f87a-121">此方法支持[OData query parameters](/graph/query_parameters)以帮助自定义响应，包括 `$search`、`$count`、 和 `$filter`</span><span class="sxs-lookup"><span data-stu-id="6f87a-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="6f87a-122">此外，还启用了 OData 强制转换，例如，您可以强制转换以仅获取该组所属的组。</span><span class="sxs-lookup"><span data-stu-id="6f87a-122">OData cast is also enabled, for example, you can cast to get just the groups the group is a member of.</span></span> <span data-ttu-id="6f87a-123">`$search`可以用在 **displayName**属性。</span><span class="sxs-lookup"><span data-stu-id="6f87a-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="6f87a-124">为该资源添加或更新项目时，将对它们进行专门索引，以便与 `$count` 和 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="6f87a-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="6f87a-125">在添加或更新项目与在索引中可用之间可能会稍有延迟。</span><span class="sxs-lookup"><span data-stu-id="6f87a-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6f87a-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="6f87a-126">Request headers</span></span>

| <span data-ttu-id="6f87a-127">名称</span><span class="sxs-lookup"><span data-stu-id="6f87a-127">Name</span></span> | <span data-ttu-id="6f87a-128">说明</span><span class="sxs-lookup"><span data-stu-id="6f87a-128">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="6f87a-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f87a-129">Authorization</span></span>  | <span data-ttu-id="6f87a-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6f87a-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6f87a-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="6f87a-132">ConsistencyLevel</span></span> | <span data-ttu-id="6f87a-133">最终。</span><span class="sxs-lookup"><span data-stu-id="6f87a-133">eventual.</span></span> <span data-ttu-id="6f87a-134">在 `$count` 使用 `$search` 、 `$filter` 、 `$orderby` 或 OData 转换查询参数时，此标头和是必需的。</span><span class="sxs-lookup"><span data-stu-id="6f87a-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="6f87a-135">它使用的索引可能不是最新的，并包含对对象的最新更改。</span><span class="sxs-lookup"><span data-stu-id="6f87a-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6f87a-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="6f87a-136">Request body</span></span>

<span data-ttu-id="6f87a-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6f87a-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6f87a-138">响应</span><span class="sxs-lookup"><span data-stu-id="6f87a-138">Response</span></span>

<span data-ttu-id="6f87a-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="6f87a-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6f87a-140">示例</span><span class="sxs-lookup"><span data-stu-id="6f87a-140">Examples</span></span>

### <a name="example-1-get-groups-and-administrative-units-that-the-group-is-a-direct-member-of"></a><span data-ttu-id="6f87a-141">示例1：获取组是组的直接成员的组和管理单元</span><span class="sxs-lookup"><span data-stu-id="6f87a-141">Example 1: Get groups and administrative units that the group is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="6f87a-142">请求</span><span class="sxs-lookup"><span data-stu-id="6f87a-142">Request</span></span>

<span data-ttu-id="6f87a-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6f87a-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6f87a-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="6f87a-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="6f87a-145">C#</span><span class="sxs-lookup"><span data-stu-id="6f87a-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6f87a-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6f87a-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6f87a-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6f87a-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="6f87a-148">响应</span><span class="sxs-lookup"><span data-stu-id="6f87a-148">Response</span></span>

<span data-ttu-id="6f87a-149">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6f87a-149">The following is an example of the response.</span></span>
><span data-ttu-id="6f87a-150">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6f87a-150">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6f87a-151">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6f87a-151">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-all-memberships"></a><span data-ttu-id="6f87a-152">示例2：仅获取所有成员身份的计数</span><span class="sxs-lookup"><span data-stu-id="6f87a-152">Example 2: Get only a count of all memberships</span></span>

#### <a name="request"></a><span data-ttu-id="6f87a-153">请求</span><span class="sxs-lookup"><span data-stu-id="6f87a-153">Request</span></span>

<span data-ttu-id="6f87a-154">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6f87a-154">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6f87a-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="6f87a-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/memberOf/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="6f87a-156">C#</span><span class="sxs-lookup"><span data-stu-id="6f87a-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6f87a-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6f87a-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6f87a-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6f87a-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6f87a-159">响应</span><span class="sxs-lookup"><span data-stu-id="6f87a-159">Response</span></span>

<span data-ttu-id="6f87a-160">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6f87a-160">The following is an example of the response.</span></span>

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

<span data-ttu-id="6f87a-161">394</span><span class="sxs-lookup"><span data-stu-id="6f87a-161">394</span></span>


### <a name="example-3-use-odata-cast-to-get-only-a-count-of-group-membership"></a><span data-ttu-id="6f87a-162">示例3：使用 OData 强制转换仅获取组成员身份的计数</span><span class="sxs-lookup"><span data-stu-id="6f87a-162">Example 3: Use OData cast to get only a count of group membership</span></span>

#### <a name="request"></a><span data-ttu-id="6f87a-163">请求</span><span class="sxs-lookup"><span data-stu-id="6f87a-163">Request</span></span>

<span data-ttu-id="6f87a-164">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6f87a-164">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6f87a-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="6f87a-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_group_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/memberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="6f87a-166">C#</span><span class="sxs-lookup"><span data-stu-id="6f87a-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-group-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6f87a-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6f87a-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-group-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6f87a-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6f87a-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-group-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6f87a-169">响应</span><span class="sxs-lookup"><span data-stu-id="6f87a-169">Response</span></span>

<span data-ttu-id="6f87a-170">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6f87a-170">The following is an example of the response.</span></span>

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

<span data-ttu-id="6f87a-171">394</span><span class="sxs-lookup"><span data-stu-id="6f87a-171">394</span></span>

### <a name="example-4-use-odata-cast-and-search-to-get-membership-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="6f87a-172">示例4：使用 OData 强制转换和 $search 获取显示名称包含字母 "Video" 的成员资格，包括返回对象的计数</span><span class="sxs-lookup"><span data-stu-id="6f87a-172">Example 4: Use OData cast and $search to get membership with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="6f87a-173">请求</span><span class="sxs-lookup"><span data-stu-id="6f87a-173">Request</span></span>

<span data-ttu-id="6f87a-174">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6f87a-174">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6f87a-175">HTTP</span><span class="sxs-lookup"><span data-stu-id="6f87a-175">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:Video"
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="6f87a-176">C#</span><span class="sxs-lookup"><span data-stu-id="6f87a-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-video-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6f87a-177">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6f87a-177">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-video-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6f87a-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6f87a-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-video-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6f87a-179">响应</span><span class="sxs-lookup"><span data-stu-id="6f87a-179">Response</span></span>

<span data-ttu-id="6f87a-180">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6f87a-180">The following is an example of the response.</span></span>
><span data-ttu-id="6f87a-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6f87a-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "value":[
    {
      "displayName":"SFA Videos",
      "mail":"SFAVideos@service.contoso.com",
      "mailNickname":"SFAVideos"
    }
  ]
}
```

### <a name="example-5-use-odata-cast-and-filter-to-get-membership-with-a-display-name-that-starts-with-the-letter-a-including-a-count-of-returned-objects"></a><span data-ttu-id="6f87a-183">示例5：使用 OData 强制转换和 $filter 获取显示名称以字母 "A" 开头的成员，其中包含返回对象的计数</span><span class="sxs-lookup"><span data-stu-id="6f87a-183">Example 5: Use OData cast and $filter to get membership with a display name that starts with the letter 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="6f87a-184">请求</span><span class="sxs-lookup"><span data-stu-id="6f87a-184">Request</span></span>

<span data-ttu-id="6f87a-185">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6f87a-185">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6f87a-186">HTTP</span><span class="sxs-lookup"><span data-stu-id="6f87a-186">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'A')
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="6f87a-187">C#</span><span class="sxs-lookup"><span data-stu-id="6f87a-187">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6f87a-188">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6f87a-188">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6f87a-189">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6f87a-189">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6f87a-190">响应</span><span class="sxs-lookup"><span data-stu-id="6f87a-190">Response</span></span>

<span data-ttu-id="6f87a-191">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6f87a-191">The following is an example of the response.</span></span>
><span data-ttu-id="6f87a-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6f87a-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
