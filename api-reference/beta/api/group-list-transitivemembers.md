---
title: List group transitive members
description: 获取组成员的列表。
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: ad0f2dbb064620d64b6abcda926775887bd0a4eb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47990856"
---
# <a name="list-group-transitive-members"></a><span data-ttu-id="be58c-103">List group transitive members</span><span class="sxs-lookup"><span data-stu-id="be58c-103">List group transitive members</span></span>

<span data-ttu-id="be58c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be58c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be58c-105">获取组成员的列表。</span><span class="sxs-lookup"><span data-stu-id="be58c-105">Get a list of the group's members.</span></span> <span data-ttu-id="be58c-106">组可以将用户、联系人、设备、服务主体和其他组作为成员。</span><span class="sxs-lookup"><span data-stu-id="be58c-106">A group can have users, contacts, devices, service principals, and other groups as members.</span></span> <span data-ttu-id="be58c-107">此操作是可传递的，并且还将返回所有嵌套成员的简单列表。</span><span class="sxs-lookup"><span data-stu-id="be58c-107">This operation is transitive and will also return a flat list of all nested members.</span></span>

## <a name="permissions"></a><span data-ttu-id="be58c-108">权限</span><span class="sxs-lookup"><span data-stu-id="be58c-108">Permissions</span></span>

<span data-ttu-id="be58c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="be58c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="be58c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="be58c-111">Permission type</span></span> | <span data-ttu-id="be58c-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="be58c-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="be58c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="be58c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="be58c-114">Directory.accessasuser.all、User.readbasic.all、用户、全部、用户、全部读取。所有</span><span class="sxs-lookup"><span data-stu-id="be58c-114">Directory.Read.All, Directory.AccessAsUser.All, User.ReadBasic.All, User.Read.All</span></span>    |
| <span data-ttu-id="be58c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="be58c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be58c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="be58c-116">Not supported.</span></span> |
| <span data-ttu-id="be58c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="be58c-117">Application</span></span> | <span data-ttu-id="be58c-118">Read. All，User. All</span><span class="sxs-lookup"><span data-stu-id="be58c-118">Directory.Read.All, User.Read.All</span></span> |

> <span data-ttu-id="be58c-119">**注意：** 若要列出隐藏的成员资格组的成员，则需要使用 Read. Hidden 权限是必需的。</span><span class="sxs-lookup"><span data-stu-id="be58c-119">**Note:** To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="be58c-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="be58c-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/transitiveMembers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="be58c-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="be58c-121">Optional query parameters</span></span>

<span data-ttu-id="be58c-122">此方法支持[OData query parameters](/graph/query_parameters)以帮助自定义响应，包括 `$search`、`$count`、 和 `$filter`</span><span class="sxs-lookup"><span data-stu-id="be58c-122">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="be58c-123">`$search`可以用在 **displayName**属性。</span><span class="sxs-lookup"><span data-stu-id="be58c-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="be58c-124">为该资源添加或更新项目时，将对它们进行专门索引，以便与 `$count` 和 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="be58c-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="be58c-125">在添加或更新项目与在索引中可用之间可能会稍有延迟。</span><span class="sxs-lookup"><span data-stu-id="be58c-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="be58c-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="be58c-126">Request headers</span></span>

| <span data-ttu-id="be58c-127">名称</span><span class="sxs-lookup"><span data-stu-id="be58c-127">Name</span></span> | <span data-ttu-id="be58c-128">说明</span><span class="sxs-lookup"><span data-stu-id="be58c-128">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="be58c-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="be58c-129">Authorization</span></span>  | <span data-ttu-id="be58c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="be58c-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="be58c-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="be58c-132">ConsistencyLevel</span></span> | <span data-ttu-id="be58c-133">最终。</span><span class="sxs-lookup"><span data-stu-id="be58c-133">eventual.</span></span> <span data-ttu-id="be58c-134">使用 `$search`、`$filter`、`$orderby` 或 OData 强制转换查询参数时，此标头和 `$count` 是必需的。</span><span class="sxs-lookup"><span data-stu-id="be58c-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="be58c-135">它使用的索引可能与对象的最新更改不同步。</span><span class="sxs-lookup"><span data-stu-id="be58c-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="be58c-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="be58c-136">Request body</span></span>

<span data-ttu-id="be58c-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="be58c-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be58c-138">响应</span><span class="sxs-lookup"><span data-stu-id="be58c-138">Response</span></span>

<span data-ttu-id="be58c-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="be58c-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="be58c-140">示例</span><span class="sxs-lookup"><span data-stu-id="be58c-140">Examples</span></span>

