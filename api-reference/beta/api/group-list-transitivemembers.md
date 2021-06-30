---
title: List group transitive members
description: 获取组的成员列表。
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 596bdaf0ba02046465cb2456f4c2c88e935f31d4
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207172"
---
# <a name="list-group-transitive-members"></a><span data-ttu-id="3aa39-103">List group transitive members</span><span class="sxs-lookup"><span data-stu-id="3aa39-103">List group transitive members</span></span>

<span data-ttu-id="3aa39-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3aa39-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3aa39-105">获取组的成员列表。</span><span class="sxs-lookup"><span data-stu-id="3aa39-105">Get a list of the group's members.</span></span> <span data-ttu-id="3aa39-106">组可以将用户、联系人、设备、服务主体和其他组作为成员。</span><span class="sxs-lookup"><span data-stu-id="3aa39-106">A group can have users, contacts, devices, service principals, and other groups as members.</span></span> <span data-ttu-id="3aa39-107">此操作是可传递的，并且还将返回简单列表嵌套成员的成员。</span><span class="sxs-lookup"><span data-stu-id="3aa39-107">This operation is transitive and will also return a flat list of all nested members.</span></span>

## <a name="permissions"></a><span data-ttu-id="3aa39-108">权限</span><span class="sxs-lookup"><span data-stu-id="3aa39-108">Permissions</span></span>

<span data-ttu-id="3aa39-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3aa39-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3aa39-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3aa39-111">Permission type</span></span> | <span data-ttu-id="3aa39-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3aa39-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="3aa39-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3aa39-113">Delegated (work or school account)</span></span> | <span data-ttu-id="3aa39-114">GroupMember.Read.All，Group.Read.All，GroupMember.ReadWrite.All，Group.ReadWrite.All，Directory.Read.All，Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3aa39-114">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
| <span data-ttu-id="3aa39-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3aa39-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3aa39-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3aa39-116">Not supported.</span></span> |
| <span data-ttu-id="3aa39-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3aa39-117">Application</span></span> | <span data-ttu-id="3aa39-118">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="3aa39-118">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All</span></span> |

> <span data-ttu-id="3aa39-119">**注意：** 若要列出隐藏成员资格组的成员， *需要 Member.Read.Hidden* 权限。</span><span class="sxs-lookup"><span data-stu-id="3aa39-119">**Note:** To list the members of a hidden membership group, the *Member.Read.Hidden* permission is required.</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="3aa39-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3aa39-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/transitiveMembers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3aa39-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3aa39-121">Optional query parameters</span></span>

<span data-ttu-id="3aa39-122">此方法支持[OData query parameters](/graph/query-parameters)以帮助自定义响应，包括 `$search`、`$count`、 和 `$filter`</span><span class="sxs-lookup"><span data-stu-id="3aa39-122">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="3aa39-123">可使用“**displayName**”和“**说明**”属性上的`$search`。</span><span class="sxs-lookup"><span data-stu-id="3aa39-123">You can use `$search` on the **displayName** and **description** properties.</span></span> <span data-ttu-id="3aa39-124">为该资源添加或更新项目时，将对它们进行专门索引，以便与 `$count` 和 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="3aa39-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="3aa39-125">在添加或更新项目与在索引中可用之间可能会稍有延迟。</span><span class="sxs-lookup"><span data-stu-id="3aa39-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

<span data-ttu-id="3aa39-126">若要筛选 OData 类型（如 或 ）上的结果， `microsoft.graph.user` `microsoft.graph.group` 必须使用 [高级查询参数](/graph/aad-advanced-queries)。</span><span class="sxs-lookup"><span data-stu-id="3aa39-126">To filter the results on the OData type, such as `microsoft.graph.user` or `microsoft.graph.group`, you must use the [advanced query parameters](/graph/aad-advanced-queries).</span></span> <span data-ttu-id="3aa39-127">即，将 **ConsistencyLevel** 标头设置为 `eventual` 和 `$count=true` 查询字符串。</span><span class="sxs-lookup"><span data-stu-id="3aa39-127">That is, the **ConsistencyLevel** header set to `eventual` and the `$count=true` query string.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3aa39-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="3aa39-128">Request headers</span></span>

