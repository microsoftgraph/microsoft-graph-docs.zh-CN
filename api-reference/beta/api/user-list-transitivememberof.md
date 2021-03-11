---
title: List user transitive memberOf
description: 获取用户是其中一个成员的组、目录角色和管理单元。 此 API 请求是可传递的，并且还将返回用户是嵌套成员的所有组。
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 20d2a8b0384a3c346a0f1f3f9f1a8b66cd9a6bfa
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720723"
---
# <a name="list-user-transitive-memberof"></a><span data-ttu-id="01f73-104">List user transitive memberOf</span><span class="sxs-lookup"><span data-stu-id="01f73-104">List user transitive memberOf</span></span>

<span data-ttu-id="01f73-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01f73-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01f73-106">获取用户是其中一个成员的组、目录角色和管理单元。</span><span class="sxs-lookup"><span data-stu-id="01f73-106">Get groups, directory roles and administrative units that the user is a member of.</span></span> <span data-ttu-id="01f73-107">此 API 请求是可传递的，并且还将返回用户是嵌套成员的所有组。</span><span class="sxs-lookup"><span data-stu-id="01f73-107">This API request is transitive, and will also return all groups the user is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="01f73-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="01f73-108">Permissions</span></span>

<span data-ttu-id="01f73-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="01f73-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="01f73-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="01f73-111">Permission type</span></span> | <span data-ttu-id="01f73-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="01f73-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="01f73-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="01f73-113">Delegated (work or school account)</span></span> | <span data-ttu-id="01f73-114">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="01f73-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
| <span data-ttu-id="01f73-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="01f73-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01f73-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="01f73-116">Not supported.</span></span> |
| <span data-ttu-id="01f73-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="01f73-117">Application</span></span> | <span data-ttu-id="01f73-118">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01f73-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="01f73-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="01f73-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id | userPrincipalName}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="01f73-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="01f73-120">Optional query parameters</span></span>

<span data-ttu-id="01f73-121">此方法支持[OData query parameters](/graph/query_parameters)以帮助自定义响应，包括 `$search`、`$count`、 和 `$filter`</span><span class="sxs-lookup"><span data-stu-id="01f73-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="01f73-122">例如，还可以启用 OData 转换，以仅获取组的可传递成员身份。</span><span class="sxs-lookup"><span data-stu-id="01f73-122">OData cast is also enabled, for example, you can cast to get just the transitive membership in groups.</span></span> <span data-ttu-id="01f73-123">`$search`可以用在 **displayName** 属性。</span><span class="sxs-lookup"><span data-stu-id="01f73-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="01f73-124">为该资源添加或更新项目时，将对它们进行专门索引，以便与 `$count` 和 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="01f73-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="01f73-125">在添加或更新项目与在索引中可用之间可能会稍有延迟。</span><span class="sxs-lookup"><span data-stu-id="01f73-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="01f73-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="01f73-126">Request headers</span></span>

| <span data-ttu-id="01f73-127">标头</span><span class="sxs-lookup"><span data-stu-id="01f73-127">Header</span></span> | <span data-ttu-id="01f73-128">值</span><span class="sxs-lookup"><span data-stu-id="01f73-128">Value</span></span> |
|:------ |:----- |
| <span data-ttu-id="01f73-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="01f73-129">Authorization</span></span>  | <span data-ttu-id="01f73-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="01f73-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="01f73-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="01f73-132">ConsistencyLevel</span></span> | <span data-ttu-id="01f73-133">最终。</span><span class="sxs-lookup"><span data-stu-id="01f73-133">eventual.</span></span> <span data-ttu-id="01f73-134">使用 `$search`、`$filter`、`$orderby` 或 OData 强制转换查询参数时，此标头和 `$count` 是必需的。</span><span class="sxs-lookup"><span data-stu-id="01f73-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="01f73-135">它使用的索引可能与对象的最新更改不同步。</span><span class="sxs-lookup"><span data-stu-id="01f73-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="01f73-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="01f73-136">Request body</span></span>

<span data-ttu-id="01f73-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="01f73-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01f73-138">响应</span><span class="sxs-lookup"><span data-stu-id="01f73-138">Response</span></span>

<span data-ttu-id="01f73-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="01f73-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="01f73-140">示例</span><span class="sxs-lookup"><span data-stu-id="01f73-140">Examples</span></span>

### <a name="example-1-get-groups-directory-roles-and-administrative-units-that-the-user-is-a-member-of"></a><span data-ttu-id="01f73-141">示例 1：获取用户是其中一个成员的组、目录角色和管理单元</span><span class="sxs-lookup"><span data-stu-id="01f73-141">Example 1: Get groups, directory roles, and administrative units that the user is a member of</span></span>

