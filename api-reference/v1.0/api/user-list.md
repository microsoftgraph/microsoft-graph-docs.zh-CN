---
title: 列出用户
description: 检索用户对象列表。
author: krbain
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 23f637bb6850fd91d17aee5d70f9200097a2378e
ms.sourcegitcommit: eafb1629e52450dab0da6a1fb6d1ddfa878777c6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2020
ms.locfileid: "49082270"
---
# <a name="list-users"></a><span data-ttu-id="724d7-103">列出用户</span><span class="sxs-lookup"><span data-stu-id="724d7-103">List users</span></span>

<span data-ttu-id="724d7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="724d7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="724d7-105">检索 [user](../resources/user.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="724d7-105">Retrieve a list of [user](../resources/user.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="724d7-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="724d7-106">Permissions</span></span>

<span data-ttu-id="724d7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="724d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="724d7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="724d7-109">Permission type</span></span>      | <span data-ttu-id="724d7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="724d7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="724d7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="724d7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="724d7-112">User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="724d7-112">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="724d7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="724d7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="724d7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="724d7-114">Not supported.</span></span>    |
|<span data-ttu-id="724d7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="724d7-115">Application</span></span> | <span data-ttu-id="724d7-116">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="724d7-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="724d7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="724d7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="724d7-118">可选查询参数</span><span class="sxs-lookup"><span data-stu-id="724d7-118">Optional query parameters</span></span>

<span data-ttu-id="724d7-p102">此方法支持使用 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应，包括 `$search`、`$count`、`$filter` 和 `$select`。你可以在 **displayName** 属性上使用 `$search`。为该资源添加或更新项目时，将为它们专门创建索引，以便与 `$count` 和 `$search` 查询参数一起使用。添加或更新项目与项目在索引中可用之间可能会稍有延迟。`$count` 和 `$search` 参数目前在 Azure AD B2C 租户中不可用。</span><span class="sxs-lookup"><span data-stu-id="724d7-p102">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, `$filter`, and `$select`. You can use `$search` on the **displayName** property. When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters. There can be a slight delay between when an item is added or updated and when it is available in the index. The `$count` and `$search` parameters are currently not available in Azure AD B2C tenants.</span></span>

<span data-ttu-id="724d7-124">默认情况下，仅返回一组有限的属性（**businessPhones**、**displayName**、**givenName**、**id**、**jobTitle**、**mail**、**mobilePhone**、**officeLocation**、**preferredLanguage**、**surname** 和 **userPrincipalName**）。</span><span class="sxs-lookup"><span data-stu-id="724d7-124">By default, only a limited set of properties are returned (**businessPhones**, **displayName**, **givenName**, **id**, **jobTitle**, **mail**, **mobilePhone**, **officeLocation**, **preferredLanguage**, **surname**, and **userPrincipalName**).</span></span> 

<span data-ttu-id="724d7-p103">若要返回其他属性集，需使用 OData `$select` 查询参数指定所需的一组 [user](../resources/user.md) 属性。例如，若要返回 **displayName**、**givenName** 和 **postalCode**，需将以下项添加到查询 `$select=displayName,givenName,postalCode`。</span><span class="sxs-lookup"><span data-stu-id="724d7-p103">To return an alternative property set, specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter. For example, to return **displayName**, **givenName**, and **postalCode**, add the following to your query `$select=displayName,givenName,postalCode`.</span></span>

<span data-ttu-id="724d7-p104">某些属性无法在用户集合中返回。以下属性仅在 [检索单个用户](./user-get.md) 时受支持：**aboutMe**、**birthday**、**hireDate**、**interests**、**mySite**、**pastProjects**、**preferredName**、**responsibilities**、**schools**、**skills**、**mailboxSettings**。</span><span class="sxs-lookup"><span data-stu-id="724d7-p104">Certain properties cannot be returned within a user collection. The following properties are only supported when [retrieving an single user](./user-get.md): **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, **skills**, **mailboxSettings**.</span></span>

## <a name="request-headers"></a><span data-ttu-id="724d7-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="724d7-129">Request headers</span></span>

| <span data-ttu-id="724d7-130">标头</span><span class="sxs-lookup"><span data-stu-id="724d7-130">Header</span></span>        | <span data-ttu-id="724d7-131">值</span><span class="sxs-lookup"><span data-stu-id="724d7-131">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="724d7-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="724d7-132">Authorization</span></span> | <span data-ttu-id="724d7-133">Bearer {token}（必需）</span><span class="sxs-lookup"><span data-stu-id="724d7-133">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="724d7-134">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="724d7-134">ConsistencyLevel</span></span> | <span data-ttu-id="724d7-p105">最终。使用 `$search` 或将 `$filter` 与 `$orderby` 查询参数一起使用时，必须提供此标头和 `$count`。它使用的索引可能未根据该对象的最新更改及时更新。</span><span class="sxs-lookup"><span data-stu-id="724d7-p105">eventual. This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter. It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="724d7-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="724d7-138">Request body</span></span>

<span data-ttu-id="724d7-139">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="724d7-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="724d7-140">响应</span><span class="sxs-lookup"><span data-stu-id="724d7-140">Response</span></span>

<span data-ttu-id="724d7-p106">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/user.md) 对象集合。如果返回大的用户集合，则可以 [在应用中使用分页](/graph/paging)。</span><span class="sxs-lookup"><span data-stu-id="724d7-p106">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body. If a large user collection is returned, you can use [paging in your app](/graph/paging).</span></span>

## <a name="examples"></a><span data-ttu-id="724d7-143">示例</span><span class="sxs-lookup"><span data-stu-id="724d7-143">Examples</span></span>

### <a name="example-1-get-all-users"></a><span data-ttu-id="724d7-144">示例 1：列出所有用户</span><span class="sxs-lookup"><span data-stu-id="724d7-144">Example 1: Get all users</span></span>

#### <a name="request"></a><span data-ttu-id="724d7-145">请求</span><span class="sxs-lookup"><span data-stu-id="724d7-145">Request</span></span>

<span data-ttu-id="724d7-146">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="724d7-146">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="724d7-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="724d7-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users
```
# <a name="c"></a>[<span data-ttu-id="724d7-148">C#</span><span class="sxs-lookup"><span data-stu-id="724d7-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="724d7-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="724d7-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="724d7-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="724d7-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="724d7-151">Java</span><span class="sxs-lookup"><span data-stu-id="724d7-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="724d7-152">响应</span><span class="sxs-lookup"><span data-stu-id="724d7-152">Response</span></span>

<span data-ttu-id="724d7-153">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="724d7-153">The following is an example of the response.</span></span>

><span data-ttu-id="724d7-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="724d7-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-a-user-account-using-a-sign-in-name"></a><span data-ttu-id="724d7-156">示例 2：使用登录名创建用户帐户</span><span class="sxs-lookup"><span data-stu-id="724d7-156">Example 2: Get a user account using a sign-in name</span></span>

#### <a name="request"></a><span data-ttu-id="724d7-157">请求</span><span class="sxs-lookup"><span data-stu-id="724d7-157">Request</span></span>

<span data-ttu-id="724d7-158">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="724d7-158">The following is an example of the request.</span></span>

><span data-ttu-id="724d7-159">**注意：** 根据 **identities** 进行筛选时，必须同时提供 **issuer** 和 **issuerAssignedId**。</span><span class="sxs-lookup"><span data-stu-id="724d7-159">**Note:** When filtering on **identities**, you must supply both **issuer** and **issuerAssignedId**.</span></span>


# <a name="http"></a>[<span data-ttu-id="724d7-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="724d7-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signinname_users"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$select=displayName,id&$filter=identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')
```
# <a name="c"></a>[<span data-ttu-id="724d7-161">C#</span><span class="sxs-lookup"><span data-stu-id="724d7-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signinname-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="724d7-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="724d7-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signinname-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="724d7-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="724d7-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signinname-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="724d7-164">Java</span><span class="sxs-lookup"><span data-stu-id="724d7-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signinname-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="724d7-165">响应</span><span class="sxs-lookup"><span data-stu-id="724d7-165">Response</span></span>

<span data-ttu-id="724d7-166">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="724d7-166">The following is an example of the response.</span></span> 

> <span data-ttu-id="724d7-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="724d7-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-3-get-users-including-their-last-sign-in-time"></a><span data-ttu-id="724d7-169">示例3：列出用户，包括其上次登录时间</span><span class="sxs-lookup"><span data-stu-id="724d7-169">Example 3: Get users including their last sign-in time</span></span>

#### <a name="request"></a><span data-ttu-id="724d7-170">请求</span><span class="sxs-lookup"><span data-stu-id="724d7-170">Request</span></span>

<span data-ttu-id="724d7-171">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="724d7-171">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="724d7-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="724d7-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$select=displayName,userPrincipalName,signInActivity
```
# <a name="c"></a>[<span data-ttu-id="724d7-173">C#</span><span class="sxs-lookup"><span data-stu-id="724d7-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="724d7-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="724d7-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="724d7-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="724d7-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="724d7-176">Java</span><span class="sxs-lookup"><span data-stu-id="724d7-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-last-time-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="724d7-177">响应</span><span class="sxs-lookup"><span data-stu-id="724d7-177">Response</span></span>

<span data-ttu-id="724d7-178">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="724d7-178">The following is an example of the response.</span></span>

><span data-ttu-id="724d7-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="724d7-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-4-list-the-last-sign-in-time-of-users-with-a-specific-display-name"></a><span data-ttu-id="724d7-181">示例 4：列出具有特定显示名称的用户的上次登录时间</span><span class="sxs-lookup"><span data-stu-id="724d7-181">Example 4: List the last sign-in time of users with a specific display name</span></span>

#### <a name="request"></a><span data-ttu-id="724d7-182">请求</span><span class="sxs-lookup"><span data-stu-id="724d7-182">Request</span></span>

<span data-ttu-id="724d7-183">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="724d7-183">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="724d7-184">HTTP</span><span class="sxs-lookup"><span data-stu-id="724d7-184">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time_filter"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'Eric')&$select=displayName,signInActivity
```
# <a name="c"></a>[<span data-ttu-id="724d7-185">C#</span><span class="sxs-lookup"><span data-stu-id="724d7-185">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-filter-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="724d7-186">JavaScript</span><span class="sxs-lookup"><span data-stu-id="724d7-186">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-filter-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="724d7-187">Objective-C</span><span class="sxs-lookup"><span data-stu-id="724d7-187">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-filter-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="724d7-188">Java</span><span class="sxs-lookup"><span data-stu-id="724d7-188">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-last-time-filter-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="724d7-189">响应</span><span class="sxs-lookup"><span data-stu-id="724d7-189">Response</span></span>

<span data-ttu-id="724d7-190">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="724d7-190">The following is an example of the response.</span></span> 

> <span data-ttu-id="724d7-p110">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="724d7-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-5-list-the-last-sign-in-time-of-users-in-a-specific-time-range"></a><span data-ttu-id="724d7-193">示例 5：列出用户在特定时间范围内的上次登录时间</span><span class="sxs-lookup"><span data-stu-id="724d7-193">Example 5: List the last sign-in time of users in a specific time range</span></span>

#### <a name="request"></a><span data-ttu-id="724d7-194">请求</span><span class="sxs-lookup"><span data-stu-id="724d7-194">Request</span></span>

<span data-ttu-id="724d7-195">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="724d7-195">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="724d7-196">HTTP</span><span class="sxs-lookup"><span data-stu-id="724d7-196">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time_range"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?filter=signInActivity/lastSignInDateTime le 2019-06-01T00:00:00Z
```
# <a name="c"></a>[<span data-ttu-id="724d7-197">C#</span><span class="sxs-lookup"><span data-stu-id="724d7-197">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="724d7-198">JavaScript</span><span class="sxs-lookup"><span data-stu-id="724d7-198">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="724d7-199">Objective-C</span><span class="sxs-lookup"><span data-stu-id="724d7-199">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="724d7-200">Java</span><span class="sxs-lookup"><span data-stu-id="724d7-200">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-last-time-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="724d7-201">响应</span><span class="sxs-lookup"><span data-stu-id="724d7-201">Response</span></span>

<span data-ttu-id="724d7-202">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="724d7-202">The following is an example of the response.</span></span> 

> <span data-ttu-id="724d7-p111">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="724d7-p111">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-6-get-only-a-count-of-users"></a><span data-ttu-id="724d7-205">示例 6：仅获取用户数量</span><span class="sxs-lookup"><span data-stu-id="724d7-205">Example 6: Get only a count of users</span></span>

#### <a name="request"></a><span data-ttu-id="724d7-206">请求</span><span class="sxs-lookup"><span data-stu-id="724d7-206">Request</span></span>

<span data-ttu-id="724d7-207">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="724d7-207">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="724d7-208">响应</span><span class="sxs-lookup"><span data-stu-id="724d7-208">Response</span></span>

<span data-ttu-id="724d7-209">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="724d7-209">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`893`

### <a name="example-7-use-filter-and-top-to-get-one-user-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="724d7-210">示例 7：使用 $filter 和 $top 获取显示名称以“a”开头（包括返回的对象数）的组。</span><span class="sxs-lookup"><span data-stu-id="724d7-210">Example 7: Use $filter and $top to get one user with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="724d7-211">请求</span><span class="sxs-lookup"><span data-stu-id="724d7-211">Request</span></span>

<span data-ttu-id="724d7-212">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="724d7-212">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'a')&$orderby=displayName&$count=true&$top=1
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="724d7-213">响应</span><span class="sxs-lookup"><span data-stu-id="724d7-213">Response</span></span>

<span data-ttu-id="724d7-214">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="724d7-214">The following is an example of the response.</span></span>

><span data-ttu-id="724d7-p112">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="724d7-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-8-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-including-a-count-of-returned-objects"></a><span data-ttu-id="724d7-217">示例 8：使用 $search 获取显示名称中包含字母“wa”（包括返回的对象数）的组。</span><span class="sxs-lookup"><span data-stu-id="724d7-217">Example 8: Use $search to get users with display names that contain the letters 'wa' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="724d7-218">请求</span><span class="sxs-lookup"><span data-stu-id="724d7-218">Request</span></span>

<span data-ttu-id="724d7-219">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="724d7-219">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_wa_count"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$search="displayName:wa"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="724d7-220">响应</span><span class="sxs-lookup"><span data-stu-id="724d7-220">Response</span></span>

<span data-ttu-id="724d7-221">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="724d7-221">The following is an example of the response.</span></span>

><span data-ttu-id="724d7-p113">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="724d7-p113">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-9-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-or-the-letters-to-including-a-count-of-returned-objects"></a><span data-ttu-id="724d7-224">示例 9：使用 $search 获取名称显示中包含字母“wa”或者包含字母“to”的的用户，包括返回对象的数量</span><span class="sxs-lookup"><span data-stu-id="724d7-224">Example 9: Use $search to get users with display names that contain the letters 'wa' or the letters 'to' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="724d7-225">请求</span><span class="sxs-lookup"><span data-stu-id="724d7-225">Request</span></span>

<span data-ttu-id="724d7-226">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="724d7-226">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_to_count"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$search="displayName:wa" OR "displayName:to"&$orderbydisplayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="724d7-227">响应</span><span class="sxs-lookup"><span data-stu-id="724d7-227">Response</span></span>

<span data-ttu-id="724d7-228">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="724d7-228">The following is an example of the response.</span></span>

> <span data-ttu-id="724d7-p114">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="724d7-p114">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
