---
title: List servicePrincipals
description: 检索 servicePrincipal 对象列表。
author: sureshja
localization_priority: Priority
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 8628a9c99c41060940bddc71d354e9bf60169835
ms.sourcegitcommit: 6d247f44a6ee4d8515c3863ee8a2683163c9f829
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2021
ms.locfileid: "53430107"
---
# <a name="list-serviceprincipals"></a><span data-ttu-id="17171-103">List servicePrincipals</span><span class="sxs-lookup"><span data-stu-id="17171-103">List servicePrincipals</span></span>

<span data-ttu-id="17171-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17171-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="17171-105">检索 [servicePrincipal](../resources/serviceprincipal.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="17171-105">Retrieve a list of [servicePrincipal](../resources/serviceprincipal.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="17171-106">权限</span><span class="sxs-lookup"><span data-stu-id="17171-106">Permissions</span></span>

<span data-ttu-id="17171-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="17171-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17171-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="17171-109">Permission type</span></span>      | <span data-ttu-id="17171-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="17171-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="17171-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="17171-111">Delegated (work or school account)</span></span> | <span data-ttu-id="17171-112">Application.Read.All、Application.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="17171-112">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="17171-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="17171-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17171-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="17171-114">Not supported.</span></span>    |
|<span data-ttu-id="17171-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="17171-115">Application</span></span> | <span data-ttu-id="17171-116">Application.Read.All、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="17171-116">Application.Read.All, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="17171-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="17171-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals
```
## <a name="optional-query-parameters"></a><span data-ttu-id="17171-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="17171-118">Optional query parameters</span></span>

<span data-ttu-id="17171-119">此方法支持使用 `$count`、`$expand`、`$filter`、`$orderBy`、`$search`、`$select` 和 `$top` [ OData 查询参数 ](/graph/query-parameters) 以帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="17171-119">This method supports the `$count`, `$expand`, `$filter`, `$orderBy`, `$search`, `$select`, and `$top` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span> <span data-ttu-id="17171-120">只有将 **ConsistencyLevel** 标头设置为 `eventual` 和 `$count` 时，才支持某些查询。</span><span class="sxs-lookup"><span data-stu-id="17171-120">Some queries are supported only when you use the **ConsistencyLevel** header set to `eventual` and `$count`.</span></span> <span data-ttu-id="17171-121">有关详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。</span><span class="sxs-lookup"><span data-stu-id="17171-121">For more information, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

## <a name="request-headers"></a><span data-ttu-id="17171-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="17171-122">Request headers</span></span>
| <span data-ttu-id="17171-123">名称</span><span class="sxs-lookup"><span data-stu-id="17171-123">Name</span></span>           | <span data-ttu-id="17171-124">说明</span><span class="sxs-lookup"><span data-stu-id="17171-124">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="17171-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="17171-125">Authorization</span></span>  | <span data-ttu-id="17171-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="17171-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="17171-128">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="17171-128">ConsistencyLevel</span></span> | <span data-ttu-id="17171-129">最终。</span><span class="sxs-lookup"><span data-stu-id="17171-129">eventual.</span></span> <span data-ttu-id="17171-130">当使用 `$search` 或将 `$filter` 与 `$orderby` 查询参数一起使用时，此标头和 `$count` 是必需的。</span><span class="sxs-lookup"><span data-stu-id="17171-130">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="17171-131">它使用的索引可能与对象的最新更改不同步。</span><span class="sxs-lookup"><span data-stu-id="17171-131">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="17171-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="17171-132">Request body</span></span>

<span data-ttu-id="17171-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="17171-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="17171-134">响应</span><span class="sxs-lookup"><span data-stu-id="17171-134">Response</span></span>

<span data-ttu-id="17171-135">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [servicePrincipal](../resources/serviceprincipal.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="17171-135">If successful, this method returns a `200 OK` response code and collection of [servicePrincipal](../resources/serviceprincipal.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="17171-136">示例</span><span class="sxs-lookup"><span data-stu-id="17171-136">Examples</span></span>

### <a name="example-1-get-a-list-of-service-principals"></a><span data-ttu-id="17171-137">示例 1：获取服务主体列表</span><span class="sxs-lookup"><span data-stu-id="17171-137">Example 1: Get a list of service principals</span></span>

#### <a name="request"></a><span data-ttu-id="17171-138">请求</span><span class="sxs-lookup"><span data-stu-id="17171-138">Request</span></span>

<span data-ttu-id="17171-139">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="17171-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="17171-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="17171-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_serviceprincipal"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals
```
# <a name="c"></a>[<span data-ttu-id="17171-141">C#</span><span class="sxs-lookup"><span data-stu-id="17171-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="17171-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="17171-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="17171-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="17171-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="17171-144">Java</span><span class="sxs-lookup"><span data-stu-id="17171-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="17171-145">响应</span><span class="sxs-lookup"><span data-stu-id="17171-145">Response</span></span>

