---
title: List servicePrincipal memberOf
description: 获取此服务主体作为直接成员所属的组和目录角色。 此操作不可传递。
localization_priority: Priority
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 64cbfffb5652e4c17303e6dd5385c06c53a58575
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50626235"
---
# <a name="list-serviceprincipal-memberof"></a><span data-ttu-id="bc674-104">List servicePrincipal memberOf</span><span class="sxs-lookup"><span data-stu-id="bc674-104">List servicePrincipal memberOf</span></span>

<span data-ttu-id="bc674-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc674-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc674-106">获取此 [servicePrincipal](../resources/serviceprincipal.md) 作为直接成员所属的组和目录角色。</span><span class="sxs-lookup"><span data-stu-id="bc674-106">Get the groups and directory roles that this [servicePrincipal](../resources/serviceprincipal.md) is a direct member of.</span></span> <span data-ttu-id="bc674-107">此操作不可传递。</span><span class="sxs-lookup"><span data-stu-id="bc674-107">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="bc674-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="bc674-108">Permissions</span></span>

<span data-ttu-id="bc674-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bc674-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc674-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="bc674-111">Permission type</span></span>      | <span data-ttu-id="bc674-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bc674-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc674-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bc674-113">Delegated (work or school account)</span></span> | <span data-ttu-id="bc674-114">Application.Read.All、Directory.Read.All、Application.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bc674-114">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bc674-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bc674-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc674-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bc674-116">Not supported.</span></span>    |
|<span data-ttu-id="bc674-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="bc674-117">Application</span></span> | <span data-ttu-id="bc674-118">Application.Read.All、Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc674-118">Application.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="bc674-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bc674-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bc674-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="bc674-120">Optional query parameters</span></span>

<span data-ttu-id="bc674-121">此方法支持[OData query parameters](/graph/query_parameters)以帮助自定义响应，包括 `$search`、`$count`、 和 `$filter`</span><span class="sxs-lookup"><span data-stu-id="bc674-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="bc674-122">还启用了 OData 强制转换，例如，你可以强制转换为仅获取用户所属的 directoryRoles。</span><span class="sxs-lookup"><span data-stu-id="bc674-122">OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of.</span></span> <span data-ttu-id="bc674-123">`$search`可以用在 **displayName** 属性。</span><span class="sxs-lookup"><span data-stu-id="bc674-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="bc674-124">为该资源添加或更新项目时，将对它们进行专门索引，以便与 `$count` 和 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="bc674-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="bc674-125">在添加或更新项目与在索引中可用之间可能会稍有延迟。</span><span class="sxs-lookup"><span data-stu-id="bc674-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bc674-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="bc674-126">Request headers</span></span>

| <span data-ttu-id="bc674-127">名称</span><span class="sxs-lookup"><span data-stu-id="bc674-127">Name</span></span>       | <span data-ttu-id="bc674-128">类型</span><span class="sxs-lookup"><span data-stu-id="bc674-128">Type</span></span> | <span data-ttu-id="bc674-129">说明</span><span class="sxs-lookup"><span data-stu-id="bc674-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="bc674-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc674-130">Authorization</span></span>  | <span data-ttu-id="bc674-131">string</span><span class="sxs-lookup"><span data-stu-id="bc674-131">string</span></span>  | <span data-ttu-id="bc674-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bc674-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bc674-134">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="bc674-134">ConsistencyLevel</span></span> | <span data-ttu-id="bc674-135">最终。</span><span class="sxs-lookup"><span data-stu-id="bc674-135">eventual.</span></span> <span data-ttu-id="bc674-136">使用 `$search`、`$filter`、`$orderby` 或 OData 强制转换查询参数时，此标头和 `$count` 是必需的。</span><span class="sxs-lookup"><span data-stu-id="bc674-136">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="bc674-137">它使用的索引可能与对象的最新更改不同步。</span><span class="sxs-lookup"><span data-stu-id="bc674-137">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bc674-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="bc674-138">Request body</span></span>
<span data-ttu-id="bc674-139">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bc674-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bc674-140">响应</span><span class="sxs-lookup"><span data-stu-id="bc674-140">Response</span></span>

<span data-ttu-id="bc674-141">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="bc674-141">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bc674-142">示例</span><span class="sxs-lookup"><span data-stu-id="bc674-142">Examples</span></span>

