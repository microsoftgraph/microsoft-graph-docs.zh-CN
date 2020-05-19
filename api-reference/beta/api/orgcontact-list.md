---
title: 列出 orgContacts
description: 检索此组织的组织联系人列表。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 471fbe6625faf3a3aaac2173bd589b43cc605c3f
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290221"
---
# <a name="list-orgcontacts"></a><span data-ttu-id="7b701-103">列出 orgContacts</span><span class="sxs-lookup"><span data-stu-id="7b701-103">List orgContacts</span></span>

<span data-ttu-id="7b701-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b701-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b701-105">获取此组织的组织联系人列表。</span><span class="sxs-lookup"><span data-stu-id="7b701-105">Get the list of organizational contacts for this organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="7b701-106">权限</span><span class="sxs-lookup"><span data-stu-id="7b701-106">Permissions</span></span>
<span data-ttu-id="7b701-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7b701-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b701-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7b701-109">Permission type</span></span>      | <span data-ttu-id="7b701-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7b701-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7b701-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7b701-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7b701-112">OrgContact、Directory.accessasuser.all、所有的目录、所有、和所有子目录。</span><span class="sxs-lookup"><span data-stu-id="7b701-112">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7b701-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7b701-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b701-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7b701-114">Not supported.</span></span>    |
|<span data-ttu-id="7b701-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7b701-115">Application</span></span> | <span data-ttu-id="7b701-116">OrgContact、所有目录、全部读取、所有读写。</span><span class="sxs-lookup"><span data-stu-id="7b701-116">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7b701-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7b701-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7b701-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7b701-118">Optional query parameters</span></span>
<span data-ttu-id="7b701-119">此方法支持[OData 查询参数](/graph/query_parameters)，以帮助自定义响应，包括 `$search` 、 `$count` 和 `$filter` 。</span><span class="sxs-lookup"><span data-stu-id="7b701-119">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="7b701-120">您可以 `$search` 在**displayName**属性上使用。</span><span class="sxs-lookup"><span data-stu-id="7b701-120">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="7b701-121">为此资源添加或更新项目时，将对其进行专门编制索引，以便 `$count` 与 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="7b701-121">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="7b701-122">在添加或更新项目以及在索引中可用时，可能会出现轻微的延迟。</span><span class="sxs-lookup"><span data-stu-id="7b701-122">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7b701-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="7b701-123">Request headers</span></span>
| <span data-ttu-id="7b701-124">名称</span><span class="sxs-lookup"><span data-stu-id="7b701-124">Name</span></span>       | <span data-ttu-id="7b701-125">说明</span><span class="sxs-lookup"><span data-stu-id="7b701-125">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="7b701-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b701-126">Authorization</span></span>  | <span data-ttu-id="7b701-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7b701-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7b701-129">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="7b701-129">ConsistencyLevel</span></span> | <span data-ttu-id="7b701-130">仍然.</span><span class="sxs-lookup"><span data-stu-id="7b701-130">eventual.</span></span> <span data-ttu-id="7b701-131">此标头 `$count` 在使用时 `$search` 或在 `$filter` 与查询参数一起使用时是必需的 `$orderby` 。</span><span class="sxs-lookup"><span data-stu-id="7b701-131">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="7b701-132">它使用的索引可能不是最新的对象更改。</span><span class="sxs-lookup"><span data-stu-id="7b701-132">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7b701-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="7b701-133">Request body</span></span>
<span data-ttu-id="7b701-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7b701-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b701-135">响应</span><span class="sxs-lookup"><span data-stu-id="7b701-135">Response</span></span>

<span data-ttu-id="7b701-136">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[orgContact](../resources/orgcontact.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="7b701-136">If successful, this method returns a `200 OK` response code and a collection of [orgContact](../resources/orgcontact.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7b701-137">示例</span><span class="sxs-lookup"><span data-stu-id="7b701-137">Examples</span></span>

### <a name="example-1-get-organizational-contacts-for-an-organization"></a><span data-ttu-id="7b701-138">示例1：获取组织的组织联系人</span><span class="sxs-lookup"><span data-stu-id="7b701-138">Example 1: Get organizational contacts for an organization</span></span>

#### <a name="request"></a><span data-ttu-id="7b701-139">请求</span><span class="sxs-lookup"><span data-stu-id="7b701-139">Request</span></span>

<span data-ttu-id="7b701-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7b701-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7b701-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="7b701-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_orgcontact"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts
```
# <a name="c"></a>[<span data-ttu-id="7b701-142">C#</span><span class="sxs-lookup"><span data-stu-id="7b701-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7b701-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7b701-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7b701-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7b701-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="7b701-145">响应</span><span class="sxs-lookup"><span data-stu-id="7b701-145">Response</span></span>

<span data-ttu-id="7b701-146">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7b701-146">Here is an example of the response.</span></span> 
><span data-ttu-id="7b701-147">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7b701-147">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7b701-148">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7b701-148">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 222

{
  "value": [
    {
      "companyName":"Contoso",
      "department":"Accounting",
      "displayName":"Eric Solomon",
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

### <a name="example-2-get-only-a-count-of-organizational-contacts"></a><span data-ttu-id="7b701-149">示例2：仅获取组织联系人的计数</span><span class="sxs-lookup"><span data-stu-id="7b701-149">Example 2: Get only a count of organizational contacts</span></span>

#### <a name="request"></a><span data-ttu-id="7b701-150">请求</span><span class="sxs-lookup"><span data-stu-id="7b701-150">Request</span></span>

<span data-ttu-id="7b701-151">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7b701-151">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="7b701-152">响应</span><span class="sxs-lookup"><span data-stu-id="7b701-152">Response</span></span>

<span data-ttu-id="7b701-153">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7b701-153">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

<span data-ttu-id="7b701-154">893</span><span class="sxs-lookup"><span data-stu-id="7b701-154">893</span></span>

### <a name="example-3-use-filter-and-top-to-get-one-organizational-contact-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="7b701-155">示例3：使用 $filter 和 $top 获取一个包含以 "a" 开头的显示名称的组织联系人，其中包含返回对象的计数</span><span class="sxs-lookup"><span data-stu-id="7b701-155">Example 3: Use $filter and $top to get one organizational contact with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="7b701-156">请求</span><span class="sxs-lookup"><span data-stu-id="7b701-156">Request</span></span>

<span data-ttu-id="7b701-157">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7b701-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts?$filter=startswith(displayName,'A')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="7b701-158">响应</span><span class="sxs-lookup"><span data-stu-id="7b701-158">Response</span></span>

<span data-ttu-id="7b701-159">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7b701-159">The following is an example of the response.</span></span>
><span data-ttu-id="7b701-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7b701-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#contacts",
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

### <a name="example-4-use-search-to-get-organizational-contacts-with-display-names-that-contain-the-letters-wa-including-a-count-of-returned-objects"></a><span data-ttu-id="7b701-162">示例4：使用 $search 获取显示名称包含字母 "wa" 的组织联系人，包括返回对象的计数</span><span class="sxs-lookup"><span data-stu-id="7b701-162">Example 4: Use $search to get organizational contacts with display names that contain the letters 'wa' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="7b701-163">请求</span><span class="sxs-lookup"><span data-stu-id="7b701-163">Request</span></span>

<span data-ttu-id="7b701-164">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7b701-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_phone_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts?$search="displayName:wa"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="7b701-165">响应</span><span class="sxs-lookup"><span data-stu-id="7b701-165">Response</span></span>

<span data-ttu-id="7b701-166">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7b701-166">The following is an example of the response.</span></span>
><span data-ttu-id="7b701-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7b701-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#contacts",
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
