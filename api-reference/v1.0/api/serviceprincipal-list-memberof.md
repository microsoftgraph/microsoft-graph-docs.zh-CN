---
title: List servicePrincipal memberOf
description: 获取此服务主体作为直接成员所属的组和目录角色。 此操作不可传递。
localization_priority: Priority
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: cae222b8a44a3493fb35c576aa9251859bde39ee
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50626115"
---
# <a name="list-serviceprincipal-memberof"></a><span data-ttu-id="3621e-104">List servicePrincipal memberOf</span><span class="sxs-lookup"><span data-stu-id="3621e-104">List servicePrincipal memberOf</span></span>

<span data-ttu-id="3621e-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3621e-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3621e-106">获取此 [servicePrincipal](../resources/serviceprincipal.md) 作为直接成员所属的组和目录角色。</span><span class="sxs-lookup"><span data-stu-id="3621e-106">Get the groups and directory roles that this [servicePrincipal](../resources/serviceprincipal.md) is a direct member of.</span></span> <span data-ttu-id="3621e-107">此操作不可传递。</span><span class="sxs-lookup"><span data-stu-id="3621e-107">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="3621e-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="3621e-108">Permissions</span></span>

<span data-ttu-id="3621e-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3621e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3621e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3621e-111">Permission type</span></span>      | <span data-ttu-id="3621e-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3621e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3621e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3621e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="3621e-114">Application.Read.All、Application.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3621e-114">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3621e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3621e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3621e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3621e-116">Not supported.</span></span>    |
|<span data-ttu-id="3621e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3621e-117">Application</span></span> | <span data-ttu-id="3621e-118">Application.Read.All、Application.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3621e-118">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="3621e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3621e-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3621e-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3621e-120">Optional query parameters</span></span>

<span data-ttu-id="3621e-121">此方法支持[OData query parameters](/graph/query_parameters)以帮助自定义响应，包括 `$search`、`$count`、 和 `$filter`</span><span class="sxs-lookup"><span data-stu-id="3621e-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="3621e-122">还启用了 OData 强制转换，例如，你可以强制转换为仅获取用户所属的 directoryRoles。</span><span class="sxs-lookup"><span data-stu-id="3621e-122">OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of.</span></span> <span data-ttu-id="3621e-123">可使用“**displayName**”和“**说明**”属性上的`$search`。</span><span class="sxs-lookup"><span data-stu-id="3621e-123">You can use `$search` on the **displayName** and **description** properties.</span></span> <span data-ttu-id="3621e-124">为该资源添加或更新项目时，将对它们进行专门索引，以便与 `$count` 和 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="3621e-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="3621e-125">在添加或更新项目与在索引中可用之间可能会稍有延迟。</span><span class="sxs-lookup"><span data-stu-id="3621e-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3621e-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="3621e-126">Request headers</span></span>
| <span data-ttu-id="3621e-127">名称</span><span class="sxs-lookup"><span data-stu-id="3621e-127">Name</span></span>           | <span data-ttu-id="3621e-128">说明</span><span class="sxs-lookup"><span data-stu-id="3621e-128">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="3621e-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="3621e-129">Authorization</span></span>  | <span data-ttu-id="3621e-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3621e-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3621e-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="3621e-132">ConsistencyLevel</span></span> | <span data-ttu-id="3621e-133">最终。</span><span class="sxs-lookup"><span data-stu-id="3621e-133">eventual.</span></span> <span data-ttu-id="3621e-134">使用 `$search`、`$filter`、`$orderby` 或 OData 强制转换查询参数时，此标头和 `$count` 是必需的。</span><span class="sxs-lookup"><span data-stu-id="3621e-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="3621e-135">它使用的索引可能与对象的最新更改不同步。</span><span class="sxs-lookup"><span data-stu-id="3621e-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3621e-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="3621e-136">Request body</span></span>

<span data-ttu-id="3621e-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3621e-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3621e-138">响应</span><span class="sxs-lookup"><span data-stu-id="3621e-138">Response</span></span>

<span data-ttu-id="3621e-139">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="3621e-139">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3621e-140">示例</span><span class="sxs-lookup"><span data-stu-id="3621e-140">Examples</span></span>

