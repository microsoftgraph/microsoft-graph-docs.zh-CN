---
title: List orgContacts
description: 检索该组织的组织联系人列表。
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 66da3d385943bcd8b983997ec708efb10ecdd42e
ms.sourcegitcommit: 6d247f44a6ee4d8515c3863ee8a2683163c9f829
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2021
ms.locfileid: "53430114"
---
# <a name="list-orgcontacts"></a><span data-ttu-id="81768-103">List orgContacts</span><span class="sxs-lookup"><span data-stu-id="81768-103">List orgContacts</span></span>

<span data-ttu-id="81768-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81768-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="81768-105">获取该组织 [的组织](../resources/orgcontact.md) 联系人列表。</span><span class="sxs-lookup"><span data-stu-id="81768-105">Get the list of [organizational contacts](../resources/orgcontact.md) for this organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="81768-106">权限</span><span class="sxs-lookup"><span data-stu-id="81768-106">Permissions</span></span>
<span data-ttu-id="81768-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="81768-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81768-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="81768-109">Permission type</span></span>      | <span data-ttu-id="81768-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="81768-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="81768-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="81768-111">Delegated (work or school account)</span></span> | <span data-ttu-id="81768-112">OrgContact.Read.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="81768-112">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="81768-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="81768-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81768-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="81768-114">Not supported.</span></span>    |
|<span data-ttu-id="81768-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="81768-115">Application</span></span> | <span data-ttu-id="81768-116">OrgContact.Read.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81768-116">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="81768-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="81768-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="81768-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="81768-118">Optional query parameters</span></span>
<span data-ttu-id="81768-119">此方法支持使用 `$count`、`$expand`、`$filter`、`$orderBy`、`$search`、`$select` 和 `$top` [ OData 查询参数 ](/graph/query-parameters) 以帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="81768-119">This method supports the `$count`, `$expand`, `$filter`, `$orderBy`, `$search`, `$select`, and `$top` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span> <span data-ttu-id="81768-120">只有将 **ConsistencyLevel** 标头设置为 `eventual` 和 `$count` 时，才支持某些查询。</span><span class="sxs-lookup"><span data-stu-id="81768-120">Some queries are supported only when you use the **ConsistencyLevel** header set to `eventual` and `$count`.</span></span> <span data-ttu-id="81768-121">有关详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。</span><span class="sxs-lookup"><span data-stu-id="81768-121">For more information, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

## <a name="request-headers"></a><span data-ttu-id="81768-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="81768-122">Request headers</span></span>
| <span data-ttu-id="81768-123">标头</span><span class="sxs-lookup"><span data-stu-id="81768-123">Header</span></span>       | <span data-ttu-id="81768-124">值</span><span class="sxs-lookup"><span data-stu-id="81768-124">Value</span></span> |
|:-----------|:----------|
| <span data-ttu-id="81768-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="81768-125">Authorization</span></span>  |<span data-ttu-id="81768-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="81768-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="81768-128">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="81768-128">ConsistencyLevel</span></span> | <span data-ttu-id="81768-129">最终。</span><span class="sxs-lookup"><span data-stu-id="81768-129">eventual.</span></span> <span data-ttu-id="81768-130">当使用 `$search` 或 `$filter` 的特定用法时，需要此标头和 `$count`。</span><span class="sxs-lookup"><span data-stu-id="81768-130">This header and `$count` are required when using `$search`, or in specific usage of `$filter`.</span></span> <span data-ttu-id="81768-131">有关使用 **ConsistencyLevel** 和 `$count` 的详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。</span><span class="sxs-lookup"><span data-stu-id="81768-131">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span> |

## <a name="request-body"></a><span data-ttu-id="81768-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="81768-132">Request body</span></span>
<span data-ttu-id="81768-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="81768-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="81768-134">响应</span><span class="sxs-lookup"><span data-stu-id="81768-134">Response</span></span>

