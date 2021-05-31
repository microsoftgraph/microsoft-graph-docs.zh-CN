---
title: 列出用户
description: 检索用户对象列表。
author: jpettere
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: cfb2043ed4fc9f885eaad407f62595203af45ce5
ms.sourcegitcommit: 612e1d796023433c6e15a9d66ba99d9bdc424cee
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/28/2021
ms.locfileid: "52703529"
---
# <a name="list-users"></a><span data-ttu-id="f4c11-103">列出用户</span><span class="sxs-lookup"><span data-stu-id="f4c11-103">List users</span></span>

<span data-ttu-id="f4c11-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4c11-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f4c11-105">检索 [user](../resources/user.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="f4c11-105">Retrieve a list of [user](../resources/user.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="f4c11-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="f4c11-106">Permissions</span></span>

<span data-ttu-id="f4c11-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f4c11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4c11-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f4c11-109">Permission type</span></span>      | <span data-ttu-id="f4c11-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f4c11-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f4c11-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f4c11-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f4c11-112">User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f4c11-112">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f4c11-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f4c11-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4c11-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f4c11-114">Not supported.</span></span>    |
|<span data-ttu-id="f4c11-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f4c11-115">Application</span></span> | <span data-ttu-id="f4c11-116">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4c11-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f4c11-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f4c11-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f4c11-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f4c11-118">Optional query parameters</span></span>

<span data-ttu-id="f4c11-119">此方法支持[OData query parameters](/graph/query-parameters)以帮助自定义响应，包括 `$search`、`$count`、 和 `$filter`</span><span class="sxs-lookup"><span data-stu-id="f4c11-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, `$filter`, and `$select`.</span></span> <span data-ttu-id="f4c11-120">`$search`可以用在 **displayName** 属性。</span><span class="sxs-lookup"><span data-stu-id="f4c11-120">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="f4c11-121">为该资源添加或更新项目时，将对它们进行专门索引，以便与 `$count` 和 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="f4c11-121">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="f4c11-122">在添加或更新项目与在索引中可用之间可能会稍有延迟。</span><span class="sxs-lookup"><span data-stu-id="f4c11-122">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span> <span data-ttu-id="f4c11-123">`$count` 和 `$search` 参数当前在 Azure AD B2C 租户中不可用。</span><span class="sxs-lookup"><span data-stu-id="f4c11-123">The `$count` and `$search` parameters are currently not available in Azure AD B2C tenants.</span></span>

<span data-ttu-id="f4c11-124">默认情况下，仅返回一组有限的属性（**businessPhones**、**displayName**、**givenName**、**id**、**jobTitle**、**mail**、**mobilePhone**、**officeLocation**、**preferredLanguage**、**surname** 和 **userPrincipalName**）。</span><span class="sxs-lookup"><span data-stu-id="f4c11-124">By default, only a limited set of properties are returned (**businessPhones**, **displayName**, **givenName**, **id**, **jobTitle**, **mail**, **mobilePhone**, **officeLocation**, **preferredLanguage**, **surname**, and **userPrincipalName**).</span></span> <span data-ttu-id="f4c11-125">若要返回其他属性，请使用 OData `$select` 查询参数指定所需的一组 [user](../resources/user.md) 属性。</span><span class="sxs-lookup"><span data-stu-id="f4c11-125">To return an alternative property set, specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter.</span></span> <span data-ttu-id="f4c11-126">例如，若要返回 **displayName**、**givenName** 和 **postalCode**，请将以下项添加到查询 `$select=displayName,givenName,postalCode`。</span><span class="sxs-lookup"><span data-stu-id="f4c11-126">For example, to return **displayName**, **givenName**, and **postalCode**, add the following to your query `$select=displayName,givenName,postalCode`.</span></span>

<span data-ttu-id="f4c11-p104">某些属性无法在用户集合中返回。以下属性仅在 [检索单个用户](./user-get.md) 时受支持：**aboutMe**、**birthday**、**hireDate**、**interests**、**mySite**、**pastProjects**、**preferredName**、**responsibilities**、**schools**、**skills**、**mailboxSettings**。</span><span class="sxs-lookup"><span data-stu-id="f4c11-p104">Certain properties cannot be returned within a user collection. The following properties are only supported when [retrieving a single user](./user-get.md): **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, **skills**, **mailboxSettings**.</span></span>

<span data-ttu-id="f4c11-129">个人 Microsoft 帐户不支持下列属性，且将为 `null`：**aboutMe**、**birthday**、**interests**、**mySite**，**pastProjects**、**preferredName**、**responsibilities**、**schools**、**skills**、**streetAddress**。</span><span class="sxs-lookup"><span data-stu-id="f4c11-129">The following properties are not supported in personal Microsoft accounts and will be `null`: **aboutMe**, **birthday**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, **skills**, **streetAddress**.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f4c11-130">请求头</span><span class="sxs-lookup"><span data-stu-id="f4c11-130">Request headers</span></span>

| <span data-ttu-id="f4c11-131">标头</span><span class="sxs-lookup"><span data-stu-id="f4c11-131">Header</span></span>        | <span data-ttu-id="f4c11-132">值</span><span class="sxs-lookup"><span data-stu-id="f4c11-132">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="f4c11-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4c11-133">Authorization</span></span> | <span data-ttu-id="f4c11-134">Bearer {token}（必需）</span><span class="sxs-lookup"><span data-stu-id="f4c11-134">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="f4c11-135">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="f4c11-135">ConsistencyLevel</span></span> | <span data-ttu-id="f4c11-136">最终。</span><span class="sxs-lookup"><span data-stu-id="f4c11-136">eventual.</span></span> <span data-ttu-id="f4c11-137">`$count` 使用 `$search`时、将 `$filter` 与 `$orderby` 查询参数一同使用时，或者将 `$filter` 与 `endsWith` 运算符一起使用时，和要求。</span><span class="sxs-lookup"><span data-stu-id="f4c11-137">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter, or `$filter` with the `endsWith` logical operator.</span></span> <span data-ttu-id="f4c11-138">它使用的索引可能与对象的最新更改不同步。</span><span class="sxs-lookup"><span data-stu-id="f4c11-138">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f4c11-139">请求正文</span><span class="sxs-lookup"><span data-stu-id="f4c11-139">Request body</span></span>

<span data-ttu-id="f4c11-140">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f4c11-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f4c11-141">响应</span><span class="sxs-lookup"><span data-stu-id="f4c11-141">Response</span></span>

<span data-ttu-id="f4c11-142">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/user.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f4c11-142">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span> <span data-ttu-id="f4c11-143">如果返回大的用户集，则可以[在应用中使用分页](/graph/paging)。</span><span class="sxs-lookup"><span data-stu-id="f4c11-143">If a large user collection is returned, you can use [paging in your app](/graph/paging).</span></span>

## <a name="examples"></a><span data-ttu-id="f4c11-144">示例</span><span class="sxs-lookup"><span data-stu-id="f4c11-144">Examples</span></span>

### <a name="example-1-get-all-users"></a><span data-ttu-id="f4c11-145">示例 1：列出所有用户</span><span class="sxs-lookup"><span data-stu-id="f4c11-145">Example 1: Get all users</span></span>

#### <a name="request"></a><span data-ttu-id="f4c11-146">请求</span><span class="sxs-lookup"><span data-stu-id="f4c11-146">Request</span></span>

<span data-ttu-id="f4c11-147">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f4c11-147">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f4c11-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="f4c11-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users_2"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users
```
# <a name="c"></a>[<span data-ttu-id="f4c11-149">C#</span><span class="sxs-lookup"><span data-stu-id="f4c11-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f4c11-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f4c11-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f4c11-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f4c11-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f4c11-152">Java</span><span class="sxs-lookup"><span data-stu-id="f4c11-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-users-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f4c11-153">响应</span><span class="sxs-lookup"><span data-stu-id="f4c11-153">Response</span></span>

<span data-ttu-id="f4c11-154">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f4c11-154">The following is an example of the response.</span></span>

><span data-ttu-id="f4c11-155">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f4c11-155">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "displayName":"contoso1",
      "mail":"'contoso1@gmail.com",
      "mailNickname":"contoso1_gmail.com#EXT#",
      "otherMails":["contoso1@gmail.com"],
      "proxyAddresses":["SMTP:contoso1@gmail.com"], 
      "userPrincipalName":"contoso1_gmail.com#EXT#@microsoft.onmicrosoft.com"
    }
  ]
}
```

### <a name="example-2-get-a-user-account-using-a-sign-in-name"></a><span data-ttu-id="f4c11-156">示例 2：使用登录名创建用户帐户</span><span class="sxs-lookup"><span data-stu-id="f4c11-156">Example 2: Get a user account using a sign-in name</span></span>

#### <a name="request"></a><span data-ttu-id="f4c11-157">请求</span><span class="sxs-lookup"><span data-stu-id="f4c11-157">Request</span></span>

<span data-ttu-id="f4c11-158">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f4c11-158">The following is an example of the request.</span></span>

><span data-ttu-id="f4c11-159">根据 **identities** 进行筛选时，必须同时提供 **issuer** 和 **issuerAssignedId**。</span><span class="sxs-lookup"><span data-stu-id="f4c11-159">**Note:** When filtering on **identities**, you must supply both **issuer** and **issuerAssignedId**.</span></span> <span data-ttu-id="f4c11-160">**issuerAssignedId** 的值必须是用户帐户的电子邮件地址，不能是用户主体名称（UPN）。</span><span class="sxs-lookup"><span data-stu-id="f4c11-160">The value of **issuerAssignedId** must be the email address of the user account, not the user principal name (UPN).</span></span> <span data-ttu-id="f4c11-161">如果使用了UPN，响应将为一个空列表。</span><span class="sxs-lookup"><span data-stu-id="f4c11-161">If a UPN is used, the response will be an empty list.</span></span>


# <a name="http"></a>[<span data-ttu-id="f4c11-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="f4c11-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signinname_users"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$select=displayName,id&$filter=identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')
```
# <a name="c"></a>[<span data-ttu-id="f4c11-163">C#</span><span class="sxs-lookup"><span data-stu-id="f4c11-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signinname-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f4c11-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f4c11-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signinname-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f4c11-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f4c11-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signinname-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f4c11-166">Java</span><span class="sxs-lookup"><span data-stu-id="f4c11-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signinname-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f4c11-167">响应</span><span class="sxs-lookup"><span data-stu-id="f4c11-167">Response</span></span>

<span data-ttu-id="f4c11-168">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f4c11-168">The following is an example of the response.</span></span> 

> <span data-ttu-id="f4c11-169">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f4c11-169">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "displayName": "John Smith"
    }
  ]
}
```
### <a name="example-3-get-only-a-count-of-users"></a><span data-ttu-id="f4c11-170">示例 3：仅获取用户数量</span><span class="sxs-lookup"><span data-stu-id="f4c11-170">Example 3: Get only a count of users</span></span>

#### <a name="request"></a><span data-ttu-id="f4c11-171">请求</span><span class="sxs-lookup"><span data-stu-id="f4c11-171">Request</span></span>

<span data-ttu-id="f4c11-172">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f4c11-172">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="f4c11-173">响应</span><span class="sxs-lookup"><span data-stu-id="f4c11-173">Response</span></span>

<span data-ttu-id="f4c11-174">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f4c11-174">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

893
```

### <a name="example-4-use-filter-and-top-to-get-one-user-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="f4c11-175">示例 4：使用 $filter 和 $top 获取显示名称以“a”开头（包括返回的对象数）的用户。</span><span class="sxs-lookup"><span data-stu-id="f4c11-175">Example 4: Use $filter and $top to get one user with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="f4c11-176">请求</span><span class="sxs-lookup"><span data-stu-id="f4c11-176">Request</span></span>

<span data-ttu-id="f4c11-177">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f4c11-177">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'a')&$orderby=displayName&$count=true&$top=1
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="f4c11-178">响应</span><span class="sxs-lookup"><span data-stu-id="f4c11-178">Response</span></span>

<span data-ttu-id="f4c11-179">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f4c11-179">The following is an example of the response.</span></span>

><span data-ttu-id="f4c11-180">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f4c11-180">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.count":1,
  "value":[
    {
      "displayName":"a",
      "mail":"a@contoso.com",
      "mailNickname":"a_contoso.com#EXT#",
      "otherMails":["a@contoso.com"],
      "proxyAddresses":["SMTP:a@contoso.com"],
      "userPrincipalName":"a_contoso.com#EXT#@microsoft.onmicrosoft.com"
    }
  ]
}
```

### <a name="example-5-use-filter-to-get-all-users-with-a-mail-that-ends-with-acontosocom-including-a-count-of-returned-objects-with-the-results-ordered-by-userprincipalname"></a><span data-ttu-id="f4c11-181">示例 5：使用 $filter 获取以 'a@contoso.com' 结尾的邮件的所有用户（包括返回对象的计数），结果按 userPrincipalName 排序</span><span class="sxs-lookup"><span data-stu-id="f4c11-181">Example 5: Use $filter to get all users with a mail that ends with 'a@contoso.com', including a count of returned objects, with the results ordered by userPrincipalName</span></span>

#### <a name="request"></a><span data-ttu-id="f4c11-182">请求</span><span class="sxs-lookup"><span data-stu-id="f4c11-182">Request</span></span>

<span data-ttu-id="f4c11-183">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f4c11-183">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f4c11-184">HTTP</span><span class="sxs-lookup"><span data-stu-id="f4c11-184">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count_endsWith"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=endswith(mail,'a@contoso.com')&$orderby=userPrincipalName&$count=true
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="f4c11-185">C#</span><span class="sxs-lookup"><span data-stu-id="f4c11-185">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-endswith-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f4c11-186">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f4c11-186">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-endswith-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f4c11-187">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f4c11-187">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-endswith-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f4c11-188">Java</span><span class="sxs-lookup"><span data-stu-id="f4c11-188">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-a-count-endswith-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f4c11-189">响应</span><span class="sxs-lookup"><span data-stu-id="f4c11-189">Response</span></span>

<span data-ttu-id="f4c11-190">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f4c11-190">The following is an example of the response.</span></span>

><span data-ttu-id="f4c11-191">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f4c11-191">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.count": 1,
  "value": [
    {
      "displayName": "Grady Archie",
      "givenName": "Grady",
      "jobTitle": "Designer",
      "mail": "GradyA@contoso.com",
      "userPrincipalName": "GradyA@contoso.com",
      "id": "e8b753b5-4117-464e-9a08-713e1ff266b3"
      }
    ]
}
```

### <a name="example-6-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-including-a-count-of-returned-objects"></a><span data-ttu-id="f4c11-192">示例 6：使用 $search 获取显示名称中包含字母“wa”或“to”（包括返回的对象数）的用户。</span><span class="sxs-lookup"><span data-stu-id="f4c11-192">Example 6: Use $search to get users with display names that contain the letters 'wa' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="f4c11-193">请求</span><span class="sxs-lookup"><span data-stu-id="f4c11-193">Request</span></span>

<span data-ttu-id="f4c11-194">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f4c11-194">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_wa_count"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$search="displayName:wa"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="f4c11-195">响应</span><span class="sxs-lookup"><span data-stu-id="f4c11-195">Response</span></span>

<span data-ttu-id="f4c11-196">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f4c11-196">The following is an example of the response.</span></span>

><span data-ttu-id="f4c11-197">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f4c11-197">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.count":7,
  "value":[
    {
      "displayName":"Oscar Ward",
      "givenName":"Oscar",
      "mail":"oscarward@contoso.com",
      "mailNickname":"oscward",
      "userPrincipalName":"oscarward@contoso.com"
    }
  ]
}
```

### <a name="example-7-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-or-the-letters-to-including-a-count-of-returned-objects"></a><span data-ttu-id="f4c11-198">示例 7：使用 $search 获取显示名称中包含字母“wa”或“to”（包括返回的对象数）的用户。</span><span class="sxs-lookup"><span data-stu-id="f4c11-198">Example 7: Use $search to get users with display names that contain the letters 'wa' or the letters 'to' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="f4c11-199">请求</span><span class="sxs-lookup"><span data-stu-id="f4c11-199">Request</span></span>

<span data-ttu-id="f4c11-200">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f4c11-200">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_to_count"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$search="displayName:wa" OR "displayName:to"&$orderbydisplayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="f4c11-201">响应</span><span class="sxs-lookup"><span data-stu-id="f4c11-201">Response</span></span>

<span data-ttu-id="f4c11-202">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f4c11-202">The following is an example of the response.</span></span>

> <span data-ttu-id="f4c11-203">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f4c11-203">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.count":7,
  "value":[
    {
      "displayName":"Oscar Ward",
      "givenName":"Oscar",
      "mail":"oscarward@contoso.com",
      "mailNickname":"oscward",
      "userPrincipalName":"oscarward@contoso.com"
    },
    {
      "displayName":"contoso1",
      "mail":"'contoso1@gmail.com",
      "mailNickname":"contoso1_gmail.com#EXT#",
      "proxyAddresses":["SMTP:contoso1@gmail.com"], 
      "userPrincipalName":"contoso1_gmail.com#EXT#@microsoft.onmicrosoft.com"
    }
  ]
}
```

### <a name="example-8-use-filter-to-get-users-who-are-assigned-a-specific-license"></a><span data-ttu-id="f4c11-204">示例 8：使用 $filter为用户分配特定许可证</span><span class="sxs-lookup"><span data-stu-id="f4c11-204">Example 8: Use $filter to get users who are assigned a specific license</span></span>

#### <a name="request"></a><span data-ttu-id="f4c11-205">请求</span><span class="sxs-lookup"><span data-stu-id="f4c11-205">Request</span></span>

<span data-ttu-id="f4c11-206">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f4c11-206">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_user_assignedLicenses"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$select=id,mail,assignedLicenses&$filter=assignedLicenses/any(u:u/skuId eq cbdc14ab-d96c-4c30-b9f4-6ada7cdc1d46)
```

#### <a name="response"></a><span data-ttu-id="f4c11-207">响应</span><span class="sxs-lookup"><span data-stu-id="f4c11-207">Response</span></span>

<span data-ttu-id="f4c11-208">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f4c11-208">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users(id,mail,assignedLicenses)",
  "value": [
    {
      "id": "cb4954e8-467f-4a6d-a8c8-28b9034fadbc",
      "mail": "admin@contoso.com",
      "assignedLicenses": [
        {
          "disabledPlans": [],
          "skuId": "cbdc14ab-d96c-4c30-b9f4-6ada7cdc1d46"
        }
      ]
    },
    {
      "id": "81a133c2-bdf2-4e67-8755-7264366b04ee",
      "mail": "DebraB@contoso.com",
      "assignedLicenses": [
        {
          "disabledPlans": [],
          "skuId": "cbdc14ab-d96c-4c30-b9f4-6ada7cdc1d46"
        }
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
