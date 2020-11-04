---
title: List group transitive members
description: 获取组成员的列表。 组可以将用户、设备、组织联系人和其他组作为成员。 此操作是可传递的，并返回所有嵌套成员的简单列表。
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 9566b3dea679b1b96566c4960e939079b8d89634
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904829"
---
# <a name="list-group-transitive-members"></a><span data-ttu-id="509d8-105">List group transitive members</span><span class="sxs-lookup"><span data-stu-id="509d8-105">List group transitive members</span></span>

<span data-ttu-id="509d8-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="509d8-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="509d8-107">获取组成员的列表。</span><span class="sxs-lookup"><span data-stu-id="509d8-107">Get a list of the group's members.</span></span> <span data-ttu-id="509d8-108">组可以将用户、设备、组织联系人和其他组作为成员。</span><span class="sxs-lookup"><span data-stu-id="509d8-108">A group can have users, devices, organizational contacts, and other groups as members.</span></span> <span data-ttu-id="509d8-109">此操作是可传递的，并返回所有嵌套成员的简单列表。</span><span class="sxs-lookup"><span data-stu-id="509d8-109">This operation is transitive and returns a flat list of all nested members.</span></span>

## <a name="permissions"></a><span data-ttu-id="509d8-110">权限</span><span class="sxs-lookup"><span data-stu-id="509d8-110">Permissions</span></span>

<span data-ttu-id="509d8-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="509d8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="509d8-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="509d8-113">Permission type</span></span>      | <span data-ttu-id="509d8-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="509d8-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="509d8-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="509d8-115">Delegated (work or school account)</span></span> | <span data-ttu-id="509d8-116">Directory.accessasuser.all、User.readbasic.all、User. all、User. all、Application、Read、all。 All</span><span class="sxs-lookup"><span data-stu-id="509d8-116">Directory.Read.All, Directory.AccessAsUser.All, User.ReadBasic.All, User.Read.All, Application.Read.All</span></span>  |
|<span data-ttu-id="509d8-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="509d8-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="509d8-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="509d8-118">Not supported.</span></span>    |
|<span data-ttu-id="509d8-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="509d8-119">Application</span></span> | <span data-ttu-id="509d8-120">Read. all、User. all、Application、Read. All</span><span class="sxs-lookup"><span data-stu-id="509d8-120">Directory.Read.All, User.Read.All, Application.Read.All</span></span> |

><span data-ttu-id="509d8-121">**注意：** 若要列出隐藏的成员资格组的成员，则需要使用 Read. Hidden 权限是必需的。</span><span class="sxs-lookup"><span data-stu-id="509d8-121">**Note:** To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="509d8-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="509d8-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/transitiveMembers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="509d8-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="509d8-123">Optional query parameters</span></span>

<span data-ttu-id="509d8-124">此方法支持[OData query parameters](/graph/query-parameters)以帮助自定义响应，包括 `$search`、`$count`、 和 `$filter`</span><span class="sxs-lookup"><span data-stu-id="509d8-124">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="509d8-125">可使用“ **displayName** ”和“ **说明** ”属性上的`$search`。</span><span class="sxs-lookup"><span data-stu-id="509d8-125">You can use `$search` on the **displayName** and **description** properties.</span></span> <span data-ttu-id="509d8-126">为该资源添加或更新项目时，将对它们进行专门索引，以便与 `$count` 和 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="509d8-126">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="509d8-127">在添加或更新项目与在索引中可用之间可能会稍有延迟。</span><span class="sxs-lookup"><span data-stu-id="509d8-127">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="509d8-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="509d8-128">Request headers</span></span>

| <span data-ttu-id="509d8-129">名称</span><span class="sxs-lookup"><span data-stu-id="509d8-129">Name</span></span> | <span data-ttu-id="509d8-130">说明</span><span class="sxs-lookup"><span data-stu-id="509d8-130">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="509d8-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="509d8-131">Authorization</span></span>  | <span data-ttu-id="509d8-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="509d8-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="509d8-134">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="509d8-134">ConsistencyLevel</span></span> | <span data-ttu-id="509d8-135">最终。</span><span class="sxs-lookup"><span data-stu-id="509d8-135">eventual.</span></span> <span data-ttu-id="509d8-136">使用 `$search`、`$filter`、`$orderby` 或 OData 强制转换查询参数时，此标头和 `$count` 是必需的。</span><span class="sxs-lookup"><span data-stu-id="509d8-136">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="509d8-137">它使用的索引可能与对象的最新更改不同步。</span><span class="sxs-lookup"><span data-stu-id="509d8-137">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="509d8-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="509d8-138">Request body</span></span>

<span data-ttu-id="509d8-139">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="509d8-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="509d8-140">响应</span><span class="sxs-lookup"><span data-stu-id="509d8-140">Response</span></span>

<span data-ttu-id="509d8-141">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="509d8-141">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="509d8-142">示例</span><span class="sxs-lookup"><span data-stu-id="509d8-142">Examples</span></span>

