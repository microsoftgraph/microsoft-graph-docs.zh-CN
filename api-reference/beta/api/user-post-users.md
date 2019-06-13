---
title: 创建用户
description: 新建用户。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 62c57763c41c034b6c93a8e0e40780a9f0ccc69b
ms.sourcegitcommit: 8aaf10f7c11d1bf481e9acac19884346dbd44cb8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/13/2019
ms.locfileid: "34914677"
---
# <a name="create-user"></a><span data-ttu-id="fc77a-103">创建用户</span><span class="sxs-lookup"><span data-stu-id="fc77a-103">Create user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc77a-104">新建用户。</span><span class="sxs-lookup"><span data-stu-id="fc77a-104">Create a new user.</span></span>
<span data-ttu-id="fc77a-105">请求正文包含要创建的用户。</span><span class="sxs-lookup"><span data-stu-id="fc77a-105">The request body contains the user to create.</span></span> <span data-ttu-id="fc77a-106">至少必须指定必需的用户属性。</span><span class="sxs-lookup"><span data-stu-id="fc77a-106">At a minimum, you must specify the required properties for the user.</span></span> <span data-ttu-id="fc77a-107">可以选择指定其他任意可写属性。</span><span class="sxs-lookup"><span data-stu-id="fc77a-107">You can optionally specify any other writable properties.</span></span>

