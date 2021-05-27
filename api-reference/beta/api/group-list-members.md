---
title: List group members
description: 获取组的直接成员列表。
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 5d61e2cf80220ed7818c0fc983e959e616f82ac8
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52681541"
---
# <a name="list-group-members"></a><span data-ttu-id="bafbf-103">List group members</span><span class="sxs-lookup"><span data-stu-id="bafbf-103">List group members</span></span>

<span data-ttu-id="bafbf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bafbf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bafbf-105">获取组的直接成员列表。</span><span class="sxs-lookup"><span data-stu-id="bafbf-105">Get a list of the group's direct members.</span></span> <span data-ttu-id="bafbf-106">组可以将用户、联系人、设备、服务主体和其他组作为成员。</span><span class="sxs-lookup"><span data-stu-id="bafbf-106">A group can have users, contacts, devices, service principals, and other groups as members.</span></span> <span data-ttu-id="bafbf-107">此操作不可传递。</span><span class="sxs-lookup"><span data-stu-id="bafbf-107">This operation is not transitive.</span></span>

<span data-ttu-id="bafbf-108">当组包含超过 100 个成员时，Microsoft Graph 将在响应中返回 `@odata.nextLink` 属性，其中包含指向下一页结果的 URL。</span><span class="sxs-lookup"><span data-stu-id="bafbf-108">When a group contains more than 100 members, Microsoft Graph returns a `@odata.nextLink` property in the response that contains a URL to the next page of results.</span></span> <span data-ttu-id="bafbf-109">如果该属性存在，请继续使用每次响应中的 `@odata.nextLink` URL 来创建额外请求，直至返回所有结果，如[在应用中对 Microsoft Graph 数据进行分页](/graph/paging)一文中所述。</span><span class="sxs-lookup"><span data-stu-id="bafbf-109">If that property is present, continue making additional requests with the `@odata.nextLink` URL in each response, until all the results are returned, as described in [paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="bafbf-110">权限</span><span class="sxs-lookup"><span data-stu-id="bafbf-110">Permissions</span></span>

<span data-ttu-id="bafbf-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bafbf-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bafbf-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="bafbf-113">Permission type</span></span> | <span data-ttu-id="bafbf-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bafbf-114">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="bafbf-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bafbf-115">Delegated (work or school account)</span></span> | <span data-ttu-id="bafbf-116">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="bafbf-116">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All</span></span> |
| <span data-ttu-id="bafbf-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bafbf-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bafbf-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="bafbf-118">Not supported.</span></span> |
| <span data-ttu-id="bafbf-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="bafbf-119">Application</span></span> | <span data-ttu-id="bafbf-120">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="bafbf-120">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All</span></span> |

> <span data-ttu-id="bafbf-121">**注意：** 若要列出隐藏成员资格组的成员，需要 Member.Read.Hidden 权限。</span><span class="sxs-lookup"><span data-stu-id="bafbf-121">**Note:** To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]
 
## <a name="http-request"></a><span data-ttu-id="bafbf-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bafbf-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bafbf-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="bafbf-123">Optional query parameters</span></span>

<span data-ttu-id="bafbf-124">此方法支持[OData query parameters](/graph/query_parameters)以帮助自定义响应，包括 `$search`、`$count`、 和 `$filter`</span><span class="sxs-lookup"><span data-stu-id="bafbf-124">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="bafbf-125">还启用了 OData 强制转换，例如，你可以通过强制转换来获取仅是组成员的用户。</span><span class="sxs-lookup"><span data-stu-id="bafbf-125">OData cast is also enabled, for example, you can cast to get just the users that are a member of the group.</span></span> <span data-ttu-id="bafbf-126">`$search`可以用在 **displayName** 属性。</span><span class="sxs-lookup"><span data-stu-id="bafbf-126">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="bafbf-127">为该资源添加或更新项目时，将对它们进行专门索引，以便与 `$count` 和 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="bafbf-127">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="bafbf-128">在添加或更新项目与在索引中可用之间可能会稍有延迟。</span><span class="sxs-lookup"><span data-stu-id="bafbf-128">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bafbf-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="bafbf-129">Request headers</span></span>

| <span data-ttu-id="bafbf-130">名称</span><span class="sxs-lookup"><span data-stu-id="bafbf-130">Name</span></span> | <span data-ttu-id="bafbf-131">说明</span><span class="sxs-lookup"><span data-stu-id="bafbf-131">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="bafbf-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="bafbf-132">Authorization</span></span> | <span data-ttu-id="bafbf-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bafbf-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bafbf-135">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="bafbf-135">ConsistencyLevel</span></span> | <span data-ttu-id="bafbf-136">最终。</span><span class="sxs-lookup"><span data-stu-id="bafbf-136">eventual.</span></span> <span data-ttu-id="bafbf-137">使用 `$search`、`$filter`、`$orderby` 或 OData 强制转换查询参数时，此标头和 `$count` 是必需的。</span><span class="sxs-lookup"><span data-stu-id="bafbf-137">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="bafbf-138">它使用的索引可能与对象的最新更改不同步。</span><span class="sxs-lookup"><span data-stu-id="bafbf-138">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bafbf-139">请求正文</span><span class="sxs-lookup"><span data-stu-id="bafbf-139">Request body</span></span>

