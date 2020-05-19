---
title: 列表组可传递的 memberOf
description: 获取组所属的组和管理单元。
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 268b1c5dbdf8678fca96fec6e5de9fcda52b9fb2
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289614"
---
# <a name="list-group-transitive-memberof"></a><span data-ttu-id="40ada-103">列表组可传递的 memberOf</span><span class="sxs-lookup"><span data-stu-id="40ada-103">List group transitive memberOf</span></span>

<span data-ttu-id="40ada-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40ada-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40ada-105">获取组所属的组和管理单元。</span><span class="sxs-lookup"><span data-stu-id="40ada-105">Get groups and administrative units that the group is a member of.</span></span>  <span data-ttu-id="40ada-106">此操作是可传递的，还将包括此组嵌套成员的所有组。</span><span class="sxs-lookup"><span data-stu-id="40ada-106">This operation is transitive and will also include all groups that this groups is a nested member of.</span></span> <span data-ttu-id="40ada-107">与获取用户的 Office 365 组不同，这将返回所有类型的组，而不只是 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="40ada-107">Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 Groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="40ada-108">权限</span><span class="sxs-lookup"><span data-stu-id="40ada-108">Permissions</span></span>

<span data-ttu-id="40ada-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="40ada-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="40ada-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="40ada-111">Permission type</span></span> | <span data-ttu-id="40ada-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="40ada-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="40ada-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="40ada-113">Delegated (work or school account)</span></span> | <span data-ttu-id="40ada-114">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="40ada-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
| <span data-ttu-id="40ada-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="40ada-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40ada-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="40ada-116">Not supported.</span></span> |
| <span data-ttu-id="40ada-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="40ada-117">Application</span></span> | <span data-ttu-id="40ada-118">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40ada-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="40ada-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="40ada-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="40ada-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="40ada-120">Optional query parameters</span></span>

<span data-ttu-id="40ada-121">此方法支持[OData 查询参数](/graph/query_parameters)，以帮助自定义响应，包括 `$search` 、 `$count` 和 `$filter` 。</span><span class="sxs-lookup"><span data-stu-id="40ada-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="40ada-122">此外，还会启用 OData 强制转换，例如，您可以强制转换以仅获取组的可传递组成员。</span><span class="sxs-lookup"><span data-stu-id="40ada-122">OData cast is also enabled, for example, you can cast to get just the transitive group members of a group.</span></span> <span data-ttu-id="40ada-123">您可以 `$search` 在**displayName**属性上使用。</span><span class="sxs-lookup"><span data-stu-id="40ada-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="40ada-124">为此资源添加或更新项目时，将对其进行专门编制索引，以便 `$count` 与 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="40ada-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="40ada-125">在添加或更新项目以及在索引中可用时，可能会出现轻微的延迟。</span><span class="sxs-lookup"><span data-stu-id="40ada-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="40ada-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="40ada-126">Request headers</span></span>

| <span data-ttu-id="40ada-127">名称</span><span class="sxs-lookup"><span data-stu-id="40ada-127">Name</span></span> | <span data-ttu-id="40ada-128">说明</span><span class="sxs-lookup"><span data-stu-id="40ada-128">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="40ada-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="40ada-129">Authorization</span></span>  | <span data-ttu-id="40ada-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="40ada-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="40ada-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="40ada-132">ConsistencyLevel</span></span> | <span data-ttu-id="40ada-133">仍然.</span><span class="sxs-lookup"><span data-stu-id="40ada-133">eventual.</span></span> <span data-ttu-id="40ada-134">在 `$count` 使用 `$search` 、 `$filter` 、 `$orderby` 或 OData 转换查询参数时，此标头和是必需的。</span><span class="sxs-lookup"><span data-stu-id="40ada-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="40ada-135">它使用的索引可能不是最新的，并包含对对象的最新更改。</span><span class="sxs-lookup"><span data-stu-id="40ada-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="40ada-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="40ada-136">Request body</span></span>

<span data-ttu-id="40ada-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="40ada-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40ada-138">响应</span><span class="sxs-lookup"><span data-stu-id="40ada-138">Response</span></span>

<span data-ttu-id="40ada-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="40ada-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="40ada-140">示例</span><span class="sxs-lookup"><span data-stu-id="40ada-140">Examples</span></span>

