---
title: 列出 servicePrincipals
description: 检索 servicePrincipal 对象列表。
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: edbd17d4730ead8e230eb7b3b38a547ac199e922
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2020
ms.locfileid: "44382669"
---
# <a name="list-serviceprincipals"></a><span data-ttu-id="69f6f-103">列出 servicePrincipals</span><span class="sxs-lookup"><span data-stu-id="69f6f-103">List servicePrincipals</span></span>

<span data-ttu-id="69f6f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69f6f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69f6f-105">检索[servicePrincipal](../resources/serviceprincipal.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="69f6f-105">Retrieve a list of [servicePrincipal](../resources/serviceprincipal.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="69f6f-106">权限</span><span class="sxs-lookup"><span data-stu-id="69f6f-106">Permissions</span></span>

<span data-ttu-id="69f6f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="69f6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="69f6f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="69f6f-109">Permission type</span></span> | <span data-ttu-id="69f6f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="69f6f-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="69f6f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="69f6f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="69f6f-112">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="69f6f-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="69f6f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="69f6f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69f6f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="69f6f-114">Not supported.</span></span> |
| <span data-ttu-id="69f6f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="69f6f-115">Application</span></span> | <span data-ttu-id="69f6f-116">Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="69f6f-116">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="69f6f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="69f6f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals
```

## <a name="optional-query-parameters"></a><span data-ttu-id="69f6f-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="69f6f-118">Optional query parameters</span></span>

<span data-ttu-id="69f6f-119">此方法支持[OData 查询参数](/graph/query_parameters)，以帮助自定义响应，包括 `$search` 、 `$count` 和 `$filter` 。</span><span class="sxs-lookup"><span data-stu-id="69f6f-119">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="69f6f-120">您可以 `$search` 在**displayName**属性上使用。</span><span class="sxs-lookup"><span data-stu-id="69f6f-120">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="69f6f-121">为此资源添加或更新项目时，将对其进行专门编制索引，以便 `$count` 与 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="69f6f-121">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="69f6f-122">在添加或更新项目以及在索引中可用时，可能会出现轻微的延迟。</span><span class="sxs-lookup"><span data-stu-id="69f6f-122">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="69f6f-123">请求头</span><span class="sxs-lookup"><span data-stu-id="69f6f-123">Request headers</span></span>

| <span data-ttu-id="69f6f-124">名称</span><span class="sxs-lookup"><span data-stu-id="69f6f-124">Name</span></span> | <span data-ttu-id="69f6f-125">说明</span><span class="sxs-lookup"><span data-stu-id="69f6f-125">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="69f6f-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="69f6f-126">Authorization</span></span> | <span data-ttu-id="69f6f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="69f6f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="69f6f-129">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="69f6f-129">ConsistencyLevel</span></span> | <span data-ttu-id="69f6f-130">仍然.</span><span class="sxs-lookup"><span data-stu-id="69f6f-130">eventual.</span></span> <span data-ttu-id="69f6f-131">此标头 `$count` 在使用时 `$search` 或在 `$filter` 与查询参数一起使用时是必需的 `$orderby` 。</span><span class="sxs-lookup"><span data-stu-id="69f6f-131">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="69f6f-132">它使用的索引可能不是最新的对象更改。</span><span class="sxs-lookup"><span data-stu-id="69f6f-132">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="69f6f-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="69f6f-133">Request body</span></span>

<span data-ttu-id="69f6f-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="69f6f-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="69f6f-135">响应</span><span class="sxs-lookup"><span data-stu-id="69f6f-135">Response</span></span>

<span data-ttu-id="69f6f-136">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[servicePrincipal](../resources/serviceprincipal.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="69f6f-136">If successful, this method returns a `200 OK` response code and collection of [servicePrincipal](../resources/serviceprincipal.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="69f6f-137">示例</span><span class="sxs-lookup"><span data-stu-id="69f6f-137">Examples</span></span>

### <a name="example-1-get-a-list-of-service-principals"></a><span data-ttu-id="69f6f-138">示例1：获取服务主体的列表</span><span class="sxs-lookup"><span data-stu-id="69f6f-138">Example 1: Get a list of service principals</span></span>

#### <a name="request"></a><span data-ttu-id="69f6f-139">请求</span><span class="sxs-lookup"><span data-stu-id="69f6f-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="69f6f-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="69f6f-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_serviceprincipal"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/serviceprincipals
```
# <a name="c"></a>[<span data-ttu-id="69f6f-141">C#</span><span class="sxs-lookup"><span data-stu-id="69f6f-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="69f6f-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="69f6f-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="69f6f-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="69f6f-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="69f6f-144">响应</span><span class="sxs-lookup"><span data-stu-id="69f6f-144">Response</span></span>

<span data-ttu-id="69f6f-145">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="69f6f-145">The following is an example of the response.</span></span>
><span data-ttu-id="69f6f-146">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="69f6f-146">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="69f6f-147">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="69f6f-147">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-service-principals"></a><span data-ttu-id="69f6f-148">示例2：仅获取服务主体的计数</span><span class="sxs-lookup"><span data-stu-id="69f6f-148">Example 2: Get only a count of service principals</span></span>

#### <a name="request"></a><span data-ttu-id="69f6f-149">请求</span><span class="sxs-lookup"><span data-stu-id="69f6f-149">Request</span></span>

<span data-ttu-id="69f6f-150">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="69f6f-150">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="69f6f-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="69f6f-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="69f6f-152">C#</span><span class="sxs-lookup"><span data-stu-id="69f6f-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="69f6f-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="69f6f-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="69f6f-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="69f6f-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="69f6f-155">响应</span><span class="sxs-lookup"><span data-stu-id="69f6f-155">Response</span></span>

<span data-ttu-id="69f6f-156">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="69f6f-156">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

<span data-ttu-id="69f6f-157">893</span><span class="sxs-lookup"><span data-stu-id="69f6f-157">893</span></span>


### <a name="example-3-use-filter-and-top-to-get-one-service-principal-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="69f6f-158">示例3：使用 $filter 和 $top 获取一个具有以 "a" 开头的显示名称的服务主体，其中包含返回对象的计数</span><span class="sxs-lookup"><span data-stu-id="69f6f-158">Example 3: Use $filter and $top to get one service principal with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="69f6f-159">请求</span><span class="sxs-lookup"><span data-stu-id="69f6f-159">Request</span></span>

<span data-ttu-id="69f6f-160">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="69f6f-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="69f6f-161">响应</span><span class="sxs-lookup"><span data-stu-id="69f6f-161">Response</span></span>

<span data-ttu-id="69f6f-162">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="69f6f-162">The following is an example of the response.</span></span>
><span data-ttu-id="69f6f-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="69f6f-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-4-use-search-to-get-service-principals-with-display-names-that-contain-the-letters-team-including-a-count-of-returned-objects"></a><span data-ttu-id="69f6f-165">示例4：使用 $search 获取显示名称包含字母 "Team" 的服务主体，其中包括返回对象的计数</span><span class="sxs-lookup"><span data-stu-id="69f6f-165">Example 4: Use $search to get service principals with display names that contain the letters 'Team' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="69f6f-166">请求</span><span class="sxs-lookup"><span data-stu-id="69f6f-166">Request</span></span>

<span data-ttu-id="69f6f-167">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="69f6f-167">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="69f6f-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="69f6f-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_team_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals?$search="displayName:Team"&$count=true
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="69f6f-169">C#</span><span class="sxs-lookup"><span data-stu-id="69f6f-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-team-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="69f6f-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="69f6f-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-team-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="69f6f-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="69f6f-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-team-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="69f6f-172">响应</span><span class="sxs-lookup"><span data-stu-id="69f6f-172">Response</span></span>

<span data-ttu-id="69f6f-173">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="69f6f-173">The following is an example of the response.</span></span>
><span data-ttu-id="69f6f-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="69f6f-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