| <span data-ttu-id="3aa39-129">名称</span><span class="sxs-lookup"><span data-stu-id="3aa39-129">Name</span></span> | <span data-ttu-id="3aa39-130">说明</span><span class="sxs-lookup"><span data-stu-id="3aa39-130">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="3aa39-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="3aa39-131">Authorization</span></span>  | <span data-ttu-id="3aa39-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3aa39-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3aa39-134">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="3aa39-134">ConsistencyLevel</span></span> | <span data-ttu-id="3aa39-135">最终。</span><span class="sxs-lookup"><span data-stu-id="3aa39-135">eventual.</span></span> <span data-ttu-id="3aa39-136">使用 `$search`、`$filter`、`$orderby` 或 OData 强制转换查询参数时，此标头和 `$count` 是必需的。</span><span class="sxs-lookup"><span data-stu-id="3aa39-136">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="3aa39-137">它使用的索引可能与对象的最新更改不同步。</span><span class="sxs-lookup"><span data-stu-id="3aa39-137">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3aa39-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="3aa39-138">Request body</span></span>

<span data-ttu-id="3aa39-139">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3aa39-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3aa39-140">响应</span><span class="sxs-lookup"><span data-stu-id="3aa39-140">Response</span></span>

<span data-ttu-id="3aa39-141">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="3aa39-141">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3aa39-142">示例</span><span class="sxs-lookup"><span data-stu-id="3aa39-142">Examples</span></span>

### <a name="example-1-get-the-transitive-membership-of-a-group"></a><span data-ttu-id="3aa39-143">示例 1：获取组的可传递成员身份</span><span class="sxs-lookup"><span data-stu-id="3aa39-143">Example 1: Get the transitive membership of a group</span></span>

#### <a name="request"></a><span data-ttu-id="3aa39-144">请求</span><span class="sxs-lookup"><span data-stu-id="3aa39-144">Request</span></span>

<span data-ttu-id="3aa39-145">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3aa39-145">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3aa39-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="3aa39-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers
```
# <a name="c"></a>[<span data-ttu-id="3aa39-147">C#</span><span class="sxs-lookup"><span data-stu-id="3aa39-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivemembers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3aa39-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3aa39-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivemembers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3aa39-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3aa39-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivemembers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3aa39-150">Java</span><span class="sxs-lookup"><span data-stu-id="3aa39-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-transitivemembers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="3aa39-151">响应</span><span class="sxs-lookup"><span data-stu-id="3aa39-151">Response</span></span>

<span data-ttu-id="3aa39-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3aa39-152">The following is an example of the response.</span></span>

><span data-ttu-id="3aa39-153">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3aa39-153">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-only-a-count-of-transitive-membership"></a><span data-ttu-id="3aa39-154">示例 2：仅获取可传递成员身份的计数</span><span class="sxs-lookup"><span data-stu-id="3aa39-154">Example 2: Get only a count of transitive membership</span></span>

#### <a name="request"></a><span data-ttu-id="3aa39-155">请求</span><span class="sxs-lookup"><span data-stu-id="3aa39-155">Request</span></span>

<span data-ttu-id="3aa39-156">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3aa39-156">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3aa39-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="3aa39-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "ignored",
  "name": "get_group_transitivemembers_count"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="3aa39-158">C#</span><span class="sxs-lookup"><span data-stu-id="3aa39-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivemembers-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3aa39-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3aa39-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivemembers-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3aa39-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3aa39-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivemembers-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3aa39-161">Java</span><span class="sxs-lookup"><span data-stu-id="3aa39-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-transitivemembers-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3aa39-162">响应</span><span class="sxs-lookup"><span data-stu-id="3aa39-162">Response</span></span>

<span data-ttu-id="3aa39-163">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3aa39-163">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

893
```


