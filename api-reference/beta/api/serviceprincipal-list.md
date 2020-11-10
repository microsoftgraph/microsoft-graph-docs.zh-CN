---
title: List servicePrincipals
description: 检索 servicePrincipal 对象列表。
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 966ffa2fee35edbc0c6b6efec2562b43f470446c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979706"
---
# <a name="list-serviceprincipals"></a><span data-ttu-id="207df-103">List servicePrincipals</span><span class="sxs-lookup"><span data-stu-id="207df-103">List servicePrincipals</span></span>

<span data-ttu-id="207df-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="207df-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="207df-105">检索 [servicePrincipal](../resources/serviceprincipal.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="207df-105">Retrieve a list of [servicePrincipal](../resources/serviceprincipal.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="207df-106">权限</span><span class="sxs-lookup"><span data-stu-id="207df-106">Permissions</span></span>

<span data-ttu-id="207df-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="207df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="207df-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="207df-109">Permission type</span></span> | <span data-ttu-id="207df-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="207df-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="207df-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="207df-111">Delegated (work or school account)</span></span> | <span data-ttu-id="207df-112">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="207df-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="207df-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="207df-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="207df-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="207df-114">Not supported.</span></span> |
| <span data-ttu-id="207df-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="207df-115">Application</span></span> | <span data-ttu-id="207df-116">Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="207df-116">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="207df-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="207df-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals
```

## <a name="optional-query-parameters"></a><span data-ttu-id="207df-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="207df-118">Optional query parameters</span></span>

<span data-ttu-id="207df-p102">此方法支持使用 [OData 查询参数](/graph/query_parameters)来帮助自定义响应，包括 `$search`、`$count` 和 `$filter`。你可以在 **displayName** 属性上使用 `$search`。为该资源添加或更新项目时，将为它们专门创建索引，以与 `$count` 和 `$search` 查询参数一起使用。添加或更新项目与项目在索引中可用之间可能会稍有延迟。</span><span class="sxs-lookup"><span data-stu-id="207df-p102">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`. You can use `$search` on the **displayName** property. When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters. There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="207df-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="207df-123">Request headers</span></span>

| <span data-ttu-id="207df-124">名称</span><span class="sxs-lookup"><span data-stu-id="207df-124">Name</span></span> | <span data-ttu-id="207df-125">说明</span><span class="sxs-lookup"><span data-stu-id="207df-125">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="207df-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="207df-126">Authorization</span></span> | <span data-ttu-id="207df-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="207df-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="207df-129">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="207df-129">ConsistencyLevel</span></span> | <span data-ttu-id="207df-p104">最终。使用 `$search` 或将 `$filter` 与 `$orderby` 查询参数一起使用时，必须提供此标头和 `$count`。它使用的索引可能未根据该对象的最新更改及时更新。</span><span class="sxs-lookup"><span data-stu-id="207df-p104">eventual. This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter. It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="207df-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="207df-133">Request body</span></span>

<span data-ttu-id="207df-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="207df-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="207df-135">响应</span><span class="sxs-lookup"><span data-stu-id="207df-135">Response</span></span>

<span data-ttu-id="207df-136">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [servicePrincipal](../resources/serviceprincipal.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="207df-136">If successful, this method returns a `200 OK` response code and collection of [servicePrincipal](../resources/serviceprincipal.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="207df-137">示例</span><span class="sxs-lookup"><span data-stu-id="207df-137">Examples</span></span>

### <a name="example-1-get-a-list-of-service-principals"></a><span data-ttu-id="207df-138">示例 1：获取服务主体列表</span><span class="sxs-lookup"><span data-stu-id="207df-138">Example 1: Get a list of service principals</span></span>

#### <a name="request"></a><span data-ttu-id="207df-139">请求</span><span class="sxs-lookup"><span data-stu-id="207df-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="207df-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="207df-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_serviceprincipal"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/serviceprincipals
```
# <a name="c"></a>[<span data-ttu-id="207df-141">C#</span><span class="sxs-lookup"><span data-stu-id="207df-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="207df-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="207df-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="207df-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="207df-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="207df-144">Java</span><span class="sxs-lookup"><span data-stu-id="207df-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="207df-145">响应</span><span class="sxs-lookup"><span data-stu-id="207df-145">Response</span></span>

<span data-ttu-id="207df-146">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="207df-146">The following is an example of the response.</span></span>
><span data-ttu-id="207df-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="207df-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-service-principals"></a><span data-ttu-id="207df-149">示例 2：仅获取服务主体的计数</span><span class="sxs-lookup"><span data-stu-id="207df-149">Example 2: Get only a count of service principals</span></span>

#### <a name="request"></a><span data-ttu-id="207df-150">请求</span><span class="sxs-lookup"><span data-stu-id="207df-150">Request</span></span>

<span data-ttu-id="207df-151">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="207df-151">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="207df-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="207df-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="207df-153">C#</span><span class="sxs-lookup"><span data-stu-id="207df-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="207df-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="207df-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="207df-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="207df-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="207df-156">Java</span><span class="sxs-lookup"><span data-stu-id="207df-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-count-only-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="207df-157">响应</span><span class="sxs-lookup"><span data-stu-id="207df-157">Response</span></span>

<span data-ttu-id="207df-158">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="207df-158">The following is an example of the response.</span></span>

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

<span data-ttu-id="207df-159">893</span><span class="sxs-lookup"><span data-stu-id="207df-159">893</span></span>


### <a name="example-3-use-filter-and-top-to-get-one-service-principal-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="207df-160">示例 3：使用 $filter 和 $top 获取一个显示名称以“a”开头的服务主体，其中包括返回的对象数</span><span class="sxs-lookup"><span data-stu-id="207df-160">Example 3: Use $filter and $top to get one service principal with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="207df-161">请求</span><span class="sxs-lookup"><span data-stu-id="207df-161">Request</span></span>

<span data-ttu-id="207df-162">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="207df-162">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="207df-163">响应</span><span class="sxs-lookup"><span data-stu-id="207df-163">Response</span></span>

<span data-ttu-id="207df-164">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="207df-164">The following is an example of the response.</span></span>
><span data-ttu-id="207df-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="207df-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-4-use-search-to-get-service-principals-with-display-names-that-contain-the-letters-team-including-a-count-of-returned-objects"></a><span data-ttu-id="207df-167">示例 4：使用 $search 获取显示名称中包含字母“Team”的服务主体，其中包括返回的对象数</span><span class="sxs-lookup"><span data-stu-id="207df-167">Example 4: Use $search to get service principals with display names that contain the letters 'Team' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="207df-168">请求</span><span class="sxs-lookup"><span data-stu-id="207df-168">Request</span></span>

<span data-ttu-id="207df-169">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="207df-169">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="207df-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="207df-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_team_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals?$search="displayName:Team"&$count=true
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="207df-171">C#</span><span class="sxs-lookup"><span data-stu-id="207df-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-team-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="207df-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="207df-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-team-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="207df-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="207df-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-team-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="207df-174">Java</span><span class="sxs-lookup"><span data-stu-id="207df-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-team-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="207df-175">响应</span><span class="sxs-lookup"><span data-stu-id="207df-175">Response</span></span>

<span data-ttu-id="207df-176">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="207df-176">The following is an example of the response.</span></span>
><span data-ttu-id="207df-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="207df-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


