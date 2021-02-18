---
title: 列出成员
description: 获取组的直接成员列表。 组可将用户、组织联系人、设备、服务主体和其他组作为成员。
localization_priority: Priority
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: a0d9c77bb6fd6bb7685fd13ae816ee5587c01f83
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272196"
---
# <a name="list-members"></a><span data-ttu-id="48841-104">列出成员</span><span class="sxs-lookup"><span data-stu-id="48841-104">List members</span></span>

<span data-ttu-id="48841-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="48841-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="48841-106">获取组的直接成员列表。</span><span class="sxs-lookup"><span data-stu-id="48841-106">Get a list of the group's direct members.</span></span> <span data-ttu-id="48841-107">组可将用户、组织联系人、设备、服务主体和其他组作为成员。</span><span class="sxs-lookup"><span data-stu-id="48841-107">A group can have users, organizational contacts, devices, service principals and other groups as members.</span></span> <span data-ttu-id="48841-108">当前，由于在 Graph V1.0 终结点上分阶段部署服务主体，因此未将服务主体列为组成员。</span><span class="sxs-lookup"><span data-stu-id="48841-108">Currently service principals are not listed as group members due to staged roll-out of service principals on Graph V1.0 endpoint.</span></span> <span data-ttu-id="48841-109">此操作不可传递。</span><span class="sxs-lookup"><span data-stu-id="48841-109">This operation is not transitive.</span></span>

