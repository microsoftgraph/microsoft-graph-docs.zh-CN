---
title: 列出用户
description: 检索用户对象列表。
author: krbain
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 767331d807f63a2b90381580cfefebfdea37ddf3
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905690"
---
# <a name="list-users"></a><span data-ttu-id="8e2ab-103">列出用户</span><span class="sxs-lookup"><span data-stu-id="8e2ab-103">List users</span></span>

<span data-ttu-id="8e2ab-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e2ab-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8e2ab-105">检索 [user](../resources/user.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="8e2ab-105">Retrieve a list of [user](../resources/user.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e2ab-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="8e2ab-106">Permissions</span></span>

<span data-ttu-id="8e2ab-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8e2ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e2ab-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8e2ab-109">Permission type</span></span>      | <span data-ttu-id="8e2ab-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8e2ab-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e2ab-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8e2ab-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8e2ab-112">User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8e2ab-112">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8e2ab-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8e2ab-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e2ab-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8e2ab-114">Not supported.</span></span>    |
|<span data-ttu-id="8e2ab-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8e2ab-115">Application</span></span> | <span data-ttu-id="8e2ab-116">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e2ab-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8e2ab-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8e2ab-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8e2ab-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8e2ab-118">Optional query parameters</span></span>

<span data-ttu-id="8e2ab-119">此方法支持 [OData 查询参数](/graph/query-parameters)以帮助自定义响应，包括 `$search`、`$count`、`$filter` 和 `$select`。</span><span class="sxs-lookup"><span data-stu-id="8e2ab-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, `$filter`, and `$select`.</span></span> <span data-ttu-id="8e2ab-120">`$search`可以用在 **displayName** 属性。</span><span class="sxs-lookup"><span data-stu-id="8e2ab-120">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="8e2ab-121">为该资源添加或更新项目时，将对它们进行专门索引，以便与 `$count` 和 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="8e2ab-121">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="8e2ab-122">在添加或更新项目与在索引中可用之间可能会稍有延迟。</span><span class="sxs-lookup"><span data-stu-id="8e2ab-122">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

<span data-ttu-id="8e2ab-123">默认情况下，仅返回一组有限的属性（ **businessPhones** 、 **displayName** 、 **givenName** 、 **id** 、 **jobTitle** 、 **mail** 、 **mobilePhone** 、 **officeLocation** 、 **preferredLanguage** 、 **surname** 和 **userPrincipalName** ）。</span><span class="sxs-lookup"><span data-stu-id="8e2ab-123">By default, only a limited set of properties are returned ( **businessPhones** , **displayName** , **givenName** , **id** , **jobTitle** , **mail** , **mobilePhone** , **officeLocation** , **preferredLanguage** , **surname** , and **userPrincipalName** ).</span></span> 

<span data-ttu-id="8e2ab-124">若要返回其他属性，请使用 OData `$select` 查询参数指定所需的一组 [user](../resources/user.md) 属性。</span><span class="sxs-lookup"><span data-stu-id="8e2ab-124">To return an alternative property set, specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter.</span></span> <span data-ttu-id="8e2ab-125">例如，若要返回 **displayName** 、 **givenName** 和 **postalCode** ，请将以下项添加到查询 `$select=displayName,givenName,postalCode`。</span><span class="sxs-lookup"><span data-stu-id="8e2ab-125">For example, to return **displayName** , **givenName** , and **postalCode** , add the following to your query `$select=displayName,givenName,postalCode`.</span></span>

<span data-ttu-id="8e2ab-126">某些属性无法在用户集合中返回。</span><span class="sxs-lookup"><span data-stu-id="8e2ab-126">Certain properties cannot be returned within a user collection.</span></span> <span data-ttu-id="8e2ab-127">以下属性仅在 [检索单个用户](./user-get.md)时受支持： **aboutMe** 、 **birthday** 、 **hireDate** 、 **interests** 、 **mySite** 、 **pastProjects** 、 **preferredName** 、 **responsibilities** 、 **schools** 、 **skills** 、 **mailboxSettings** 。</span><span class="sxs-lookup"><span data-stu-id="8e2ab-127">The following properties are only supported when [retrieving an single user](./user-get.md): **aboutMe** , **birthday** , **hireDate** , **interests** , **mySite** , **pastProjects** , **preferredName** , **responsibilities** , **schools** , **skills** , **mailboxSettings**.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8e2ab-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="8e2ab-128">Request headers</span></span>

| <span data-ttu-id="8e2ab-129">标头</span><span class="sxs-lookup"><span data-stu-id="8e2ab-129">Header</span></span>        | <span data-ttu-id="8e2ab-130">值</span><span class="sxs-lookup"><span data-stu-id="8e2ab-130">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="8e2ab-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e2ab-131">Authorization</span></span> | <span data-ttu-id="8e2ab-132">Bearer {token}（必需）</span><span class="sxs-lookup"><span data-stu-id="8e2ab-132">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="8e2ab-133">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="8e2ab-133">ConsistencyLevel</span></span> | <span data-ttu-id="8e2ab-134">最终。</span><span class="sxs-lookup"><span data-stu-id="8e2ab-134">eventual.</span></span> <span data-ttu-id="8e2ab-135">当使用 `$search` 或将 `$filter` 与 `$orderby` 查询参数一起使用时，此标头和 `$count` 是必需的。</span><span class="sxs-lookup"><span data-stu-id="8e2ab-135">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="8e2ab-136">它使用的索引可能与对象的最新更改不同步。</span><span class="sxs-lookup"><span data-stu-id="8e2ab-136">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8e2ab-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="8e2ab-137">Request body</span></span>

<span data-ttu-id="8e2ab-138">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8e2ab-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e2ab-139">响应</span><span class="sxs-lookup"><span data-stu-id="8e2ab-139">Response</span></span>

<span data-ttu-id="8e2ab-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/user.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="8e2ab-140">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span> <span data-ttu-id="8e2ab-141">如果返回大的用户集，则可以[在应用中使用分页](/graph/paging)。</span><span class="sxs-lookup"><span data-stu-id="8e2ab-141">If a large user collection is returned, you can use [paging in your app](/graph/paging).</span></span>

## <a name="examples"></a><span data-ttu-id="8e2ab-142">示例</span><span class="sxs-lookup"><span data-stu-id="8e2ab-142">Examples</span></span>

### <a name="example-1-get-all-users"></a><span data-ttu-id="8e2ab-143">示例 1：列出所有用户</span><span class="sxs-lookup"><span data-stu-id="8e2ab-143">Example 1: Get all users</span></span>

#### <a name="request"></a><span data-ttu-id="8e2ab-144">请求</span><span class="sxs-lookup"><span data-stu-id="8e2ab-144">Request</span></span>

<span data-ttu-id="8e2ab-145">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8e2ab-145">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8e2ab-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e2ab-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users
```
# <a name="c"></a>[<span data-ttu-id="8e2ab-147">C#</span><span class="sxs-lookup"><span data-stu-id="8e2ab-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8e2ab-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e2ab-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8e2ab-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8e2ab-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8e2ab-150">Java</span><span class="sxs-lookup"><span data-stu-id="8e2ab-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8e2ab-151">响应</span><span class="sxs-lookup"><span data-stu-id="8e2ab-151">Response</span></span>

<span data-ttu-id="8e2ab-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8e2ab-152">The following is an example of the response.</span></span>

><span data-ttu-id="8e2ab-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8e2ab-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-a-user-account-using-a-sign-in-name"></a><span data-ttu-id="8e2ab-155">示例 2：使用登录名创建用户帐户</span><span class="sxs-lookup"><span data-stu-id="8e2ab-155">Example 2: Get a user account using a sign-in name</span></span>

#### <a name="request"></a><span data-ttu-id="8e2ab-156">请求</span><span class="sxs-lookup"><span data-stu-id="8e2ab-156">Request</span></span>

<span data-ttu-id="8e2ab-157">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8e2ab-157">The following is an example of the request.</span></span>

><span data-ttu-id="8e2ab-158">**注意：** 根据 **identities** 进行筛选时，必须同时提供 **issuer** 和 **issuerAssignedId** 。</span><span class="sxs-lookup"><span data-stu-id="8e2ab-158">**Note:** When filtering on **identities** , you must supply both **issuer** and **issuerAssignedId**.</span></span>


# <a name="http"></a>[<span data-ttu-id="8e2ab-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e2ab-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signinname_users"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$select=displayName,id&$filter=identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')
```
# <a name="c"></a>[<span data-ttu-id="8e2ab-160">C#</span><span class="sxs-lookup"><span data-stu-id="8e2ab-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signinname-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8e2ab-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e2ab-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signinname-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8e2ab-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8e2ab-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signinname-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8e2ab-163">Java</span><span class="sxs-lookup"><span data-stu-id="8e2ab-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signinname-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8e2ab-164">响应</span><span class="sxs-lookup"><span data-stu-id="8e2ab-164">Response</span></span>

<span data-ttu-id="8e2ab-165">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8e2ab-165">The following is an example of the response.</span></span> 

> <span data-ttu-id="8e2ab-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8e2ab-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-3-get-users-including-their-last-sign-in-time"></a><span data-ttu-id="8e2ab-168">示例3：列出用户，包括其上次登录时间</span><span class="sxs-lookup"><span data-stu-id="8e2ab-168">Example 3: Get users including their last sign-in time</span></span>

#### <a name="request"></a><span data-ttu-id="8e2ab-169">请求</span><span class="sxs-lookup"><span data-stu-id="8e2ab-169">Request</span></span>

<span data-ttu-id="8e2ab-170">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8e2ab-170">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8e2ab-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e2ab-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$select=displayName,userPrincipalName,signInActivity
```
# <a name="c"></a>[<span data-ttu-id="8e2ab-172">C#</span><span class="sxs-lookup"><span data-stu-id="8e2ab-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8e2ab-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e2ab-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8e2ab-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8e2ab-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8e2ab-175">Java</span><span class="sxs-lookup"><span data-stu-id="8e2ab-175">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-last-time-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8e2ab-176">响应</span><span class="sxs-lookup"><span data-stu-id="8e2ab-176">Response</span></span>

<span data-ttu-id="8e2ab-177">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8e2ab-177">The following is an example of the response.</span></span>

><span data-ttu-id="8e2ab-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8e2ab-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-4-list-the-last-sign-in-time-of-users-with-a-specific-display-name"></a><span data-ttu-id="8e2ab-180">示例 4：列出具有特定显示名称的用户的上次登录时间</span><span class="sxs-lookup"><span data-stu-id="8e2ab-180">Example 4: List the last sign-in time of users with a specific display name</span></span>

#### <a name="request"></a><span data-ttu-id="8e2ab-181">请求</span><span class="sxs-lookup"><span data-stu-id="8e2ab-181">Request</span></span>

<span data-ttu-id="8e2ab-182">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8e2ab-182">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8e2ab-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e2ab-183">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time_filter"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'Eric')&$select=displayName,signInActivity
```
# <a name="c"></a>[<span data-ttu-id="8e2ab-184">C#</span><span class="sxs-lookup"><span data-stu-id="8e2ab-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-filter-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8e2ab-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e2ab-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-filter-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8e2ab-186">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8e2ab-186">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-filter-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8e2ab-187">Java</span><span class="sxs-lookup"><span data-stu-id="8e2ab-187">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-last-time-filter-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8e2ab-188">响应</span><span class="sxs-lookup"><span data-stu-id="8e2ab-188">Response</span></span>

<span data-ttu-id="8e2ab-189">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8e2ab-189">The following is an example of the response.</span></span> 

> <span data-ttu-id="8e2ab-p110">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8e2ab-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-5-list-the-last-sign-in-time-of-users-in-a-specific-time-range"></a><span data-ttu-id="8e2ab-192">示例 5：列出用户在特定时间范围内的上次登录时间</span><span class="sxs-lookup"><span data-stu-id="8e2ab-192">Example 5: List the last sign-in time of users in a specific time range</span></span>

#### <a name="request"></a><span data-ttu-id="8e2ab-193">请求</span><span class="sxs-lookup"><span data-stu-id="8e2ab-193">Request</span></span>

<span data-ttu-id="8e2ab-194">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8e2ab-194">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8e2ab-195">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e2ab-195">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time_range"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?filter=signInActivity/lastSignInDateTime le 2019-06-01T00:00:00Z
```
# <a name="c"></a>[<span data-ttu-id="8e2ab-196">C#</span><span class="sxs-lookup"><span data-stu-id="8e2ab-196">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8e2ab-197">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e2ab-197">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8e2ab-198">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8e2ab-198">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8e2ab-199">Java</span><span class="sxs-lookup"><span data-stu-id="8e2ab-199">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-last-time-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8e2ab-200">响应</span><span class="sxs-lookup"><span data-stu-id="8e2ab-200">Response</span></span>

<span data-ttu-id="8e2ab-201">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8e2ab-201">The following is an example of the response.</span></span> 

> <span data-ttu-id="8e2ab-p111">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8e2ab-p111">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-6-get-only-a-count-of-users"></a><span data-ttu-id="8e2ab-204">示例 6：仅获取用户数量</span><span class="sxs-lookup"><span data-stu-id="8e2ab-204">Example 6: Get only a count of users</span></span>

#### <a name="request"></a><span data-ttu-id="8e2ab-205">请求</span><span class="sxs-lookup"><span data-stu-id="8e2ab-205">Request</span></span>

<span data-ttu-id="8e2ab-206">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8e2ab-206">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8e2ab-207">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e2ab-207">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="8e2ab-208">C#</span><span class="sxs-lookup"><span data-stu-id="8e2ab-208">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8e2ab-209">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e2ab-209">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8e2ab-210">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8e2ab-210">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8e2ab-211">Java</span><span class="sxs-lookup"><span data-stu-id="8e2ab-211">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-count-only-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8e2ab-212">响应</span><span class="sxs-lookup"><span data-stu-id="8e2ab-212">Response</span></span>

<span data-ttu-id="8e2ab-213">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8e2ab-213">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`893`

### <a name="example-7-use-filter-and-top-to-get-one-user-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="8e2ab-214">示例 7：使用 $filter 和 $top 获取显示名称以“a”开头（包括返回的对象数）的组。</span><span class="sxs-lookup"><span data-stu-id="8e2ab-214">Example 7: Use $filter and $top to get one user with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="8e2ab-215">请求</span><span class="sxs-lookup"><span data-stu-id="8e2ab-215">Request</span></span>

<span data-ttu-id="8e2ab-216">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8e2ab-216">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8e2ab-217">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e2ab-217">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'a')&$orderby=displayName&$count=true&$top=1
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="8e2ab-218">C#</span><span class="sxs-lookup"><span data-stu-id="8e2ab-218">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8e2ab-219">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e2ab-219">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8e2ab-220">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8e2ab-220">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8e2ab-221">Java</span><span class="sxs-lookup"><span data-stu-id="8e2ab-221">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-a-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8e2ab-222">响应</span><span class="sxs-lookup"><span data-stu-id="8e2ab-222">Response</span></span>

<span data-ttu-id="8e2ab-223">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8e2ab-223">The following is an example of the response.</span></span>

><span data-ttu-id="8e2ab-p112">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8e2ab-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-8-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-including-a-count-of-returned-objects"></a><span data-ttu-id="8e2ab-226">示例 8：使用 $search 获取显示名称中包含字母“wa”（包括返回的对象数）的组。</span><span class="sxs-lookup"><span data-stu-id="8e2ab-226">Example 8: Use $search to get users with display names that contain the letters 'wa' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="8e2ab-227">请求</span><span class="sxs-lookup"><span data-stu-id="8e2ab-227">Request</span></span>

<span data-ttu-id="8e2ab-228">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8e2ab-228">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8e2ab-229">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e2ab-229">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_wa_count"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$search="displayName:wa"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="8e2ab-230">C#</span><span class="sxs-lookup"><span data-stu-id="8e2ab-230">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-wa-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8e2ab-231">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e2ab-231">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-wa-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8e2ab-232">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8e2ab-232">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-wa-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8e2ab-233">Java</span><span class="sxs-lookup"><span data-stu-id="8e2ab-233">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-wa-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8e2ab-234">响应</span><span class="sxs-lookup"><span data-stu-id="8e2ab-234">Response</span></span>

<span data-ttu-id="8e2ab-235">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8e2ab-235">The following is an example of the response.</span></span>

><span data-ttu-id="8e2ab-p113">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8e2ab-p113">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-9-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-or-the-letters-to-including-a-count-of-returned-objects"></a><span data-ttu-id="8e2ab-238">示例 9：使用 $search 获取名称显示中包含字母“wa”或者包含字母“to”的的用户，包括返回对象的数量</span><span class="sxs-lookup"><span data-stu-id="8e2ab-238">Example 9: Use $search to get users with display names that contain the letters 'wa' or the letters 'to' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="8e2ab-239">请求</span><span class="sxs-lookup"><span data-stu-id="8e2ab-239">Request</span></span>

<span data-ttu-id="8e2ab-240">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8e2ab-240">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_to_count"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$search="displayName:wa" OR "displayName:to"&$orderbydisplayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="8e2ab-241">响应</span><span class="sxs-lookup"><span data-stu-id="8e2ab-241">Response</span></span>

<span data-ttu-id="8e2ab-242">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8e2ab-242">The following is an example of the response.</span></span>

> <span data-ttu-id="8e2ab-p114">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8e2ab-p114">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
