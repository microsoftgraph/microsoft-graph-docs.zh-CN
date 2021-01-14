---
title: 列出应用程序
description: 获取该组织中应用程序的列表。
author: sureshja
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0f27f917e2fcf2f7f7ae00738ae22a5d9c2bdd5f
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844809"
---
# <a name="list-applications"></a><span data-ttu-id="a23e5-103">列出应用程序</span><span class="sxs-lookup"><span data-stu-id="a23e5-103">List applications</span></span>

<span data-ttu-id="a23e5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a23e5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a23e5-105">获取该组织中[应用程序](../resources/application.md)的列表。</span><span class="sxs-lookup"><span data-stu-id="a23e5-105">Get the list of [applications](../resources/application.md) in this organization.</span></span>

> [!NOTE]
> <span data-ttu-id="a23e5-106">使用为个人 Microsoft 帐户颁发的令牌调用此 API 时，将返回个人 Microsoft 帐户所拥有的应用。</span><span class="sxs-lookup"><span data-stu-id="a23e5-106">When calling this API using tokens issued for a personal Microsoft account, it will return the apps owned by the personal Microsoft account.</span></span> <span data-ttu-id="a23e5-107">个人 Microsoft 帐户不存在组织概念。</span><span class="sxs-lookup"><span data-stu-id="a23e5-107">The notion of organizations doesn't exist for personal Microsoft accounts.</span></span> <span data-ttu-id="a23e5-108">为了列出特定个人 Microsoft 帐户所拥有的应用程序，此 API 需要用户。除 Application.Read.All 或 Application.ReadWrite.All 之外，还读取权限。</span><span class="sxs-lookup"><span data-stu-id="a23e5-108">In order to list applications owned by specific personal Microsoft accounts, this API requires User.Read permission in addition to Application.Read.All or Application.ReadWrite.All.</span></span>

## <a name="permissions"></a><span data-ttu-id="a23e5-109">权限</span><span class="sxs-lookup"><span data-stu-id="a23e5-109">Permissions</span></span>
<span data-ttu-id="a23e5-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a23e5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a23e5-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="a23e5-112">Permission type</span></span>      | <span data-ttu-id="a23e5-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a23e5-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a23e5-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a23e5-114">Delegated (work or school account)</span></span> | <span data-ttu-id="a23e5-115">Application.Read.All、 Application.ReadWrite.All、 Directory.Read.All、 Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a23e5-115">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a23e5-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a23e5-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a23e5-117">Application.Read.All 和 User.Read， Application.ReadWrite.All 和 User.Read</span><span class="sxs-lookup"><span data-stu-id="a23e5-117">Application.Read.All and User.Read, Application.ReadWrite.All and User.Read</span></span> |
|<span data-ttu-id="a23e5-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="a23e5-118">Application</span></span> | <span data-ttu-id="a23e5-119">Application.Read.All、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="a23e5-119">Application.Read.All, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a23e5-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a23e5-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a23e5-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a23e5-121">Optional query parameters</span></span>

<span data-ttu-id="a23e5-122">此方法支持[OData query parameters](/graph/query-parameters)以帮助自定义响应，包括 `$search`、`$count`、 和 `$filter`</span><span class="sxs-lookup"><span data-stu-id="a23e5-122">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="a23e5-123">可使用“**displayName**”和“**说明**”属性上的`$search`。</span><span class="sxs-lookup"><span data-stu-id="a23e5-123">You can use `$search` on the **displayName** and **description** properties.</span></span> <span data-ttu-id="a23e5-124">为该资源添加或更新项目时，将对它们进行专门索引，以便与 `$count` 和 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="a23e5-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="a23e5-125">在添加或更新项目与在索引中可用之间可能会稍有延迟。</span><span class="sxs-lookup"><span data-stu-id="a23e5-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a23e5-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="a23e5-126">Request headers</span></span>

