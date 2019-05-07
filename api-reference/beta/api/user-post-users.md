---
title: 创建用户
description: 使用此 API 创建新用户。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5efcc4bd793ca876d1db5860785c3ba67d447ade
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637120"
---
# <a name="create-user"></a><span data-ttu-id="1ddd9-103">创建用户</span><span class="sxs-lookup"><span data-stu-id="1ddd9-103">Create user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ddd9-p101">使用此 API 创建新用户。请求正文包含要创建的用户。必须至少为用户指定所需的属性。您可以选择指定任何其他可写属性。</span><span class="sxs-lookup"><span data-stu-id="1ddd9-p101">Use this API to create a new user. The request body contains the user to create. At a minimum, you must specify the required properties for the user. You can optionally specify any other writable properties.</span></span>
## <a name="permissions"></a><span data-ttu-id="1ddd9-108">权限</span><span class="sxs-lookup"><span data-stu-id="1ddd9-108">Permissions</span></span>
<span data-ttu-id="1ddd9-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1ddd9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ddd9-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1ddd9-111">Permission type</span></span>      | <span data-ttu-id="1ddd9-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1ddd9-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1ddd9-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1ddd9-113">Delegated (work or school account)</span></span> | <span data-ttu-id="1ddd9-114">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1ddd9-114">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1ddd9-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1ddd9-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ddd9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1ddd9-116">Not supported.</span></span>    |
|<span data-ttu-id="1ddd9-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1ddd9-117">Application</span></span> | <span data-ttu-id="1ddd9-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ddd9-118">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1ddd9-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1ddd9-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users
```
## <a name="request-headers"></a><span data-ttu-id="1ddd9-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1ddd9-120">Request headers</span></span>
| <span data-ttu-id="1ddd9-121">标头</span><span class="sxs-lookup"><span data-stu-id="1ddd9-121">Header</span></span>       | <span data-ttu-id="1ddd9-122">值</span><span class="sxs-lookup"><span data-stu-id="1ddd9-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1ddd9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ddd9-123">Authorization</span></span>  | <span data-ttu-id="1ddd9-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1ddd9-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1ddd9-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1ddd9-126">Content-Type</span></span>  | <span data-ttu-id="1ddd9-127">application/json</span><span class="sxs-lookup"><span data-stu-id="1ddd9-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1ddd9-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="1ddd9-128">Request body</span></span>
<span data-ttu-id="1ddd9-129">在请求正文中，提供 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1ddd9-129">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

<span data-ttu-id="1ddd9-130">下表显示创建用户时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1ddd9-130">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="1ddd9-131">参数</span><span class="sxs-lookup"><span data-stu-id="1ddd9-131">Parameter</span></span> | <span data-ttu-id="1ddd9-132">类型</span><span class="sxs-lookup"><span data-stu-id="1ddd9-132">Type</span></span> | <span data-ttu-id="1ddd9-133">说明</span><span class="sxs-lookup"><span data-stu-id="1ddd9-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1ddd9-134">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="1ddd9-134">accountEnabled</span></span> |<span data-ttu-id="1ddd9-135">boolean</span><span class="sxs-lookup"><span data-stu-id="1ddd9-135">boolean</span></span> |<span data-ttu-id="1ddd9-136">启用此帐户时为 true，否则为 false。</span><span class="sxs-lookup"><span data-stu-id="1ddd9-136">true if the account is enabled; otherwise, false.</span></span>|
|<span data-ttu-id="1ddd9-137">displayName</span><span class="sxs-lookup"><span data-stu-id="1ddd9-137">displayName</span></span> |<span data-ttu-id="1ddd9-138">string</span><span class="sxs-lookup"><span data-stu-id="1ddd9-138">string</span></span> |<span data-ttu-id="1ddd9-139">要在用户的通讯簿中显示的名称。</span><span class="sxs-lookup"><span data-stu-id="1ddd9-139">The name to display in the address book for the user.</span></span>|
|<span data-ttu-id="1ddd9-140">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="1ddd9-140">onPremisesImmutableId</span></span> |<span data-ttu-id="1ddd9-141">string</span><span class="sxs-lookup"><span data-stu-id="1ddd9-141">string</span></span> |<span data-ttu-id="1ddd9-142">如果你对用户的 userPrincipalName (UPN) 属性使用联盟域，只需在创建新用户帐户时指定。</span><span class="sxs-lookup"><span data-stu-id="1ddd9-142">Only needs to be specified when creating a new user account if you are using a federated domain for the user's userPrincipalName (UPN) property.</span></span>|
|<span data-ttu-id="1ddd9-143">mailNickname</span><span class="sxs-lookup"><span data-stu-id="1ddd9-143">mailNickname</span></span> |<span data-ttu-id="1ddd9-144">string</span><span class="sxs-lookup"><span data-stu-id="1ddd9-144">string</span></span> |<span data-ttu-id="1ddd9-145">用户的邮件别名。</span><span class="sxs-lookup"><span data-stu-id="1ddd9-145">The mail alias for the user.</span></span>|
|<span data-ttu-id="1ddd9-146">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="1ddd9-146">passwordProfile</span></span>|[<span data-ttu-id="1ddd9-147">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="1ddd9-147">PasswordProfile</span></span>](../resources/passwordprofile.md) |<span data-ttu-id="1ddd9-148">用户的密码配置文件。</span><span class="sxs-lookup"><span data-stu-id="1ddd9-148">The password profile for the user.</span></span>|
|<span data-ttu-id="1ddd9-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1ddd9-149">userPrincipalName</span></span> |<span data-ttu-id="1ddd9-150">string</span><span class="sxs-lookup"><span data-stu-id="1ddd9-150">string</span></span> |<span data-ttu-id="1ddd9-151">用户主体名称 (someuser@contoso.com)。</span><span class="sxs-lookup"><span data-stu-id="1ddd9-151">The user principal name (someuser@contoso.com).</span></span>|

<span data-ttu-id="1ddd9-152">由于**用户**资源支持[扩展](/graph/extensibility-overview), 因此您可以使用`POST`操作, 并在创建用户实例时向用户实例中添加自定义属性和您自己的数据。</span><span class="sxs-lookup"><span data-stu-id="1ddd9-152">Since the **user** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the user instance while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="1ddd9-153">响应</span><span class="sxs-lookup"><span data-stu-id="1ddd9-153">Response</span></span>

<span data-ttu-id="1ddd9-154">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [user](../resources/user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1ddd9-154">If successful, this method returns `201 Created` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ddd9-155">示例</span><span class="sxs-lookup"><span data-stu-id="1ddd9-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1ddd9-156">请求</span><span class="sxs-lookup"><span data-stu-id="1ddd9-156">Request</span></span>
<span data-ttu-id="1ddd9-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1ddd9-157">Here is an example of the request.</span></span>
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
<span data-ttu-id="1ddd9-158">在请求正文中，提供 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1ddd9-158">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="1ddd9-159">响应</span><span class="sxs-lookup"><span data-stu-id="1ddd9-159">Response</span></span>
<span data-ttu-id="1ddd9-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1ddd9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="1ddd9-163">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="1ddd9-163">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1ddd9-164">语言</span><span class="sxs-lookup"><span data-stu-id="1ddd9-164">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_user_from_users_2-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1ddd9-165">Javascript</span><span class="sxs-lookup"><span data-stu-id="1ddd9-165">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_user_from_users_2-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="1ddd9-166">另请参阅</span><span class="sxs-lookup"><span data-stu-id="1ddd9-166">See also</span></span>

- [<span data-ttu-id="1ddd9-167">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="1ddd9-167">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="1ddd9-168">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="1ddd9-168">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="1ddd9-169">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="1ddd9-169">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