### <a name="example-1-get-the-transitive-membership-of-a-group"></a><span data-ttu-id="be58c-141">示例1：获取组的可传递成员身份</span><span class="sxs-lookup"><span data-stu-id="be58c-141">Example 1: Get the transitive membership of a group</span></span>

#### <a name="request"></a><span data-ttu-id="be58c-142">请求</span><span class="sxs-lookup"><span data-stu-id="be58c-142">Request</span></span>

<span data-ttu-id="be58c-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="be58c-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="be58c-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="be58c-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers
```
# <a name="c"></a>[<span data-ttu-id="be58c-145">C#</span><span class="sxs-lookup"><span data-stu-id="be58c-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivemembers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="be58c-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="be58c-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivemembers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="be58c-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="be58c-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivemembers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="be58c-148">响应</span><span class="sxs-lookup"><span data-stu-id="be58c-148">Response</span></span>

<span data-ttu-id="be58c-149">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="be58c-149">The following is an example of the response.</span></span>

><span data-ttu-id="be58c-150">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="be58c-150">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="be58c-151">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="be58c-151">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-transitive-membership"></a><span data-ttu-id="be58c-152">示例2：仅获取可传递成员身份的计数</span><span class="sxs-lookup"><span data-stu-id="be58c-152">Example 2: Get only a count of transitive membership</span></span>

#### <a name="request"></a><span data-ttu-id="be58c-153">请求</span><span class="sxs-lookup"><span data-stu-id="be58c-153">Request</span></span>

<span data-ttu-id="be58c-154">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="be58c-154">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="be58c-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="be58c-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers_count"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="be58c-156">C#</span><span class="sxs-lookup"><span data-stu-id="be58c-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivemembers-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="be58c-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="be58c-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivemembers-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="be58c-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="be58c-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivemembers-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="be58c-159">响应</span><span class="sxs-lookup"><span data-stu-id="be58c-159">Response</span></span>

<span data-ttu-id="be58c-160">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="be58c-160">The following is an example of the response.</span></span>
><span data-ttu-id="be58c-161">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="be58c-161">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="be58c-162">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="be58c-162">All the properties will be returned from an actual call.</span></span>

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

<span data-ttu-id="be58c-163">893</span><span class="sxs-lookup"><span data-stu-id="be58c-163">893</span></span>


### <a name="example-3-use-odata-cast-and-search-to-get-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="be58c-164">示例3：使用 OData 强制转换和 $search 获取包含包含字母 "层" 的组的组成员身份，其中包括返回的对象的计数</span><span class="sxs-lookup"><span data-stu-id="be58c-164">Example 3: Use OData cast and $search to get membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="be58c-165">请求</span><span class="sxs-lookup"><span data-stu-id="be58c-165">Request</span></span>

<span data-ttu-id="be58c-166">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="be58c-166">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="be58c-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="be58c-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers/microsoft.graph.user?$count=true&$orderBy=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="be58c-168">C#</span><span class="sxs-lookup"><span data-stu-id="be58c-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tier-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="be58c-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="be58c-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tier-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="be58c-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="be58c-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tier-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="be58c-171">响应</span><span class="sxs-lookup"><span data-stu-id="be58c-171">Response</span></span>

<span data-ttu-id="be58c-172">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="be58c-172">The following is an example of the response.</span></span>
><span data-ttu-id="be58c-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="be58c-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-4-use-odata-cast-and-filter-to-get-user-membership-in-groups-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="be58c-175">示例4：使用 OData 强制转换和 $filter 获取显示名称以 "A" 开头的组中的用户成员，其中包含返回对象的计数</span><span class="sxs-lookup"><span data-stu-id="be58c-175">Example 4: Use OData cast and $filter to get user membership in groups with a display name that starts with 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="be58c-176">请求</span><span class="sxs-lookup"><span data-stu-id="be58c-176">Request</span></span>

<span data-ttu-id="be58c-177">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="be58c-177">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="be58c-178">HTTP</span><span class="sxs-lookup"><span data-stu-id="be58c-178">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers/microsoft.graph.users?$count=true&$orderBy=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="be58c-179">C#</span><span class="sxs-lookup"><span data-stu-id="be58c-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="be58c-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="be58c-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="be58c-181">Objective-C</span><span class="sxs-lookup"><span data-stu-id="be58c-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="be58c-182">响应</span><span class="sxs-lookup"><span data-stu-id="be58c-182">Response</span></span>

<span data-ttu-id="be58c-183">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="be58c-183">The following is an example of the response.</span></span>
><span data-ttu-id="be58c-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="be58c-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