### <a name="example-1-get-groups-and-directory-roles-that-the-service-principal-is-a-direct-member-of"></a><span data-ttu-id="bc674-143">示例 1：获取此服务主体作为直接成员所属的组和目录角色</span><span class="sxs-lookup"><span data-stu-id="bc674-143">Example 1: Get groups and directory roles that the service principal is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="bc674-144">请求</span><span class="sxs-lookup"><span data-stu-id="bc674-144">Request</span></span>

<span data-ttu-id="bc674-145">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bc674-145">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="bc674-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="bc674-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="bc674-147">C#</span><span class="sxs-lookup"><span data-stu-id="bc674-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceprincipal-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bc674-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bc674-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceprincipal-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bc674-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bc674-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceprincipal-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bc674-150">Java</span><span class="sxs-lookup"><span data-stu-id="bc674-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-serviceprincipal-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="bc674-151">响应</span><span class="sxs-lookup"><span data-stu-id="bc674-151">Response</span></span>

<span data-ttu-id="bc674-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bc674-152">The following is an example of the response.</span></span> 
> <span data-ttu-id="bc674-153">**注意：** 为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="bc674-153">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="bc674-154">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bc674-154">All of the properties will be returned from an actual call.</span></span>

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
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-all-memberships"></a><span data-ttu-id="bc674-155">示例 2：仅获取所有可成员身份的计数</span><span class="sxs-lookup"><span data-stu-id="bc674-155">Example 2: Get only a count of all memberships</span></span>

#### <a name="request"></a><span data-ttu-id="bc674-156">请求</span><span class="sxs-lookup"><span data-stu-id="bc674-156">Request</span></span>

<span data-ttu-id="bc674-157">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bc674-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="bc674-158">响应</span><span class="sxs-lookup"><span data-stu-id="bc674-158">Response</span></span>

<span data-ttu-id="bc674-159">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bc674-159">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

394
```

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-group-membership"></a><span data-ttu-id="bc674-160">示例 3：使用 OData 强制转换以仅获取组成员身份的计数</span><span class="sxs-lookup"><span data-stu-id="bc674-160">Example 3: Use OData cast to get only a count of group membership</span></span>

#### <a name="request"></a><span data-ttu-id="bc674-161">请求</span><span class="sxs-lookup"><span data-stu-id="bc674-161">Request</span></span>

<span data-ttu-id="bc674-162">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bc674-162">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_group_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="bc674-163">响应</span><span class="sxs-lookup"><span data-stu-id="bc674-163">Response</span></span>

<span data-ttu-id="bc674-164">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bc674-164">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

394
```

### <a name="example-4-use-search-and-odata-cast-to-get-group-membership-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="bc674-165">示例 4：使用 $search 和 OData 强制转换获取显示名称中包含字母“Video”（包括返回的对象数）的组成员身份</span><span class="sxs-lookup"><span data-stu-id="bc674-165">Example 4: Use $search and OData cast to get group membership with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="bc674-166">请求</span><span class="sxs-lookup"><span data-stu-id="bc674-166">Request</span></span>

<span data-ttu-id="bc674-167">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bc674-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search=”displayName:Video" 
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="bc674-168">响应</span><span class="sxs-lookup"><span data-stu-id="bc674-168">Response</span></span>

<span data-ttu-id="bc674-169">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bc674-169">The following is an example of the response.</span></span>
><span data-ttu-id="bc674-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="bc674-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.count":1396,
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All videos for the company",
      "displayName": "All Videos",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true
    }
  ]
}
```

### <a name="example-5-use-filter-and-odata-cast-to-get-group-membership-with-a-display-name-that-starts-with-the-letter-a-including-a-count-of-returned-objects"></a><span data-ttu-id="bc674-172">示例 5：使用 $filter 和 OData 强制转换获取显示名称以字母“A”开头（包括返回的对象数）的组成员身份</span><span class="sxs-lookup"><span data-stu-id="bc674-172">Example 5: Use $filter and OData cast to get group membership with a display name that starts with the letter 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="bc674-173">请求</span><span class="sxs-lookup"><span data-stu-id="bc674-173">Request</span></span>

<span data-ttu-id="bc674-174">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bc674-174">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'A')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="bc674-175">响应</span><span class="sxs-lookup"><span data-stu-id="bc674-175">Response</span></span>

<span data-ttu-id="bc674-176">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bc674-176">The following is an example of the response.</span></span>
><span data-ttu-id="bc674-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="bc674-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.count":76,
  "value":[
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All videos for the company",
      "displayName": "All Videos",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List servicePrincipal memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->



