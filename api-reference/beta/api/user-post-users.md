---
title: 创建用户
description: 新建用户。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e09525eaa1889a195d3a0d1c05793e6148d40ef1
ms.sourcegitcommit: bd0daf5c133ab29af9337a5edd3b8509fd2313d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/17/2020
ms.locfileid: "41232040"
---
# <a name="create-user"></a><span data-ttu-id="2ebbc-103">创建用户</span><span class="sxs-lookup"><span data-stu-id="2ebbc-103">Create user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ebbc-p101">创建新[用户](../resources/user.md)。请求正文包含要创建的用户。至少要为该用户指定必需的属性。可以选择指定其他任意可写属性。</span><span class="sxs-lookup"><span data-stu-id="2ebbc-p101">Create a new [user](../resources/user.md). The request body contains the user to create. At a minimum, you must specify the required properties for the user. You can optionally specify any other writable properties.</span></span>

<span data-ttu-id="2ebbc-108">此操作默认情况下仅返回每个用户的属性子集。</span><span class="sxs-lookup"><span data-stu-id="2ebbc-108">This operation returns by default only a subset of the properties for each user.</span></span> <span data-ttu-id="2ebbc-109">这些默认属性将记录在[属性](../resources/user.md#properties)部分中。</span><span class="sxs-lookup"><span data-stu-id="2ebbc-109">These default properties are noted in the [Properties](../resources/user.md#properties) section.</span></span> <span data-ttu-id="2ebbc-110">若要获取非默认返回的属性，请执行 [GET 操作](user-get.md)，并在 `$select` OData 查询选项中指定这些属性。</span><span class="sxs-lookup"><span data-stu-id="2ebbc-110">To get properties that are not returned by default, do a [GET operation](user-get.md) and specify the properties in a `$select` OData query option.</span></span>

>[!NOTE]
><span data-ttu-id="2ebbc-111">若要创建外部用户，请使用[邀请 API](invitation-post.md)。</span><span class="sxs-lookup"><span data-stu-id="2ebbc-111">To create external users, use the [invitation API](invitation-post.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2ebbc-112">权限</span><span class="sxs-lookup"><span data-stu-id="2ebbc-112">Permissions</span></span>

<span data-ttu-id="2ebbc-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2ebbc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ebbc-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="2ebbc-115">Permission type</span></span>      | <span data-ttu-id="2ebbc-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2ebbc-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2ebbc-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2ebbc-117">Delegated (work or school account)</span></span> | <span data-ttu-id="2ebbc-118">User.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2ebbc-118">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2ebbc-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2ebbc-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ebbc-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="2ebbc-120">Not supported.</span></span>    |
|<span data-ttu-id="2ebbc-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="2ebbc-121">Application</span></span> | <span data-ttu-id="2ebbc-122">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ebbc-122">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ebbc-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2ebbc-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users
```
## <a name="request-headers"></a><span data-ttu-id="2ebbc-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="2ebbc-124">Request headers</span></span>
| <span data-ttu-id="2ebbc-125">标头</span><span class="sxs-lookup"><span data-stu-id="2ebbc-125">Header</span></span>       | <span data-ttu-id="2ebbc-126">值</span><span class="sxs-lookup"><span data-stu-id="2ebbc-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2ebbc-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ebbc-127">Authorization</span></span>  | <span data-ttu-id="2ebbc-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2ebbc-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2ebbc-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2ebbc-130">Content-Type</span></span>  | <span data-ttu-id="2ebbc-131">application/json</span><span class="sxs-lookup"><span data-stu-id="2ebbc-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2ebbc-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="2ebbc-132">Request body</span></span>

<span data-ttu-id="2ebbc-133">在请求正文中，提供 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2ebbc-133">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

<span data-ttu-id="2ebbc-134">下表列出了创建用户时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2ebbc-134">The following table lists the properties that are required when you create a user.</span></span> <span data-ttu-id="2ebbc-135">如果您正在创建的用户包含一个**标识**属性，则不需要列出所有属性。</span><span class="sxs-lookup"><span data-stu-id="2ebbc-135">If you're including an **identities** property for the user you're creating, not all the properties listed are required.</span></span> <span data-ttu-id="2ebbc-136">对于[B2C 本地帐户标识](../resources/objectidentity.md)，只有**passwordProfile**是必需的，并且必须将**passwordPolicy**设置为`DisablePasswordExpiration`。</span><span class="sxs-lookup"><span data-stu-id="2ebbc-136">For a [B2C local account identity](../resources/objectidentity.md), only  **passwordProfile** is required, and **passwordPolicy** must be set to `DisablePasswordExpiration`.</span></span> <span data-ttu-id="2ebbc-137">对于社会标识，不需要任何属性。</span><span class="sxs-lookup"><span data-stu-id="2ebbc-137">For a social identity, none of the properties are required.</span></span>

| <span data-ttu-id="2ebbc-138">参数</span><span class="sxs-lookup"><span data-stu-id="2ebbc-138">Parameter</span></span> | <span data-ttu-id="2ebbc-139">类型</span><span class="sxs-lookup"><span data-stu-id="2ebbc-139">Type</span></span> | <span data-ttu-id="2ebbc-140">说明</span><span class="sxs-lookup"><span data-stu-id="2ebbc-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2ebbc-141">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="2ebbc-141">accountEnabled</span></span> |<span data-ttu-id="2ebbc-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ebbc-142">Boolean</span></span> |<span data-ttu-id="2ebbc-143">如果帐户已启用，则为 True;否则为 false。</span><span class="sxs-lookup"><span data-stu-id="2ebbc-143">True if the account is enabled; otherwise, false.</span></span>|
|<span data-ttu-id="2ebbc-144">displayName</span><span class="sxs-lookup"><span data-stu-id="2ebbc-144">displayName</span></span> |<span data-ttu-id="2ebbc-145">string</span><span class="sxs-lookup"><span data-stu-id="2ebbc-145">string</span></span> |<span data-ttu-id="2ebbc-146">要在用户的通讯簿中显示的名称。</span><span class="sxs-lookup"><span data-stu-id="2ebbc-146">The name to display in the address book for the user.</span></span>|
|<span data-ttu-id="2ebbc-147">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="2ebbc-147">onPremisesImmutableId</span></span> |<span data-ttu-id="2ebbc-148">string</span><span class="sxs-lookup"><span data-stu-id="2ebbc-148">string</span></span> |<span data-ttu-id="2ebbc-149">如果你对用户的 userPrincipalName (UPN) 属性使用联盟域，只需在创建新用户帐户时指定。</span><span class="sxs-lookup"><span data-stu-id="2ebbc-149">Only needs to be specified when creating a new user account if you are using a federated domain for the user's userPrincipalName (UPN) property.</span></span>|
|<span data-ttu-id="2ebbc-150">mailNickname</span><span class="sxs-lookup"><span data-stu-id="2ebbc-150">mailNickname</span></span> |<span data-ttu-id="2ebbc-151">string</span><span class="sxs-lookup"><span data-stu-id="2ebbc-151">string</span></span> |<span data-ttu-id="2ebbc-152">用户的邮件别名。</span><span class="sxs-lookup"><span data-stu-id="2ebbc-152">The mail alias for the user.</span></span>|
|<span data-ttu-id="2ebbc-153">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="2ebbc-153">passwordProfile</span></span>|[<span data-ttu-id="2ebbc-154">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="2ebbc-154">PasswordProfile</span></span>](../resources/passwordprofile.md) |<span data-ttu-id="2ebbc-155">用户的密码配置文件。</span><span class="sxs-lookup"><span data-stu-id="2ebbc-155">The password profile for the user.</span></span>|
|<span data-ttu-id="2ebbc-156">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2ebbc-156">userPrincipalName</span></span> |<span data-ttu-id="2ebbc-157">string</span><span class="sxs-lookup"><span data-stu-id="2ebbc-157">string</span></span> |<span data-ttu-id="2ebbc-158">用户主体名称 (someuser@contoso.com)。</span><span class="sxs-lookup"><span data-stu-id="2ebbc-158">The user principal name (someuser@contoso.com).</span></span>|

<span data-ttu-id="2ebbc-159">由于**用户**资源支持[扩展](/graph/extensibility-overview)，因此可以使用 `POST` 操作，并在创建用户实例时向其添加含有自己的数据的自定义属性。</span><span class="sxs-lookup"><span data-stu-id="2ebbc-159">Because the **user** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the user instance while creating it.</span></span>

<span data-ttu-id="2ebbc-160">默认情况下，通过此 API 创建的联合用户将被强制每隔12小时登录一次。</span><span class="sxs-lookup"><span data-stu-id="2ebbc-160">Federated users created via this API will be forced to sign in every 12 hours by default.</span></span> <span data-ttu-id="2ebbc-161">有关如何更改此操作的信息，请参阅[令牌生存期异常](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions)。</span><span class="sxs-lookup"><span data-stu-id="2ebbc-161">For information about how to change this, see [Exceptions for token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions).</span></span>

>[!NOTE]
><span data-ttu-id="2ebbc-162">不允许将[B2C 本地帐户](../resources/objectidentity.md)添加到现有的**user**对象，除非该**用户**对象已包含本地帐户标识。</span><span class="sxs-lookup"><span data-stu-id="2ebbc-162">Adding a [B2C local account](../resources/objectidentity.md) to an existing **user** object is not allowed, unless the **user** object already contains a local account identity.</span></span>

## <a name="response"></a><span data-ttu-id="2ebbc-163">响应</span><span class="sxs-lookup"><span data-stu-id="2ebbc-163">Response</span></span>

<span data-ttu-id="2ebbc-164">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [user](../resources/user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2ebbc-164">If successful, this method returns a `201 Created` response code and a [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ebbc-165">示例</span><span class="sxs-lookup"><span data-stu-id="2ebbc-165">Example</span></span>

### <a name="example-1-create-a-user"></a><span data-ttu-id="2ebbc-166">示例1：创建用户</span><span class="sxs-lookup"><span data-stu-id="2ebbc-166">Example 1: Create a user</span></span>

#### <a name="request"></a><span data-ttu-id="2ebbc-167">请求</span><span class="sxs-lookup"><span data-stu-id="2ebbc-167">Request</span></span>
<span data-ttu-id="2ebbc-168">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2ebbc-168">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2ebbc-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ebbc-169">HTTP</span></span>](#tab/http)
<!-- {  
  "blockType": "request",   
  "name": "create_user_from_users_2"    
}-->

```http
POST https://graph.microsoft.com/beta/users
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="2ebbc-170">C#</span><span class="sxs-lookup"><span data-stu-id="2ebbc-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-user-from-users-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2ebbc-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ebbc-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-user-from-users-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2ebbc-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2ebbc-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-user-from-users-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="2ebbc-173">在请求正文中，提供 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2ebbc-173">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="2ebbc-174">响应</span><span class="sxs-lookup"><span data-stu-id="2ebbc-174">Response</span></span>
<span data-ttu-id="2ebbc-175">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="2ebbc-175">Here is an example of the response.</span></span> 

>[!NOTE]
><span data-ttu-id="2ebbc-176">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2ebbc-176">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2ebbc-177">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="2ebbc-177">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-create-a-user-with-social-and-local-account-identities"></a><span data-ttu-id="2ebbc-178">示例2：创建具有社交和本地帐户标识的用户</span><span class="sxs-lookup"><span data-stu-id="2ebbc-178">Example 2: Create a user with social and local account identities</span></span>

<span data-ttu-id="2ebbc-179">使用具有登录名的本地帐户标识、电子邮件地址（登录）和社交身份来创建新用户。</span><span class="sxs-lookup"><span data-stu-id="2ebbc-179">Create a new user, with a local account identity with a sign-in name, an email address as sign-in, and with a social identity.</span></span> <span data-ttu-id="2ebbc-180">此示例通常用于 B2C 租户中的迁移方案。</span><span class="sxs-lookup"><span data-stu-id="2ebbc-180">This example is typically used for migration scenarios in B2C tenants.</span></span>  

>[!NOTE] 
><span data-ttu-id="2ebbc-181">对于本地帐户标识，必须禁用密码过期，并且必须同时禁用 "在下次登录时强制更改密码"。</span><span class="sxs-lookup"><span data-stu-id="2ebbc-181">For local account identities, password expirations must be disabled, and force change password at next sign-in must also be disabled.</span></span>

#### <a name="request"></a><span data-ttu-id="2ebbc-182">请求</span><span class="sxs-lookup"><span data-stu-id="2ebbc-182">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="2ebbc-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ebbc-183">HTTP</span></span>](#tab/http)
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
    "password": "password-value"
  },
  "passwordPolicies": "DisablePasswordExpiration"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2ebbc-184">C#</span><span class="sxs-lookup"><span data-stu-id="2ebbc-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-user-from-users-identities-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2ebbc-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ebbc-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-user-from-users-identities-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2ebbc-186">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2ebbc-186">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-user-from-users-identities-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2ebbc-187">响应</span><span class="sxs-lookup"><span data-stu-id="2ebbc-187">Response</span></span>

<span data-ttu-id="2ebbc-188">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="2ebbc-188">Here is an example of the response.</span></span> 

> <span data-ttu-id="2ebbc-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="2ebbc-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="2ebbc-191">另请参阅</span><span class="sxs-lookup"><span data-stu-id="2ebbc-191">See also</span></span>

- [<span data-ttu-id="2ebbc-192">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="2ebbc-192">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="2ebbc-193">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="2ebbc-193">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="2ebbc-194">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="2ebbc-194">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