### <a name="example-1-get-the-transitive-membership-of-a-group"></a><span data-ttu-id="509d8-143">示例1：获取组的可传递成员身份</span><span class="sxs-lookup"><span data-stu-id="509d8-143">Example 1: Get the transitive membership of a group</span></span>

#### <a name="request"></a><span data-ttu-id="509d8-144">请求</span><span class="sxs-lookup"><span data-stu-id="509d8-144">Request</span></span>

<span data-ttu-id="509d8-145">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="509d8-145">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="509d8-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="509d8-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMembers
```
# <a name="c"></a>[<span data-ttu-id="509d8-147">C#</span><span class="sxs-lookup"><span data-stu-id="509d8-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivemembers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="509d8-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="509d8-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivemembers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="509d8-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="509d8-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivemembers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="509d8-150">Java</span><span class="sxs-lookup"><span data-stu-id="509d8-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-transitivemembers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="509d8-151">响应</span><span class="sxs-lookup"><span data-stu-id="509d8-151">Response</span></span>

<span data-ttu-id="509d8-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="509d8-152">The following is an example of the response.</span></span>

><span data-ttu-id="509d8-153">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="509d8-153">**Note** : The response object shown here might be shortened for readability.</span></span>

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
      "@odata.type": "#microsoft.graph.user",
      "id": "11111111-2222-3333-4444-555555555555",
      "mail": "group1@contoso.com"
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-transitive-membership"></a><span data-ttu-id="509d8-154">示例2：仅获取可传递成员身份的计数</span><span class="sxs-lookup"><span data-stu-id="509d8-154">Example 2: Get only a count of transitive membership</span></span>

#### <a name="request"></a><span data-ttu-id="509d8-155">请求</span><span class="sxs-lookup"><span data-stu-id="509d8-155">Request</span></span>

<span data-ttu-id="509d8-156">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="509d8-156">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="509d8-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="509d8-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers_count"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMembers/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="509d8-158">C#</span><span class="sxs-lookup"><span data-stu-id="509d8-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivemembers-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="509d8-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="509d8-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivemembers-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="509d8-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="509d8-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivemembers-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="509d8-161">Java</span><span class="sxs-lookup"><span data-stu-id="509d8-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-transitivemembers-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="509d8-162">响应</span><span class="sxs-lookup"><span data-stu-id="509d8-162">Response</span></span>

<span data-ttu-id="509d8-163">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="509d8-163">The following is an example of the response.</span></span>

><span data-ttu-id="509d8-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="509d8-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`893`

### <a name="example-3-use-odata-cast-and-search-to-get-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="509d8-166">示例3：使用 OData 强制转换和 $search 获取包含包含字母 "层" 的组的组成员身份，其中包括返回的对象的计数</span><span class="sxs-lookup"><span data-stu-id="509d8-166">Example 3: Use OData cast and $search to get membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="509d8-167">请求</span><span class="sxs-lookup"><span data-stu-id="509d8-167">Request</span></span>

<span data-ttu-id="509d8-168">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="509d8-168">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="509d8-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="509d8-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMembers/microsoft.graph.user?$count=true&$orderBy=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="509d8-170">C#</span><span class="sxs-lookup"><span data-stu-id="509d8-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tier-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="509d8-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="509d8-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tier-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="509d8-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="509d8-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tier-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="509d8-173">Java</span><span class="sxs-lookup"><span data-stu-id="509d8-173">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tier-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="509d8-174">响应</span><span class="sxs-lookup"><span data-stu-id="509d8-174">Response</span></span>

<span data-ttu-id="509d8-175">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="509d8-175">The following is an example of the response.</span></span>

><span data-ttu-id="509d8-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="509d8-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    }
  ]
}
```

### <a name="example-4-use-odata-cast-and-filter-to-get-user-membership-in-groups-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="509d8-178">示例4：使用 OData 强制转换和 $filter 获取显示名称以 "A" 开头的组中的用户成员，其中包含返回对象的计数</span><span class="sxs-lookup"><span data-stu-id="509d8-178">Example 4: Use OData cast and $filter to get user membership in groups with a display name that starts with 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="509d8-179">请求</span><span class="sxs-lookup"><span data-stu-id="509d8-179">Request</span></span>

<span data-ttu-id="509d8-180">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="509d8-180">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="509d8-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="509d8-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMembers/microsoft.graph.users?$count=true&$orderBy=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="509d8-182">C#</span><span class="sxs-lookup"><span data-stu-id="509d8-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="509d8-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="509d8-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="509d8-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="509d8-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="509d8-185">Java</span><span class="sxs-lookup"><span data-stu-id="509d8-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-a-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="509d8-186">响应</span><span class="sxs-lookup"><span data-stu-id="509d8-186">Response</span></span>

<span data-ttu-id="509d8-187">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="509d8-187">The following is an example of the response.</span></span>

><span data-ttu-id="509d8-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="509d8-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
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
  "description": "List transitive group members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