<span data-ttu-id="81768-135">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [orgContact](../resources/orgcontact.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="81768-135">If successful, this method returns a `200 OK` response code and a collection of [orgContact](../resources/orgcontact.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="81768-136">示例</span><span class="sxs-lookup"><span data-stu-id="81768-136">Examples</span></span>

### <a name="example-1-get-organizational-contacts-for-an-organization"></a><span data-ttu-id="81768-137">示例 1：获取组织的组织联系人</span><span class="sxs-lookup"><span data-stu-id="81768-137">Example 1: Get organizational contacts for an organization</span></span>

#### <a name="request"></a><span data-ttu-id="81768-138">请求</span><span class="sxs-lookup"><span data-stu-id="81768-138">Request</span></span>

<span data-ttu-id="81768-139">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="81768-139">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="81768-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="81768-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_orgcontact"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts
```
# <a name="c"></a>[<span data-ttu-id="81768-141">C#</span><span class="sxs-lookup"><span data-stu-id="81768-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="81768-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="81768-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="81768-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="81768-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="81768-144">Java</span><span class="sxs-lookup"><span data-stu-id="81768-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-orgcontact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="81768-145">响应</span><span class="sxs-lookup"><span data-stu-id="81768-145">Response</span></span>

<span data-ttu-id="81768-146">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="81768-146">The following is an example of the response.</span></span>

><span data-ttu-id="81768-147">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="81768-147">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "companyName": "Contoso",
      "department": "Marketing",
      "displayName": "Eric S",
      "givenName":"Eric",
      "jobTitle":"Accountant",
      "mail":"erics@contoso.com",
      "mailNickname":"erics",
      "surname":"Solomon",
      "addresses":[
        {
          "city":"MyCity",
          "countryOrRegion":"United States",
          "officeLocation":"MyCity",
          "postalCode":"98000",
          "state":"WA",
          "street":"Contoso Way"
        }
      ],
      "phones":[
        {
          "number":"111-1111",
          "type":"businessFax"
        }
      ]
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-organizational-contacts"></a><span data-ttu-id="81768-148">示例 2：仅获取组织联系人的计数</span><span class="sxs-lookup"><span data-stu-id="81768-148">Example 2: Get only a count of organizational contacts</span></span>

#### <a name="request"></a><span data-ttu-id="81768-149">请求</span><span class="sxs-lookup"><span data-stu-id="81768-149">Request</span></span>

<span data-ttu-id="81768-150">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="81768-150">The following is an example of the request.</span></span> <span data-ttu-id="81768-151">此请求要求将 **ConsistencyLevel** 标头设置为 `eventual`，因为在请求中有 `$count`。</span><span class="sxs-lookup"><span data-stu-id="81768-151">This request requires the **ConsistencyLevel** header set to `eventual` because `$count` is in the request.</span></span> <span data-ttu-id="81768-152">有关使用 **ConsistencyLevel** 和 `$count` 的详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。</span><span class="sxs-lookup"><span data-stu-id="81768-152">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="81768-153">响应</span><span class="sxs-lookup"><span data-stu-id="81768-153">Response</span></span>

<span data-ttu-id="81768-154">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="81768-154">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

893
```


### <a name="example-3-use-filter-and-top-to-get-one-organizational-contact-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="81768-155">示例 3：使用 $filter 和 $top 获取一个组织联系人，显示名称以"a"开头（包括返回的对象计数）</span><span class="sxs-lookup"><span data-stu-id="81768-155">Example 3: Use $filter and $top to get one organizational contact with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="81768-156">请求</span><span class="sxs-lookup"><span data-stu-id="81768-156">Request</span></span>

<span data-ttu-id="81768-157">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="81768-157">The following is an example of the request.</span></span> <span data-ttu-id="81768-158">此请求需要将 **ConsistencyLevel** 标头设置为 `eventual` 和 `$count=true` 查询字符串，因为请求同时具有 `$orderBy` 和 `$filter` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="81768-158">This request requires the **ConsistencyLevel** header set to `eventual` and the `$count=true` query string because the request has both the `$orderBy` and `$filter` query parameters.</span></span> <span data-ttu-id="81768-159">有关使用 **ConsistencyLevel** 和 `$count` 的详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。</span><span class="sxs-lookup"><span data-stu-id="81768-159">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts?$filter=startswith(displayName,'A')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="81768-160">响应</span><span class="sxs-lookup"><span data-stu-id="81768-160">Response</span></span>

<span data-ttu-id="81768-161">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="81768-161">The following is an example of the response.</span></span>

><span data-ttu-id="81768-162">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="81768-162">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#contacts",
  "@odata.count":1,
  "value":[
    {
      "displayName":"Abigail Jackson",
      "mail":"abigailJ@contoso.com",
      "mailNickname":"abigailJ"
    }
  ]
}
```

### <a name="example-4-use-search-to-get-organizational-contacts-with-display-names-that-contain-the-letters-wa-including-a-count-of-returned-objects"></a><span data-ttu-id="81768-163">示例 4：使用 $search 获取显示名称包含字母"wa"的组织联系人，包括返回的对象计数</span><span class="sxs-lookup"><span data-stu-id="81768-163">Example 4: Use $search to get organizational contacts with display names that contain the letters 'wa' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="81768-164">请求</span><span class="sxs-lookup"><span data-stu-id="81768-164">Request</span></span>

<span data-ttu-id="81768-165">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="81768-165">The following is an example of the request.</span></span> <span data-ttu-id="81768-166">此请求需要 **将 ConsistencyLevel** 标头设置为 `eventual` ，因为 `$search` 查询 `$count=true` 字符串位于请求中。</span><span class="sxs-lookup"><span data-stu-id="81768-166">This request requires the **ConsistencyLevel** header set to `eventual` because `$search` and the `$count=true` query string is in the request.</span></span> <span data-ttu-id="81768-167">有关使用 **ConsistencyLevel** 和 `$count` 的详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。</span><span class="sxs-lookup"><span data-stu-id="81768-167">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "request",
  "name": "get_phone_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts?$search="displayName:wa"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="81768-168">响应</span><span class="sxs-lookup"><span data-stu-id="81768-168">Response</span></span>

<span data-ttu-id="81768-169">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="81768-169">The following is an example of the response.</span></span>

><span data-ttu-id="81768-170">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="81768-170">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#contacts",
  "@odata.count":22,
  "value":[
    {
      "displayName":"Nicole Wagner",
      "mail":"nicolewa@contoso.com",
      "mailNickname":"nicolewa"
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List orgContact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