### <a name="example-1-get-groups-and-administrative-units-that-the-group-is-a-transitive-member-of"></a><span data-ttu-id="40ada-141">示例1：获取组是该组的可传递成员的组和管理单元</span><span class="sxs-lookup"><span data-stu-id="40ada-141">Example 1: Get groups and administrative units that the group is a transitive member of</span></span>

#### <a name="request"></a><span data-ttu-id="40ada-142">请求</span><span class="sxs-lookup"><span data-stu-id="40ada-142">Request</span></span>

<span data-ttu-id="40ada-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="40ada-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="40ada-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="40ada-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="40ada-145">C#</span><span class="sxs-lookup"><span data-stu-id="40ada-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="40ada-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="40ada-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="40ada-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="40ada-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="40ada-148">响应</span><span class="sxs-lookup"><span data-stu-id="40ada-148">Response</span></span>

<span data-ttu-id="40ada-149">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="40ada-149">The following is an example of the response.</span></span>
><span data-ttu-id="40ada-150">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="40ada-150">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="40ada-151">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="40ada-151">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-all-transitive-membership"></a><span data-ttu-id="40ada-152">示例2：仅获取所有可传递成员身份的计数</span><span class="sxs-lookup"><span data-stu-id="40ada-152">Example 2: Get only a count of all transitive membership</span></span>

#### <a name="request"></a><span data-ttu-id="40ada-153">请求</span><span class="sxs-lookup"><span data-stu-id="40ada-153">Request</span></span>

<span data-ttu-id="40ada-154">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="40ada-154">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="40ada-155">响应</span><span class="sxs-lookup"><span data-stu-id="40ada-155">Response</span></span>

<span data-ttu-id="40ada-156">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="40ada-156">The following is an example of the response.</span></span>

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

<span data-ttu-id="40ada-157">294</span><span class="sxs-lookup"><span data-stu-id="40ada-157">294</span></span>

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-transitive-membership-in-groups"></a><span data-ttu-id="40ada-158">示例3：使用 OData 强制转换仅获取组中的可传递成员身份数</span><span class="sxs-lookup"><span data-stu-id="40ada-158">Example 3: Use OData cast to get only a count of transitive membership in groups</span></span>

#### <a name="request"></a><span data-ttu-id="40ada-159">请求</span><span class="sxs-lookup"><span data-stu-id="40ada-159">Request</span></span>

<span data-ttu-id="40ada-160">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="40ada-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="40ada-161">响应</span><span class="sxs-lookup"><span data-stu-id="40ada-161">Response</span></span>

<span data-ttu-id="40ada-162">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="40ada-162">The following is an example of the response.</span></span>

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

<span data-ttu-id="40ada-163">294</span><span class="sxs-lookup"><span data-stu-id="40ada-163">294</span></span>


### <a name="example-4-use-odata-cast-and-search-to-get-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="40ada-164">示例4：使用 OData 强制转换和 $search 获取包含包含字母 "层" 的组的组成员身份，其中包括返回的对象的计数</span><span class="sxs-lookup"><span data-stu-id="40ada-164">Example 4: Use OData cast and $search to get membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="40ada-165">请求</span><span class="sxs-lookup"><span data-stu-id="40ada-165">Request</span></span>

<span data-ttu-id="40ada-166">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="40ada-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="40ada-167">响应</span><span class="sxs-lookup"><span data-stu-id="40ada-167">Response</span></span>

<span data-ttu-id="40ada-168">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="40ada-168">The following is an example of the response.</span></span>
><span data-ttu-id="40ada-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="40ada-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-5-use-odata-cast-and-filter-to-get-membership-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="40ada-171">示例5：使用 OData 强制转换和 $filter 获取显示名称以 "A" 开头的成员身份，其中包含返回对象的计数</span><span class="sxs-lookup"><span data-stu-id="40ada-171">Example 5: Use OData cast and $filter to get membership with a display name that starts with 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="40ada-172">请求</span><span class="sxs-lookup"><span data-stu-id="40ada-172">Request</span></span>

<span data-ttu-id="40ada-173">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="40ada-173">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="40ada-174">响应</span><span class="sxs-lookup"><span data-stu-id="40ada-174">Response</span></span>

<span data-ttu-id="40ada-175">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="40ada-175">The following is an example of the response.</span></span>
><span data-ttu-id="40ada-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="40ada-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
