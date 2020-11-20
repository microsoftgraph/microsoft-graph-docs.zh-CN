---
title: 列出用户
description: 检索用户对象列表。
author: krbain
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: c948dff47d95d3cb8229793c2966c7bb60f21a40
ms.sourcegitcommit: ea3b1a8b781a347015d9542826c5c0c24d50d35d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/19/2020
ms.locfileid: "49352198"
---
# <a name="list-users"></a><span data-ttu-id="cdc91-103">列出用户</span><span class="sxs-lookup"><span data-stu-id="cdc91-103">List users</span></span>

<span data-ttu-id="cdc91-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cdc91-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cdc91-105">检索 [user](../resources/user.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="cdc91-105">Retrieve a list of [user](../resources/user.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="cdc91-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="cdc91-106">Permissions</span></span>

<span data-ttu-id="cdc91-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cdc91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdc91-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cdc91-109">Permission type</span></span>      | <span data-ttu-id="cdc91-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cdc91-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cdc91-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cdc91-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cdc91-112">User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cdc91-112">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cdc91-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cdc91-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cdc91-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="cdc91-114">Not supported.</span></span>    |
|<span data-ttu-id="cdc91-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="cdc91-115">Application</span></span> | <span data-ttu-id="cdc91-116">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdc91-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cdc91-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cdc91-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cdc91-118">可选查询参数</span><span class="sxs-lookup"><span data-stu-id="cdc91-118">Optional query parameters</span></span>

<span data-ttu-id="cdc91-p102">此方法支持使用 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应，包括 `$search`、`$count`、`$filter` 和 `$select`。你可以在 **displayName** 属性上使用 `$search`。为该资源添加或更新项目时，将为它们专门创建索引，以便与 `$count` 和 `$search` 查询参数一起使用。添加或更新项目与项目在索引中可用之间可能会稍有延迟。`$count` 和 `$search` 参数目前在 Azure AD B2C 租户中不可用。</span><span class="sxs-lookup"><span data-stu-id="cdc91-p102">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, `$filter`, and `$select`. You can use `$search` on the **displayName** property. When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters. There can be a slight delay between when an item is added or updated and when it is available in the index. The `$count` and `$search` parameters are currently not available in Azure AD B2C tenants.</span></span>

<span data-ttu-id="cdc91-124">默认情况下，仅返回一组有限的属性（**businessPhones**、**displayName**、**givenName**、**id**、**jobTitle**、**mail**、**mobilePhone**、**officeLocation**、**preferredLanguage**、**surname** 和 **userPrincipalName**）。</span><span class="sxs-lookup"><span data-stu-id="cdc91-124">By default, only a limited set of properties are returned (**businessPhones**, **displayName**, **givenName**, **id**, **jobTitle**, **mail**, **mobilePhone**, **officeLocation**, **preferredLanguage**, **surname**, and **userPrincipalName**).</span></span> 

<span data-ttu-id="cdc91-p103">若要返回其他属性集，需使用 OData `$select` 查询参数指定所需的一组 [user](../resources/user.md) 属性。例如，若要返回 **displayName**、**givenName** 和 **postalCode**，需将以下项添加到查询 `$select=displayName,givenName,postalCode`。</span><span class="sxs-lookup"><span data-stu-id="cdc91-p103">To return an alternative property set, specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter. For example, to return **displayName**, **givenName**, and **postalCode**, add the following to your query `$select=displayName,givenName,postalCode`.</span></span>

<span data-ttu-id="cdc91-p104">某些属性无法在用户集合中返回。以下属性仅在 [检索单个用户](./user-get.md) 时受支持：**aboutMe**、**birthday**、**hireDate**、**interests**、**mySite**、**pastProjects**、**preferredName**、**responsibilities**、**schools**、**skills**、**mailboxSettings**。</span><span class="sxs-lookup"><span data-stu-id="cdc91-p104">Certain properties cannot be returned within a user collection. The following properties are only supported when [retrieving an single user](./user-get.md): **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, **skills**, **mailboxSettings**.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cdc91-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="cdc91-129">Request headers</span></span>

| <span data-ttu-id="cdc91-130">标头</span><span class="sxs-lookup"><span data-stu-id="cdc91-130">Header</span></span>        | <span data-ttu-id="cdc91-131">值</span><span class="sxs-lookup"><span data-stu-id="cdc91-131">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="cdc91-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="cdc91-132">Authorization</span></span> | <span data-ttu-id="cdc91-133">Bearer {token}（必需）</span><span class="sxs-lookup"><span data-stu-id="cdc91-133">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="cdc91-134">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="cdc91-134">ConsistencyLevel</span></span> | <span data-ttu-id="cdc91-p105">最终。使用 `$search` 或将 `$filter` 与 `$orderby` 查询参数一起使用时，必须提供此标头和 `$count`。它使用的索引可能未根据该对象的最新更改及时更新。</span><span class="sxs-lookup"><span data-stu-id="cdc91-p105">eventual. This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter. It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cdc91-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="cdc91-138">Request body</span></span>

<span data-ttu-id="cdc91-139">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cdc91-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cdc91-140">响应</span><span class="sxs-lookup"><span data-stu-id="cdc91-140">Response</span></span>

<span data-ttu-id="cdc91-p106">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/user.md) 对象集合。如果返回大的用户集合，则可以 [在应用中使用分页](/graph/paging)。</span><span class="sxs-lookup"><span data-stu-id="cdc91-p106">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body. If a large user collection is returned, you can use [paging in your app](/graph/paging).</span></span>

## <a name="examples"></a><span data-ttu-id="cdc91-143">示例</span><span class="sxs-lookup"><span data-stu-id="cdc91-143">Examples</span></span>

### <a name="example-1-get-all-users"></a><span data-ttu-id="cdc91-144">示例 1：列出所有用户</span><span class="sxs-lookup"><span data-stu-id="cdc91-144">Example 1: Get all users</span></span>

#### <a name="request"></a><span data-ttu-id="cdc91-145">请求</span><span class="sxs-lookup"><span data-stu-id="cdc91-145">Request</span></span>

<span data-ttu-id="cdc91-146">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cdc91-146">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="cdc91-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="cdc91-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users
```
# <a name="c"></a>[<span data-ttu-id="cdc91-148">C#</span><span class="sxs-lookup"><span data-stu-id="cdc91-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cdc91-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cdc91-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cdc91-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cdc91-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cdc91-151">Java</span><span class="sxs-lookup"><span data-stu-id="cdc91-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cdc91-152">响应</span><span class="sxs-lookup"><span data-stu-id="cdc91-152">Response</span></span>

<span data-ttu-id="cdc91-153">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cdc91-153">The following is an example of the response.</span></span>

><span data-ttu-id="cdc91-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="cdc91-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-a-user-account-using-a-sign-in-name"></a><span data-ttu-id="cdc91-156">示例 2：使用登录名创建用户帐户</span><span class="sxs-lookup"><span data-stu-id="cdc91-156">Example 2: Get a user account using a sign-in name</span></span>

#### <a name="request"></a><span data-ttu-id="cdc91-157">请求</span><span class="sxs-lookup"><span data-stu-id="cdc91-157">Request</span></span>

<span data-ttu-id="cdc91-158">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cdc91-158">The following is an example of the request.</span></span>

><span data-ttu-id="cdc91-159">**注意：** 根据 **identities** 进行筛选时，必须同时提供 **issuer** 和 **issuerAssignedId**。</span><span class="sxs-lookup"><span data-stu-id="cdc91-159">**Note:** When filtering on **identities**, you must supply both **issuer** and **issuerAssignedId**.</span></span> <span data-ttu-id="cdc91-160">**issuerAssignedId** 的值必须是用户帐户的电子邮件地址，不能是用户主体名称（UPN）。</span><span class="sxs-lookup"><span data-stu-id="cdc91-160">The value of **issuerAssignedId** must be the email address of the user account, not the user principal name (UPN).</span></span> <span data-ttu-id="cdc91-161">如果使用了UPN，响应将为一个空列表。</span><span class="sxs-lookup"><span data-stu-id="cdc91-161">If a UPN is used, the response will be an empty list.</span></span>


# <a name="http"></a>[<span data-ttu-id="cdc91-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="cdc91-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signinname_users"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$select=displayName,id&$filter=identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')
```
# <a name="c"></a>[<span data-ttu-id="cdc91-163">C#</span><span class="sxs-lookup"><span data-stu-id="cdc91-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signinname-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cdc91-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cdc91-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signinname-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cdc91-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cdc91-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signinname-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cdc91-166">Java</span><span class="sxs-lookup"><span data-stu-id="cdc91-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signinname-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cdc91-167">响应</span><span class="sxs-lookup"><span data-stu-id="cdc91-167">Response</span></span>

<span data-ttu-id="cdc91-168">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cdc91-168">The following is an example of the response.</span></span> 

> <span data-ttu-id="cdc91-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="cdc91-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-3-get-users-including-their-last-sign-in-time"></a><span data-ttu-id="cdc91-171">示例3：列出用户，包括其上次登录时间</span><span class="sxs-lookup"><span data-stu-id="cdc91-171">Example 3: Get users including their last sign-in time</span></span>

#### <a name="request"></a><span data-ttu-id="cdc91-172">请求</span><span class="sxs-lookup"><span data-stu-id="cdc91-172">Request</span></span>

<span data-ttu-id="cdc91-173">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cdc91-173">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="cdc91-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="cdc91-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$select=displayName,userPrincipalName,signInActivity
```
# <a name="c"></a>[<span data-ttu-id="cdc91-175">C#</span><span class="sxs-lookup"><span data-stu-id="cdc91-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cdc91-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cdc91-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cdc91-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cdc91-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cdc91-178">Java</span><span class="sxs-lookup"><span data-stu-id="cdc91-178">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-last-time-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cdc91-179">响应</span><span class="sxs-lookup"><span data-stu-id="cdc91-179">Response</span></span>

<span data-ttu-id="cdc91-180">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cdc91-180">The following is an example of the response.</span></span>

><span data-ttu-id="cdc91-p110">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="cdc91-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users(displayName,userPrincipalName,signInActivity)",
  "value": [
    {
      "displayName": "Adele Vance",
      "userPrincipalName": "AdeleV@contoso.com",
      "signInActivity": {
        "lastSignInDateTime": "2017-09-04T15:35:02Z",
        "lastSignInRequestId": "c7df2760-2c81-4ef7-b578-5b5392b571df"
      }
    },
    {
      "displayName": "Alex Wilber",
      "userPrincipalName": "AlexW@contoso.com",
      "signInActivity": {
        "lastSignInDateTime": "2017-07-29T02:16:18Z",
        "lastSignInRequestId": "90d8b3f8-712e-4f7b-aa1e-62e7ae6cbe96"
      }
    }
  ]
}
```

### <a name="example-4-list-the-last-sign-in-time-of-users-with-a-specific-display-name"></a><span data-ttu-id="cdc91-183">示例 4：列出具有特定显示名称的用户的上次登录时间</span><span class="sxs-lookup"><span data-stu-id="cdc91-183">Example 4: List the last sign-in time of users with a specific display name</span></span>

#### <a name="request"></a><span data-ttu-id="cdc91-184">请求</span><span class="sxs-lookup"><span data-stu-id="cdc91-184">Request</span></span>

<span data-ttu-id="cdc91-185">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cdc91-185">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="cdc91-186">HTTP</span><span class="sxs-lookup"><span data-stu-id="cdc91-186">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time_filter"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'Eric')&$select=displayName,signInActivity
```
# <a name="c"></a>[<span data-ttu-id="cdc91-187">C#</span><span class="sxs-lookup"><span data-stu-id="cdc91-187">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-filter-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cdc91-188">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cdc91-188">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-filter-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cdc91-189">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cdc91-189">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-filter-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cdc91-190">Java</span><span class="sxs-lookup"><span data-stu-id="cdc91-190">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-last-time-filter-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cdc91-191">响应</span><span class="sxs-lookup"><span data-stu-id="cdc91-191">Response</span></span>

<span data-ttu-id="cdc91-192">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cdc91-192">The following is an example of the response.</span></span> 

> <span data-ttu-id="cdc91-p111">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="cdc91-p111">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'Eric')&$select=displayName,signInActivity",
  "value": [
    {
      "displayName": "Eric Solomon",
      "signInActivity": {
        "lastSignInDateTime": "2017-09-04T15:35:02Z",
        "lastSignInRequestId": "c7df2760-2c81-4ef7-b578-5b5392b571df"
      }
    }
  ]
}
```

