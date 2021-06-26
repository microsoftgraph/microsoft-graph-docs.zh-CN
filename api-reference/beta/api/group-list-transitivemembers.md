---
title: List group transitive members
description: 获取组的成员列表。
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 752483696ea527a760fe6c5d97bd0932cb41078c
ms.sourcegitcommit: 0ca0a1e2810701c2392e5c685e984fbfb6785579
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2021
ms.locfileid: "53151480"
---
# <a name="list-group-transitive-members"></a><span data-ttu-id="6632c-103">List group transitive members</span><span class="sxs-lookup"><span data-stu-id="6632c-103">List group transitive members</span></span>

<span data-ttu-id="6632c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6632c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6632c-105">获取组的成员列表。</span><span class="sxs-lookup"><span data-stu-id="6632c-105">Get a list of the group's members.</span></span> <span data-ttu-id="6632c-106">组可以将用户、联系人、设备、服务主体和其他组作为成员。</span><span class="sxs-lookup"><span data-stu-id="6632c-106">A group can have users, contacts, devices, service principals, and other groups as members.</span></span> <span data-ttu-id="6632c-107">此操作是可传递的，并且还将返回简单列表嵌套成员的成员。</span><span class="sxs-lookup"><span data-stu-id="6632c-107">This operation is transitive and will also return a flat list of all nested members.</span></span>

## <a name="permissions"></a><span data-ttu-id="6632c-108">权限</span><span class="sxs-lookup"><span data-stu-id="6632c-108">Permissions</span></span>

<span data-ttu-id="6632c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6632c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6632c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6632c-111">Permission type</span></span> | <span data-ttu-id="6632c-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6632c-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="6632c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6632c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="6632c-114">GroupMember.Read.All，Group.Read.All，GroupMember.ReadWrite.All，Group.ReadWrite.All，Directory.Read.All，Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6632c-114">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
| <span data-ttu-id="6632c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6632c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6632c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6632c-116">Not supported.</span></span> |
| <span data-ttu-id="6632c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6632c-117">Application</span></span> | <span data-ttu-id="6632c-118">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="6632c-118">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All</span></span> |

> <span data-ttu-id="6632c-119">**注意：** 若要列出隐藏成员资格组的成员， *需要 Member.Read.Hidden* 权限。</span><span class="sxs-lookup"><span data-stu-id="6632c-119">**Note:** To list the members of a hidden membership group, the *Member.Read.Hidden* permission is required.</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="6632c-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6632c-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/transitiveMembers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6632c-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6632c-121">Optional query parameters</span></span>

<span data-ttu-id="6632c-122">此方法支持[OData query parameters](/graph/query-parameters)以帮助自定义响应，包括 `$search`、`$count`、 和 `$filter`</span><span class="sxs-lookup"><span data-stu-id="6632c-122">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="6632c-123">可使用“**displayName**”和“**说明**”属性上的`$search`。</span><span class="sxs-lookup"><span data-stu-id="6632c-123">You can use `$search` on the **displayName** and **description** properties.</span></span> <span data-ttu-id="6632c-124">为该资源添加或更新项目时，将对它们进行专门索引，以便与 `$count` 和 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="6632c-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="6632c-125">在添加或更新项目与在索引中可用之间可能会稍有延迟。</span><span class="sxs-lookup"><span data-stu-id="6632c-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

<span data-ttu-id="6632c-126">若要筛选 OData 类型（如 或 ）上的结果， `microsoft.graph.user` `microsoft.graph.group` 必须使用 [高级查询参数](/graph/aad-advanced-queries)。</span><span class="sxs-lookup"><span data-stu-id="6632c-126">To filter the results on the OData type, such as `microsoft.graph.user` or `microsoft.graph.group`, you must use the [advanced query parameters](/graph/aad-advanced-queries).</span></span> <span data-ttu-id="6632c-127">即，将 **ConsistencyLevel** 标头设置为 `eventual` 和 `$count=true` 查询字符串。</span><span class="sxs-lookup"><span data-stu-id="6632c-127">That is, the **ConsistencyLevel** header set to `eventual` and the `$count=true` query string.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6632c-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="6632c-128">Request headers</span></span>

| <span data-ttu-id="6632c-129">名称</span><span class="sxs-lookup"><span data-stu-id="6632c-129">Name</span></span> | <span data-ttu-id="6632c-130">说明</span><span class="sxs-lookup"><span data-stu-id="6632c-130">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="6632c-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="6632c-131">Authorization</span></span>  | <span data-ttu-id="6632c-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6632c-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6632c-134">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="6632c-134">ConsistencyLevel</span></span> | <span data-ttu-id="6632c-135">最终。</span><span class="sxs-lookup"><span data-stu-id="6632c-135">eventual.</span></span> <span data-ttu-id="6632c-136">使用 `$search`、`$filter`、`$orderby` 或 OData 强制转换查询参数时，此标头和 `$count` 是必需的。</span><span class="sxs-lookup"><span data-stu-id="6632c-136">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="6632c-137">它使用的索引可能与对象的最新更改不同步。</span><span class="sxs-lookup"><span data-stu-id="6632c-137">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6632c-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="6632c-138">Request body</span></span>

<span data-ttu-id="6632c-139">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6632c-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6632c-140">响应</span><span class="sxs-lookup"><span data-stu-id="6632c-140">Response</span></span>

<span data-ttu-id="6632c-141">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="6632c-141">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6632c-142">示例</span><span class="sxs-lookup"><span data-stu-id="6632c-142">Examples</span></span>

### <a name="example-1-get-the-transitive-membership-of-a-group"></a><span data-ttu-id="6632c-143">示例 1：获取组的可传递成员身份</span><span class="sxs-lookup"><span data-stu-id="6632c-143">Example 1: Get the transitive membership of a group</span></span>

