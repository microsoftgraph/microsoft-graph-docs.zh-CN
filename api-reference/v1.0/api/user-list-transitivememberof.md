---
title: List user transitive memberOf
description: 获取用户所属的组和目录角色。 此 API 请求是可传递的，并且还将返回用户是其嵌套成员的所有组。
author: krbain
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: ec5d1dbd1cdb61df9f10704c450ceb660cd562f0
ms.sourcegitcommit: d9457ac1b8c2e8ac4b9604dd9e116fd547d2bfbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/29/2020
ms.locfileid: "48796939"
---
# <a name="list-user-transitive-memberof"></a><span data-ttu-id="a845b-104">List user transitive memberOf</span><span class="sxs-lookup"><span data-stu-id="a845b-104">List user transitive memberOf</span></span>

<span data-ttu-id="a845b-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a845b-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a845b-106">获取用户所属的组和目录角色。</span><span class="sxs-lookup"><span data-stu-id="a845b-106">Get groups, directory roles that the user is a member of.</span></span> <span data-ttu-id="a845b-107">此 API 请求是可传递的，并且还将返回用户是其嵌套成员的所有组。</span><span class="sxs-lookup"><span data-stu-id="a845b-107">This API request is transitive, and will also return all groups the user is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="a845b-108">权限</span><span class="sxs-lookup"><span data-stu-id="a845b-108">Permissions</span></span>

<span data-ttu-id="a845b-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a845b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a845b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a845b-111">Permission type</span></span>      | <span data-ttu-id="a845b-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a845b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a845b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a845b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a845b-114">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a845b-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a845b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a845b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a845b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a845b-116">Not supported.</span></span>    |
|<span data-ttu-id="a845b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a845b-117">Application</span></span> | <span data-ttu-id="a845b-118">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a845b-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="a845b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a845b-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id | userPrincipalName}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a845b-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a845b-120">Optional query parameters</span></span>

<span data-ttu-id="a845b-121">此方法支持[OData query parameters](/graph/query-parameters)以帮助自定义响应，包括 `$search`、`$count`、 和 `$filter`</span><span class="sxs-lookup"><span data-stu-id="a845b-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="a845b-122">还会启用 OData 强制转换，例如，您可以强制转换以仅获取组中的可传递成员资格。</span><span class="sxs-lookup"><span data-stu-id="a845b-122">OData cast is also enabled, for example, you can cast to get just the transitive membership in groups.</span></span> <span data-ttu-id="a845b-123">`$search`可以用在 **displayName** 属性。</span><span class="sxs-lookup"><span data-stu-id="a845b-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="a845b-124">为该资源添加或更新项目时，将对它们进行专门索引，以便与 `$count` 和 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="a845b-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="a845b-125">在添加或更新项目与在索引中可用之间可能会稍有延迟。</span><span class="sxs-lookup"><span data-stu-id="a845b-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a845b-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="a845b-126">Request headers</span></span>

| <span data-ttu-id="a845b-127">标头</span><span class="sxs-lookup"><span data-stu-id="a845b-127">Header</span></span>       | <span data-ttu-id="a845b-128">值</span><span class="sxs-lookup"><span data-stu-id="a845b-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a845b-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="a845b-129">Authorization</span></span>  | <span data-ttu-id="a845b-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a845b-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a845b-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="a845b-132">ConsistencyLevel</span></span> | <span data-ttu-id="a845b-133">最终。</span><span class="sxs-lookup"><span data-stu-id="a845b-133">eventual.</span></span> <span data-ttu-id="a845b-134">使用 `$search`、`$filter`、`$orderby` 或 OData 强制转换查询参数时，此标头和 `$count` 是必需的。</span><span class="sxs-lookup"><span data-stu-id="a845b-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="a845b-135">它使用的索引可能与对象的最新更改不同步。</span><span class="sxs-lookup"><span data-stu-id="a845b-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a845b-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="a845b-136">Request body</span></span>

<span data-ttu-id="a845b-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a845b-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a845b-138">响应</span><span class="sxs-lookup"><span data-stu-id="a845b-138">Response</span></span>

<span data-ttu-id="a845b-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a845b-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a845b-140">示例</span><span class="sxs-lookup"><span data-stu-id="a845b-140">Examples</span></span>

### <a name="example-1-get-groups-directory-roles-and-administrative-units-that-the-user-is-a-member-of"></a><span data-ttu-id="a845b-141">示例1：获取用户所属的组、目录角色和管理单元</span><span class="sxs-lookup"><span data-stu-id="a845b-141">Example 1: Get groups, directory roles, and administrative units that the user is a member of</span></span>

