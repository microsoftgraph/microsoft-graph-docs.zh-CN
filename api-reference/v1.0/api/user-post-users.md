---
title: 创建用户
description: 使用此 API 新建用户。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: aebd847d9bb922867b7293d6f06f0ae65f23c8cb
ms.sourcegitcommit: bd0daf5c133ab29af9337a5edd3b8509fd2313d5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/17/2020
ms.locfileid: "41232026"
---
# <a name="create-user"></a><span data-ttu-id="dcd15-103">创建用户</span><span class="sxs-lookup"><span data-stu-id="dcd15-103">Create User</span></span>

<span data-ttu-id="dcd15-p101">创建新[用户](../resources/user.md)。请求正文包含要创建的用户。至少要为该用户指定必需的属性。可以选择指定其他任意可写属性。</span><span class="sxs-lookup"><span data-stu-id="dcd15-p101">Create a new [user](../resources/user.md). The request body contains the user to create. At a minimum, you must specify the required properties for the user. You can optionally specify any other writable properties.</span></span>

>[!NOTE]
><span data-ttu-id="dcd15-108">若要创建外部用户，请使用[邀请 API](invitation-post.md)。</span><span class="sxs-lookup"><span data-stu-id="dcd15-108">To create external users, use the [invitation API](invitation-post.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="dcd15-109">权限</span><span class="sxs-lookup"><span data-stu-id="dcd15-109">Permissions</span></span>

<span data-ttu-id="dcd15-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dcd15-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dcd15-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="dcd15-112">Permission type</span></span>      | <span data-ttu-id="dcd15-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dcd15-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dcd15-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dcd15-114">Delegated (work or school account)</span></span> | <span data-ttu-id="dcd15-115">User.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dcd15-115">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="dcd15-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dcd15-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dcd15-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="dcd15-117">Not supported.</span></span>    |
|<span data-ttu-id="dcd15-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="dcd15-118">Application</span></span> | <span data-ttu-id="dcd15-119">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dcd15-119">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dcd15-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dcd15-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="dcd15-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="dcd15-121">Request headers</span></span>

| <span data-ttu-id="dcd15-122">标头</span><span class="sxs-lookup"><span data-stu-id="dcd15-122">Header</span></span>       | <span data-ttu-id="dcd15-123">值</span><span class="sxs-lookup"><span data-stu-id="dcd15-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="dcd15-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="dcd15-124">Authorization</span></span>  | <span data-ttu-id="dcd15-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dcd15-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="dcd15-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dcd15-127">Content-Type</span></span>  | <span data-ttu-id="dcd15-128">application/json</span><span class="sxs-lookup"><span data-stu-id="dcd15-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dcd15-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="dcd15-129">Request body</span></span>

<span data-ttu-id="dcd15-130">在请求正文中，提供 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dcd15-130">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

<span data-ttu-id="dcd15-131">下表列出了创建用户时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="dcd15-131">The following table shows the properties that are required when you create a user.</span></span> <span data-ttu-id="dcd15-132">如果要为正在创建的用户包括 **identities** 属性，并非所有列出的属性都是必需的。</span><span class="sxs-lookup"><span data-stu-id="dcd15-132">If you're including an **identities** property for the user you're creating, not all the properties listed are required.</span></span> <span data-ttu-id="dcd15-133">对于 [B2C 本地帐户标识](../resources/objectidentity.md)，只需要 **passwordProfile**，且 **passwordPolicy** 必须设置为 `DisablePasswordExpiration`。</span><span class="sxs-lookup"><span data-stu-id="dcd15-133">For a [B2C local account identity](../resources/objectidentity.md), only  **passwordProfile** is required, and **passwordPolicy** must be set to `DisablePasswordExpiration`.</span></span> <span data-ttu-id="dcd15-134">对于社交标识，则无需任何属性。</span><span class="sxs-lookup"><span data-stu-id="dcd15-134">For a social identity, none of the properties are required.</span></span>

| <span data-ttu-id="dcd15-135">参数</span><span class="sxs-lookup"><span data-stu-id="dcd15-135">Parameter</span></span> | <span data-ttu-id="dcd15-136">类型</span><span class="sxs-lookup"><span data-stu-id="dcd15-136">Type</span></span> | <span data-ttu-id="dcd15-137">说明</span><span class="sxs-lookup"><span data-stu-id="dcd15-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dcd15-138">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="dcd15-138">accountEnabled</span></span> |<span data-ttu-id="dcd15-139">boolean</span><span class="sxs-lookup"><span data-stu-id="dcd15-139">boolean</span></span> |<span data-ttu-id="dcd15-140">启用此帐户时为 true，否则为 false。</span><span class="sxs-lookup"><span data-stu-id="dcd15-140">true if the account is enabled; otherwise, false.</span></span>|
|<span data-ttu-id="dcd15-141">displayName</span><span class="sxs-lookup"><span data-stu-id="dcd15-141">displayName</span></span> |<span data-ttu-id="dcd15-142">string</span><span class="sxs-lookup"><span data-stu-id="dcd15-142">string</span></span> |<span data-ttu-id="dcd15-143">要在用户的通讯簿中显示的名称。</span><span class="sxs-lookup"><span data-stu-id="dcd15-143">The name to display in the address book for the user.</span></span>|
|<span data-ttu-id="dcd15-144">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="dcd15-144">onPremisesImmutableId</span></span> |<span data-ttu-id="dcd15-145">string</span><span class="sxs-lookup"><span data-stu-id="dcd15-145">string</span></span> |<span data-ttu-id="dcd15-146">如果你对用户的 userPrincipalName (UPN) 属性使用联盟域，只需在创建新用户帐户时指定。</span><span class="sxs-lookup"><span data-stu-id="dcd15-146">Only needs to be specified when creating a new user account if you are using a federated domain for the user's userPrincipalName (UPN) property.</span></span>|
|<span data-ttu-id="dcd15-147">mailNickname</span><span class="sxs-lookup"><span data-stu-id="dcd15-147">mailNickname</span></span> |<span data-ttu-id="dcd15-148">string</span><span class="sxs-lookup"><span data-stu-id="dcd15-148">string</span></span> |<span data-ttu-id="dcd15-149">用户的邮件别名。</span><span class="sxs-lookup"><span data-stu-id="dcd15-149">The mail alias for the user.</span></span>|
|<span data-ttu-id="dcd15-150">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="dcd15-150">passwordProfile</span></span>|[<span data-ttu-id="dcd15-151">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="dcd15-151">PasswordProfile</span></span>](../resources/passwordprofile.md) |<span data-ttu-id="dcd15-152">用户的密码配置文件。</span><span class="sxs-lookup"><span data-stu-id="dcd15-152">The password profile for the user.</span></span>|
|<span data-ttu-id="dcd15-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="dcd15-153">userPrincipalName</span></span> |<span data-ttu-id="dcd15-154">string</span><span class="sxs-lookup"><span data-stu-id="dcd15-154">string</span></span> |<span data-ttu-id="dcd15-155">用户主体名称 (someuser@contoso.com)。</span><span class="sxs-lookup"><span data-stu-id="dcd15-155">The user principal name (someuser@contoso.com).</span></span>|

<span data-ttu-id="dcd15-156">由于**用户**资源支持[扩展](/graph/extensibility-overview)，因此可以使用 `POST` 操作，并在创建用户实例时向其添加含有自己的数据的自定义属性。</span><span class="sxs-lookup"><span data-stu-id="dcd15-156">Because the **user** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the user instance while creating it.</span></span>

>[!NOTE]
><span data-ttu-id="dcd15-157">默认情况下，使用此 API 创建的联合用户将被强制每 12 小时登录一次。</span><span class="sxs-lookup"><span data-stu-id="dcd15-157">Federated users created using this API will be forced to sign-in every 12 hours by default.</span></span>  <span data-ttu-id="dcd15-158">有关如何对其进行更改的详细信息，请参阅[令牌生存期的例外](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions)。</span><span class="sxs-lookup"><span data-stu-id="dcd15-158">For more information on how to change this, see [Exceptions for token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions).</span></span>

## <a name="response"></a><span data-ttu-id="dcd15-159">响应</span><span class="sxs-lookup"><span data-stu-id="dcd15-159">Response</span></span>

<span data-ttu-id="dcd15-160">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [user](../resources/user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dcd15-160">If successful, this method returns `201 Created` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dcd15-161">示例</span><span class="sxs-lookup"><span data-stu-id="dcd15-161">Example</span></span>

### <a name="example-1-create-a-user"></a><span data-ttu-id="dcd15-162">示例 1：创建用户</span><span class="sxs-lookup"><span data-stu-id="dcd15-162">Example 1: Create a user</span></span>

#### <a name="request"></a><span data-ttu-id="dcd15-163">请求</span><span class="sxs-lookup"><span data-stu-id="dcd15-163">Request</span></span>

<span data-ttu-id="dcd15-164">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dcd15-164">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="dcd15-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="dcd15-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_user_from_users"
}-->

```http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json

{
  "accountEnabled": true,
  "displayName": "displayName-value",
  "mailNickname": "mailNickname-value",
  "userPrincipalName": "upn-value@tenant-value.onmicrosoft.com",
  "passwordProfile" : {
    "forceChangePasswordNextSignIn": true,
    "password": "password-value"
  }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dcd15-166">C#</span><span class="sxs-lookup"><span data-stu-id="dcd15-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-user-from-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dcd15-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dcd15-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-user-from-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dcd15-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dcd15-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-user-from-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="dcd15-169">Java</span><span class="sxs-lookup"><span data-stu-id="dcd15-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-user-from-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="dcd15-170">在请求正文中，提供 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dcd15-170">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

#### <a name="response"></a><span data-ttu-id="dcd15-171">响应</span><span class="sxs-lookup"><span data-stu-id="dcd15-171">Response</span></span>

<span data-ttu-id="dcd15-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dcd15-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "id": "id-value",
    "businessPhones": [],
    "displayName": "displayName-value",
    "givenName": null,
    "jobTitle": null,
    "mail": null,
    "mobilePhone": null,
    "officeLocation": null,
    "preferredLanguage": null,
    "surname": null,
    "userPrincipalName": "upn-value@tenant-value.onmicrosoft.com"
}
```

### <a name="example-2-create-a-user-with-social-and-local-account-identities"></a><span data-ttu-id="dcd15-175">示例 2：创建具有社交和本地帐户标识的用户</span><span class="sxs-lookup"><span data-stu-id="dcd15-175">Example 2: Create a user with social and local account identities</span></span>

<span data-ttu-id="dcd15-176">创建一个新用户，该用户具有本地帐户标识（以登录名和电子邮件地址为登录凭据），并且具有社交标识。</span><span class="sxs-lookup"><span data-stu-id="dcd15-176">Create a new user, with a local account identity with a sign-in name, an email address as sign-in, and with a social identity.</span></span> <span data-ttu-id="dcd15-177">此示例通常用于 B2C 租户中的迁移方案。</span><span class="sxs-lookup"><span data-stu-id="dcd15-177">This example is typically used for migration scenarios in B2C tenants.</span></span>  

>[!NOTE] 
><span data-ttu-id="dcd15-178">对于本地帐户标识，必须禁用密码过期，并且还必须禁用下次登录时强制更改密码。</span><span class="sxs-lookup"><span data-stu-id="dcd15-178">For local account identities, password expirations must be disabled, and force change password at next sign-in must also be disabled.</span></span>

#### <a name="request"></a><span data-ttu-id="dcd15-179">请求</span><span class="sxs-lookup"><span data-stu-id="dcd15-179">Request</span></span>

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
    "password": "password-value"
  },
  "passwordPolicies": "DisablePasswordExpiration"
}
```

---

#### <a name="response"></a><span data-ttu-id="dcd15-180">响应</span><span class="sxs-lookup"><span data-stu-id="dcd15-180">Response</span></span>

<span data-ttu-id="dcd15-181">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="dcd15-181">Here is an example of the response.</span></span> 

> <span data-ttu-id="dcd15-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="dcd15-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
## <a name="see-also"></a><span data-ttu-id="dcd15-184">另请参阅</span><span class="sxs-lookup"><span data-stu-id="dcd15-184">See also</span></span>

- [<span data-ttu-id="dcd15-185">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="dcd15-185">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="dcd15-186">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="dcd15-186">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)

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