| <span data-ttu-id="a23e5-127">名称</span><span class="sxs-lookup"><span data-stu-id="a23e5-127">Name</span></span>           | <span data-ttu-id="a23e5-128">说明</span><span class="sxs-lookup"><span data-stu-id="a23e5-128">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="a23e5-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="a23e5-129">Authorization</span></span>  | <span data-ttu-id="a23e5-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a23e5-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a23e5-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="a23e5-132">ConsistencyLevel</span></span> | <span data-ttu-id="a23e5-133">最终。</span><span class="sxs-lookup"><span data-stu-id="a23e5-133">eventual.</span></span> <span data-ttu-id="a23e5-134">当使用 `$search` 或将 `$filter` 与 `$orderby` 查询参数一起使用时，此标头和 `$count` 是必需的。</span><span class="sxs-lookup"><span data-stu-id="a23e5-134">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="a23e5-135">它使用的索引可能与对象的最新更改不同步。</span><span class="sxs-lookup"><span data-stu-id="a23e5-135">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a23e5-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="a23e5-136">Request body</span></span>
<span data-ttu-id="a23e5-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a23e5-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a23e5-138">响应</span><span class="sxs-lookup"><span data-stu-id="a23e5-138">Response</span></span>

<span data-ttu-id="a23e5-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [application](../resources/application.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a23e5-139">If successful, this method returns a `200 OK` response code and a collection of [application](../resources/application.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a23e5-140">示例</span><span class="sxs-lookup"><span data-stu-id="a23e5-140">Examples</span></span>

### <a name="example-1-get-the-list-of-applications"></a><span data-ttu-id="a23e5-141">示例 1：获取应用程序列表</span><span class="sxs-lookup"><span data-stu-id="a23e5-141">Example 1: Get the list of applications</span></span>

#### <a name="request"></a><span data-ttu-id="a23e5-142">请求</span><span class="sxs-lookup"><span data-stu-id="a23e5-142">Request</span></span>

<span data-ttu-id="a23e5-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a23e5-143">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a23e5-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="a23e5-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_application"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications
```
# <a name="c"></a>[<span data-ttu-id="a23e5-145">C#</span><span class="sxs-lookup"><span data-stu-id="a23e5-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a23e5-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a23e5-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a23e5-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a23e5-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a23e5-148">Java</span><span class="sxs-lookup"><span data-stu-id="a23e5-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a23e5-149">响应</span><span class="sxs-lookup"><span data-stu-id="a23e5-149">Response</span></span>

<span data-ttu-id="a23e5-150">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a23e5-150">Here is an example of the response.</span></span>

> <span data-ttu-id="a23e5-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a23e5-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-applications"></a><span data-ttu-id="a23e5-153">示例 2：仅获取应用程序计数</span><span class="sxs-lookup"><span data-stu-id="a23e5-153">Example 2: Get only a count of applications</span></span>

#### <a name="request"></a><span data-ttu-id="a23e5-154">请求</span><span class="sxs-lookup"><span data-stu-id="a23e5-154">Request</span></span>

<span data-ttu-id="a23e5-155">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a23e5-155">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="a23e5-156">响应</span><span class="sxs-lookup"><span data-stu-id="a23e5-156">Response</span></span>

<span data-ttu-id="a23e5-157">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a23e5-157">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`893`

### <a name="example-3-use-filter-and-top-to-get-one-application-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="a23e5-158">示例 3：使用 $filter 和 $top 获取一个显示名称以“a”开头的应用程序，其中包括返回的对象数</span><span class="sxs-lookup"><span data-stu-id="a23e5-158">Example 3: Use $filter and $top to get one application with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="a23e5-159">请求</span><span class="sxs-lookup"><span data-stu-id="a23e5-159">Request</span></span>

<span data-ttu-id="a23e5-160">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a23e5-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="a23e5-161">响应</span><span class="sxs-lookup"><span data-stu-id="a23e5-161">Response</span></span>

<span data-ttu-id="a23e5-162">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a23e5-162">The following is an example of the response.</span></span>

><span data-ttu-id="a23e5-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a23e5-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-4-use-search-to-get-applications-with-display-names-that-contain-the-letters-web-including-a-count-of-returned-objects"></a><span data-ttu-id="a23e5-165">示例 4：使用 $search 获取显示名称中包含字母“Web”的应用程序，其中包括返回的对象数</span><span class="sxs-lookup"><span data-stu-id="a23e5-165">Example 4: Use $search to get applications with display names that contain the letters 'Web' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="a23e5-166">请求</span><span class="sxs-lookup"><span data-stu-id="a23e5-166">Request</span></span>

<span data-ttu-id="a23e5-167">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a23e5-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_web_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications?$search="displayName:Web"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="a23e5-168">响应</span><span class="sxs-lookup"><span data-stu-id="a23e5-168">Response</span></span>

<span data-ttu-id="a23e5-169">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a23e5-169">The following is an example of the response.</span></span>

><span data-ttu-id="a23e5-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a23e5-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
