---
title: 创建用户
description: 使用此 API 创建新用户。
ms.openlocfilehash: 17df752fb3767e82b72e46857e9ce6a2a8769db7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042567"
---
# <a name="create-user"></a><span data-ttu-id="12052-103">创建用户</span><span class="sxs-lookup"><span data-stu-id="12052-103">Create user</span></span>

> <span data-ttu-id="12052-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="12052-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="12052-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="12052-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="12052-106">使用此 API 创建新用户。</span><span class="sxs-lookup"><span data-stu-id="12052-106">Use this API to create a new user.</span></span>
<span data-ttu-id="12052-107">在请求正文中包含用户创建。</span><span class="sxs-lookup"><span data-stu-id="12052-107">The request body contains the user to create.</span></span> <span data-ttu-id="12052-108">至少，您必须指定用户的必需的属性。</span><span class="sxs-lookup"><span data-stu-id="12052-108">At a minimum, you must specify the required properties for the user.</span></span> <span data-ttu-id="12052-109">您可以选择指定任何其他可写属性。</span><span class="sxs-lookup"><span data-stu-id="12052-109">You can optionally specify any other writable properties.</span></span>
## <a name="permissions"></a><span data-ttu-id="12052-110">权限</span><span class="sxs-lookup"><span data-stu-id="12052-110">Permissions</span></span>
<span data-ttu-id="12052-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="12052-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12052-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="12052-113">Permission type</span></span>      | <span data-ttu-id="12052-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="12052-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="12052-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="12052-115">Delegated (work or school account)</span></span> | <span data-ttu-id="12052-116">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="12052-116">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="12052-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="12052-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12052-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="12052-118">Not supported.</span></span>    |
|<span data-ttu-id="12052-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="12052-119">Application</span></span> | <span data-ttu-id="12052-120">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12052-120">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="12052-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="12052-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users
```
## <a name="request-headers"></a><span data-ttu-id="12052-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="12052-122">Request headers</span></span>
| <span data-ttu-id="12052-123">标头</span><span class="sxs-lookup"><span data-stu-id="12052-123">Header</span></span>       | <span data-ttu-id="12052-124">值</span><span class="sxs-lookup"><span data-stu-id="12052-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="12052-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="12052-125">Authorization</span></span>  | <span data-ttu-id="12052-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="12052-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="12052-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="12052-128">Content-Type</span></span>  | <span data-ttu-id="12052-129">application/json</span><span class="sxs-lookup"><span data-stu-id="12052-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="12052-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="12052-130">Request body</span></span>
<span data-ttu-id="12052-131">在请求正文中，提供 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="12052-131">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

<span data-ttu-id="12052-132">下表显示创建用户时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="12052-132">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="12052-133">参数</span><span class="sxs-lookup"><span data-stu-id="12052-133">Parameter</span></span> | <span data-ttu-id="12052-134">类型</span><span class="sxs-lookup"><span data-stu-id="12052-134">Type</span></span> | <span data-ttu-id="12052-135">说明</span><span class="sxs-lookup"><span data-stu-id="12052-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="12052-136">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="12052-136">accountEnabled</span></span> |<span data-ttu-id="12052-137">boolean</span><span class="sxs-lookup"><span data-stu-id="12052-137">boolean</span></span> |<span data-ttu-id="12052-138">启用此帐户时为 true，否则为 false。</span><span class="sxs-lookup"><span data-stu-id="12052-138">true if the account is enabled; otherwise, false.</span></span>|
|<span data-ttu-id="12052-139">displayName</span><span class="sxs-lookup"><span data-stu-id="12052-139">displayName</span></span> |<span data-ttu-id="12052-140">string</span><span class="sxs-lookup"><span data-stu-id="12052-140">string</span></span> |<span data-ttu-id="12052-141">要在用户的通讯簿中显示的名称。</span><span class="sxs-lookup"><span data-stu-id="12052-141">The name to display in the address book for the user.</span></span>|
|<span data-ttu-id="12052-142">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="12052-142">onPremisesImmutableId</span></span> |<span data-ttu-id="12052-143">string</span><span class="sxs-lookup"><span data-stu-id="12052-143">string</span></span> |<span data-ttu-id="12052-144">如果你对用户的 userPrincipalName (UPN) 属性使用联盟域，只需在创建新用户帐户时指定。</span><span class="sxs-lookup"><span data-stu-id="12052-144">Only needs to be specified when creating a new user account if you are using a federated domain for the user's userPrincipalName (UPN) property.</span></span>|
|<span data-ttu-id="12052-145">mailNickname</span><span class="sxs-lookup"><span data-stu-id="12052-145">mailNickname</span></span> |<span data-ttu-id="12052-146">string</span><span class="sxs-lookup"><span data-stu-id="12052-146">string</span></span> |<span data-ttu-id="12052-147">用户的邮件别名。</span><span class="sxs-lookup"><span data-stu-id="12052-147">The mail alias for the user.</span></span>|
|<span data-ttu-id="12052-148">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="12052-148">passwordProfile</span></span>|[<span data-ttu-id="12052-149">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="12052-149">PasswordProfile</span></span>](../resources/passwordprofile.md) |<span data-ttu-id="12052-150">用户的密码配置文件。</span><span class="sxs-lookup"><span data-stu-id="12052-150">The password profile for the user.</span></span>|
|<span data-ttu-id="12052-151">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="12052-151">userPrincipalName</span></span> |<span data-ttu-id="12052-152">string</span><span class="sxs-lookup"><span data-stu-id="12052-152">string</span></span> |<span data-ttu-id="12052-153">用户主体名称 (someuser@contoso.com)。</span><span class="sxs-lookup"><span data-stu-id="12052-153">The user principal name (someuser@contoso.com).</span></span>|

<span data-ttu-id="12052-154">由于**用户**资源支持[扩展](/graph/extensibility-overview)，您可以使用`POST`操作并创建它时将使用您自己的数据的自定义属性添加到用户实例。</span><span class="sxs-lookup"><span data-stu-id="12052-154">Since the **user** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the user instance while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="12052-155">响应</span><span class="sxs-lookup"><span data-stu-id="12052-155">Response</span></span>

<span data-ttu-id="12052-156">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [user](../resources/user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="12052-156">If successful, this method returns `201 Created` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12052-157">示例</span><span class="sxs-lookup"><span data-stu-id="12052-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="12052-158">请求</span><span class="sxs-lookup"><span data-stu-id="12052-158">Request</span></span>
<span data-ttu-id="12052-159">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="12052-159">Here is an example of the request.</span></span>
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
  "userPrincipalName": "upn-value@tenant-value@onmicrosoft.com",
  "passwordProfile" : {
    "forceChangePasswordNextSignIn": true,
    "password": "password-value"
  }
}
```
<span data-ttu-id="12052-160">在请求正文中，提供 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="12052-160">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="12052-161">响应</span><span class="sxs-lookup"><span data-stu-id="12052-161">Response</span></span>
<span data-ttu-id="12052-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="12052-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
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

## <a name="see-also"></a><span data-ttu-id="12052-165">另请参阅</span><span class="sxs-lookup"><span data-stu-id="12052-165">See also</span></span>

- [<span data-ttu-id="12052-166">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="12052-166">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="12052-167">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="12052-167">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="12052-168">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="12052-168">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create User",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