<span data-ttu-id="48841-110">当组包含超过 100 个成员时，Microsoft Graph 将在响应中返回 `@odata.nextLink` 属性，其中包含指向下一页结果的 URL。</span><span class="sxs-lookup"><span data-stu-id="48841-110">When a group contains more than 100 members, Microsoft Graph returns a `@odata.nextLink` property in the response that contains a URL to the next page of results.</span></span> <span data-ttu-id="48841-111">如果该属性存在，请继续使用每次响应中的 `@odata.nextLink` URL 来创建额外请求，直至返回所有结果，如[在应用中对 Microsoft Graph 数据进行分页](/graph/paging)一文中所述。</span><span class="sxs-lookup"><span data-stu-id="48841-111">If that property is present, continue making additional requests with the `@odata.nextLink` URL in each response, until all the results are returned, as described in [paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="48841-112">权限</span><span class="sxs-lookup"><span data-stu-id="48841-112">Permissions</span></span>
<span data-ttu-id="48841-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="48841-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48841-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="48841-115">Permission type</span></span>      | <span data-ttu-id="48841-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="48841-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="48841-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="48841-117">Delegated (work or school account)</span></span> | <span data-ttu-id="48841-118">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="48841-118">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All</span></span>  |
|<span data-ttu-id="48841-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="48841-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48841-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="48841-120">Not supported.</span></span>    |
|<span data-ttu-id="48841-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="48841-121">Application</span></span> | <span data-ttu-id="48841-122">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="48841-122">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="48841-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="48841-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="48841-124">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="48841-124">Optional query parameters</span></span>

<span data-ttu-id="48841-125">此方法支持[OData query parameters](/graph/query-parameters)以帮助自定义响应，包括 `$search`、`$count`、 和 `$filter`</span><span class="sxs-lookup"><span data-stu-id="48841-125">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="48841-126">还启用了 OData 强制转换，例如，你可以通过强制转换来获取仅是组成员的用户。</span><span class="sxs-lookup"><span data-stu-id="48841-126">OData cast is also enabled, for example, you can cast to get just the users that are a member of the group.</span></span> <span data-ttu-id="48841-127">可使用“**displayName**”和“**说明**”属性上的`$search`。</span><span class="sxs-lookup"><span data-stu-id="48841-127">You can use `$search` on the **displayName** and **description** properties.</span></span> <span data-ttu-id="48841-128">为该资源添加或更新项目时，将对它们进行专门索引，以便与 `$count` 和 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="48841-128">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="48841-129">在添加或更新项目与在索引中可用之间可能会稍有延迟。</span><span class="sxs-lookup"><span data-stu-id="48841-129">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="48841-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="48841-130">Request headers</span></span>

| <span data-ttu-id="48841-131">标头</span><span class="sxs-lookup"><span data-stu-id="48841-131">Header</span></span>       | <span data-ttu-id="48841-132">值</span><span class="sxs-lookup"><span data-stu-id="48841-132">Value</span></span> |
|:-----------|:----------|
| <span data-ttu-id="48841-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="48841-133">Authorization</span></span>  | <span data-ttu-id="48841-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="48841-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="48841-136">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="48841-136">ConsistencyLevel</span></span> | <span data-ttu-id="48841-137">最终。</span><span class="sxs-lookup"><span data-stu-id="48841-137">eventual.</span></span> <span data-ttu-id="48841-138">使用 `$search`、`$filter`、`$orderby` 或 OData 强制转换查询参数时，此标头和 `$count` 是必需的。</span><span class="sxs-lookup"><span data-stu-id="48841-138">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="48841-139">它使用的索引可能与对象的最新更改不同步。</span><span class="sxs-lookup"><span data-stu-id="48841-139">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="48841-140">请求正文</span><span class="sxs-lookup"><span data-stu-id="48841-140">Request body</span></span>
<span data-ttu-id="48841-141">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="48841-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="48841-142">响应</span><span class="sxs-lookup"><span data-stu-id="48841-142">Response</span></span>
<span data-ttu-id="48841-143">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="48841-143">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="48841-144">示例</span><span class="sxs-lookup"><span data-stu-id="48841-144">Examples</span></span>

### <a name="example-1-get-the-direct-membership-in-a-group"></a><span data-ttu-id="48841-145">示例1：获取组中的直接成员身份</span><span class="sxs-lookup"><span data-stu-id="48841-145">Example 1: Get the direct membership in a group</span></span>

#### <a name="request"></a><span data-ttu-id="48841-146">请求</span><span class="sxs-lookup"><span data-stu-id="48841-146">Request</span></span>

<span data-ttu-id="48841-147">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="48841-147">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="48841-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="48841-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/members
```
# <a name="c"></a>[<span data-ttu-id="48841-149">C#</span><span class="sxs-lookup"><span data-stu-id="48841-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="48841-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="48841-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="48841-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="48841-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="48841-152">Java</span><span class="sxs-lookup"><span data-stu-id="48841-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="48841-153">响应</span><span class="sxs-lookup"><span data-stu-id="48841-153">Response</span></span>

<span data-ttu-id="48841-154">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="48841-154">The following is an example of the response.</span></span>

><span data-ttu-id="48841-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="48841-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryObjects",
  "value": [
    {
      "id": "11111111-2222-3333-4444-555555555555",
      "mail": "user1@contoso.com"
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-all-membership"></a><span data-ttu-id="48841-157">示例 2：仅获取所有会员资格的计数</span><span class="sxs-lookup"><span data-stu-id="48841-157">Example 2: Get only a count of all membership</span></span>

#### <a name="request"></a><span data-ttu-id="48841-158">请求</span><span class="sxs-lookup"><span data-stu-id="48841-158">Request</span></span>

<span data-ttu-id="48841-159">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="48841-159">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/members/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="48841-160">响应</span><span class="sxs-lookup"><span data-stu-id="48841-160">Response</span></span>

<span data-ttu-id="48841-161">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="48841-161">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`893`


### <a name="example-3-use-odata-cast-to-get-only-a-count-of-user-membership"></a><span data-ttu-id="48841-162">示例 3：使用 OData 强制转换获取仅用户会员资格的计数</span><span class="sxs-lookup"><span data-stu-id="48841-162">Example 3: Use OData cast to get only a count of user membership</span></span>

#### <a name="request"></a><span data-ttu-id="48841-163">请求</span><span class="sxs-lookup"><span data-stu-id="48841-163">Request</span></span>

<span data-ttu-id="48841-164">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="48841-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_user_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/members/microsoft.graph.user/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="48841-165">响应</span><span class="sxs-lookup"><span data-stu-id="48841-165">Response</span></span>

<span data-ttu-id="48841-166">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="48841-166">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`893`

### <a name="example-4-use-searchand-odata-cast-to-get-user-membership-in-groups-with-display-names-that-contain-the-letters-pr-including-a-count-of-returned-objects"></a><span data-ttu-id="48841-167">示例 4：使用 $search 和 OData 强制转换获取显示名称中包含字母“Pr”（包括返回的对象数）的用户成员身份</span><span class="sxs-lookup"><span data-stu-id="48841-167">Example 4: Use $searchand OData cast to get user membership in groups with display names that contain the letters 'Pr' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="48841-168">请求</span><span class="sxs-lookup"><span data-stu-id="48841-168">Request</span></span>

<span data-ttu-id="48841-169">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="48841-169">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_pr_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/members/microsoft.graph.user?$count=true&$orderby=displayName&$search="displayName:Pr"&$select=displayName,id
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="48841-170">响应</span><span class="sxs-lookup"><span data-stu-id="48841-170">Response</span></span>

<span data-ttu-id="48841-171">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="48841-171">The following is an example of the response.</span></span>

><span data-ttu-id="48841-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="48841-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users(displayName,id)",
  "@odata.count":7,
  "value":[
    {
      "displayName":"Joseph Price",
      "id":"11111111-2222-3333-4444-555555555555"
    },
    {
      "displayName":"Preston Morales",
      "id":"66666666-7777-8888-9999-000000000000"
    }
  ]
}
```

### <a name="example-5-use-filter-to-get-group-membership-with-a-display-name-that-starts-with-the-letter-a-including-a-count-of-returned-objects"></a><span data-ttu-id="48841-174">示例 5：使用 $filter 来获取显示名称以字母 “A” 开头（包括返回的对象数目）的组会员资格</span><span class="sxs-lookup"><span data-stu-id="48841-174">Example 5: Use $filter to get group membership with a display name that starts with the letter 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="48841-175">请求</span><span class="sxs-lookup"><span data-stu-id="48841-175">Request</span></span>

<span data-ttu-id="48841-176">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="48841-176">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/members?$count=true&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="48841-177">响应</span><span class="sxs-lookup"><span data-stu-id="48841-177">Response</span></span>

<span data-ttu-id="48841-178">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="48841-178">The following is an example of the response.</span></span>

><span data-ttu-id="48841-p110">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="48841-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#directoryObjects",
  "@odata.count":76,
  "value":[
    {
      "displayName":"AAD Contoso Users",
      "mail":"AADContoso_Users@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
