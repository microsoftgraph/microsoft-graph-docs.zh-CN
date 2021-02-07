---
title: List servicePrincipals
description: 检索 servicePrincipal 对象列表。
author: sureshja
localization_priority: Priority
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 70e7bdde1261d26ae62712964223d724cba971dc
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134461"
---
# <a name="list-serviceprincipals"></a><span data-ttu-id="49540-103">List servicePrincipals</span><span class="sxs-lookup"><span data-stu-id="49540-103">List servicePrincipals</span></span>

<span data-ttu-id="49540-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49540-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="49540-105">检索 [servicePrincipal](../resources/serviceprincipal.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="49540-105">Retrieve a list of [servicePrincipal](../resources/serviceprincipal.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="49540-106">权限</span><span class="sxs-lookup"><span data-stu-id="49540-106">Permissions</span></span>

<span data-ttu-id="49540-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="49540-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49540-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="49540-109">Permission type</span></span>      | <span data-ttu-id="49540-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="49540-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49540-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="49540-111">Delegated (work or school account)</span></span> | <span data-ttu-id="49540-112">Application.Read.All、Application.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="49540-112">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="49540-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="49540-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49540-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="49540-114">Not supported.</span></span>    |
|<span data-ttu-id="49540-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="49540-115">Application</span></span> | <span data-ttu-id="49540-116">Application.Read.All、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="49540-116">Application.Read.All, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="49540-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="49540-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals
```
## <a name="optional-query-parameters"></a><span data-ttu-id="49540-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="49540-118">Optional query parameters</span></span>

<span data-ttu-id="49540-119">此方法支持[OData query parameters](/graph/query-parameters)以帮助自定义响应，包括 `$search`、`$count`、 和 `$filter`</span><span class="sxs-lookup"><span data-stu-id="49540-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="49540-120">`$search`可以用在 **displayName** 属性。</span><span class="sxs-lookup"><span data-stu-id="49540-120">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="49540-121">为该资源添加或更新项目时，将对它们进行专门索引，以便与 `$count` 和 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="49540-121">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="49540-122">在添加或更新项目与在索引中可用之间可能会稍有延迟。</span><span class="sxs-lookup"><span data-stu-id="49540-122">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="49540-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="49540-123">Request headers</span></span>
| <span data-ttu-id="49540-124">名称</span><span class="sxs-lookup"><span data-stu-id="49540-124">Name</span></span>           | <span data-ttu-id="49540-125">说明</span><span class="sxs-lookup"><span data-stu-id="49540-125">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="49540-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="49540-126">Authorization</span></span>  | <span data-ttu-id="49540-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="49540-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="49540-129">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="49540-129">ConsistencyLevel</span></span> | <span data-ttu-id="49540-130">最终。</span><span class="sxs-lookup"><span data-stu-id="49540-130">eventual.</span></span> <span data-ttu-id="49540-131">当使用 `$search` 或将 `$filter` 与 `$orderby` 查询参数一起使用时，此标头和 `$count` 是必需的。</span><span class="sxs-lookup"><span data-stu-id="49540-131">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="49540-132">它使用的索引可能与对象的最新更改不同步。</span><span class="sxs-lookup"><span data-stu-id="49540-132">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="49540-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="49540-133">Request body</span></span>

<span data-ttu-id="49540-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="49540-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="49540-135">响应</span><span class="sxs-lookup"><span data-stu-id="49540-135">Response</span></span>

<span data-ttu-id="49540-136">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [servicePrincipal](../resources/serviceprincipal.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="49540-136">If successful, this method returns a `200 OK` response code and collection of [servicePrincipal](../resources/serviceprincipal.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="49540-137">示例</span><span class="sxs-lookup"><span data-stu-id="49540-137">Examples</span></span>

### <a name="example-1-get-a-list-of-service-principals"></a><span data-ttu-id="49540-138">示例 1：获取服务主体列表</span><span class="sxs-lookup"><span data-stu-id="49540-138">Example 1: Get a list of service principals</span></span>

#### <a name="request"></a><span data-ttu-id="49540-139">请求</span><span class="sxs-lookup"><span data-stu-id="49540-139">Request</span></span>

<span data-ttu-id="49540-140">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="49540-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="49540-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="49540-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_serviceprincipal"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals
```
# <a name="c"></a>[<span data-ttu-id="49540-142">C#</span><span class="sxs-lookup"><span data-stu-id="49540-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="49540-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="49540-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="49540-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="49540-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="49540-145">Java</span><span class="sxs-lookup"><span data-stu-id="49540-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="49540-146">响应</span><span class="sxs-lookup"><span data-stu-id="49540-146">Response</span></span>

<span data-ttu-id="49540-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="49540-147">The following is an example of the response.</span></span>

><span data-ttu-id="49540-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="49540-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "publisherName":"Contoso",
      "servicePrincipalType":"Application",
      "signInAudience":"AzureADMyOrg"
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-service-principals"></a><span data-ttu-id="49540-150">示例 2：仅获取服务主体的计数</span><span class="sxs-lookup"><span data-stu-id="49540-150">Example 2: Get only a count of service principals</span></span>

#### <a name="request"></a><span data-ttu-id="49540-151">请求</span><span class="sxs-lookup"><span data-stu-id="49540-151">Request</span></span>

<span data-ttu-id="49540-152">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="49540-152">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="49540-153">响应</span><span class="sxs-lookup"><span data-stu-id="49540-153">Response</span></span>

<span data-ttu-id="49540-154">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="49540-154">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`893`

### <a name="example-3-use-filter-and-top-to-get-one-service-principal-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="49540-155">示例 3：使用 $filter 和 $top 获取一个显示名称以“a”开头的服务主体，其中包括返回的对象数</span><span class="sxs-lookup"><span data-stu-id="49540-155">Example 3: Use $filter and $top to get one service principal with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="49540-156">请求</span><span class="sxs-lookup"><span data-stu-id="49540-156">Request</span></span>

<span data-ttu-id="49540-157">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="49540-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="49540-158">响应</span><span class="sxs-lookup"><span data-stu-id="49540-158">Response</span></span>

<span data-ttu-id="49540-159">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="49540-159">The following is an example of the response.</span></span>

><span data-ttu-id="49540-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="49540-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "publisherName":"Contoso",
      "servicePrincipalType":"Application",
      "signInAudience":"AzureADMyOrg"
    }
  ]
}
```

### <a name="example-4-use-search-to-get-service-principals-with-display-names-that-contain-the-letters-team-including-a-count-of-returned-objects"></a><span data-ttu-id="49540-162">示例 4：使用 $search 获取显示名称中包含字母“Team”的服务主体，其中包括返回的对象数</span><span class="sxs-lookup"><span data-stu-id="49540-162">Example 4: Use $search to get service principals with display names that contain the letters 'Team' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="49540-163">请求</span><span class="sxs-lookup"><span data-stu-id="49540-163">Request</span></span>

<span data-ttu-id="49540-164">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="49540-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_team_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals?$search="displayName:Team"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="49540-165">响应</span><span class="sxs-lookup"><span data-stu-id="49540-165">Response</span></span>

<span data-ttu-id="49540-166">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="49540-166">The following is an example of the response.</span></span>

><span data-ttu-id="49540-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="49540-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "publisherName":"Contoso",
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
