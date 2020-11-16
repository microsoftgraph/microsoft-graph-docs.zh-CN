---
title: List orgContacts
description: 检索此组织的组织联系人列表。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 26c7b65298b0f644c1dcadb11104b73dc0ff15a3
ms.sourcegitcommit: eafb1629e52450dab0da6a1fb6d1ddfa878777c6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2020
ms.locfileid: "49082221"
---
# <a name="list-orgcontacts"></a><span data-ttu-id="aabb6-103">List orgContacts</span><span class="sxs-lookup"><span data-stu-id="aabb6-103">List orgContacts</span></span>

<span data-ttu-id="aabb6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aabb6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="aabb6-105">获取此组织的 [组织联系人](../resources/orgcontact.md) 列表。</span><span class="sxs-lookup"><span data-stu-id="aabb6-105">Get the list of [organizational contacts](../resources/orgcontact.md) for this organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="aabb6-106">权限</span><span class="sxs-lookup"><span data-stu-id="aabb6-106">Permissions</span></span>
<span data-ttu-id="aabb6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aabb6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aabb6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="aabb6-109">Permission type</span></span>      | <span data-ttu-id="aabb6-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aabb6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aabb6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aabb6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="aabb6-112">OrgContact、Directory.accessasuser.all、所有的目录、所有、和所有子目录。</span><span class="sxs-lookup"><span data-stu-id="aabb6-112">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="aabb6-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aabb6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aabb6-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="aabb6-114">Not supported.</span></span>    |
|<span data-ttu-id="aabb6-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="aabb6-115">Application</span></span> | <span data-ttu-id="aabb6-116">OrgContact、所有目录、全部读取、所有读写。</span><span class="sxs-lookup"><span data-stu-id="aabb6-116">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aabb6-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aabb6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="aabb6-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="aabb6-118">Optional query parameters</span></span>
<span data-ttu-id="aabb6-119">此方法支持 [OData 查询参数](/graph/query-parameters) ，以帮助自定义响应，包括、、、、 `$count` `$expand` `$filter` `$search` `$select` 和 `$top` 。</span><span class="sxs-lookup"><span data-stu-id="aabb6-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$count`, `$expand`, `$filter`, `$search`,`$select`, and `$top`.</span></span> <span data-ttu-id="aabb6-120">`$search`可以用在 **displayName** 属性。</span><span class="sxs-lookup"><span data-stu-id="aabb6-120">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="aabb6-121">为该资源添加或更新项目时，将对它们进行专门索引，以便与 `$count` 和 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="aabb6-121">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="aabb6-122">在添加或更新项目与在索引中可用之间可能会稍有延迟。</span><span class="sxs-lookup"><span data-stu-id="aabb6-122">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aabb6-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="aabb6-123">Request headers</span></span>
| <span data-ttu-id="aabb6-124">标头</span><span class="sxs-lookup"><span data-stu-id="aabb6-124">Header</span></span>       | <span data-ttu-id="aabb6-125">值</span><span class="sxs-lookup"><span data-stu-id="aabb6-125">Value</span></span> |
|:-----------|:----------|
| <span data-ttu-id="aabb6-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="aabb6-126">Authorization</span></span>  |<span data-ttu-id="aabb6-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="aabb6-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="aabb6-129">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="aabb6-129">ConsistencyLevel</span></span> | <span data-ttu-id="aabb6-p104">最终。使用 `$search` 或将 `$filter` 与 `$orderby` 查询参数一起使用时，必须提供此标头和 `$count`。它使用的索引可能未根据该对象的最新更改及时更新。</span><span class="sxs-lookup"><span data-stu-id="aabb6-p104">eventual. This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter. It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aabb6-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="aabb6-133">Request body</span></span>
<span data-ttu-id="aabb6-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="aabb6-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aabb6-135">响应</span><span class="sxs-lookup"><span data-stu-id="aabb6-135">Response</span></span>

