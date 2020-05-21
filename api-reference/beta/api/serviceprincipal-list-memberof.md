---
title: 列出 servicePrincipal memberOf
description: 获取此服务主体是其直接成员的组和目录角色。 此操作不可传递。
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 467811318ba3a68c8e901ebc2067cba8f337f6fa
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44336459"
---
# <a name="list-serviceprincipal-memberof"></a><span data-ttu-id="8d808-104">列出 servicePrincipal memberOf</span><span class="sxs-lookup"><span data-stu-id="8d808-104">List servicePrincipal memberOf</span></span>

<span data-ttu-id="8d808-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d808-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d808-106">获取此[servicePrincipal](../resources/serviceprincipal.md)是其直接成员的组和目录角色。</span><span class="sxs-lookup"><span data-stu-id="8d808-106">Get the groups and directory roles that this [servicePrincipal](../resources/serviceprincipal.md) is a direct member of.</span></span> <span data-ttu-id="8d808-107">此操作不可传递。</span><span class="sxs-lookup"><span data-stu-id="8d808-107">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="8d808-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="8d808-108">Permissions</span></span>

<span data-ttu-id="8d808-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8d808-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d808-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8d808-111">Permission type</span></span>      | <span data-ttu-id="8d808-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8d808-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d808-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8d808-113">Delegated (work or school account)</span></span> | <span data-ttu-id="8d808-114">"Application"、"all"、"Directory.accessasuser.all"、"全部"、"全部"、"全部"、"全部"、"所有"</span><span class="sxs-lookup"><span data-stu-id="8d808-114">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8d808-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8d808-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d808-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8d808-116">Not supported.</span></span>    |
|<span data-ttu-id="8d808-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="8d808-117">Application</span></span> | <span data-ttu-id="8d808-118">"Application.readwrite.ownedby"、"全部"、"全部"、"全部"、"全部"、"全部"、"全部"、"全部"、"目录"</span><span class="sxs-lookup"><span data-stu-id="8d808-118">Application.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="8d808-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8d808-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8d808-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8d808-120">Optional query parameters</span></span>

<span data-ttu-id="8d808-121">此方法支持[OData 查询参数](/graph/query_parameters)，以帮助自定义响应，包括 `$search` 、 `$count` 和 `$filter` 。</span><span class="sxs-lookup"><span data-stu-id="8d808-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="8d808-122">此外，还会启用 OData 强制转换，例如，您可以强制转换为仅获取用户所属的 directoryRoles。</span><span class="sxs-lookup"><span data-stu-id="8d808-122">OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of.</span></span> <span data-ttu-id="8d808-123">您可以 `$search` 在**displayName**属性上使用。</span><span class="sxs-lookup"><span data-stu-id="8d808-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="8d808-124">为此资源添加或更新项目时，将对其进行专门编制索引，以便 `$count` 与 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="8d808-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="8d808-125">在添加或更新项目以及在索引中可用时，可能会出现轻微的延迟。</span><span class="sxs-lookup"><span data-stu-id="8d808-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8d808-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="8d808-126">Request headers</span></span>

| <span data-ttu-id="8d808-127">名称</span><span class="sxs-lookup"><span data-stu-id="8d808-127">Name</span></span>       | <span data-ttu-id="8d808-128">类型</span><span class="sxs-lookup"><span data-stu-id="8d808-128">Type</span></span> | <span data-ttu-id="8d808-129">说明</span><span class="sxs-lookup"><span data-stu-id="8d808-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8d808-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d808-130">Authorization</span></span>  | <span data-ttu-id="8d808-131">string</span><span class="sxs-lookup"><span data-stu-id="8d808-131">string</span></span>  | <span data-ttu-id="8d808-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8d808-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8d808-134">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="8d808-134">ConsistencyLevel</span></span> | <span data-ttu-id="8d808-135">仍然.</span><span class="sxs-lookup"><span data-stu-id="8d808-135">eventual.</span></span> <span data-ttu-id="8d808-136">在 `$count` 使用 `$search` 、 `$filter` 、 `$orderby` 或 OData 转换查询参数时，此标头和是必需的。</span><span class="sxs-lookup"><span data-stu-id="8d808-136">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="8d808-137">它使用的索引可能不是最新的，并包含对对象的最新更改。</span><span class="sxs-lookup"><span data-stu-id="8d808-137">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8d808-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="8d808-138">Request body</span></span>
<span data-ttu-id="8d808-139">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8d808-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d808-140">响应</span><span class="sxs-lookup"><span data-stu-id="8d808-140">Response</span></span>

<span data-ttu-id="8d808-141">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="8d808-141">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8d808-142">示例</span><span class="sxs-lookup"><span data-stu-id="8d808-142">Examples</span></span>

