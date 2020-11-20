---
title: 列出用户
description: 检索用户对象列表。
author: krbain
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: bd56e0b6849626bc31a5397ce47fae8a1279aed2
ms.sourcegitcommit: ea3b1a8b781a347015d9542826c5c0c24d50d35d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/19/2020
ms.locfileid: "49352394"
---
# <a name="list-users"></a><span data-ttu-id="6338a-103">列出用户</span><span class="sxs-lookup"><span data-stu-id="6338a-103">List users</span></span>

<span data-ttu-id="6338a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6338a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6338a-105">检索 [用户](../resources/user.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="6338a-105">Retrieve a list of [user](../resources/user.md) objects.</span></span>

<span data-ttu-id="6338a-p101">此操作在默认情况下仅返回每个用户较常见的属性子集。这些 _默认_ 属性在 [属性](../resources/user.md#properties)部分进行了说明。要获取默认情况下 _不_ 返回的属性，可以对用户执行 [GET 操作](user-get.md)并在 `$select`OData 查询选项中指定属性。</span><span class="sxs-lookup"><span data-stu-id="6338a-p101">This operation returns by default only a subset of the more commonly used properties for each user. These _default_ properties are noted in the [Properties](../resources/user.md#properties) section. To get properties that are _not_ returned by default, do a [GET operation](user-get.md) for the user and specify the properties in a `$select` OData query option.</span></span>

## <a name="permissions"></a><span data-ttu-id="6338a-109">权限</span><span class="sxs-lookup"><span data-stu-id="6338a-109">Permissions</span></span>

<span data-ttu-id="6338a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6338a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6338a-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="6338a-112">Permission type</span></span>      | <span data-ttu-id="6338a-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6338a-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6338a-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6338a-114">Delegated (work or school account)</span></span> | <span data-ttu-id="6338a-115">User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6338a-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="6338a-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6338a-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6338a-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="6338a-117">Not supported.</span></span>    |
|<span data-ttu-id="6338a-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="6338a-118">Application</span></span> | <span data-ttu-id="6338a-119">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6338a-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6338a-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6338a-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6338a-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6338a-121">Optional query parameters</span></span>

<span data-ttu-id="6338a-p103">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应，包括 `$search`、`$count` 和 `$filter`。你可以在 **displayName** 属性上使用 `$search`。为该资源添加或更新项目时，将为它们专门创建索引，以便与 `$count` 和 `$search` 查询参数一起使用。在添加或更新项目与其在索引中可用之间可能会稍有延迟。`$count` 和 `$search`参数目前在 Azure AD B2C 租户中不可用。</span><span class="sxs-lookup"><span data-stu-id="6338a-p103">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`. You can use `$search` on the **displayName** property. When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters. There can be a slight delay between when an item is added or updated and when it is available in the index. The `$count` and `$search` parameters are currently not available in Azure AD B2C tenants.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6338a-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="6338a-127">Request headers</span></span>

| <span data-ttu-id="6338a-128">标头</span><span class="sxs-lookup"><span data-stu-id="6338a-128">Header</span></span> | <span data-ttu-id="6338a-129">值</span><span class="sxs-lookup"><span data-stu-id="6338a-129">Value</span></span> |
|:------ |:----- |
| <span data-ttu-id="6338a-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="6338a-130">Authorization</span></span> | <span data-ttu-id="6338a-131">Bearer {token}（必需）</span><span class="sxs-lookup"><span data-stu-id="6338a-131">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="6338a-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="6338a-132">ConsistencyLevel</span></span> | <span data-ttu-id="6338a-p104">最终。使用 `$search` 或将 `$filter` 与 `$orderby` 查询参数一起使用时，必须提供此标头和 `$count`。它使用的索引可能未根据该对象的最新更改及时更新。</span><span class="sxs-lookup"><span data-stu-id="6338a-p104">eventual. This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter. It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6338a-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="6338a-136">Request body</span></span>

<span data-ttu-id="6338a-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6338a-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6338a-138">响应</span><span class="sxs-lookup"><span data-stu-id="6338a-138">Response</span></span>

<span data-ttu-id="6338a-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/user.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="6338a-139">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6338a-140">示例</span><span class="sxs-lookup"><span data-stu-id="6338a-140">Examples</span></span>

### <a name="example-1-get-all-users"></a><span data-ttu-id="6338a-141">示例 1：列出所有用户</span><span class="sxs-lookup"><span data-stu-id="6338a-141">Example 1: Get all users</span></span>

#### <a name="request"></a><span data-ttu-id="6338a-142">请求</span><span class="sxs-lookup"><span data-stu-id="6338a-142">Request</span></span>

<span data-ttu-id="6338a-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6338a-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6338a-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="6338a-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users
```
# <a name="c"></a>[<span data-ttu-id="6338a-145">C#</span><span class="sxs-lookup"><span data-stu-id="6338a-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6338a-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6338a-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6338a-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6338a-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6338a-148">Java</span><span class="sxs-lookup"><span data-stu-id="6338a-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="6338a-149">响应</span><span class="sxs-lookup"><span data-stu-id="6338a-149">Response</span></span>

<span data-ttu-id="6338a-150">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6338a-150">The following is an example of the response.</span></span> 
><span data-ttu-id="6338a-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6338a-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "value":[
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

### <a name="example-2-get-a-user-account-using-a-sign-in-name"></a><span data-ttu-id="6338a-153">示例 2：使用登录名创建用户帐户</span><span class="sxs-lookup"><span data-stu-id="6338a-153">Example 2: Get a user account using a sign-in name</span></span>

<span data-ttu-id="6338a-154">使用登录名（也称为本地帐户）查找用户帐户。</span><span class="sxs-lookup"><span data-stu-id="6338a-154">Find a user account using a sign-in name (also known as a local account).</span></span>

>[!NOTE]
><span data-ttu-id="6338a-155">根据 **identities** 进行筛选时，必须同时提供 **issuer** 和 **issuerAssignedId**。</span><span class="sxs-lookup"><span data-stu-id="6338a-155">When filtering on **identities**, you must supply both **issuer** and **issuerAssignedId**.</span></span> <span data-ttu-id="6338a-156">**issuerAssignedId** 的值必须是用户帐户的电子邮件地址，不能是用户主体名称（UPN）。</span><span class="sxs-lookup"><span data-stu-id="6338a-156">The value of **issuerAssignedId** must be the email address of the user account, not the user principal name (UPN).</span></span> <span data-ttu-id="6338a-157">如果使用了UPN，响应将为一个空列表。</span><span class="sxs-lookup"><span data-stu-id="6338a-157">If a UPN is used, the response will be an empty list.</span></span>

#### <a name="request"></a><span data-ttu-id="6338a-158">请求</span><span class="sxs-lookup"><span data-stu-id="6338a-158">Request</span></span>

<span data-ttu-id="6338a-159">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6338a-159">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6338a-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="6338a-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signinname_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=displayName,id&$filter=identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')
```
# <a name="c"></a>[<span data-ttu-id="6338a-161">C#</span><span class="sxs-lookup"><span data-stu-id="6338a-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signinname-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6338a-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6338a-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signinname-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6338a-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6338a-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signinname-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6338a-164">Java</span><span class="sxs-lookup"><span data-stu-id="6338a-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signinname-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="6338a-165">响应</span><span class="sxs-lookup"><span data-stu-id="6338a-165">Response</span></span>

<span data-ttu-id="6338a-166">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6338a-166">The following is an example of the response.</span></span> 
> <span data-ttu-id="6338a-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6338a-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-3-get-users-including-their-last-sign-in-time"></a><span data-ttu-id="6338a-169">示例3：列出用户，包括其上次登录时间</span><span class="sxs-lookup"><span data-stu-id="6338a-169">Example 3: Get users including their last sign-in time</span></span>

#### <a name="request"></a><span data-ttu-id="6338a-170">请求</span><span class="sxs-lookup"><span data-stu-id="6338a-170">Request</span></span>

<span data-ttu-id="6338a-171">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6338a-171">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6338a-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="6338a-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=displayName,userPrincipalName,signInActivity
```
# <a name="c"></a>[<span data-ttu-id="6338a-173">C#</span><span class="sxs-lookup"><span data-stu-id="6338a-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6338a-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6338a-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6338a-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6338a-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6338a-176">Java</span><span class="sxs-lookup"><span data-stu-id="6338a-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-last-time-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="6338a-177">响应</span><span class="sxs-lookup"><span data-stu-id="6338a-177">Response</span></span>

<span data-ttu-id="6338a-178">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6338a-178">The following is an example of the response.</span></span> 
> <span data-ttu-id="6338a-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6338a-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users(displayName,userPrincipalName,signInActivity)",
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

### <a name="example-4-list-the-last-sign-in-time-of-users-with-a-specific-display-name"></a><span data-ttu-id="6338a-181">示例 4：列出具有特定显示名称的用户的上次登录时间</span><span class="sxs-lookup"><span data-stu-id="6338a-181">Example 4: List the last sign-in time of users with a specific display name</span></span>

#### <a name="request"></a><span data-ttu-id="6338a-182">请求</span><span class="sxs-lookup"><span data-stu-id="6338a-182">Request</span></span>

<span data-ttu-id="6338a-183">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6338a-183">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6338a-184">HTTP</span><span class="sxs-lookup"><span data-stu-id="6338a-184">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time_filter"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$filter=startswith(displayName,'Eric')&$select=displayName,signInActivity
```
# <a name="c"></a>[<span data-ttu-id="6338a-185">C#</span><span class="sxs-lookup"><span data-stu-id="6338a-185">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-filter-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6338a-186">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6338a-186">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-filter-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6338a-187">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6338a-187">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-filter-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6338a-188">Java</span><span class="sxs-lookup"><span data-stu-id="6338a-188">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-last-time-filter-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6338a-189">响应</span><span class="sxs-lookup"><span data-stu-id="6338a-189">Response</span></span>

<span data-ttu-id="6338a-190">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6338a-190">The following is an example of the response.</span></span> 
> <span data-ttu-id="6338a-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6338a-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/beta/users?$filter=startswith(displayName,'Eric')&$select=displayName,signInActivity",
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

### <a name="example-5-list-the-last-sign-in-time-of-users-in-a-specific-time-range"></a><span data-ttu-id="6338a-193">示例 5：列出用户在特定时间范围内的上次登录时间</span><span class="sxs-lookup"><span data-stu-id="6338a-193">Example 5: List the last sign-in time of users in a specific time range</span></span>

#### <a name="request"></a><span data-ttu-id="6338a-194">请求</span><span class="sxs-lookup"><span data-stu-id="6338a-194">Request</span></span>

<span data-ttu-id="6338a-195">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6338a-195">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6338a-196">HTTP</span><span class="sxs-lookup"><span data-stu-id="6338a-196">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time_range"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?filter=signInActivity/lastSignInDateTime le 2019-06-01T00:00:00Z
```
# <a name="c"></a>[<span data-ttu-id="6338a-197">C#</span><span class="sxs-lookup"><span data-stu-id="6338a-197">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6338a-198">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6338a-198">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6338a-199">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6338a-199">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6338a-200">Java</span><span class="sxs-lookup"><span data-stu-id="6338a-200">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-last-time-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6338a-201">响应</span><span class="sxs-lookup"><span data-stu-id="6338a-201">Response</span></span>

<span data-ttu-id="6338a-202">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6338a-202">The following is an example of the response.</span></span> 
> <span data-ttu-id="6338a-p110">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6338a-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/beta/users?filter=signInActivity/lastSignInDateTime le 2019-06-01T00:00:00Z",
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

### <a name="example-6-get-only-a-count-of-users"></a><span data-ttu-id="6338a-205">示例 6：仅获取用户数量</span><span class="sxs-lookup"><span data-stu-id="6338a-205">Example 6: Get only a count of users</span></span>

#### <a name="request"></a><span data-ttu-id="6338a-206">请求</span><span class="sxs-lookup"><span data-stu-id="6338a-206">Request</span></span>

<span data-ttu-id="6338a-207">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6338a-207">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="6338a-208">响应</span><span class="sxs-lookup"><span data-stu-id="6338a-208">Response</span></span>

<span data-ttu-id="6338a-209">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6338a-209">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

<span data-ttu-id="6338a-210">893</span><span class="sxs-lookup"><span data-stu-id="6338a-210">893</span></span>


### <a name="example-7-use-filter-and-top-to-get-one-user-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="6338a-211">示例 7：使用 $filter 和 $top 获取显示名称以“a”开头（包括返回的对象数）的组。</span><span class="sxs-lookup"><span data-stu-id="6338a-211">Example 7: Use $filter and $top to get one user with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="6338a-212">请求</span><span class="sxs-lookup"><span data-stu-id="6338a-212">Request</span></span>

<span data-ttu-id="6338a-213">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6338a-213">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$filter=startswith(displayName,'a')&$orderby=displayName&$count=true&$top=1
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="6338a-214">响应</span><span class="sxs-lookup"><span data-stu-id="6338a-214">Response</span></span>

<span data-ttu-id="6338a-215">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6338a-215">The following is an example of the response.</span></span>
><span data-ttu-id="6338a-p111">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6338a-p111">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users",
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

### <a name="example-8-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-including-a-count-of-returned-objects"></a><span data-ttu-id="6338a-218">示例 8：使用 $search 获取显示名称中包含字母“wa”（包括返回的对象数）的组。</span><span class="sxs-lookup"><span data-stu-id="6338a-218">Example 8: Use $search to get users with display names that contain the letters 'wa' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="6338a-219">请求</span><span class="sxs-lookup"><span data-stu-id="6338a-219">Request</span></span>

<span data-ttu-id="6338a-220">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6338a-220">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_wa_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$search="displayName:wa"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="6338a-221">响应</span><span class="sxs-lookup"><span data-stu-id="6338a-221">Response</span></span>

<span data-ttu-id="6338a-222">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6338a-222">The following is an example of the response.</span></span>
><span data-ttu-id="6338a-p112">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6338a-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users",
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

### <a name="example-9-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-or-the-letters-to-including-a-count-of-returned-objects"></a><span data-ttu-id="6338a-225">示例 9：使用 $search 获取名称显示中包含字母“wa”或者包含字母“to”的的用户，包括返回对象的数量</span><span class="sxs-lookup"><span data-stu-id="6338a-225">Example 9: Use $search to get users with display names that contain the letters 'wa' or the letters 'to' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="6338a-226">请求</span><span class="sxs-lookup"><span data-stu-id="6338a-226">Request</span></span>

<span data-ttu-id="6338a-227">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6338a-227">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_to_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$search="displayName:wa" OR "displayName:to"&$orderbydisplayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="6338a-228">响应</span><span class="sxs-lookup"><span data-stu-id="6338a-228">Response</span></span>

<span data-ttu-id="6338a-229">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6338a-229">The following is an example of the response.</span></span> 
> <span data-ttu-id="6338a-p113">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6338a-p113">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users",
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
<!--
{
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