#### <a name="request"></a><span data-ttu-id="a845b-142">请求</span><span class="sxs-lookup"><span data-stu-id="a845b-142">Request</span></span>

<span data-ttu-id="a845b-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a845b-143">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/transitiveMemberOf
```

#### <a name="response"></a><span data-ttu-id="a845b-144">响应</span><span class="sxs-lookup"><span data-stu-id="a845b-144">Response</span></span>

<span data-ttu-id="a845b-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a845b-145">The following is an example of the response.</span></span>

><span data-ttu-id="a845b-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a845b-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "value":[
    {
      "@odata.type":"#microsoft.graph.group",
      "displayName":"All_Contoso_Licensing",
      "mailEnabled":true,
      "mailNickname":"ContosoMailNickName",
      "securityEnabled":true
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-transitive-membership-in-groups-directory-roles-and-administrative-units"></a><span data-ttu-id="a845b-148">示例2：仅获取组、目录角色和管理单元中可传递成员身份的计数</span><span class="sxs-lookup"><span data-stu-id="a845b-148">Example 2: Get only a count of transitive membership in groups, directory roles, and administrative units</span></span>

#### <a name="request"></a><span data-ttu-id="a845b-149">请求</span><span class="sxs-lookup"><span data-stu-id="a845b-149">Request</span></span>

<span data-ttu-id="a845b-150">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a845b-150">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/transitiveMemberOf/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="a845b-151">响应</span><span class="sxs-lookup"><span data-stu-id="a845b-151">Response</span></span>

<span data-ttu-id="a845b-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a845b-152">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`893`

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-transitive-membership-in-groups"></a><span data-ttu-id="a845b-153">示例 3：使用 OData 强制转换以仅获取组中可传递成员身份的计数</span><span class="sxs-lookup"><span data-stu-id="a845b-153">Example 3: Use OData cast to get only a count of transitive membership in groups</span></span>

#### <a name="request"></a><span data-ttu-id="a845b-154">请求</span><span class="sxs-lookup"><span data-stu-id="a845b-154">Request</span></span>

<span data-ttu-id="a845b-155">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a845b-155">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/transitiveMemberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="a845b-156">响应</span><span class="sxs-lookup"><span data-stu-id="a845b-156">Response</span></span>

<span data-ttu-id="a845b-157">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a845b-157">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
  } -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`588`

### <a name="example-4-use-search-and-odata-cast-to-get-transitive-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="a845b-158">示例4：使用 $search 和 OData cast 以使用包含字母 "层" 的显示名称获取组中的可传递成员身份，包括返回对象的计数</span><span class="sxs-lookup"><span data-stu-id="a845b-158">Example 4: Use $search and OData cast to get transitive membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="a845b-159">请求</span><span class="sxs-lookup"><span data-stu-id="a845b-159">Request</span></span>

<span data-ttu-id="a845b-160">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a845b-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="a845b-161">响应</span><span class="sxs-lookup"><span data-stu-id="a845b-161">Response</span></span>

<span data-ttu-id="a845b-162">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a845b-162">The following is an example of the response.</span></span>

><span data-ttu-id="a845b-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a845b-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups(displayName,id)",
  "@odata.count":7,
  "value":[
    {
      "displayName":"Contoso-tier Query Notification",
      "id":"11111111-2222-3333-4444-555555555555"
    }
  ]
}
```

### <a name="example-5-use-filter-and-odata-cast-to-get-transitive-membership-in-groups-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="a845b-165">示例5：使用 $filter 和 OData 强制转换来获取具有以 "a" 开头的显示名称的组中的可传递成员身份，其中包含返回对象的计数</span><span class="sxs-lookup"><span data-stu-id="a845b-165">Example 5: Use $filter and OData cast to get transitive membership in groups with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="a845b-166">请求</span><span class="sxs-lookup"><span data-stu-id="a845b-166">Request</span></span>

<span data-ttu-id="a845b-167">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a845b-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="a845b-168">响应</span><span class="sxs-lookup"><span data-stu-id="a845b-168">Response</span></span>

<span data-ttu-id="a845b-169">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a845b-169">The following is an example of the response.</span></span>

><span data-ttu-id="a845b-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a845b-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
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
<!-- {
  "type": "#page.annotation",
  "description": "List transitiveMsemberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