<span data-ttu-id="17171-146">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="17171-146">The following is an example of the response.</span></span>

><span data-ttu-id="17171-147">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="17171-147">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "accountEnabled":true,
      "displayName":"amasf",
      "servicePrincipalType":"Application",
      "signInAudience":"AzureADMyOrg"
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-service-principals"></a><span data-ttu-id="17171-148">示例 2：仅获取服务主体的计数</span><span class="sxs-lookup"><span data-stu-id="17171-148">Example 2: Get only a count of service principals</span></span>

#### <a name="request"></a><span data-ttu-id="17171-149">请求</span><span class="sxs-lookup"><span data-stu-id="17171-149">Request</span></span>

<span data-ttu-id="17171-150">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="17171-150">The following is an example of the request.</span></span> <span data-ttu-id="17171-151">此请求要求将 **ConsistencyLevel** 标头设置为 `eventual`，因为在请求中有 `$count`。</span><span class="sxs-lookup"><span data-stu-id="17171-151">This request requires the **ConsistencyLevel** header set to `eventual` because `$count` is in the request.</span></span> <span data-ttu-id="17171-152">有关使用 **ConsistencyLevel** 和 `$count` 的详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。</span><span class="sxs-lookup"><span data-stu-id="17171-152">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="17171-153">响应</span><span class="sxs-lookup"><span data-stu-id="17171-153">Response</span></span>

<span data-ttu-id="17171-154">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="17171-154">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

893
```

### <a name="example-3-use-filter-and-top-to-get-one-service-principal-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="17171-155">示例 3：使用 $filter 和 $top 获取一个显示名称以“a”开头的服务主体，其中包括返回的对象数</span><span class="sxs-lookup"><span data-stu-id="17171-155">Example 3: Use $filter and $top to get one service principal with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="17171-156">请求</span><span class="sxs-lookup"><span data-stu-id="17171-156">Request</span></span>

<span data-ttu-id="17171-157">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="17171-157">The following is an example of the request.</span></span> <span data-ttu-id="17171-158">此请求需要将 **ConsistencyLevel** 标头设置为 `eventual` 和 `$count=true` 查询字符串，因为请求同时具有 `$orderBy` 和 `$filter` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="17171-158">This request requires the **ConsistencyLevel** header set to `eventual` and the `$count=true` query string because the request has both the `$orderBy` and `$filter` query parameters.</span></span> <span data-ttu-id="17171-159">有关使用 **ConsistencyLevel** 和 `$count` 的详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。</span><span class="sxs-lookup"><span data-stu-id="17171-159">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="17171-160">响应</span><span class="sxs-lookup"><span data-stu-id="17171-160">Response</span></span>

<span data-ttu-id="17171-161">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="17171-161">The following is an example of the response.</span></span>

><span data-ttu-id="17171-162">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="17171-162">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#servicePrinciples",
  "@odata.count":1,
  "value":[
    {
      "accountEnabled":true,
      "displayName":"a",
      "servicePrincipalType":"Application",
      "signInAudience":"AzureADMyOrg"
    }
  ]
}
```

### <a name="example-4-use-search-to-get-service-principals-with-display-names-that-contain-the-letters-team-including-a-count-of-returned-objects"></a><span data-ttu-id="17171-163">示例 4：使用 $search 获取显示名称中包含字母“Team”的服务主体，其中包括返回的对象数</span><span class="sxs-lookup"><span data-stu-id="17171-163">Example 4: Use $search to get service principals with display names that contain the letters 'Team' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="17171-164">请求</span><span class="sxs-lookup"><span data-stu-id="17171-164">Request</span></span>

<span data-ttu-id="17171-165">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="17171-165">The following is an example of the request.</span></span> <span data-ttu-id="17171-166">此请求要求将 **ConsistencyLevel** 标头设置为`eventual`，因为在请求中有`$search`和`$count=true`查询字符串。</span><span class="sxs-lookup"><span data-stu-id="17171-166">This request requires the **ConsistencyLevel** header set to `eventual` because `$search` and the `$count=true` query string is in the request.</span></span> <span data-ttu-id="17171-167">有关使用 **ConsistencyLevel** 和 `$count` 的详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。</span><span class="sxs-lookup"><span data-stu-id="17171-167">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "request",
  "name": "get_team_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals?$search="displayName:Team"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="17171-168">响应</span><span class="sxs-lookup"><span data-stu-id="17171-168">Response</span></span>

<span data-ttu-id="17171-169">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="17171-169">The following is an example of the response.</span></span>

><span data-ttu-id="17171-170">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="17171-170">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#servicePrincipals",
  "@odata.count":1396,
  "value":[
    {
      "accountEnabled":true,
      "displayName":"myContosoTeam",
      "servicePrincipalType":"Application",
      "signInAudience":"AzureADMyOrg"
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List servicePrincipals",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