### <a name="example-5-list-the-last-sign-in-time-of-users-in-a-specific-time-range"></a><span data-ttu-id="cdc91-195">示例 5：列出用户在特定时间范围内的上次登录时间</span><span class="sxs-lookup"><span data-stu-id="cdc91-195">Example 5: List the last sign-in time of users in a specific time range</span></span>

#### <a name="request"></a><span data-ttu-id="cdc91-196">请求</span><span class="sxs-lookup"><span data-stu-id="cdc91-196">Request</span></span>

<span data-ttu-id="cdc91-197">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cdc91-197">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="cdc91-198">HTTP</span><span class="sxs-lookup"><span data-stu-id="cdc91-198">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time_range"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?filter=signInActivity/lastSignInDateTime le 2019-06-01T00:00:00Z
```
# <a name="c"></a>[<span data-ttu-id="cdc91-199">C#</span><span class="sxs-lookup"><span data-stu-id="cdc91-199">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cdc91-200">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cdc91-200">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cdc91-201">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cdc91-201">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cdc91-202">Java</span><span class="sxs-lookup"><span data-stu-id="cdc91-202">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-last-time-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cdc91-203">响应</span><span class="sxs-lookup"><span data-stu-id="cdc91-203">Response</span></span>

<span data-ttu-id="cdc91-204">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cdc91-204">The following is an example of the response.</span></span> 

> <span data-ttu-id="cdc91-p112">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="cdc91-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/v1.0/users?filter=signInActivity/lastSignInDateTime le 2019-06-01T00:00:00Z",
  "value": [
    {
      "displayName": "Adele Vance",
      "userPrincipalName": "AdeleV@contoso.com",
      "signInActivity": {
        "lastSignInDateTime": "2019-05-04T15:35:02Z",
        "lastSignInRequestId": "c7df2760-2c81-4ef7-b578-5b5392b571df"
      }
    },
    {
      "displayName": "Alex Wilber",
      "userPrincipalName": "AlexW@contoso.com",
      "signInActivity": {
        "lastSignInDateTime": "2019-04-29T02:16:18Z",
        "lastSignInRequestId": "90d8b3f8-712e-4f7b-aa1e-62e7ae6cbe96"
      }
    }
  ]
}
```

