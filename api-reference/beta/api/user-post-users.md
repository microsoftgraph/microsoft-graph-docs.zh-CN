---
title: 创建用户
description: 新建用户。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4604fdf6bed68d378c7a3ab12f9fa126c1a37bcb
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356805"
---
# <a name="create-user"></a><span data-ttu-id="627e5-103">创建用户</span><span class="sxs-lookup"><span data-stu-id="627e5-103">Create user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="627e5-104">创建新[用户](../resources/user.md)。</span><span class="sxs-lookup"><span data-stu-id="627e5-104">Create a new [user](../resources/user.md).</span></span>
<span data-ttu-id="627e5-105">请求正文包含要创建的用户。</span><span class="sxs-lookup"><span data-stu-id="627e5-105">The request body contains the user to create.</span></span> <span data-ttu-id="627e5-106">至少必须指定必需的用户属性。</span><span class="sxs-lookup"><span data-stu-id="627e5-106">At a minimum, you must specify the required properties for the user.</span></span> <span data-ttu-id="627e5-107">可以选择指定其他任意可写属性。</span><span class="sxs-lookup"><span data-stu-id="627e5-107">You can optionally specify any other writable properties.</span></span>

>[!NOTE]
><span data-ttu-id="627e5-108">若要创建外部用户，请使用[邀请 API](invitation-post.md)。</span><span class="sxs-lookup"><span data-stu-id="627e5-108">To create external users, use the [invitation API](invitation-post.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="627e5-109">权限</span><span class="sxs-lookup"><span data-stu-id="627e5-109">Permissions</span></span>

<span data-ttu-id="627e5-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="627e5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="627e5-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="627e5-112">Permission type</span></span>      | <span data-ttu-id="627e5-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="627e5-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="627e5-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="627e5-114">Delegated (work or school account)</span></span> | <span data-ttu-id="627e5-115">User.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="627e5-115">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="627e5-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="627e5-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="627e5-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="627e5-117">Not supported.</span></span>    |
|<span data-ttu-id="627e5-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="627e5-118">Application</span></span> | <span data-ttu-id="627e5-119">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="627e5-119">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="627e5-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="627e5-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users
```
## <a name="request-headers"></a><span data-ttu-id="627e5-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="627e5-121">Request headers</span></span>
| <span data-ttu-id="627e5-122">标头</span><span class="sxs-lookup"><span data-stu-id="627e5-122">Header</span></span>       | <span data-ttu-id="627e5-123">值</span><span class="sxs-lookup"><span data-stu-id="627e5-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="627e5-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="627e5-124">Authorization</span></span>  | <span data-ttu-id="627e5-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="627e5-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="627e5-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="627e5-127">Content-Type</span></span>  | <span data-ttu-id="627e5-128">application/json</span><span class="sxs-lookup"><span data-stu-id="627e5-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="627e5-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="627e5-129">Request body</span></span>

<span data-ttu-id="627e5-130">在请求正文中，提供 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="627e5-130">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

<span data-ttu-id="627e5-131">下表列出了创建用户时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="627e5-131">The following table lists the properties that are required when you create a user.</span></span> <span data-ttu-id="627e5-132">如果您正在创建的用户包含一个**标识**属性，则不需要列出所有属性。</span><span class="sxs-lookup"><span data-stu-id="627e5-132">If you're including an **identities** property for the user you're creating, not all the properties listed are required.</span></span> <span data-ttu-id="627e5-133">对于[B2C 本地帐户标识](../resources/objectidentity.md)，只有**passwordProfile**是必需的。</span><span class="sxs-lookup"><span data-stu-id="627e5-133">For a [B2C local account identity](../resources/objectidentity.md), only  **passwordProfile** is required.</span></span> <span data-ttu-id="627e5-134">对于社会标识，不需要任何属性。</span><span class="sxs-lookup"><span data-stu-id="627e5-134">For a social identity, none of the properties are required.</span></span>

| <span data-ttu-id="627e5-135">参数</span><span class="sxs-lookup"><span data-stu-id="627e5-135">Parameter</span></span> | <span data-ttu-id="627e5-136">类型</span><span class="sxs-lookup"><span data-stu-id="627e5-136">Type</span></span> | <span data-ttu-id="627e5-137">说明</span><span class="sxs-lookup"><span data-stu-id="627e5-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="627e5-138">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="627e5-138">accountEnabled</span></span> |<span data-ttu-id="627e5-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="627e5-139">Boolean</span></span> |<span data-ttu-id="627e5-140">如果帐户已启用，则为 True;否则为 false。</span><span class="sxs-lookup"><span data-stu-id="627e5-140">True if the account is enabled; otherwise, false.</span></span>|
|<span data-ttu-id="627e5-141">displayName</span><span class="sxs-lookup"><span data-stu-id="627e5-141">displayName</span></span> |<span data-ttu-id="627e5-142">string</span><span class="sxs-lookup"><span data-stu-id="627e5-142">string</span></span> |<span data-ttu-id="627e5-143">要在用户的通讯簿中显示的名称。</span><span class="sxs-lookup"><span data-stu-id="627e5-143">The name to display in the address book for the user.</span></span>|
|<span data-ttu-id="627e5-144">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="627e5-144">onPremisesImmutableId</span></span> |<span data-ttu-id="627e5-145">string</span><span class="sxs-lookup"><span data-stu-id="627e5-145">string</span></span> |<span data-ttu-id="627e5-146">如果你对用户的 userPrincipalName (UPN) 属性使用联盟域，只需在创建新用户帐户时指定。</span><span class="sxs-lookup"><span data-stu-id="627e5-146">Only needs to be specified when creating a new user account if you are using a federated domain for the user's userPrincipalName (UPN) property.</span></span>|
|<span data-ttu-id="627e5-147">mailNickname</span><span class="sxs-lookup"><span data-stu-id="627e5-147">mailNickname</span></span> |<span data-ttu-id="627e5-148">string</span><span class="sxs-lookup"><span data-stu-id="627e5-148">string</span></span> |<span data-ttu-id="627e5-149">用户的邮件别名。</span><span class="sxs-lookup"><span data-stu-id="627e5-149">The mail alias for the user.</span></span>|
|<span data-ttu-id="627e5-150">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="627e5-150">passwordProfile</span></span>|[<span data-ttu-id="627e5-151">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="627e5-151">PasswordProfile</span></span>](../resources/passwordprofile.md) |<span data-ttu-id="627e5-152">用户的密码配置文件。</span><span class="sxs-lookup"><span data-stu-id="627e5-152">The password profile for the user.</span></span>|
|<span data-ttu-id="627e5-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="627e5-153">userPrincipalName</span></span> |<span data-ttu-id="627e5-154">string</span><span class="sxs-lookup"><span data-stu-id="627e5-154">string</span></span> |<span data-ttu-id="627e5-155">用户主体名称 (someuser@contoso.com)。</span><span class="sxs-lookup"><span data-stu-id="627e5-155">The user principal name (someuser@contoso.com).</span></span>|

<span data-ttu-id="627e5-156">由于**用户**资源支持[扩展](/graph/extensibility-overview)，因此您可以使用`POST`操作，并在创建用户实例时将自己的数据添加到用户实例中的自定义属性。</span><span class="sxs-lookup"><span data-stu-id="627e5-156">Because the **user** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the user instance while creating it.</span></span>

<span data-ttu-id="627e5-157">默认情况下，通过此 API 创建的联合用户将被强制每隔12小时登录一次。</span><span class="sxs-lookup"><span data-stu-id="627e5-157">Federated users created via this API will be forced to sign in every 12 hours by default.</span></span> <span data-ttu-id="627e5-158">有关如何更改此操作的信息，请参阅[令牌生存期异常](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions)。</span><span class="sxs-lookup"><span data-stu-id="627e5-158">For information about how to change this, see [Exceptions for token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions).</span></span>

>[!NOTE]
><span data-ttu-id="627e5-159">不允许将[B2C 本地帐户](../resources/objectidentity.md)添加到现有的**user**对象，除非该**用户**对象已包含本地帐户标识。</span><span class="sxs-lookup"><span data-stu-id="627e5-159">Adding a [B2C local account](../resources/objectidentity.md) to an existing **user** object is not allowed, unless the **user** object already contains a local account identity.</span></span>

## <a name="response"></a><span data-ttu-id="627e5-160">响应</span><span class="sxs-lookup"><span data-stu-id="627e5-160">Response</span></span>

<span data-ttu-id="627e5-161">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [user](../resources/user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="627e5-161">If successful, this method returns a `201 Created` response code and a [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="627e5-162">示例</span><span class="sxs-lookup"><span data-stu-id="627e5-162">Example</span></span>

### <a name="example-1-create-a-user"></a><span data-ttu-id="627e5-163">示例1：创建用户</span><span class="sxs-lookup"><span data-stu-id="627e5-163">Example 1: Create a user</span></span>

#### <a name="request"></a><span data-ttu-id="627e5-164">请求</span><span class="sxs-lookup"><span data-stu-id="627e5-164">Request</span></span>
<span data-ttu-id="627e5-165">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="627e5-165">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="627e5-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="627e5-166">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="627e5-167">C#</span><span class="sxs-lookup"><span data-stu-id="627e5-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-user-from-users-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="627e5-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="627e5-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-user-from-users-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="627e5-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="627e5-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-user-from-users-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="627e5-170">在请求正文中，提供 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="627e5-170">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="627e5-171">响应</span><span class="sxs-lookup"><span data-stu-id="627e5-171">Response</span></span>
<span data-ttu-id="627e5-172">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="627e5-172">Here is an example of the response.</span></span> 

[!NOTE]
<span data-ttu-id="627e5-173">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="627e5-173">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="627e5-174">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="627e5-174">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-create-a-user-with-social-and-local-account-identities"></a><span data-ttu-id="627e5-175">示例2：创建具有社交和本地帐户标识的用户</span><span class="sxs-lookup"><span data-stu-id="627e5-175">Example 2: Create a user with social and local account identities</span></span>

<span data-ttu-id="627e5-176">使用具有登录名的本地帐户标识和社交标识创建新用户。</span><span class="sxs-lookup"><span data-stu-id="627e5-176">Create a new user, with a local account identity with a sign-in name, and with a social identity.</span></span> <span data-ttu-id="627e5-177">此示例通常用于迁移方案。</span><span class="sxs-lookup"><span data-stu-id="627e5-177">This example is typically used for migration scenarios.</span></span>

#### <a name="request"></a><span data-ttu-id="627e5-178">请求</span><span class="sxs-lookup"><span data-stu-id="627e5-178">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="627e5-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="627e5-179">HTTP</span></span>](#tab/http)
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
      "signInType": "signInName",
      "issuer": "contoso.onmicrosoft.com",
      "issuerAssignedId": "johnsmith"
    },
    {
      "signInType": "federated",
      "issuer": "facebook.com",
      "issuerAssignedId": "5eecb0cd"
    }
  ],
  "passwordProfile" : {
    "forceChangePasswordNextSignIn": true,
    "password": "password-value"
  }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="627e5-180">C#</span><span class="sxs-lookup"><span data-stu-id="627e5-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-user-from-users-identities-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="627e5-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="627e5-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-user-from-users-identities-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="627e5-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="627e5-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-user-from-users-identities-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="627e5-183">响应</span><span class="sxs-lookup"><span data-stu-id="627e5-183">Response</span></span>

<span data-ttu-id="627e5-184">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="627e5-184">Here is an example of the response.</span></span> 

> <span data-ttu-id="627e5-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="627e5-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "signInType": "signInName",
      "issuer": "contoso.onmicrosoft.com",
      "issuerAssignedId": "johnsmith"
    },
    {
      "signInType": "federated",
      "issuer": "facebook.com",
      "issuerAssignedId": "5eecb0cd"
    }
  ],
  "passwordProfile" : {
    "forceChangePasswordNextSignIn": true,
    "password": null
  }
}
```

## <a name="see-also"></a><span data-ttu-id="627e5-187">另请参阅</span><span class="sxs-lookup"><span data-stu-id="627e5-187">See also</span></span>

- [<span data-ttu-id="627e5-188">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="627e5-188">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="627e5-189">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="627e5-189">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="627e5-190">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="627e5-190">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