>[!NOTE]
><span data-ttu-id="fc77a-108">必须通过邀请创建外部用户。</span><span class="sxs-lookup"><span data-stu-id="fc77a-108">External users must be created through an invitation.</span></span> <span data-ttu-id="fc77a-109">如果需要启用外部用户的创建, 请参阅[邀请](../resources/invitation.md)。</span><span class="sxs-lookup"><span data-stu-id="fc77a-109">If you need to enable the creation of external users, see [invitation](../resources/invitation.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fc77a-110">权限</span><span class="sxs-lookup"><span data-stu-id="fc77a-110">Permissions</span></span>

<span data-ttu-id="fc77a-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fc77a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc77a-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="fc77a-113">Permission type</span></span>      | <span data-ttu-id="fc77a-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fc77a-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc77a-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fc77a-115">Delegated (work or school account)</span></span> | <span data-ttu-id="fc77a-116">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fc77a-116">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fc77a-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fc77a-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc77a-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="fc77a-118">Not supported.</span></span>    |
|<span data-ttu-id="fc77a-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="fc77a-119">Application</span></span> | <span data-ttu-id="fc77a-120">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc77a-120">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc77a-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fc77a-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users
```
## <a name="request-headers"></a><span data-ttu-id="fc77a-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="fc77a-122">Request headers</span></span>
| <span data-ttu-id="fc77a-123">标头</span><span class="sxs-lookup"><span data-stu-id="fc77a-123">Header</span></span>       | <span data-ttu-id="fc77a-124">值</span><span class="sxs-lookup"><span data-stu-id="fc77a-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fc77a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc77a-125">Authorization</span></span>  | <span data-ttu-id="fc77a-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fc77a-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fc77a-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fc77a-128">Content-Type</span></span>  | <span data-ttu-id="fc77a-129">application/json</span><span class="sxs-lookup"><span data-stu-id="fc77a-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fc77a-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="fc77a-130">Request body</span></span>

<span data-ttu-id="fc77a-131">在请求正文中，提供 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fc77a-131">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

<span data-ttu-id="fc77a-132">下表显示创建用户时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="fc77a-132">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="fc77a-133">参数</span><span class="sxs-lookup"><span data-stu-id="fc77a-133">Parameter</span></span> | <span data-ttu-id="fc77a-134">类型</span><span class="sxs-lookup"><span data-stu-id="fc77a-134">Type</span></span> | <span data-ttu-id="fc77a-135">说明</span><span class="sxs-lookup"><span data-stu-id="fc77a-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fc77a-136">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="fc77a-136">accountEnabled</span></span> |<span data-ttu-id="fc77a-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc77a-137">Boolean</span></span> |<span data-ttu-id="fc77a-138">启用此帐户时为 true，否则为 false。</span><span class="sxs-lookup"><span data-stu-id="fc77a-138">true if the account is enabled; otherwise, false.</span></span>|
|<span data-ttu-id="fc77a-139">displayName</span><span class="sxs-lookup"><span data-stu-id="fc77a-139">displayName</span></span> |<span data-ttu-id="fc77a-140">string</span><span class="sxs-lookup"><span data-stu-id="fc77a-140">string</span></span> |<span data-ttu-id="fc77a-141">要在用户的通讯簿中显示的名称。</span><span class="sxs-lookup"><span data-stu-id="fc77a-141">The name to display in the address book for the user.</span></span>|
|<span data-ttu-id="fc77a-142">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="fc77a-142">onPremisesImmutableId</span></span> |<span data-ttu-id="fc77a-143">string</span><span class="sxs-lookup"><span data-stu-id="fc77a-143">string</span></span> |<span data-ttu-id="fc77a-144">如果你对用户的 userPrincipalName (UPN) 属性使用联盟域，只需在创建新用户帐户时指定。</span><span class="sxs-lookup"><span data-stu-id="fc77a-144">Only needs to be specified when creating a new user account if you are using a federated domain for the user's userPrincipalName (UPN) property.</span></span>|
|<span data-ttu-id="fc77a-145">mailNickname</span><span class="sxs-lookup"><span data-stu-id="fc77a-145">mailNickname</span></span> |<span data-ttu-id="fc77a-146">string</span><span class="sxs-lookup"><span data-stu-id="fc77a-146">string</span></span> |<span data-ttu-id="fc77a-147">用户的邮件别名。</span><span class="sxs-lookup"><span data-stu-id="fc77a-147">The mail alias for the user.</span></span>|
|<span data-ttu-id="fc77a-148">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="fc77a-148">passwordProfile</span></span>|[<span data-ttu-id="fc77a-149">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="fc77a-149">PasswordProfile</span></span>](../resources/passwordprofile.md) |<span data-ttu-id="fc77a-150">用户的密码配置文件。</span><span class="sxs-lookup"><span data-stu-id="fc77a-150">The password profile for the user.</span></span>|
|<span data-ttu-id="fc77a-151">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="fc77a-151">userPrincipalName</span></span> |<span data-ttu-id="fc77a-152">string</span><span class="sxs-lookup"><span data-stu-id="fc77a-152">string</span></span> |<span data-ttu-id="fc77a-153">用户主体名称 (someuser@contoso.com)。</span><span class="sxs-lookup"><span data-stu-id="fc77a-153">The user principal name (someuser@contoso.com).</span></span>|

<span data-ttu-id="fc77a-154">由于**用户**资源支持[扩展](/graph/extensibility-overview), 因此您可以使用`POST`操作, 并在创建用户实例时将自己的数据添加到用户实例中的自定义属性。</span><span class="sxs-lookup"><span data-stu-id="fc77a-154">Because the **user** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the user instance while creating it.</span></span>

>[!NOTE]
><span data-ttu-id="fc77a-155">默认情况下, 使用此 API 创建的联合用户将被强制每隔12小时登录一次。</span><span class="sxs-lookup"><span data-stu-id="fc77a-155">Federated users created using this API will be forced to sign in every 12 hours by default.</span></span> <span data-ttu-id="fc77a-156">有关如何更改此操作的详细信息, 请参阅[令牌生存期异常](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions)。</span><span class="sxs-lookup"><span data-stu-id="fc77a-156">For more information about how to change this, see [Exceptions for token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions).</span></span>

## <a name="response"></a><span data-ttu-id="fc77a-157">响应</span><span class="sxs-lookup"><span data-stu-id="fc77a-157">Response</span></span>

<span data-ttu-id="fc77a-158">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [user](../resources/user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fc77a-158">If successful, this method returns a `201 Created` response code and a [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc77a-159">示例</span><span class="sxs-lookup"><span data-stu-id="fc77a-159">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fc77a-160">请求</span><span class="sxs-lookup"><span data-stu-id="fc77a-160">Request</span></span>
<span data-ttu-id="fc77a-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fc77a-161">Here is an example of the request.</span></span>
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
<span data-ttu-id="fc77a-162">在请求正文中，提供 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fc77a-162">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="fc77a-163">响应</span><span class="sxs-lookup"><span data-stu-id="fc77a-163">Response</span></span>
<span data-ttu-id="fc77a-164">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="fc77a-164">Here is an example of the response.</span></span> 

[!NOTE]
<span data-ttu-id="fc77a-165">为了提高可读性, 可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="fc77a-165">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="fc77a-166">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="fc77a-166">All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="fc77a-167">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="fc77a-167">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="fc77a-168">C#</span><span class="sxs-lookup"><span data-stu-id="fc77a-168">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_user_from_users_2-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fc77a-169">Javascript</span><span class="sxs-lookup"><span data-stu-id="fc77a-169">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_user_from_users_2-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="fc77a-170">另请参阅</span><span class="sxs-lookup"><span data-stu-id="fc77a-170">See also</span></span>

- [<span data-ttu-id="fc77a-171">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="fc77a-171">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="fc77a-172">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="fc77a-172">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="fc77a-173">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="fc77a-173">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
    "Error: /api-reference/beta/api/user-post-users.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-post-users.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