### <a name="example-6-get-only-a-count-of-users"></a><span data-ttu-id="cdc91-207">示例 6：仅获取用户数量</span><span class="sxs-lookup"><span data-stu-id="cdc91-207">Example 6: Get only a count of users</span></span>

#### <a name="request"></a><span data-ttu-id="cdc91-208">请求</span><span class="sxs-lookup"><span data-stu-id="cdc91-208">Request</span></span>

<span data-ttu-id="cdc91-209">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cdc91-209">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="cdc91-210">响应</span><span class="sxs-lookup"><span data-stu-id="cdc91-210">Response</span></span>

<span data-ttu-id="cdc91-211">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="cdc91-211">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`893`

### <a name="example-7-use-filter-and-top-to-get-one-user-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="cdc91-212">示例 7：使用 $filter 和 $top 获取显示名称以“a”开头（包括返回的对象数）的组。</span><span class="sxs-lookup"><span data-stu-id="cdc91-212">Example 7: Use $filter and $top to get one user with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="cdc91-213">请求</span><span class="sxs-lookup"><span data-stu-id="cdc91-213">Request</span></span>

<span data-ttu-id="cdc91-214">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cdc91-214">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'a')&$orderby=displayName&$count=true&$top=1
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="cdc91-215">响应</span><span class="sxs-lookup"><span data-stu-id="cdc91-215">Response</span></span>

