---
title: 列出应用程序
description: 获取该组织中应用程序的列表。
author: sureshja
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2517a88aa136851c33595697c5b67548ffc836a1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47996848"
---
# <a name="list-applications"></a><span data-ttu-id="e02e6-103">列出应用程序</span><span class="sxs-lookup"><span data-stu-id="e02e6-103">List applications</span></span>

<span data-ttu-id="e02e6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e02e6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e02e6-105">获取该组织中[应用程序](../resources/application.md)的列表。</span><span class="sxs-lookup"><span data-stu-id="e02e6-105">Get the list of [applications](../resources/application.md) in this organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="e02e6-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="e02e6-106">Permissions</span></span>

<span data-ttu-id="e02e6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e02e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e02e6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e02e6-109">Permission type</span></span> | <span data-ttu-id="e02e6-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e02e6-110">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="e02e6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e02e6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e02e6-112">Application.Read.All、Application.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e02e6-112">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
| <span data-ttu-id="e02e6-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e02e6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e02e6-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e02e6-114">Not supported.</span></span> |
| <span data-ttu-id="e02e6-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e02e6-115">Application</span></span> | <span data-ttu-id="e02e6-116">Application.Read.All、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="e02e6-116">Application.Read.All, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e02e6-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e02e6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /applications
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e02e6-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e02e6-118">Optional query parameters</span></span>

<span data-ttu-id="e02e6-119">此方法支持[OData query parameters](/graph/query-parameters)以帮助自定义响应，包括 `$search`、`$count`、 和 `$filter`</span><span class="sxs-lookup"><span data-stu-id="e02e6-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="e02e6-120">`$search`可以用在 **displayName**属性。</span><span class="sxs-lookup"><span data-stu-id="e02e6-120">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="e02e6-121">为该资源添加或更新项目时，将对它们进行专门索引，以便与 `$count` 和 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="e02e6-121">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="e02e6-122">在添加或更新项目与在索引中可用之间可能会稍有延迟。</span><span class="sxs-lookup"><span data-stu-id="e02e6-122">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e02e6-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="e02e6-123">Request headers</span></span>

| <span data-ttu-id="e02e6-124">名称</span><span class="sxs-lookup"><span data-stu-id="e02e6-124">Name</span></span> | <span data-ttu-id="e02e6-125">说明</span><span class="sxs-lookup"><span data-stu-id="e02e6-125">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="e02e6-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="e02e6-126">Authorization</span></span>  | <span data-ttu-id="e02e6-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e02e6-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e02e6-129">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="e02e6-129">ConsistencyLevel</span></span> | <span data-ttu-id="e02e6-130">最终。</span><span class="sxs-lookup"><span data-stu-id="e02e6-130">eventual.</span></span> <span data-ttu-id="e02e6-131">当使用 `$search` 或将 `$filter` 与 `$orderby` 查询参数一起使用时，此标头和 `$count` 是必需的。</span><span class="sxs-lookup"><span data-stu-id="e02e6-131">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="e02e6-132">它使用的索引可能与对象的最新更改不同步。</span><span class="sxs-lookup"><span data-stu-id="e02e6-132">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e02e6-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="e02e6-133">Request body</span></span>

<span data-ttu-id="e02e6-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e02e6-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e02e6-135">响应</span><span class="sxs-lookup"><span data-stu-id="e02e6-135">Response</span></span>

