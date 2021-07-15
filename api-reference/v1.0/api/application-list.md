---
title: 列出应用程序
description: 获取该组织中应用程序的列表。
author: sureshja
localization_priority: Priority
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 28eca7aee974f8fc60f4c6bd5db211429e3cde61
ms.sourcegitcommit: 6d247f44a6ee4d8515c3863ee8a2683163c9f829
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2021
ms.locfileid: "53430240"
---
# <a name="list-applications"></a><span data-ttu-id="79622-103">列出应用程序</span><span class="sxs-lookup"><span data-stu-id="79622-103">List applications</span></span>

<span data-ttu-id="79622-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79622-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="79622-105">获取该组织中[应用程序](../resources/application.md)的列表。</span><span class="sxs-lookup"><span data-stu-id="79622-105">Get the list of [applications](../resources/application.md) in this organization.</span></span>

> [!NOTE]
> <span data-ttu-id="79622-106">使用为个人 Microsoft 帐户颁发的令牌调用此 API 时，将返回个人 Microsoft 帐户所拥有的应用。</span><span class="sxs-lookup"><span data-stu-id="79622-106">When calling this API using tokens issued for a personal Microsoft account, it will return the apps owned by the personal Microsoft account.</span></span> <span data-ttu-id="79622-107">个人 Microsoft 帐户不存在组织概念。</span><span class="sxs-lookup"><span data-stu-id="79622-107">The notion of organizations doesn't exist for personal Microsoft accounts.</span></span> <span data-ttu-id="79622-108">为了列出特定个人 Microsoft 帐户所拥有的应用程序，此 API 需要用户。除 Application.Read.All 或 Application.ReadWrite.All 之外，还读取权限。</span><span class="sxs-lookup"><span data-stu-id="79622-108">In order to list applications owned by specific personal Microsoft accounts, this API requires User.Read permission in addition to Application.Read.All or Application.ReadWrite.All.</span></span>

## <a name="permissions"></a><span data-ttu-id="79622-109">权限</span><span class="sxs-lookup"><span data-stu-id="79622-109">Permissions</span></span>
<span data-ttu-id="79622-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="79622-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="79622-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="79622-112">Permission type</span></span>      | <span data-ttu-id="79622-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="79622-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="79622-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="79622-114">Delegated (work or school account)</span></span> | <span data-ttu-id="79622-115">Application.Read.All、 Application.ReadWrite.All、 Directory.Read.All、 Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="79622-115">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="79622-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="79622-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79622-117">Application.Read.All 和 User.Read， Application.ReadWrite.All 和 User.Read</span><span class="sxs-lookup"><span data-stu-id="79622-117">Application.Read.All and User.Read, Application.ReadWrite.All and User.Read</span></span> |
|<span data-ttu-id="79622-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="79622-118">Application</span></span> | <span data-ttu-id="79622-119">Application.Read.All、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="79622-119">Application.Read.All, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="79622-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="79622-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications
```
## <a name="optional-query-parameters"></a><span data-ttu-id="79622-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="79622-121">Optional query parameters</span></span>

<span data-ttu-id="79622-122">此方法支持使用 `$count`、`$expand`、`$filter`、`$orderBy`、`$search`、`$select` 和 `$top` [ OData 查询参数 ](/graph/query-parameters) 以帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="79622-122">This method supports the `$count`, `$expand`, `$filter`, `$orderBy`, `$search`, `$select`, and `$top` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span> <span data-ttu-id="79622-123">只有将 **ConsistencyLevel** 标头设置为 `eventual` 和 `$count` 时，才支持某些查询。</span><span class="sxs-lookup"><span data-stu-id="79622-123">Some queries are supported only when you use the **ConsistencyLevel** header set to `eventual` and `$count`.</span></span> <span data-ttu-id="79622-124">有关详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。</span><span class="sxs-lookup"><span data-stu-id="79622-124">For more information, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

## <a name="request-headers"></a><span data-ttu-id="79622-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="79622-125">Request headers</span></span>

| <span data-ttu-id="79622-126">名称</span><span class="sxs-lookup"><span data-stu-id="79622-126">Name</span></span>           | <span data-ttu-id="79622-127">说明</span><span class="sxs-lookup"><span data-stu-id="79622-127">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="79622-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="79622-128">Authorization</span></span>  | <span data-ttu-id="79622-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="79622-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="79622-131">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="79622-131">ConsistencyLevel</span></span> | <span data-ttu-id="79622-132">最终。</span><span class="sxs-lookup"><span data-stu-id="79622-132">eventual.</span></span> <span data-ttu-id="79622-133">当使用 `$search` 或 `$filter` 的特定用法时，需要此标头和 `$count`。</span><span class="sxs-lookup"><span data-stu-id="79622-133">This header and `$count` are required when using `$search`, or in specific usage of `$filter`.</span></span> <span data-ttu-id="79622-134">有关使用 **ConsistencyLevel** 和 `$count` 的详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。</span><span class="sxs-lookup"><span data-stu-id="79622-134">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span> |

## <a name="request-body"></a><span data-ttu-id="79622-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="79622-135">Request body</span></span>
<span data-ttu-id="79622-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="79622-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79622-137">响应</span><span class="sxs-lookup"><span data-stu-id="79622-137">Response</span></span>

<span data-ttu-id="79622-138">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [application](../resources/application.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="79622-138">If successful, this method returns a `200 OK` response code and a collection of [application](../resources/application.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="79622-139">示例</span><span class="sxs-lookup"><span data-stu-id="79622-139">Examples</span></span>

### <a name="example-1-get-the-list-of-applications"></a><span data-ttu-id="79622-140">示例 1：获取应用程序列表</span><span class="sxs-lookup"><span data-stu-id="79622-140">Example 1: Get the list of applications</span></span>

#### <a name="request"></a><span data-ttu-id="79622-141">请求</span><span class="sxs-lookup"><span data-stu-id="79622-141">Request</span></span>

<span data-ttu-id="79622-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="79622-142">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="79622-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="79622-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_application"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications
```
# <a name="c"></a>[<span data-ttu-id="79622-144">C#</span><span class="sxs-lookup"><span data-stu-id="79622-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="79622-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="79622-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="79622-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="79622-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="79622-147">Java</span><span class="sxs-lookup"><span data-stu-id="79622-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="79622-148">响应</span><span class="sxs-lookup"><span data-stu-id="79622-148">Response</span></span>