<span data-ttu-id="cdc91-216">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cdc91-216">The following is an example of the response.</span></span>

><span data-ttu-id="cdc91-p113">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="cdc91-p113">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-8-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-including-a-count-of-returned-objects"></a><span data-ttu-id="cdc91-219">示例 8：使用 $search 获取显示名称中包含字母“wa”（包括返回的对象数）的组。</span><span class="sxs-lookup"><span data-stu-id="cdc91-219">Example 8: Use $search to get users with display names that contain the letters 'wa' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="cdc91-220">请求</span><span class="sxs-lookup"><span data-stu-id="cdc91-220">Request</span></span>

<span data-ttu-id="cdc91-221">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cdc91-221">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_wa_count"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$search="displayName:wa"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="cdc91-222">响应</span><span class="sxs-lookup"><span data-stu-id="cdc91-222">Response</span></span>

<span data-ttu-id="cdc91-223">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cdc91-223">The following is an example of the response.</span></span>

><span data-ttu-id="cdc91-p114">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="cdc91-p114">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-9-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-or-the-letters-to-including-a-count-of-returned-objects"></a><span data-ttu-id="cdc91-226">示例 9：使用 $search 获取名称显示中包含字母“wa”或者包含字母“to”的的用户，包括返回对象的数量</span><span class="sxs-lookup"><span data-stu-id="cdc91-226">Example 9: Use $search to get users with display names that contain the letters 'wa' or the letters 'to' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="cdc91-227">请求</span><span class="sxs-lookup"><span data-stu-id="cdc91-227">Request</span></span>

<span data-ttu-id="cdc91-228">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cdc91-228">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_to_count"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$search="displayName:wa" OR "displayName:to"&$orderbydisplayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="cdc91-229">响应</span><span class="sxs-lookup"><span data-stu-id="cdc91-229">Response</span></span>

<span data-ttu-id="cdc91-230">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cdc91-230">The following is an example of the response.</span></span>

> <span data-ttu-id="cdc91-p115">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="cdc91-p115">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