### <a name="example-1-get-groups-and-directory-roles-that-the-service-principal-is-a-direct-member-of"></a><span data-ttu-id="8d808-143">示例1：获取服务主体是其直接成员的组和目录角色</span><span class="sxs-lookup"><span data-stu-id="8d808-143">Example 1: Get groups and directory roles that the service principal is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="8d808-144">请求</span><span class="sxs-lookup"><span data-stu-id="8d808-144">Request</span></span>

<span data-ttu-id="8d808-145">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8d808-145">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8d808-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="8d808-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="8d808-147">C#</span><span class="sxs-lookup"><span data-stu-id="8d808-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceprincipal-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8d808-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8d808-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceprincipal-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8d808-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8d808-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceprincipal-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8d808-150">响应</span><span class="sxs-lookup"><span data-stu-id="8d808-150">Response</span></span>

<span data-ttu-id="8d808-151">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8d808-151">The following is an example of the response.</span></span> 
> <span data-ttu-id="8d808-152">**注意：** 为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8d808-152">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="8d808-153">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8d808-153">All of the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-all-memberships"></a><span data-ttu-id="8d808-154">示例2：仅获取所有成员身份的计数</span><span class="sxs-lookup"><span data-stu-id="8d808-154">Example 2: Get only a count of all memberships</span></span>

#### <a name="request"></a><span data-ttu-id="8d808-155">请求</span><span class="sxs-lookup"><span data-stu-id="8d808-155">Request</span></span>

<span data-ttu-id="8d808-156">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8d808-156">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8d808-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="8d808-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="8d808-158">C#</span><span class="sxs-lookup"><span data-stu-id="8d808-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8d808-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8d808-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8d808-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8d808-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8d808-161">响应</span><span class="sxs-lookup"><span data-stu-id="8d808-161">Response</span></span>

<span data-ttu-id="8d808-162">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8d808-162">The following is an example of the response.</span></span>

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

<span data-ttu-id="8d808-163">394</span><span class="sxs-lookup"><span data-stu-id="8d808-163">394</span></span>

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-group-membership"></a><span data-ttu-id="8d808-164">示例3：使用 OData 强制转换仅获取组成员身份的计数</span><span class="sxs-lookup"><span data-stu-id="8d808-164">Example 3: Use OData cast to get only a count of group membership</span></span>

#### <a name="request"></a><span data-ttu-id="8d808-165">请求</span><span class="sxs-lookup"><span data-stu-id="8d808-165">Request</span></span>

<span data-ttu-id="8d808-166">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8d808-166">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8d808-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="8d808-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_group_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="8d808-168">C#</span><span class="sxs-lookup"><span data-stu-id="8d808-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-group-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8d808-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8d808-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-group-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8d808-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8d808-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-group-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8d808-171">响应</span><span class="sxs-lookup"><span data-stu-id="8d808-171">Response</span></span>

<span data-ttu-id="8d808-172">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8d808-172">The following is an example of the response.</span></span>

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

<span data-ttu-id="8d808-173">394</span><span class="sxs-lookup"><span data-stu-id="8d808-173">394</span></span>

### <a name="example-4-use-search-and-odata-cast-to-get-group-membership-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="8d808-174">示例4：使用 $search 和 OData 强制转换来获取具有包含字母 "Video" 的显示名称的组成员身份，其中包括返回的对象的计数</span><span class="sxs-lookup"><span data-stu-id="8d808-174">Example 4: Use $search and OData cast to get group membership with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="8d808-175">请求</span><span class="sxs-lookup"><span data-stu-id="8d808-175">Request</span></span>

<span data-ttu-id="8d808-176">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8d808-176">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET iv. https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search=”displayName:Video" 
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="8d808-177">响应</span><span class="sxs-lookup"><span data-stu-id="8d808-177">Response</span></span>

<span data-ttu-id="8d808-178">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8d808-178">The following is an example of the response.</span></span>
><span data-ttu-id="8d808-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8d808-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-5-use-filter-and-odata-cast-to-get-group-membership-with-a-display-name-that-starts-with-the-letter-a-including-a-count-of-returned-objects"></a><span data-ttu-id="8d808-181">示例5：使用 $filter 和 OData 强制转换来获取具有以字母 "A" 开头的显示名称的组成员身份，其中包括返回对象的计数</span><span class="sxs-lookup"><span data-stu-id="8d808-181">Example 5: Use $filter and OData cast to get group membership with a display name that starts with the letter 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="8d808-182">请求</span><span class="sxs-lookup"><span data-stu-id="8d808-182">Request</span></span>

<span data-ttu-id="8d808-183">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8d808-183">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'A')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="8d808-184">响应</span><span class="sxs-lookup"><span data-stu-id="8d808-184">Response</span></span>

<span data-ttu-id="8d808-185">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8d808-185">The following is an example of the response.</span></span>
><span data-ttu-id="8d808-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8d808-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
