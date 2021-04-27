---
title: List group transitive memberOf
description: 获取组是该组的一个成员的组和管理单元。
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: a5225c10540c2f142eb25249100e4a49751471ff
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52041399"
---
# <a name="list-group-transitive-memberof"></a><span data-ttu-id="4ec5a-103">List group transitive memberOf</span><span class="sxs-lookup"><span data-stu-id="4ec5a-103">List group transitive memberOf</span></span>

<span data-ttu-id="4ec5a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ec5a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ec5a-105">获取组是该组的一个成员的组和管理单元。</span><span class="sxs-lookup"><span data-stu-id="4ec5a-105">Get groups and administrative units that the group is a member of.</span></span>  <span data-ttu-id="4ec5a-106">此操作是可传递的，并且还将包含此组是嵌套成员的所有组。</span><span class="sxs-lookup"><span data-stu-id="4ec5a-106">This operation is transitive and will also include all groups that this groups is a nested member of.</span></span> <span data-ttu-id="4ec5a-107">与获取用户的组Microsoft 365不同，这将返回所有类型的组，而不只是Microsoft 365组。</span><span class="sxs-lookup"><span data-stu-id="4ec5a-107">Unlike getting a user's Microsoft 365 groups, this returns all types of groups, not just Microsoft 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="4ec5a-108">权限</span><span class="sxs-lookup"><span data-stu-id="4ec5a-108">Permissions</span></span>

<span data-ttu-id="4ec5a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4ec5a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4ec5a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4ec5a-111">Permission type</span></span> | <span data-ttu-id="4ec5a-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4ec5a-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="4ec5a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4ec5a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="4ec5a-114">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4ec5a-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
| <span data-ttu-id="4ec5a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4ec5a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ec5a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4ec5a-116">Not supported.</span></span> |
| <span data-ttu-id="4ec5a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="4ec5a-117">Application</span></span> | <span data-ttu-id="4ec5a-118">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ec5a-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="4ec5a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4ec5a-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4ec5a-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4ec5a-120">Optional query parameters</span></span>

<span data-ttu-id="4ec5a-121">此方法支持[OData query parameters](/graph/query_parameters)以帮助自定义响应，包括 `$search`、`$count`、 和 `$filter`</span><span class="sxs-lookup"><span data-stu-id="4ec5a-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="4ec5a-122">此外，还启用了 OData 转换，例如，您可以转换以仅获取组的可传递的组成员。</span><span class="sxs-lookup"><span data-stu-id="4ec5a-122">OData cast is also enabled, for example, you can cast to get just the transitive group members of a group.</span></span> <span data-ttu-id="4ec5a-123">`$search`可以用在 **displayName** 属性。</span><span class="sxs-lookup"><span data-stu-id="4ec5a-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="4ec5a-124">为该资源添加或更新项目时，将对它们进行专门索引，以便与 `$count` 和 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="4ec5a-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="4ec5a-125">在添加或更新项目与在索引中可用之间可能会稍有延迟。</span><span class="sxs-lookup"><span data-stu-id="4ec5a-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4ec5a-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="4ec5a-126">Request headers</span></span>

| <span data-ttu-id="4ec5a-127">名称</span><span class="sxs-lookup"><span data-stu-id="4ec5a-127">Name</span></span> | <span data-ttu-id="4ec5a-128">说明</span><span class="sxs-lookup"><span data-stu-id="4ec5a-128">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="4ec5a-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ec5a-129">Authorization</span></span>  | <span data-ttu-id="4ec5a-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4ec5a-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4ec5a-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="4ec5a-132">ConsistencyLevel</span></span> | <span data-ttu-id="4ec5a-133">最终。</span><span class="sxs-lookup"><span data-stu-id="4ec5a-133">eventual.</span></span> <span data-ttu-id="4ec5a-134">使用 `$search`、`$filter`、`$orderby` 或 OData 强制转换查询参数时，此标头和 `$count` 是必需的。</span><span class="sxs-lookup"><span data-stu-id="4ec5a-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="4ec5a-135">它使用的索引可能与对象的最新更改不同步。</span><span class="sxs-lookup"><span data-stu-id="4ec5a-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4ec5a-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="4ec5a-136">Request body</span></span>

<span data-ttu-id="4ec5a-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4ec5a-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ec5a-138">响应</span><span class="sxs-lookup"><span data-stu-id="4ec5a-138">Response</span></span>

<span data-ttu-id="4ec5a-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="4ec5a-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4ec5a-140">示例</span><span class="sxs-lookup"><span data-stu-id="4ec5a-140">Examples</span></span>