<span data-ttu-id="79622-149">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="79622-149">Here is an example of the response.</span></span>

> <span data-ttu-id="79622-150">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="79622-150">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#applications",
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

### <a name="example-2-get-only-a-count-of-applications"></a><span data-ttu-id="79622-151">示例 2：仅获取应用程序计数</span><span class="sxs-lookup"><span data-stu-id="79622-151">Example 2: Get only a count of applications</span></span>

#### <a name="request"></a><span data-ttu-id="79622-152">请求</span><span class="sxs-lookup"><span data-stu-id="79622-152">Request</span></span>

<span data-ttu-id="79622-153">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="79622-153">The following is an example of the request.</span></span> <span data-ttu-id="79622-154">此请求要求将 **ConsistencyLevel** 标头设置为 `eventual`，因为在请求中有 `$count`。</span><span class="sxs-lookup"><span data-stu-id="79622-154">This request requires the **ConsistencyLevel** header set to `eventual` because `$count` is in the request.</span></span> <span data-ttu-id="79622-155">有关使用 **ConsistencyLevel** 和 `$count` 的详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。</span><span class="sxs-lookup"><span data-stu-id="79622-155">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="79622-156">响应</span><span class="sxs-lookup"><span data-stu-id="79622-156">Response</span></span>

<span data-ttu-id="79622-157">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="79622-157">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

893
```


### <a name="example-3-use-filter-and-top-to-get-one-application-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="79622-158">示例 3：使用 $filter 和 $top 获取一个显示名称以“a”开头的应用程序，其中包括返回的对象数</span><span class="sxs-lookup"><span data-stu-id="79622-158">Example 3: Use $filter and $top to get one application with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="79622-159">请求</span><span class="sxs-lookup"><span data-stu-id="79622-159">Request</span></span>

<span data-ttu-id="79622-160">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="79622-160">The following is an example of the request.</span></span> <span data-ttu-id="79622-161">此请求需要将 **ConsistencyLevel** 标头设置为 `eventual` 和 `$count=true` 查询字符串，因为请求同时具有 `$orderBy` 和 `$filter` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="79622-161">This request requires the **ConsistencyLevel** header set to `eventual` and the `$count=true` query string because the request has both the `$orderBy` and `$filter` query parameters.</span></span> <span data-ttu-id="79622-162">有关使用 **ConsistencyLevel** 和 `$count` 的详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。</span><span class="sxs-lookup"><span data-stu-id="79622-162">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="79622-163">响应</span><span class="sxs-lookup"><span data-stu-id="79622-163">Response</span></span>

<span data-ttu-id="79622-164">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="79622-164">The following is an example of the response.</span></span>

><span data-ttu-id="79622-165">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="79622-165">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#applications",
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

### <a name="example-4-use-search-to-get-applications-with-display-names-that-contain-the-letters-web-including-a-count-of-returned-objects"></a><span data-ttu-id="79622-166">示例 4：使用 $search 获取显示名称中包含字母“Web”的应用程序，其中包括返回的对象数</span><span class="sxs-lookup"><span data-stu-id="79622-166">Example 4: Use $search to get applications with display names that contain the letters 'Web' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="79622-167">请求</span><span class="sxs-lookup"><span data-stu-id="79622-167">Request</span></span>

<span data-ttu-id="79622-168">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="79622-168">The following is an example of the request.</span></span> <span data-ttu-id="79622-169">此请求要求将 **ConsistencyLevel** 标头设置为`eventual`，因为在请求中有`$search`和`$count=true`查询字符串。</span><span class="sxs-lookup"><span data-stu-id="79622-169">This request requires the **ConsistencyLevel** header set to `eventual` because `$search` and the `$count=true` query string is in the request.</span></span> <span data-ttu-id="79622-170">有关使用 **ConsistencyLevel** 和 `$count` 的详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。</span><span class="sxs-lookup"><span data-stu-id="79622-170">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "request",
  "name": "get_web_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications?$search="displayName:Web"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="79622-171">响应</span><span class="sxs-lookup"><span data-stu-id="79622-171">Response</span></span>

<span data-ttu-id="79622-172">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="79622-172">The following is an example of the response.</span></span>

><span data-ttu-id="79622-173">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="79622-173">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#applications",
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