<span data-ttu-id="aabb6-136">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [orgContact](../resources/orgcontact.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="aabb6-136">If successful, this method returns a `200 OK` response code and a collection of [orgContact](../resources/orgcontact.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="aabb6-137">示例</span><span class="sxs-lookup"><span data-stu-id="aabb6-137">Examples</span></span>

### <a name="example-1-get-organizational-contacts-for-an-organization"></a><span data-ttu-id="aabb6-138">示例1：获取组织的组织联系人</span><span class="sxs-lookup"><span data-stu-id="aabb6-138">Example 1: Get organizational contacts for an organization</span></span>

#### <a name="request"></a><span data-ttu-id="aabb6-139">请求</span><span class="sxs-lookup"><span data-stu-id="aabb6-139">Request</span></span>

<span data-ttu-id="aabb6-140">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="aabb6-140">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="aabb6-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="aabb6-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_orgcontact"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts
```
# <a name="c"></a>[<span data-ttu-id="aabb6-142">C#</span><span class="sxs-lookup"><span data-stu-id="aabb6-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aabb6-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aabb6-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aabb6-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aabb6-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="aabb6-145">Java</span><span class="sxs-lookup"><span data-stu-id="aabb6-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-orgcontact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="aabb6-146">响应</span><span class="sxs-lookup"><span data-stu-id="aabb6-146">Response</span></span>

<span data-ttu-id="aabb6-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="aabb6-147">The following is an example of the response.</span></span>

><span data-ttu-id="aabb6-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="aabb6-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-organizational-contacts"></a><span data-ttu-id="aabb6-150">示例2：仅获取组织联系人的计数</span><span class="sxs-lookup"><span data-stu-id="aabb6-150">Example 2: Get only a count of organizational contacts</span></span>

#### <a name="request"></a><span data-ttu-id="aabb6-151">请求</span><span class="sxs-lookup"><span data-stu-id="aabb6-151">Request</span></span>

<span data-ttu-id="aabb6-152">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="aabb6-152">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="aabb6-153">响应</span><span class="sxs-lookup"><span data-stu-id="aabb6-153">Response</span></span>

<span data-ttu-id="aabb6-154">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="aabb6-154">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`893`

### <a name="example-3-use-filter-and-top-to-get-one-organizational-contact-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="aabb6-155">示例3：使用 $filter 和 $top 获取一个包含以 "a" 开头的显示名称的组织联系人，其中包含返回对象的计数</span><span class="sxs-lookup"><span data-stu-id="aabb6-155">Example 3: Use $filter and $top to get one organizational contact with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="aabb6-156">请求</span><span class="sxs-lookup"><span data-stu-id="aabb6-156">Request</span></span>

<span data-ttu-id="aabb6-157">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="aabb6-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts?$filter=startswith(displayName,'A')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="aabb6-158">响应</span><span class="sxs-lookup"><span data-stu-id="aabb6-158">Response</span></span>

<span data-ttu-id="aabb6-159">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="aabb6-159">The following is an example of the response.</span></span>

><span data-ttu-id="aabb6-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="aabb6-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-4-use-search-to-get-organizational-contacts-with-display-names-that-contain-the-letters-wa-including-a-count-of-returned-objects"></a><span data-ttu-id="aabb6-162">示例4：使用 $search 获取显示名称包含字母 "wa" 的组织联系人，包括返回对象的计数</span><span class="sxs-lookup"><span data-stu-id="aabb6-162">Example 4: Use $search to get organizational contacts with display names that contain the letters 'wa' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="aabb6-163">请求</span><span class="sxs-lookup"><span data-stu-id="aabb6-163">Request</span></span>

<span data-ttu-id="aabb6-164">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="aabb6-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_phone_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts?$search="displayName:wa"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="aabb6-165">响应</span><span class="sxs-lookup"><span data-stu-id="aabb6-165">Response</span></span>

<span data-ttu-id="aabb6-166">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="aabb6-166">The following is an example of the response.</span></span>

><span data-ttu-id="aabb6-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="aabb6-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