#### <a name="request"></a><span data-ttu-id="6632c-144">请求</span><span class="sxs-lookup"><span data-stu-id="6632c-144">Request</span></span>

<span data-ttu-id="6632c-145">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6632c-145">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6632c-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="6632c-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers
```
# <a name="c"></a>[<span data-ttu-id="6632c-147">C#</span><span class="sxs-lookup"><span data-stu-id="6632c-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivemembers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6632c-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6632c-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivemembers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6632c-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6632c-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivemembers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6632c-150">Java</span><span class="sxs-lookup"><span data-stu-id="6632c-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-transitivemembers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="6632c-151">响应</span><span class="sxs-lookup"><span data-stu-id="6632c-151">Response</span></span>

<span data-ttu-id="6632c-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6632c-152">The following is an example of the response.</span></span>

><span data-ttu-id="6632c-153">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6632c-153">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-only-a-count-of-transitive-membership"></a><span data-ttu-id="6632c-154">示例 2：仅获取可传递成员身份的计数</span><span class="sxs-lookup"><span data-stu-id="6632c-154">Example 2: Get only a count of transitive membership</span></span>

#### <a name="request"></a><span data-ttu-id="6632c-155">请求</span><span class="sxs-lookup"><span data-stu-id="6632c-155">Request</span></span>

<span data-ttu-id="6632c-156">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6632c-156">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers_count"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="6632c-157">响应</span><span class="sxs-lookup"><span data-stu-id="6632c-157">Response</span></span>

<span data-ttu-id="6632c-158">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6632c-158">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

```

`893`


### <a name="example-3-use-the-microsoftgraphgroup-odata-cast-to-get-only-members-that-are-groups"></a><span data-ttu-id="6632c-159">示例 3：使用 microsoft.graph.group OData 转换仅获取作为组的成员</span><span class="sxs-lookup"><span data-stu-id="6632c-159">Example 3: Use the microsoft.graph.group OData cast to get only members that are groups</span></span>

#### <a name="request"></a><span data-ttu-id="6632c-160">请求</span><span class="sxs-lookup"><span data-stu-id="6632c-160">Request</span></span>

<span data-ttu-id="6632c-161">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6632c-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers_odataCast"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitivemembers/microsoft.graph.group?$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="6632c-162">响应</span><span class="sxs-lookup"><span data-stu-id="6632c-162">Response</span></span>

<span data-ttu-id="6632c-163">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6632c-163">The following is an example of the response.</span></span>

><span data-ttu-id="6632c-164">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6632c-164">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups",
  "@odata.count": 2,
  "value": [
    {
      "@odata.id": "https://graph.microsoft.com/v2/927c6607-8060-4f4a-a5f8-34964ac78d70/directoryObjects/4d0ef681-e88f-42a3-a2db-e6bf1e249e10/Microsoft.DirectoryServices.Group",
      "id": "4d0ef681-e88f-42a3-a2db-e6bf1e249e10",
      "organizationId": "927c6607-8060-4f4a-a5f8-34964ac78d70",
      "description": null,
      "displayName": "Executives",
      "groupTypes": [],
      "mail": "Executives@contoso.com",
      "mailEnabled": true,
      "mailNickname": "Executives",
    },
    {
      "@odata.id": "https://graph.microsoft.com/v2/927c6607-8060-4f4a-a5f8-34964ac78d70/directoryObjects/d9fb0c47-c783-40a1-bce1-53b52ada51fc/Microsoft.DirectoryServices.Group",
      "id": "d9fb0c47-c783-40a1-bce1-53b52ada51fc",
      "organizationId": "927c6607-8060-4f4a-a5f8-34964ac78d70",
      "displayName": "Project Falcon",
      "groupTypes": [],
      "mail": "Falcon@contoso.com",
      "mailEnabled": true,
      "mailNickname": "Falcon",
    }
  ]
}
```

### <a name="example-4-use-odata-cast-and-search-to-get-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="6632c-165">示例 4：使用 OData cast 和 $search 获取显示名称包含字母"tier"（包括返回对象计数）的组的成员身份</span><span class="sxs-lookup"><span data-stu-id="6632c-165">Example 4: Use OData cast and $search to get membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="6632c-166">请求</span><span class="sxs-lookup"><span data-stu-id="6632c-166">Request</span></span>

<span data-ttu-id="6632c-167">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6632c-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers/microsoft.graph.user?$count=true&$orderBy=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="6632c-168">响应</span><span class="sxs-lookup"><span data-stu-id="6632c-168">Response</span></span>

<span data-ttu-id="6632c-169">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6632c-169">The following is an example of the response.</span></span>
><span data-ttu-id="6632c-170">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6632c-170">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-5-use-odata-cast-and-filter-to-get-user-membership-in-groups-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="6632c-171">示例 5：使用 OData 强制转换$filter获取组的用户成员资格，组显示名称以"A"开头（包括返回的对象计数）</span><span class="sxs-lookup"><span data-stu-id="6632c-171">Example 5: Use OData cast and $filter to get user membership in groups with a display name that starts with 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="6632c-172">请求</span><span class="sxs-lookup"><span data-stu-id="6632c-172">Request</span></span>

<span data-ttu-id="6632c-173">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6632c-173">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers/microsoft.graph.user?$count=true&$orderBy=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="6632c-174">响应</span><span class="sxs-lookup"><span data-stu-id="6632c-174">Response</span></span>

<span data-ttu-id="6632c-175">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6632c-175">The following is an example of the response.</span></span>
><span data-ttu-id="6632c-176">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6632c-176">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "description": "List transitive group members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