<span data-ttu-id="bafbf-140">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bafbf-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bafbf-141">响应</span><span class="sxs-lookup"><span data-stu-id="bafbf-141">Response</span></span>

<span data-ttu-id="bafbf-142">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="bafbf-142">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bafbf-143">示例</span><span class="sxs-lookup"><span data-stu-id="bafbf-143">Examples</span></span>

### <a name="example-1-get-the-direct-membership-in-a-group"></a><span data-ttu-id="bafbf-144">示例1：获取组中的直接成员身份</span><span class="sxs-lookup"><span data-stu-id="bafbf-144">Example 1: Get the direct membership in a group</span></span>

#### <a name="request"></a><span data-ttu-id="bafbf-145">请求</span><span class="sxs-lookup"><span data-stu-id="bafbf-145">Request</span></span>

<span data-ttu-id="bafbf-146">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bafbf-146">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bafbf-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="bafbf-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/members
```
# <a name="c"></a>[<span data-ttu-id="bafbf-148">C#</span><span class="sxs-lookup"><span data-stu-id="bafbf-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bafbf-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bafbf-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bafbf-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bafbf-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bafbf-151">Java</span><span class="sxs-lookup"><span data-stu-id="bafbf-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="bafbf-152">响应</span><span class="sxs-lookup"><span data-stu-id="bafbf-152">Response</span></span>

<span data-ttu-id="bafbf-153">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bafbf-153">The following is an example of the response.</span></span>
><span data-ttu-id="bafbf-154">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="bafbf-154">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-only-a-count-of-all-membership"></a><span data-ttu-id="bafbf-155">示例 2：仅获取所有会员资格的计数</span><span class="sxs-lookup"><span data-stu-id="bafbf-155">Example 2: Get only a count of all membership</span></span>

#### <a name="request"></a><span data-ttu-id="bafbf-156">请求</span><span class="sxs-lookup"><span data-stu-id="bafbf-156">Request</span></span>

<span data-ttu-id="bafbf-157">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bafbf-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/members/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="bafbf-158">响应</span><span class="sxs-lookup"><span data-stu-id="bafbf-158">Response</span></span>

<span data-ttu-id="bafbf-159">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bafbf-159">The following is an example of the response.</span></span>

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

<span data-ttu-id="bafbf-160">893</span><span class="sxs-lookup"><span data-stu-id="bafbf-160">893</span></span>

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-user-membership"></a><span data-ttu-id="bafbf-161">示例 3：使用 OData 强制转换获取仅用户会员资格的计数</span><span class="sxs-lookup"><span data-stu-id="bafbf-161">Example 3: Use OData cast to get only a count of user membership</span></span>

#### <a name="request"></a><span data-ttu-id="bafbf-162">请求</span><span class="sxs-lookup"><span data-stu-id="bafbf-162">Request</span></span>

<span data-ttu-id="bafbf-163">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bafbf-163">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_user_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/members/microsoft.graph.user/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="bafbf-164">响应</span><span class="sxs-lookup"><span data-stu-id="bafbf-164">Response</span></span>

<span data-ttu-id="bafbf-165">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bafbf-165">The following is an example of the response.</span></span>

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

<span data-ttu-id="bafbf-166">893</span><span class="sxs-lookup"><span data-stu-id="bafbf-166">893</span></span>

### <a name="example-4-use-search-and-odata-cast-to-get-user-membership-in-groups-with-display-names-that-contain-the-letters-pr-including-a-count-of-returned-objects"></a><span data-ttu-id="bafbf-167">示例 4：使用 $search 和 OData 转换获取显示名称包含字母"Pr"（包括返回对象计数）的组的用户成员资格</span><span class="sxs-lookup"><span data-stu-id="bafbf-167">Example 4: Use $search and OData cast to get user membership in groups with display names that contain the letters 'Pr' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="bafbf-168">请求</span><span class="sxs-lookup"><span data-stu-id="bafbf-168">Request</span></span>

<span data-ttu-id="bafbf-169">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bafbf-169">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_pr_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/members/microsoft.graph.user?$count=true&$orderby=displayName&$search="displayName:Pr"&$select=displayName,id
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="bafbf-170">响应</span><span class="sxs-lookup"><span data-stu-id="bafbf-170">Response</span></span>

<span data-ttu-id="bafbf-171">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bafbf-171">The following is an example of the response.</span></span>
><span data-ttu-id="bafbf-172">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="bafbf-172">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-5-use-filter-to-get-group-membership-with-a-display-name-that-starts-with-the-letter-a-including-a-count-of-returned-objects"></a><span data-ttu-id="bafbf-173">示例 5：使用 $filter 来获取显示名称以字母 “A” 开头（包括返回的对象数目）的组会员资格</span><span class="sxs-lookup"><span data-stu-id="bafbf-173">Example 5: Use $filter to get group membership with a display name that starts with the letter 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="bafbf-174">请求</span><span class="sxs-lookup"><span data-stu-id="bafbf-174">Request</span></span>

<span data-ttu-id="bafbf-175">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bafbf-175">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/members?$count=true&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="bafbf-176">响应</span><span class="sxs-lookup"><span data-stu-id="bafbf-176">Response</span></span>

<span data-ttu-id="bafbf-177">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bafbf-177">The following is an example of the response.</span></span>
><span data-ttu-id="bafbf-178">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="bafbf-178">**Note:** The response object shown here might be shortened for readability.</span></span>

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