### <a name="example-1-get-groups-and-directory-roles-that-the-service-principal-is-a-direct-member-of"></a><span data-ttu-id="3621e-141">示例 1：获取此服务主体作为直接成员所属的组和目录角色</span><span class="sxs-lookup"><span data-stu-id="3621e-141">Example 1: Get groups and directory roles that the service principal is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="3621e-142">请求</span><span class="sxs-lookup"><span data-stu-id="3621e-142">Request</span></span>

<span data-ttu-id="3621e-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3621e-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3621e-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="3621e-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="3621e-145">C#</span><span class="sxs-lookup"><span data-stu-id="3621e-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceprincipal-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3621e-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3621e-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceprincipal-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3621e-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3621e-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceprincipal-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3621e-148">Java</span><span class="sxs-lookup"><span data-stu-id="3621e-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-serviceprincipal-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="3621e-149">响应</span><span class="sxs-lookup"><span data-stu-id="3621e-149">Response</span></span>

<span data-ttu-id="3621e-150">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3621e-150">The following is an example of the response.</span></span>

> <span data-ttu-id="3621e-151">**注意：** 为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3621e-151">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3621e-152">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3621e-152">All of the properties will be returned from an actual call.</span></span>

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
      "securityEnabled": true
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-all-memberships"></a><span data-ttu-id="3621e-153">示例 2：仅获取所有可成员身份的计数</span><span class="sxs-lookup"><span data-stu-id="3621e-153">Example 2: Get only a count of all memberships</span></span>

#### <a name="request"></a><span data-ttu-id="3621e-154">请求</span><span class="sxs-lookup"><span data-stu-id="3621e-154">Request</span></span>

<span data-ttu-id="3621e-155">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3621e-155">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/memberOf/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="3621e-156">响应</span><span class="sxs-lookup"><span data-stu-id="3621e-156">Response</span></span>

<span data-ttu-id="3621e-157">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3621e-157">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

394
```

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-group-membership"></a><span data-ttu-id="3621e-158">示例 3：使用 OData 强制转换以仅获取组成员身份的计数</span><span class="sxs-lookup"><span data-stu-id="3621e-158">Example 3: Use OData cast to get only a count of group membership</span></span>

#### <a name="request"></a><span data-ttu-id="3621e-159">请求</span><span class="sxs-lookup"><span data-stu-id="3621e-159">Request</span></span>

<span data-ttu-id="3621e-160">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3621e-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_group_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/memberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="3621e-161">响应</span><span class="sxs-lookup"><span data-stu-id="3621e-161">Response</span></span>

<span data-ttu-id="3621e-162">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3621e-162">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

394
```

### <a name="example-4-use-search-and-odata-cast-to-get-group-membership-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="3621e-163">示例 4：使用 $search 和 OData 强制转换获取显示名称中包含字母“Video”（包括返回的对象数）的组成员身份</span><span class="sxs-lookup"><span data-stu-id="3621e-163">Example 4: Use $search and OData cast to get group membership with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="3621e-164">请求</span><span class="sxs-lookup"><span data-stu-id="3621e-164">Request</span></span>

<span data-ttu-id="3621e-165">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3621e-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search=”displayName:Video" 
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="3621e-166">响应</span><span class="sxs-lookup"><span data-stu-id="3621e-166">Response</span></span>

<span data-ttu-id="3621e-167">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3621e-167">The following is an example of the response.</span></span>

><span data-ttu-id="3621e-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="3621e-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-5-use-filter-and-odata-cast-to-get-group-membership-with-a-display-name-that-starts-with-the-letter-a-including-a-count-of-returned-objects"></a><span data-ttu-id="3621e-170">示例 5：使用 $filter 和 OData 强制转换获取显示名称以字母“A”开头（包括返回的对象数）的组成员身份</span><span class="sxs-lookup"><span data-stu-id="3621e-170">Example 5: Use $filter and OData cast to get group membership with a display name that starts with the letter 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="3621e-171">请求</span><span class="sxs-lookup"><span data-stu-id="3621e-171">Request</span></span>

<span data-ttu-id="3621e-172">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3621e-172">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'A')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="3621e-173">响应</span><span class="sxs-lookup"><span data-stu-id="3621e-173">Response</span></span>

<span data-ttu-id="3621e-174">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3621e-174">The following is an example of the response.</span></span>

><span data-ttu-id="3621e-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="3621e-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
