---
title: 创建用户
description: 新建用户。
author: jpettere
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: e04afb007f70788b21253323adfb517ebab7ade6
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911359"
---
# <a name="create-user"></a><span data-ttu-id="62506-103">创建用户</span><span class="sxs-lookup"><span data-stu-id="62506-103">Create user</span></span>

<span data-ttu-id="62506-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62506-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62506-p101">创建新[用户](../resources/user.md)。请求正文包含要创建的用户。至少要为该用户指定必需的属性。可以选择指定其他任意可写属性。</span><span class="sxs-lookup"><span data-stu-id="62506-p101">Create a new [user](../resources/user.md). The request body contains the user to create. At a minimum, you must specify the required properties for the user. You can optionally specify any other writable properties.</span></span>

<span data-ttu-id="62506-109">默认情况下，此操作仅返回每个用户的一部分属性。</span><span class="sxs-lookup"><span data-stu-id="62506-109">This operation returns by default only a subset of the properties for each user.</span></span> <span data-ttu-id="62506-110">这些默认属性将记录在[属性](../resources/user.md#properties)部分中。</span><span class="sxs-lookup"><span data-stu-id="62506-110">These default properties are noted in the [Properties](../resources/user.md#properties) section.</span></span> <span data-ttu-id="62506-111">若要获取非默认返回的属性，请执行 [GET 操作](user-get.md)，并在 `$select` OData 查询选项中指定这些属性。</span><span class="sxs-lookup"><span data-stu-id="62506-111">To get properties that are not returned by default, do a [GET operation](user-get.md) and specify the properties in a `$select` OData query option.</span></span>

>[!NOTE]
><span data-ttu-id="62506-112">若要创建外部用户，请使用[邀请 API](invitation-post.md)。</span><span class="sxs-lookup"><span data-stu-id="62506-112">To create external users, use the [invitation API](invitation-post.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="62506-113">权限</span><span class="sxs-lookup"><span data-stu-id="62506-113">Permissions</span></span>

<span data-ttu-id="62506-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="62506-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62506-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="62506-116">Permission type</span></span>      | <span data-ttu-id="62506-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="62506-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="62506-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="62506-118">Delegated (work or school account)</span></span> | <span data-ttu-id="62506-119">User.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="62506-119">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="62506-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="62506-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62506-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="62506-121">Not supported.</span></span>    |
|<span data-ttu-id="62506-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="62506-122">Application</span></span> | <span data-ttu-id="62506-123">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62506-123">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="62506-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="62506-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users
```
## <a name="request-headers"></a><span data-ttu-id="62506-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="62506-125">Request headers</span></span>
| <span data-ttu-id="62506-126">标头</span><span class="sxs-lookup"><span data-stu-id="62506-126">Header</span></span>       | <span data-ttu-id="62506-127">值</span><span class="sxs-lookup"><span data-stu-id="62506-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="62506-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="62506-128">Authorization</span></span>  | <span data-ttu-id="62506-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="62506-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="62506-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="62506-131">Content-Type</span></span>  | <span data-ttu-id="62506-132">application/json</span><span class="sxs-lookup"><span data-stu-id="62506-132">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="62506-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="62506-133">Request body</span></span>

<span data-ttu-id="62506-134">在请求正文中，提供 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="62506-134">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

<span data-ttu-id="62506-135">下表列出了创建用户时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="62506-135">The following table lists the properties that are required when you create a user.</span></span> <span data-ttu-id="62506-136">如果要为正在创建的用户包括 **identities** 属性，并非所有列出的属性都是必需的。</span><span class="sxs-lookup"><span data-stu-id="62506-136">If you're including an **identities** property for the user you're creating, not all the properties listed are required.</span></span> <span data-ttu-id="62506-137">对于 [B2C 本地帐户标识](../resources/objectidentity.md)，只需要 **passwordProfile，passwordPolicies** 必须设置为 `DisablePasswordExpiration` 。</span><span class="sxs-lookup"><span data-stu-id="62506-137">For a [B2C local account identity](../resources/objectidentity.md), only  **passwordProfile** is required, and **passwordPolicies** must be set to `DisablePasswordExpiration`.</span></span> <span data-ttu-id="62506-138">对于社交标识，则无需任何属性。</span><span class="sxs-lookup"><span data-stu-id="62506-138">For a social identity, none of the properties are required.</span></span>

| <span data-ttu-id="62506-139">参数</span><span class="sxs-lookup"><span data-stu-id="62506-139">Parameter</span></span> | <span data-ttu-id="62506-140">类型</span><span class="sxs-lookup"><span data-stu-id="62506-140">Type</span></span> | <span data-ttu-id="62506-141">说明</span><span class="sxs-lookup"><span data-stu-id="62506-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="62506-142">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="62506-142">accountEnabled</span></span> |<span data-ttu-id="62506-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="62506-143">Boolean</span></span> |<span data-ttu-id="62506-144">如果启用帐户，则其参数为 True;否则为 false。</span><span class="sxs-lookup"><span data-stu-id="62506-144">True if the account is enabled; otherwise, false.</span></span>|
|<span data-ttu-id="62506-145">displayName</span><span class="sxs-lookup"><span data-stu-id="62506-145">displayName</span></span> |<span data-ttu-id="62506-146">string</span><span class="sxs-lookup"><span data-stu-id="62506-146">string</span></span> |<span data-ttu-id="62506-147">要在用户的通讯簿中显示的名称。</span><span class="sxs-lookup"><span data-stu-id="62506-147">The name to display in the address book for the user.</span></span>|
|<span data-ttu-id="62506-148">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="62506-148">onPremisesImmutableId</span></span> |<span data-ttu-id="62506-149">string</span><span class="sxs-lookup"><span data-stu-id="62506-149">string</span></span> |<span data-ttu-id="62506-150">如果你对用户的 userPrincipalName (UPN) 属性使用联盟域，只需在创建新用户帐户时指定。</span><span class="sxs-lookup"><span data-stu-id="62506-150">Only needs to be specified when creating a new user account if you are using a federated domain for the user's userPrincipalName (UPN) property.</span></span>|
|<span data-ttu-id="62506-151">mailNickname</span><span class="sxs-lookup"><span data-stu-id="62506-151">mailNickname</span></span> |<span data-ttu-id="62506-152">string</span><span class="sxs-lookup"><span data-stu-id="62506-152">string</span></span> |<span data-ttu-id="62506-153">用户的邮件别名。</span><span class="sxs-lookup"><span data-stu-id="62506-153">The mail alias for the user.</span></span>|
|<span data-ttu-id="62506-154">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="62506-154">passwordProfile</span></span>|[<span data-ttu-id="62506-155">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="62506-155">PasswordProfile</span></span>](../resources/passwordprofile.md) |<span data-ttu-id="62506-156">用户的密码配置文件。</span><span class="sxs-lookup"><span data-stu-id="62506-156">The password profile for the user.</span></span> <span data-ttu-id="62506-157">对于 Azure B2C 租户 **，forceChangePasswordNextSignIn** 属性应设置为 ，改为使用自定义策略在首次登录 `false` 时强制重置密码。</span><span class="sxs-lookup"><span data-stu-id="62506-157">For Azure B2C tenants, the **forceChangePasswordNextSignIn** property should be set to `false` and instead use custom policies to force password reset at first sign in.</span></span>|
|<span data-ttu-id="62506-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="62506-158">userPrincipalName</span></span> |<span data-ttu-id="62506-159">string</span><span class="sxs-lookup"><span data-stu-id="62506-159">string</span></span> |<span data-ttu-id="62506-160">用户主体名称 (someuser@contoso.com)。</span><span class="sxs-lookup"><span data-stu-id="62506-160">The user principal name (someuser@contoso.com).</span></span>|

<span data-ttu-id="62506-161">由于 **用户** 资源支持 [扩展](/graph/extensibility-overview)，因此可以使用 `POST` 操作，并在创建用户实例时向其添加含有自己的数据的自定义属性。</span><span class="sxs-lookup"><span data-stu-id="62506-161">Because the **user** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the user instance while creating it.</span></span>

<span data-ttu-id="62506-162">默认情况下，将强制通过此 API 创建的联盟用户每 12 小时登录一次。</span><span class="sxs-lookup"><span data-stu-id="62506-162">Federated users created via this API will be forced to sign in every 12 hours by default.</span></span> <span data-ttu-id="62506-163">若要了解如何更改此限制，请参阅 [令牌生存期的例外](/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions)。</span><span class="sxs-lookup"><span data-stu-id="62506-163">For information about how to change this, see [Exceptions for token lifetimes](/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions).</span></span>

>[!NOTE]
><span data-ttu-id="62506-164">不允许向现有 [用户对象添加 B2C](../resources/objectidentity.md)本地帐户，除非 **用户** 对象已包含本地帐户标识。</span><span class="sxs-lookup"><span data-stu-id="62506-164">Adding a [B2C local account](../resources/objectidentity.md) to an existing **user** object is not allowed, unless the **user** object already contains a local account identity.</span></span>

## <a name="response"></a><span data-ttu-id="62506-165">响应</span><span class="sxs-lookup"><span data-stu-id="62506-165">Response</span></span>

<span data-ttu-id="62506-166">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [user](../resources/user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="62506-166">If successful, this method returns a `201 Created` response code and a [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62506-167">示例</span><span class="sxs-lookup"><span data-stu-id="62506-167">Example</span></span>

### <a name="example-1-create-a-user"></a><span data-ttu-id="62506-168">示例 1：创建用户</span><span class="sxs-lookup"><span data-stu-id="62506-168">Example 1: Create a user</span></span>

#### <a name="request"></a><span data-ttu-id="62506-169">请求</span><span class="sxs-lookup"><span data-stu-id="62506-169">Request</span></span>
<span data-ttu-id="62506-170">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="62506-170">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="62506-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="62506-171">HTTP</span></span>](#tab/http)
<!-- {  
  "blockType": "request",   
  "name": "create_user_from_users_2"    
}-->

```http
POST https://graph.microsoft.com/beta/users
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
# <a name="c"></a>[<span data-ttu-id="62506-172">C#</span><span class="sxs-lookup"><span data-stu-id="62506-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-user-from-users-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="62506-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="62506-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-user-from-users-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="62506-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="62506-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-user-from-users-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="62506-175">Java</span><span class="sxs-lookup"><span data-stu-id="62506-175">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-user-from-users-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="62506-176">在请求正文中，提供 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="62506-176">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="62506-177">响应</span><span class="sxs-lookup"><span data-stu-id="62506-177">Response</span></span>
<span data-ttu-id="62506-178">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="62506-178">Here is an example of the response.</span></span> 

>[!NOTE]
><span data-ttu-id="62506-179">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="62506-179">The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users/$entity",
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

### <a name="example-2-create-a-user-with-social-and-local-account-identities"></a><span data-ttu-id="62506-180">示例 2：创建具有社交和本地帐户标识的用户</span><span class="sxs-lookup"><span data-stu-id="62506-180">Example 2: Create a user with social and local account identities</span></span>

<span data-ttu-id="62506-181">创建一个新用户，该用户具有本地帐户标识（以登录名和电子邮件地址为登录凭据），并且具有社交标识。</span><span class="sxs-lookup"><span data-stu-id="62506-181">Create a new user, with a local account identity with a sign-in name, an email address as sign-in, and with a social identity.</span></span> <span data-ttu-id="62506-182">此示例通常用于 B2C 租户中的迁移方案。</span><span class="sxs-lookup"><span data-stu-id="62506-182">This example is typically used for migration scenarios in B2C tenants.</span></span>  

>[!NOTE] 
><span data-ttu-id="62506-183">对于本地帐户标识，必须禁用密码过期，并且还必须禁用下次登录时强制更改密码。</span><span class="sxs-lookup"><span data-stu-id="62506-183">For local account identities, password expirations must be disabled, and force change password at next sign-in must also be disabled.</span></span>

#### <a name="request"></a><span data-ttu-id="62506-184">请求</span><span class="sxs-lookup"><span data-stu-id="62506-184">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="62506-185">HTTP</span><span class="sxs-lookup"><span data-stu-id="62506-185">HTTP</span></span>](#tab/http)
<!-- {  
  "blockType": "request",   
  "name": "create_user_from_users_identities"   
}-->

```http
POST https://graph.microsoft.com/beta/users
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
# <a name="c"></a>[<span data-ttu-id="62506-186">C#</span><span class="sxs-lookup"><span data-stu-id="62506-186">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-user-from-users-identities-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="62506-187">JavaScript</span><span class="sxs-lookup"><span data-stu-id="62506-187">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-user-from-users-identities-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="62506-188">Objective-C</span><span class="sxs-lookup"><span data-stu-id="62506-188">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-user-from-users-identities-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="62506-189">Java</span><span class="sxs-lookup"><span data-stu-id="62506-189">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-user-from-users-identities-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="62506-190">响应</span><span class="sxs-lookup"><span data-stu-id="62506-190">Response</span></span>

<span data-ttu-id="62506-191">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="62506-191">Here is an example of the response.</span></span> 

> <span data-ttu-id="62506-192">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="62506-192">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users/$entity",
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

## <a name="see-also"></a><span data-ttu-id="62506-193">另请参阅</span><span class="sxs-lookup"><span data-stu-id="62506-193">See also</span></span>

- [<span data-ttu-id="62506-194">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="62506-194">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="62506-195">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="62506-195">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="62506-196">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="62506-196">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create User",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
