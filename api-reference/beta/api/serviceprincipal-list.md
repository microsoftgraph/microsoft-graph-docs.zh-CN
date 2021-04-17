---
title: List servicePrincipals
description: 检索 servicePrincipal 对象列表。
localization_priority: Priority
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 71f78ef680f3904f8be3026598bf80b27e4642c4
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882619"
---
# <a name="list-serviceprincipals"></a><span data-ttu-id="2399c-103">List servicePrincipals</span><span class="sxs-lookup"><span data-stu-id="2399c-103">List servicePrincipals</span></span>

<span data-ttu-id="2399c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2399c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2399c-105">检索 [servicePrincipal](../resources/serviceprincipal.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="2399c-105">Retrieve a list of [servicePrincipal](../resources/serviceprincipal.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="2399c-106">权限</span><span class="sxs-lookup"><span data-stu-id="2399c-106">Permissions</span></span>

<span data-ttu-id="2399c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2399c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2399c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2399c-109">Permission type</span></span> | <span data-ttu-id="2399c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2399c-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="2399c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2399c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2399c-112">Application.Read.All、Application.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2399c-112">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="2399c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2399c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2399c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2399c-114">Not supported.</span></span> |
| <span data-ttu-id="2399c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2399c-115">Application</span></span> | <span data-ttu-id="2399c-116">Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="2399c-116">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2399c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2399c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2399c-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2399c-118">Optional query parameters</span></span>

<span data-ttu-id="2399c-119">此方法支持[OData query parameters](/graph/query_parameters)以帮助自定义响应，包括 `$search`、`$count`、 和 `$filter`</span><span class="sxs-lookup"><span data-stu-id="2399c-119">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="2399c-120">`$search`可以用在 **displayName** 属性。</span><span class="sxs-lookup"><span data-stu-id="2399c-120">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="2399c-121">为该资源添加或更新项目时，将对它们进行专门索引，以便与 `$count` 和 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="2399c-121">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="2399c-122">在添加或更新项目与在索引中可用之间可能会稍有延迟。</span><span class="sxs-lookup"><span data-stu-id="2399c-122">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2399c-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="2399c-123">Request headers</span></span>

| <span data-ttu-id="2399c-124">名称</span><span class="sxs-lookup"><span data-stu-id="2399c-124">Name</span></span> | <span data-ttu-id="2399c-125">说明</span><span class="sxs-lookup"><span data-stu-id="2399c-125">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="2399c-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="2399c-126">Authorization</span></span> | <span data-ttu-id="2399c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2399c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2399c-129">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="2399c-129">ConsistencyLevel</span></span> | <span data-ttu-id="2399c-130">最终。</span><span class="sxs-lookup"><span data-stu-id="2399c-130">eventual.</span></span> <span data-ttu-id="2399c-131">当使用 `$search` 或将 `$filter` 与 `$orderby` 查询参数一起使用时，此标头和 `$count` 是必需的。</span><span class="sxs-lookup"><span data-stu-id="2399c-131">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="2399c-132">它使用的索引可能与对象的最新更改不同步。</span><span class="sxs-lookup"><span data-stu-id="2399c-132">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2399c-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="2399c-133">Request body</span></span>

<span data-ttu-id="2399c-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2399c-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2399c-135">响应</span><span class="sxs-lookup"><span data-stu-id="2399c-135">Response</span></span>

<span data-ttu-id="2399c-136">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [servicePrincipal](../resources/serviceprincipal.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="2399c-136">If successful, this method returns a `200 OK` response code and collection of [servicePrincipal](../resources/serviceprincipal.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2399c-137">示例</span><span class="sxs-lookup"><span data-stu-id="2399c-137">Examples</span></span>

### <a name="example-1-get-a-list-of-service-principals"></a><span data-ttu-id="2399c-138">示例 1：获取服务主体列表</span><span class="sxs-lookup"><span data-stu-id="2399c-138">Example 1: Get a list of service principals</span></span>

#### <a name="request"></a><span data-ttu-id="2399c-139">请求</span><span class="sxs-lookup"><span data-stu-id="2399c-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="2399c-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="2399c-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_serviceprincipal"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals
```
# <a name="c"></a>[<span data-ttu-id="2399c-141">C#</span><span class="sxs-lookup"><span data-stu-id="2399c-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2399c-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2399c-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2399c-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2399c-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2399c-144">Java</span><span class="sxs-lookup"><span data-stu-id="2399c-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2399c-145">响应</span><span class="sxs-lookup"><span data-stu-id="2399c-145">Response</span></span>

<span data-ttu-id="2399c-146">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2399c-146">The following is an example of the response.</span></span>
><span data-ttu-id="2399c-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="2399c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-service-principals"></a><span data-ttu-id="2399c-149">示例 2：仅获取服务主体的计数</span><span class="sxs-lookup"><span data-stu-id="2399c-149">Example 2: Get only a count of service principals</span></span>

#### <a name="request"></a><span data-ttu-id="2399c-150">请求</span><span class="sxs-lookup"><span data-stu-id="2399c-150">Request</span></span>

<span data-ttu-id="2399c-151">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2399c-151">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="2399c-152">响应</span><span class="sxs-lookup"><span data-stu-id="2399c-152">Response</span></span>

<span data-ttu-id="2399c-153">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2399c-153">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

893
```

### <a name="example-3-use-filter-and-top-to-get-one-service-principal-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="2399c-154">示例 3：使用 $filter 和 $top 获取一个显示名称以“a”开头的服务主体，其中包括返回的对象数</span><span class="sxs-lookup"><span data-stu-id="2399c-154">Example 3: Use $filter and $top to get one service principal with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="2399c-155">请求</span><span class="sxs-lookup"><span data-stu-id="2399c-155">Request</span></span>

<span data-ttu-id="2399c-156">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2399c-156">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="2399c-157">响应</span><span class="sxs-lookup"><span data-stu-id="2399c-157">Response</span></span>

<span data-ttu-id="2399c-158">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2399c-158">The following is an example of the response.</span></span>
><span data-ttu-id="2399c-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="2399c-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#servicePrinciples",
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

### <a name="example-4-use-search-to-get-service-principals-with-display-names-that-contain-the-letters-team-including-a-count-of-returned-objects"></a><span data-ttu-id="2399c-161">示例 4：使用 $search 获取显示名称中包含字母“Team”的服务主体，其中包括返回的对象数</span><span class="sxs-lookup"><span data-stu-id="2399c-161">Example 4: Use $search to get service principals with display names that contain the letters 'Team' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="2399c-162">请求</span><span class="sxs-lookup"><span data-stu-id="2399c-162">Request</span></span>

<span data-ttu-id="2399c-163">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2399c-163">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_team_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals?$search="displayName:Team"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="2399c-164">响应</span><span class="sxs-lookup"><span data-stu-id="2399c-164">Response</span></span>

<span data-ttu-id="2399c-165">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2399c-165">The following is an example of the response.</span></span>
><span data-ttu-id="2399c-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="2399c-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#servicePrincipals",
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



