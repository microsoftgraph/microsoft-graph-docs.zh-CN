---
title: 创建用户
description: 使用此 API 新建用户。
author: jpettere
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: d0d3501916a2c2a2f5a08881c8e6be8ba4384823
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053760"
---
# <a name="create-user"></a><span data-ttu-id="65af0-103">创建用户</span><span class="sxs-lookup"><span data-stu-id="65af0-103">Create User</span></span>

<span data-ttu-id="65af0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65af0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="65af0-p101">创建新[用户](../resources/user.md)。请求正文包含要创建的用户。至少要为该用户指定必需的属性。可以选择指定其他任意可写属性。</span><span class="sxs-lookup"><span data-stu-id="65af0-p101">Create a new [user](../resources/user.md). The request body contains the user to create. At a minimum, you must specify the required properties for the user. You can optionally specify any other writable properties.</span></span>

>[!NOTE]
><span data-ttu-id="65af0-109">若要创建外部用户，请使用[邀请 API](invitation-post.md)。</span><span class="sxs-lookup"><span data-stu-id="65af0-109">To create external users, use the [invitation API](invitation-post.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="65af0-110">权限</span><span class="sxs-lookup"><span data-stu-id="65af0-110">Permissions</span></span>

<span data-ttu-id="65af0-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="65af0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65af0-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="65af0-113">Permission type</span></span>      | <span data-ttu-id="65af0-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="65af0-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="65af0-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="65af0-115">Delegated (work or school account)</span></span> | <span data-ttu-id="65af0-116">User.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="65af0-116">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="65af0-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="65af0-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65af0-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="65af0-118">Not supported.</span></span>    |
|<span data-ttu-id="65af0-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="65af0-119">Application</span></span> | <span data-ttu-id="65af0-120">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65af0-120">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="65af0-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="65af0-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="65af0-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="65af0-122">Request headers</span></span>

| <span data-ttu-id="65af0-123">标头</span><span class="sxs-lookup"><span data-stu-id="65af0-123">Header</span></span>       | <span data-ttu-id="65af0-124">值</span><span class="sxs-lookup"><span data-stu-id="65af0-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="65af0-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="65af0-125">Authorization</span></span>  | <span data-ttu-id="65af0-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="65af0-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="65af0-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="65af0-128">Content-Type</span></span>  | <span data-ttu-id="65af0-129">application/json</span><span class="sxs-lookup"><span data-stu-id="65af0-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="65af0-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="65af0-130">Request body</span></span>

<span data-ttu-id="65af0-131">在请求正文中，提供 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="65af0-131">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

<span data-ttu-id="65af0-132">下表列出了创建用户时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="65af0-132">The following table lists the properties that are required when you create a user.</span></span> <span data-ttu-id="65af0-133">如果要为正在创建的用户包括 **identities** 属性，并非所有列出的属性都是必需的。</span><span class="sxs-lookup"><span data-stu-id="65af0-133">If you're including an **identities** property for the user you're creating, not all the properties listed are required.</span></span> <span data-ttu-id="65af0-134">对于 [B2C 本地帐户标识](../resources/objectidentity.md)，只需要 **passwordProfile**，且 **passwordPolicy** 必须设置为 `DisablePasswordExpiration`。</span><span class="sxs-lookup"><span data-stu-id="65af0-134">For a [B2C local account identity](../resources/objectidentity.md), only  **passwordProfile** is required, and **passwordPolicy** must be set to `DisablePasswordExpiration`.</span></span> <span data-ttu-id="65af0-135">对于社交标识，则无需任何属性。</span><span class="sxs-lookup"><span data-stu-id="65af0-135">For a social identity, none of the properties are required.</span></span>

| <span data-ttu-id="65af0-136">参数</span><span class="sxs-lookup"><span data-stu-id="65af0-136">Parameter</span></span> | <span data-ttu-id="65af0-137">类型</span><span class="sxs-lookup"><span data-stu-id="65af0-137">Type</span></span> | <span data-ttu-id="65af0-138">说明</span><span class="sxs-lookup"><span data-stu-id="65af0-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="65af0-139">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="65af0-139">accountEnabled</span></span> |<span data-ttu-id="65af0-140">boolean</span><span class="sxs-lookup"><span data-stu-id="65af0-140">boolean</span></span> |<span data-ttu-id="65af0-141">启用此帐户时为 true，否则为 false。</span><span class="sxs-lookup"><span data-stu-id="65af0-141">true if the account is enabled; otherwise, false.</span></span>|
|<span data-ttu-id="65af0-142">displayName</span><span class="sxs-lookup"><span data-stu-id="65af0-142">displayName</span></span> |<span data-ttu-id="65af0-143">string</span><span class="sxs-lookup"><span data-stu-id="65af0-143">string</span></span> |<span data-ttu-id="65af0-144">要在用户的通讯簿中显示的名称。</span><span class="sxs-lookup"><span data-stu-id="65af0-144">The name to display in the address book for the user.</span></span>|
|<span data-ttu-id="65af0-145">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="65af0-145">onPremisesImmutableId</span></span> |<span data-ttu-id="65af0-146">string</span><span class="sxs-lookup"><span data-stu-id="65af0-146">string</span></span> |<span data-ttu-id="65af0-147">如果你对用户的 userPrincipalName (UPN) 属性使用联盟域，只需在创建新用户帐户时指定。</span><span class="sxs-lookup"><span data-stu-id="65af0-147">Only needs to be specified when creating a new user account if you are using a federated domain for the user's userPrincipalName (UPN) property.</span></span>|
|<span data-ttu-id="65af0-148">mailNickname</span><span class="sxs-lookup"><span data-stu-id="65af0-148">mailNickname</span></span> |<span data-ttu-id="65af0-149">string</span><span class="sxs-lookup"><span data-stu-id="65af0-149">string</span></span> |<span data-ttu-id="65af0-150">用户的邮件别名。</span><span class="sxs-lookup"><span data-stu-id="65af0-150">The mail alias for the user.</span></span>|
|<span data-ttu-id="65af0-151">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="65af0-151">passwordProfile</span></span>|[<span data-ttu-id="65af0-152">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="65af0-152">PasswordProfile</span></span>](../resources/passwordprofile.md) |<span data-ttu-id="65af0-153">用户的密码配置文件。</span><span class="sxs-lookup"><span data-stu-id="65af0-153">The password profile for the user.</span></span>|
|<span data-ttu-id="65af0-154">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="65af0-154">userPrincipalName</span></span> |<span data-ttu-id="65af0-155">string</span><span class="sxs-lookup"><span data-stu-id="65af0-155">string</span></span> |<span data-ttu-id="65af0-156">用户主体名称 (someuser@contoso.com)。</span><span class="sxs-lookup"><span data-stu-id="65af0-156">The user principal name (someuser@contoso.com).</span></span>|

<span data-ttu-id="65af0-157">由于 **用户** 资源支持 [扩展](/graph/extensibility-overview)，因此可以使用 `POST` 操作，并在创建用户实例时向其添加含有自己的数据的自定义属性。</span><span class="sxs-lookup"><span data-stu-id="65af0-157">Because the **user** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the user instance while creating it.</span></span>

>[!NOTE]
><span data-ttu-id="65af0-158">默认情况下，使用此 API 创建的联合用户将被强制每 12 小时登录一次。</span><span class="sxs-lookup"><span data-stu-id="65af0-158">Federated users created using this API will be forced to sign-in every 12 hours by default.</span></span>  <span data-ttu-id="65af0-159">有关如何对其进行更改的详细信息，请参阅[令牌生存期的例外](/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions)。</span><span class="sxs-lookup"><span data-stu-id="65af0-159">For more information on how to change this, see [Exceptions for token lifetimes](/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions).</span></span>

## <a name="response"></a><span data-ttu-id="65af0-160">响应</span><span class="sxs-lookup"><span data-stu-id="65af0-160">Response</span></span>

<span data-ttu-id="65af0-161">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [user](../resources/user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="65af0-161">If successful, this method returns `201 Created` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65af0-162">示例</span><span class="sxs-lookup"><span data-stu-id="65af0-162">Example</span></span>

### <a name="example-1-create-a-user"></a><span data-ttu-id="65af0-163">示例 1：创建用户</span><span class="sxs-lookup"><span data-stu-id="65af0-163">Example 1: Create a user</span></span>

#### <a name="request"></a><span data-ttu-id="65af0-164">请求</span><span class="sxs-lookup"><span data-stu-id="65af0-164">Request</span></span>

<span data-ttu-id="65af0-165">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="65af0-165">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="65af0-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="65af0-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_user_from_users"
}-->

```http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json

{
  "accountEnabled": true,
  "displayName": "Adele Vance",
  "mailNickname": "AdeleV",
  "userPrincipalName": "AdeleV@contoso.onmicrosoft.com",
  "passwordProfile" : {
    "forceChangePasswordNextSignIn": true,
    "password": "xWwvJ]6NMw+bWH-d"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="65af0-167">C#</span><span class="sxs-lookup"><span data-stu-id="65af0-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-user-from-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="65af0-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="65af0-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-user-from-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="65af0-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="65af0-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-user-from-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="65af0-170">Java</span><span class="sxs-lookup"><span data-stu-id="65af0-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-user-from-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="65af0-171">在请求正文中，提供 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="65af0-171">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

#### <a name="response"></a><span data-ttu-id="65af0-172">响应</span><span class="sxs-lookup"><span data-stu-id="65af0-172">Response</span></span>

<span data-ttu-id="65af0-173">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="65af0-173">Here is an example of the response.</span></span> <span data-ttu-id="65af0-174">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="65af0-174">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
    "id": "87d349ed-44d7-43e1-9a83-5f2406dee5bd",
    "businessPhones": [],
    "displayName": "Adele Vance",
    "givenName": "Adele",
    "jobTitle": "Product Marketing Manager",
    "mail": "AdeleV@contoso.onmicrosoft.com",
    "mobilePhone": "+1 425 555 0109",
    "officeLocation": "18/2111",
    "preferredLanguage": "en-US",
    "surname": "Vance",
    "userPrincipalName": "AdeleV@contoso.onmicrosoft.com"
}
```

### <a name="example-2-create-a-user-with-social-and-local-account-identities"></a><span data-ttu-id="65af0-175">示例 2：创建具有社交和本地帐户标识的用户</span><span class="sxs-lookup"><span data-stu-id="65af0-175">Example 2: Create a user with social and local account identities</span></span>

<span data-ttu-id="65af0-176">创建一个新用户，该用户具有本地帐户标识（以登录名和电子邮件地址为登录凭据），并且具有社交标识。</span><span class="sxs-lookup"><span data-stu-id="65af0-176">Create a new user, with a local account identity with a sign-in name, an email address as sign-in, and with a social identity.</span></span> <span data-ttu-id="65af0-177">此示例通常用于 B2C 租户中的迁移方案。</span><span class="sxs-lookup"><span data-stu-id="65af0-177">This example is typically used for migration scenarios in B2C tenants.</span></span>  

>[!NOTE] 
><span data-ttu-id="65af0-178">对于本地帐户标识，必须禁用密码过期，并且还必须禁用下次登录时强制更改密码。</span><span class="sxs-lookup"><span data-stu-id="65af0-178">For local account identities, password expirations must be disabled, and force change password at next sign-in must also be disabled.</span></span>

#### <a name="request"></a><span data-ttu-id="65af0-179">请求</span><span class="sxs-lookup"><span data-stu-id="65af0-179">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="65af0-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="65af0-180">HTTP</span></span>](#tab/http)
<!-- {  
  "blockType": "request",   
  "name": "create_user_from_users_identities"   
}-->

```http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json

{
  "displayName": "John Smith",
  "identities": [
    {
      "signInType": "userName",
      "issuer": "contoso.onmicrosoft.com",
      "issuerAssignedId": "johnsmith"
    },
    {
      "signInType": "emailAddress",
      "issuer": "contoso.onmicrosoft.com",
      "issuerAssignedId": "jsmith@yahoo.com"
    },
    {
      "signInType": "federated",
      "issuer": "facebook.com",
      "issuerAssignedId": "5eecb0cd"
    }
  ],
  "passwordProfile" : {
    "password": "password-value",
    "forceChangePasswordNextSignIn": false
  },
  "passwordPolicies": "DisablePasswordExpiration"
}
```
# <a name="c"></a>[<span data-ttu-id="65af0-181">C#</span><span class="sxs-lookup"><span data-stu-id="65af0-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-user-from-users-identities-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="65af0-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="65af0-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-user-from-users-identities-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="65af0-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="65af0-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-user-from-users-identities-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="65af0-184">Java</span><span class="sxs-lookup"><span data-stu-id="65af0-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-user-from-users-identities-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="65af0-185">响应</span><span class="sxs-lookup"><span data-stu-id="65af0-185">Response</span></span>

<span data-ttu-id="65af0-186">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="65af0-186">Here is an example of the response.</span></span> 

> <span data-ttu-id="65af0-187">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="65af0-187">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
  "displayName": "John Smith",
  "id": "4c7be08b-361f-41a8-b1ef-1712f7a3dfb2",
  "identities": [
    {
      "signInType": "userName",
      "issuer": "contoso.onmicrosoft.com",
      "issuerAssignedId": "johnsmith"
    },
    {
      "signInType": "emailAddress",
      "issuer": "contoso.onmicrosoft.com",
      "issuerAssignedId": "jsmith@yahoo.com"
    },
    {
      "signInType": "federated",
      "issuer": "facebook.com",
      "issuerAssignedId": "5eecb0cd"
    }
  ],
  "passwordPolicies": "DisablePasswordExpiration"
}
```
## <a name="see-also"></a><span data-ttu-id="65af0-188">另请参阅</span><span class="sxs-lookup"><span data-stu-id="65af0-188">See also</span></span>

- [<span data-ttu-id="65af0-189">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="65af0-189">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="65af0-190">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="65af0-190">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create User",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
