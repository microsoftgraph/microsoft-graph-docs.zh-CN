---
title: 创建用户
description: 新建用户。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8e7653095ded6d4146c07c37660260ba53190df5
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34479054"
---
# <a name="create-user"></a><span data-ttu-id="89f51-103">创建用户</span><span class="sxs-lookup"><span data-stu-id="89f51-103">Create user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89f51-104">新建用户。</span><span class="sxs-lookup"><span data-stu-id="89f51-104">Create a new user.</span></span>
<span data-ttu-id="89f51-105">请求正文包含要创建的用户。</span><span class="sxs-lookup"><span data-stu-id="89f51-105">The request body contains the user to create.</span></span> <span data-ttu-id="89f51-106">至少必须指定必需的用户属性。</span><span class="sxs-lookup"><span data-stu-id="89f51-106">At a minimum, you must specify the required properties for the user.</span></span> <span data-ttu-id="89f51-107">可以选择指定其他任意可写属性。</span><span class="sxs-lookup"><span data-stu-id="89f51-107">You can optionally specify any other writable properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="89f51-108">权限</span><span class="sxs-lookup"><span data-stu-id="89f51-108">Permissions</span></span>

<span data-ttu-id="89f51-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="89f51-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89f51-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="89f51-111">Permission type</span></span>      | <span data-ttu-id="89f51-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="89f51-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="89f51-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="89f51-113">Delegated (work or school account)</span></span> | <span data-ttu-id="89f51-114">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="89f51-114">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="89f51-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="89f51-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89f51-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="89f51-116">Not supported.</span></span>    |
|<span data-ttu-id="89f51-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="89f51-117">Application</span></span> | <span data-ttu-id="89f51-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89f51-118">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="89f51-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="89f51-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users
```
## <a name="request-headers"></a><span data-ttu-id="89f51-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="89f51-120">Request headers</span></span>
| <span data-ttu-id="89f51-121">标头</span><span class="sxs-lookup"><span data-stu-id="89f51-121">Header</span></span>       | <span data-ttu-id="89f51-122">值</span><span class="sxs-lookup"><span data-stu-id="89f51-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="89f51-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="89f51-123">Authorization</span></span>  | <span data-ttu-id="89f51-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="89f51-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="89f51-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="89f51-126">Content-Type</span></span>  | <span data-ttu-id="89f51-127">application/json</span><span class="sxs-lookup"><span data-stu-id="89f51-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="89f51-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="89f51-128">Request body</span></span>

<span data-ttu-id="89f51-129">在请求正文中，提供 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="89f51-129">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

<span data-ttu-id="89f51-130">下表显示创建用户时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="89f51-130">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="89f51-131">参数</span><span class="sxs-lookup"><span data-stu-id="89f51-131">Parameter</span></span> | <span data-ttu-id="89f51-132">类型</span><span class="sxs-lookup"><span data-stu-id="89f51-132">Type</span></span> | <span data-ttu-id="89f51-133">说明</span><span class="sxs-lookup"><span data-stu-id="89f51-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="89f51-134">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="89f51-134">accountEnabled</span></span> |<span data-ttu-id="89f51-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="89f51-135">Boolean</span></span> |<span data-ttu-id="89f51-136">启用此帐户时为 true，否则为 false。</span><span class="sxs-lookup"><span data-stu-id="89f51-136">true if the account is enabled; otherwise, false.</span></span>|
|<span data-ttu-id="89f51-137">displayName</span><span class="sxs-lookup"><span data-stu-id="89f51-137">displayName</span></span> |<span data-ttu-id="89f51-138">string</span><span class="sxs-lookup"><span data-stu-id="89f51-138">string</span></span> |<span data-ttu-id="89f51-139">要在用户的通讯簿中显示的名称。</span><span class="sxs-lookup"><span data-stu-id="89f51-139">The name to display in the address book for the user.</span></span>|
|<span data-ttu-id="89f51-140">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="89f51-140">onPremisesImmutableId</span></span> |<span data-ttu-id="89f51-141">string</span><span class="sxs-lookup"><span data-stu-id="89f51-141">string</span></span> |<span data-ttu-id="89f51-142">如果你对用户的 userPrincipalName (UPN) 属性使用联盟域，只需在创建新用户帐户时指定。</span><span class="sxs-lookup"><span data-stu-id="89f51-142">Only needs to be specified when creating a new user account if you are using a federated domain for the user's userPrincipalName (UPN) property.</span></span>|
|<span data-ttu-id="89f51-143">mailNickname</span><span class="sxs-lookup"><span data-stu-id="89f51-143">mailNickname</span></span> |<span data-ttu-id="89f51-144">string</span><span class="sxs-lookup"><span data-stu-id="89f51-144">string</span></span> |<span data-ttu-id="89f51-145">用户的邮件别名。</span><span class="sxs-lookup"><span data-stu-id="89f51-145">The mail alias for the user.</span></span>|
|<span data-ttu-id="89f51-146">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="89f51-146">passwordProfile</span></span>|[<span data-ttu-id="89f51-147">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="89f51-147">PasswordProfile</span></span>](../resources/passwordprofile.md) |<span data-ttu-id="89f51-148">用户的密码配置文件。</span><span class="sxs-lookup"><span data-stu-id="89f51-148">The password profile for the user.</span></span>|
|<span data-ttu-id="89f51-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="89f51-149">userPrincipalName</span></span> |<span data-ttu-id="89f51-150">string</span><span class="sxs-lookup"><span data-stu-id="89f51-150">string</span></span> |<span data-ttu-id="89f51-151">用户主体名称 (someuser@contoso.com)。</span><span class="sxs-lookup"><span data-stu-id="89f51-151">The user principal name (someuser@contoso.com).</span></span>|

<span data-ttu-id="89f51-152">由于**用户**资源支持[扩展](/graph/extensibility-overview), 因此您可以使用`POST`操作, 并在创建用户实例时将自己的数据添加到用户实例中的自定义属性。</span><span class="sxs-lookup"><span data-stu-id="89f51-152">Because the **user** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the user instance while creating it.</span></span>

[!NOTE]
<span data-ttu-id="89f51-153">默认情况下, 使用此 API 创建的联合用户将被强制每隔12小时登录一次。</span><span class="sxs-lookup"><span data-stu-id="89f51-153">Federated users created using this API will be forced to sign in every 12 hours by default.</span></span> <span data-ttu-id="89f51-154">有关如何更改此操作的详细信息, 请参阅[令牌生存期异常](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions)。</span><span class="sxs-lookup"><span data-stu-id="89f51-154">For more information about how to change this, see [Exceptions for token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions).</span></span>

## <a name="response"></a><span data-ttu-id="89f51-155">响应</span><span class="sxs-lookup"><span data-stu-id="89f51-155">Response</span></span>

<span data-ttu-id="89f51-156">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [user](../resources/user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="89f51-156">If successful, this method returns a `201 Created` response code and a [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89f51-157">示例</span><span class="sxs-lookup"><span data-stu-id="89f51-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="89f51-158">请求</span><span class="sxs-lookup"><span data-stu-id="89f51-158">Request</span></span>
<span data-ttu-id="89f51-159">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="89f51-159">Here is an example of the request.</span></span>
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
<span data-ttu-id="89f51-160">在请求正文中，提供 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="89f51-160">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="89f51-161">响应</span><span class="sxs-lookup"><span data-stu-id="89f51-161">Response</span></span>
<span data-ttu-id="89f51-162">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="89f51-162">Here is an example of the response.</span></span> 

[!NOTE]
<span data-ttu-id="89f51-163">为了提高可读性, 可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="89f51-163">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="89f51-164">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="89f51-164">All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="89f51-165">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="89f51-165">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="89f51-166">C#</span><span class="sxs-lookup"><span data-stu-id="89f51-166">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_user_from_users_2-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="89f51-167">Javascript</span><span class="sxs-lookup"><span data-stu-id="89f51-167">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_user_from_users_2-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="89f51-168">另请参阅</span><span class="sxs-lookup"><span data-stu-id="89f51-168">See also</span></span>

- [<span data-ttu-id="89f51-169">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="89f51-169">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="89f51-170">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="89f51-170">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="89f51-171">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="89f51-171">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