<span data-ttu-id="e02e6-136">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [application](../resources/application.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e02e6-136">If successful, this method returns a `200 OK` response code and a collection of [application](../resources/application.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e02e6-137">示例</span><span class="sxs-lookup"><span data-stu-id="e02e6-137">Examples</span></span>

### <a name="example-1-get-the-list-of-applications"></a><span data-ttu-id="e02e6-138">示例 1：获取应用程序列表</span><span class="sxs-lookup"><span data-stu-id="e02e6-138">Example 1: Get the list of applications</span></span>

#### <a name="request"></a><span data-ttu-id="e02e6-139">请求</span><span class="sxs-lookup"><span data-stu-id="e02e6-139">Request</span></span>

<span data-ttu-id="e02e6-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e02e6-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e02e6-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="e02e6-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_application"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/applications
```
# <a name="c"></a>[<span data-ttu-id="e02e6-142">C#</span><span class="sxs-lookup"><span data-stu-id="e02e6-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e02e6-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e02e6-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e02e6-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e02e6-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="e02e6-145">响应</span><span class="sxs-lookup"><span data-stu-id="e02e6-145">Response</span></span>

<span data-ttu-id="e02e6-146">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e02e6-146">Here is an example of the response.</span></span>
> <span data-ttu-id="e02e6-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e02e6-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#applications",
  "value": [
    {
      "appId": "00000000-0000-0000-0000-000000000000",
      "identifierUris": [ "http://contoso/" ],
      "displayName": "My app",
      "publisherDomain": "contoso.com",
      "signInAudience": "AzureADMyOrg"
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-applications"></a><span data-ttu-id="e02e6-149">示例 2：仅获取应用程序计数</span><span class="sxs-lookup"><span data-stu-id="e02e6-149">Example 2: Get only a count of applications</span></span>

#### <a name="request"></a><span data-ttu-id="e02e6-150">请求</span><span class="sxs-lookup"><span data-stu-id="e02e6-150">Request</span></span>

<span data-ttu-id="e02e6-151">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e02e6-151">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e02e6-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="e02e6-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/applications/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="e02e6-153">C#</span><span class="sxs-lookup"><span data-stu-id="e02e6-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e02e6-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e02e6-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e02e6-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e02e6-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e02e6-156">响应</span><span class="sxs-lookup"><span data-stu-id="e02e6-156">Response</span></span>

<span data-ttu-id="e02e6-157">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e02e6-157">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

<span data-ttu-id="e02e6-158">893</span><span class="sxs-lookup"><span data-stu-id="e02e6-158">893</span></span>


### <a name="example-3-use-filter-and-top-to-get-one-application-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="e02e6-159">示例 3：使用 $filter 和 $top 获取一个显示名称以“a”开头的应用程序，其中包括返回的对象数</span><span class="sxs-lookup"><span data-stu-id="e02e6-159">Example 3: Use $filter and $top to get one application with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="e02e6-160">请求</span><span class="sxs-lookup"><span data-stu-id="e02e6-160">Request</span></span>

<span data-ttu-id="e02e6-161">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e02e6-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/applications?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="e02e6-162">响应</span><span class="sxs-lookup"><span data-stu-id="e02e6-162">Response</span></span>

<span data-ttu-id="e02e6-163">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e02e6-163">The following is an example of the response.</span></span>
><span data-ttu-id="e02e6-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e02e6-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#applications",
  "@odata.count":1,
  "value":[
    {
      "appId": "00000000-0000-0000-0000-000000000000",
      "identifierUris": [ "http://contoso/" ],
      "displayName":"a",
      "publisherDomain": "contoso.com",
      "signInAudience": "AzureADMyOrg"
    }
  ]
}
```

### <a name="example-4-use-search-to-get-applications-with-display-names-that-contain-the-letters-web-including-a-count-of-returned-objects"></a><span data-ttu-id="e02e6-166">示例 4：使用 $search 获取显示名称中包含字母“Web”的应用程序，其中包括返回的对象数</span><span class="sxs-lookup"><span data-stu-id="e02e6-166">Example 4: Use $search to get applications with display names that contain the letters 'Web' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="e02e6-167">请求</span><span class="sxs-lookup"><span data-stu-id="e02e6-167">Request</span></span>

<span data-ttu-id="e02e6-168">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e02e6-168">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e02e6-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="e02e6-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_web_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/applications?$search="displayName:Web"&$count=true
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="e02e6-170">C#</span><span class="sxs-lookup"><span data-stu-id="e02e6-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-web-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e02e6-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e02e6-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-web-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e02e6-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e02e6-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-web-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e02e6-173">响应</span><span class="sxs-lookup"><span data-stu-id="e02e6-173">Response</span></span>

<span data-ttu-id="e02e6-174">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e02e6-174">The following is an example of the response.</span></span>
><span data-ttu-id="e02e6-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e02e6-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#applications",
  "@odata.count":1396,
  "value":[
    {
      "appId": "00000000-0000-0000-0000-000000000000",
      "identifierUris": [ "http://contoso/" ],
      "displayName":"'DotNetWeb-App' ",
      "publisherDomain": "contoso.com",
      "signInAudience": "AzureADMyOrg"
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List applications",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