### <a name="example-3-use-the-microsoftgraphgroup-odata-cast-to-get-only-members-that-are-groups"></a><span data-ttu-id="3aa39-164">示例 3：使用 microsoft.graph.group OData 转换仅获取作为组的成员</span><span class="sxs-lookup"><span data-stu-id="3aa39-164">Example 3: Use the microsoft.graph.group OData cast to get only members that are groups</span></span>

#### <a name="request"></a><span data-ttu-id="3aa39-165">请求</span><span class="sxs-lookup"><span data-stu-id="3aa39-165">Request</span></span>

<span data-ttu-id="3aa39-166">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3aa39-166">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3aa39-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="3aa39-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers_odataCast"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitivemembers/microsoft.graph.group?$count=true
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="3aa39-168">C#</span><span class="sxs-lookup"><span data-stu-id="3aa39-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivemembers-odatacast-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3aa39-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3aa39-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivemembers-odatacast-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3aa39-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3aa39-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivemembers-odatacast-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3aa39-171">Java</span><span class="sxs-lookup"><span data-stu-id="3aa39-171">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-transitivemembers-odatacast-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3aa39-172">响应</span><span class="sxs-lookup"><span data-stu-id="3aa39-172">Response</span></span>

<span data-ttu-id="3aa39-173">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3aa39-173">The following is an example of the response.</span></span>

><span data-ttu-id="3aa39-174">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3aa39-174">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-4-use-odata-cast-and-search-to-get-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="3aa39-175">示例 4：使用 OData cast 和 $search 获取显示名称包含字母"tier"（包括返回对象计数）的组的成员身份</span><span class="sxs-lookup"><span data-stu-id="3aa39-175">Example 4: Use OData cast and $search to get membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="3aa39-176">请求</span><span class="sxs-lookup"><span data-stu-id="3aa39-176">Request</span></span>

<span data-ttu-id="3aa39-177">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3aa39-177">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3aa39-178">HTTP</span><span class="sxs-lookup"><span data-stu-id="3aa39-178">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers/microsoft.graph.user?$count=true&$orderBy=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="3aa39-179">C#</span><span class="sxs-lookup"><span data-stu-id="3aa39-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tier-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3aa39-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3aa39-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tier-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3aa39-181">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3aa39-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tier-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3aa39-182">Java</span><span class="sxs-lookup"><span data-stu-id="3aa39-182">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tier-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3aa39-183">响应</span><span class="sxs-lookup"><span data-stu-id="3aa39-183">Response</span></span>

<span data-ttu-id="3aa39-184">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3aa39-184">The following is an example of the response.</span></span>
><span data-ttu-id="3aa39-185">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3aa39-185">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-5-use-odata-cast-and-filter-to-get-user-membership-in-groups-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="3aa39-186">示例 5：使用 OData 强制转换$filter获取组的用户成员资格，组显示名称以"A"开头（包括返回的对象计数）</span><span class="sxs-lookup"><span data-stu-id="3aa39-186">Example 5: Use OData cast and $filter to get user membership in groups with a display name that starts with 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="3aa39-187">请求</span><span class="sxs-lookup"><span data-stu-id="3aa39-187">Request</span></span>

<span data-ttu-id="3aa39-188">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3aa39-188">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3aa39-189">HTTP</span><span class="sxs-lookup"><span data-stu-id="3aa39-189">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers/microsoft.graph.user?$count=true&$orderBy=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="3aa39-190">C#</span><span class="sxs-lookup"><span data-stu-id="3aa39-190">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3aa39-191">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3aa39-191">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3aa39-192">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3aa39-192">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3aa39-193">Java</span><span class="sxs-lookup"><span data-stu-id="3aa39-193">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-a-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3aa39-194">响应</span><span class="sxs-lookup"><span data-stu-id="3aa39-194">Response</span></span>

<span data-ttu-id="3aa39-195">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3aa39-195">The following is an example of the response.</span></span>
><span data-ttu-id="3aa39-196">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3aa39-196">**Note:** The response object shown here might be shortened for readability.</span></span>

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