#### <a name="request"></a><span data-ttu-id="01f73-142">请求</span><span class="sxs-lookup"><span data-stu-id="01f73-142">Request</span></span>

<span data-ttu-id="01f73-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="01f73-143">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="01f73-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="01f73-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="01f73-145">C#</span><span class="sxs-lookup"><span data-stu-id="01f73-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="01f73-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="01f73-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="01f73-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="01f73-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="01f73-148">Java</span><span class="sxs-lookup"><span data-stu-id="01f73-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-transitivememberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="01f73-149">响应</span><span class="sxs-lookup"><span data-stu-id="01f73-149">Response</span></span>

<span data-ttu-id="01f73-150">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="01f73-150">The following is an example of the response.</span></span>
><span data-ttu-id="01f73-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="01f73-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "value":[
    {
      "@odata.type":"#microsoft.graph.group",
      "displayName":"All_Contoso_Licensing",
      "mailEnabled":true,
      "mailNickname":"ContosoMailNickName",
      "securityEnabled":true
    },
    {
      "@odata.type":"#microsoft.graph.group",
      "displayName":"ContosoAudience_PugetSound",
      "mailEnabled":true,
      "mailNickname":"Contoso_PugetSound",
      "securityEnabled":true
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-transitive-membership-in-groups-directory-roles-and-administrative-units"></a><span data-ttu-id="01f73-153">示例 2：仅获取组、目录角色和管理单元中的可传递成员身份计数</span><span class="sxs-lookup"><span data-stu-id="01f73-153">Example 2: Get only a count of transitive membership in groups, directory roles, and administrative units</span></span>

#### <a name="request"></a><span data-ttu-id="01f73-154">请求</span><span class="sxs-lookup"><span data-stu-id="01f73-154">Request</span></span>

<span data-ttu-id="01f73-155">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="01f73-155">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/transitiveMemberOf/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="01f73-156">响应</span><span class="sxs-lookup"><span data-stu-id="01f73-156">Response</span></span>

<span data-ttu-id="01f73-157">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="01f73-157">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

893
```

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-transitive-membership-in-groups"></a><span data-ttu-id="01f73-158">示例 3：使用 OData 强制转换以仅获取组中可传递成员身份的计数</span><span class="sxs-lookup"><span data-stu-id="01f73-158">Example 3: Use OData cast to get only a count of transitive membership in groups</span></span>

#### <a name="request"></a><span data-ttu-id="01f73-159">请求</span><span class="sxs-lookup"><span data-stu-id="01f73-159">Request</span></span>

<span data-ttu-id="01f73-160">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="01f73-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/transitiveMemberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="01f73-161">响应</span><span class="sxs-lookup"><span data-stu-id="01f73-161">Response</span></span>

<span data-ttu-id="01f73-162">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="01f73-162">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

588
```

### <a name="example-4-use-search-and-odata-cast-to-get-transitive-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="01f73-163">示例 4：使用 $search 和 OData 强制转换获取显示名称包含字母"tier"（包括返回对象计数）的组的可传递成员身份</span><span class="sxs-lookup"><span data-stu-id="01f73-163">Example 4: Use $search and OData cast to get transitive membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="01f73-164">请求</span><span class="sxs-lookup"><span data-stu-id="01f73-164">Request</span></span>

<span data-ttu-id="01f73-165">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="01f73-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="01f73-166">响应</span><span class="sxs-lookup"><span data-stu-id="01f73-166">Response</span></span>

<span data-ttu-id="01f73-167">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="01f73-167">The following is an example of the response.</span></span>
><span data-ttu-id="01f73-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="01f73-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-5-use-filter-and-odata-cast-to-get-transitive-membership-in-groups-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="01f73-170">示例 5：使用 $filter 和 OData 强制转换在具有以"a"开头（包括返回对象计数）的组显示名称获取可传递成员身份</span><span class="sxs-lookup"><span data-stu-id="01f73-170">Example 5: Use $filter and OData cast to get transitive membership in groups with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="01f73-171">请求</span><span class="sxs-lookup"><span data-stu-id="01f73-171">Request</span></span>

<span data-ttu-id="01f73-172">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="01f73-172">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="01f73-173">响应</span><span class="sxs-lookup"><span data-stu-id="01f73-173">Response</span></span>

<span data-ttu-id="01f73-174">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="01f73-174">The following is an example of the response.</span></span>
><span data-ttu-id="01f73-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="01f73-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "List transitiveMsemberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