### <a name="example-1-get-groups-and-administrative-units-that-the-group-is-a-transitive-member-of"></a><span data-ttu-id="4ec5a-141">示例 1：获取组是其可传递成员组和管理单元</span><span class="sxs-lookup"><span data-stu-id="4ec5a-141">Example 1: Get groups and administrative units that the group is a transitive member of</span></span>

#### <a name="request"></a><span data-ttu-id="4ec5a-142">请求</span><span class="sxs-lookup"><span data-stu-id="4ec5a-142">Request</span></span>

<span data-ttu-id="4ec5a-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4ec5a-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4ec5a-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="4ec5a-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="4ec5a-145">C#</span><span class="sxs-lookup"><span data-stu-id="4ec5a-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4ec5a-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4ec5a-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4ec5a-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4ec5a-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4ec5a-148">Java</span><span class="sxs-lookup"><span data-stu-id="4ec5a-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-transitivememberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="4ec5a-149">响应</span><span class="sxs-lookup"><span data-stu-id="4ec5a-149">Response</span></span>

<span data-ttu-id="4ec5a-150">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4ec5a-150">The following is an example of the response.</span></span>
><span data-ttu-id="4ec5a-151">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4ec5a-151">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-only-a-count-of-all-transitive-membership"></a><span data-ttu-id="4ec5a-152">示例 2：仅获取所有可传递成员身份的计数</span><span class="sxs-lookup"><span data-stu-id="4ec5a-152">Example 2: Get only a count of all transitive membership</span></span>

#### <a name="request"></a><span data-ttu-id="4ec5a-153">请求</span><span class="sxs-lookup"><span data-stu-id="4ec5a-153">Request</span></span>

<span data-ttu-id="4ec5a-154">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4ec5a-154">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="4ec5a-155">响应</span><span class="sxs-lookup"><span data-stu-id="4ec5a-155">Response</span></span>

<span data-ttu-id="4ec5a-156">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4ec5a-156">The following is an example of the response.</span></span>

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

<span data-ttu-id="4ec5a-157">294</span><span class="sxs-lookup"><span data-stu-id="4ec5a-157">294</span></span>

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-transitive-membership-in-groups"></a><span data-ttu-id="4ec5a-158">示例 3：使用 OData 强制转换以仅获取组中可传递成员身份的计数</span><span class="sxs-lookup"><span data-stu-id="4ec5a-158">Example 3: Use OData cast to get only a count of transitive membership in groups</span></span>

#### <a name="request"></a><span data-ttu-id="4ec5a-159">请求</span><span class="sxs-lookup"><span data-stu-id="4ec5a-159">Request</span></span>

<span data-ttu-id="4ec5a-160">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4ec5a-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="4ec5a-161">响应</span><span class="sxs-lookup"><span data-stu-id="4ec5a-161">Response</span></span>

<span data-ttu-id="4ec5a-162">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4ec5a-162">The following is an example of the response.</span></span>

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

<span data-ttu-id="4ec5a-163">294</span><span class="sxs-lookup"><span data-stu-id="4ec5a-163">294</span></span>


### <a name="example-4-use-odata-cast-and-search-to-get-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="4ec5a-164">示例 4：使用 OData cast 和 $search 获取显示名称包含字母"tier"（包括返回对象计数）的组的成员身份</span><span class="sxs-lookup"><span data-stu-id="4ec5a-164">Example 4: Use OData cast and $search to get membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="4ec5a-165">请求</span><span class="sxs-lookup"><span data-stu-id="4ec5a-165">Request</span></span>

<span data-ttu-id="4ec5a-166">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4ec5a-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="4ec5a-167">响应</span><span class="sxs-lookup"><span data-stu-id="4ec5a-167">Response</span></span>

<span data-ttu-id="4ec5a-168">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4ec5a-168">The following is an example of the response.</span></span>
><span data-ttu-id="4ec5a-169">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4ec5a-169">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-5-use-odata-cast-and-filter-to-get-membership-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="4ec5a-170">示例 5：使用 OData 转换$filter获取以"A"开头显示名称（包括返回对象计数）的组成员身份</span><span class="sxs-lookup"><span data-stu-id="4ec5a-170">Example 5: Use OData cast and $filter to get membership with a display name that starts with 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="4ec5a-171">请求</span><span class="sxs-lookup"><span data-stu-id="4ec5a-171">Request</span></span>

<span data-ttu-id="4ec5a-172">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4ec5a-172">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="4ec5a-173">响应</span><span class="sxs-lookup"><span data-stu-id="4ec5a-173">Response</span></span>

<span data-ttu-id="4ec5a-174">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4ec5a-174">The following is an example of the response.</span></span>
><span data-ttu-id="4ec5a-175">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4ec5a-175">**Note:** The response object shown here might be shortened for readability.</span></span>

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


