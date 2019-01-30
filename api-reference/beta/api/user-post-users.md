---
title: 创建用户
description: 使用此 API 创建新用户。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9d1e98ffa4be67141d1e5ae679f9f51a71ef92fd
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642525"
---
# <a name="create-user"></a><span data-ttu-id="ee3f4-103">创建用户</span><span class="sxs-lookup"><span data-stu-id="ee3f4-103">Create user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee3f4-104">使用此 API 创建新用户。</span><span class="sxs-lookup"><span data-stu-id="ee3f4-104">Use this API to create a new user.</span></span>
<span data-ttu-id="ee3f4-105">在请求正文中包含用户创建。</span><span class="sxs-lookup"><span data-stu-id="ee3f4-105">The request body contains the user to create.</span></span> <span data-ttu-id="ee3f4-106">至少，您必须指定用户的必需的属性。</span><span class="sxs-lookup"><span data-stu-id="ee3f4-106">At a minimum, you must specify the required properties for the user.</span></span> <span data-ttu-id="ee3f4-107">您可以选择指定任何其他可写属性。</span><span class="sxs-lookup"><span data-stu-id="ee3f4-107">You can optionally specify any other writable properties.</span></span>
## <a name="permissions"></a><span data-ttu-id="ee3f4-108">权限</span><span class="sxs-lookup"><span data-stu-id="ee3f4-108">Permissions</span></span>
<span data-ttu-id="ee3f4-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ee3f4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee3f4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ee3f4-111">Permission type</span></span>      | <span data-ttu-id="ee3f4-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ee3f4-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee3f4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ee3f4-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ee3f4-114">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ee3f4-114">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ee3f4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ee3f4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee3f4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ee3f4-116">Not supported.</span></span>    |
|<span data-ttu-id="ee3f4-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ee3f4-117">Application</span></span> | <span data-ttu-id="ee3f4-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee3f4-118">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ee3f4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ee3f4-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users
```
## <a name="request-headers"></a><span data-ttu-id="ee3f4-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ee3f4-120">Request headers</span></span>
| <span data-ttu-id="ee3f4-121">标头</span><span class="sxs-lookup"><span data-stu-id="ee3f4-121">Header</span></span>       | <span data-ttu-id="ee3f4-122">值</span><span class="sxs-lookup"><span data-stu-id="ee3f4-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ee3f4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee3f4-123">Authorization</span></span>  | <span data-ttu-id="ee3f4-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ee3f4-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ee3f4-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ee3f4-126">Content-Type</span></span>  | <span data-ttu-id="ee3f4-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ee3f4-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ee3f4-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="ee3f4-128">Request body</span></span>
<span data-ttu-id="ee3f4-129">在请求正文中，提供 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ee3f4-129">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

<span data-ttu-id="ee3f4-130">下表显示创建用户时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ee3f4-130">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="ee3f4-131">参数</span><span class="sxs-lookup"><span data-stu-id="ee3f4-131">Parameter</span></span> | <span data-ttu-id="ee3f4-132">类型</span><span class="sxs-lookup"><span data-stu-id="ee3f4-132">Type</span></span> | <span data-ttu-id="ee3f4-133">说明</span><span class="sxs-lookup"><span data-stu-id="ee3f4-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ee3f4-134">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="ee3f4-134">accountEnabled</span></span> |<span data-ttu-id="ee3f4-135">boolean</span><span class="sxs-lookup"><span data-stu-id="ee3f4-135">boolean</span></span> |<span data-ttu-id="ee3f4-136">启用此帐户时为 true，否则为 false。</span><span class="sxs-lookup"><span data-stu-id="ee3f4-136">true if the account is enabled; otherwise, false.</span></span>|
|<span data-ttu-id="ee3f4-137">displayName</span><span class="sxs-lookup"><span data-stu-id="ee3f4-137">displayName</span></span> |<span data-ttu-id="ee3f4-138">string</span><span class="sxs-lookup"><span data-stu-id="ee3f4-138">string</span></span> |<span data-ttu-id="ee3f4-139">要在用户的通讯簿中显示的名称。</span><span class="sxs-lookup"><span data-stu-id="ee3f4-139">The name to display in the address book for the user.</span></span>|
|<span data-ttu-id="ee3f4-140">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="ee3f4-140">onPremisesImmutableId</span></span> |<span data-ttu-id="ee3f4-141">string</span><span class="sxs-lookup"><span data-stu-id="ee3f4-141">string</span></span> |<span data-ttu-id="ee3f4-142">如果你对用户的 userPrincipalName (UPN) 属性使用联盟域，只需在创建新用户帐户时指定。</span><span class="sxs-lookup"><span data-stu-id="ee3f4-142">Only needs to be specified when creating a new user account if you are using a federated domain for the user's userPrincipalName (UPN) property.</span></span>|
|<span data-ttu-id="ee3f4-143">mailNickname</span><span class="sxs-lookup"><span data-stu-id="ee3f4-143">mailNickname</span></span> |<span data-ttu-id="ee3f4-144">string</span><span class="sxs-lookup"><span data-stu-id="ee3f4-144">string</span></span> |<span data-ttu-id="ee3f4-145">用户的邮件别名。</span><span class="sxs-lookup"><span data-stu-id="ee3f4-145">The mail alias for the user.</span></span>|
|<span data-ttu-id="ee3f4-146">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="ee3f4-146">passwordProfile</span></span>|[<span data-ttu-id="ee3f4-147">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="ee3f4-147">PasswordProfile</span></span>](../resources/passwordprofile.md) |<span data-ttu-id="ee3f4-148">用户的密码配置文件。</span><span class="sxs-lookup"><span data-stu-id="ee3f4-148">The password profile for the user.</span></span>|
|<span data-ttu-id="ee3f4-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ee3f4-149">userPrincipalName</span></span> |<span data-ttu-id="ee3f4-150">string</span><span class="sxs-lookup"><span data-stu-id="ee3f4-150">string</span></span> |<span data-ttu-id="ee3f4-151">用户主体名称 (someuser@contoso.com)。</span><span class="sxs-lookup"><span data-stu-id="ee3f4-151">The user principal name (someuser@contoso.com).</span></span>|

<span data-ttu-id="ee3f4-152">由于**用户**资源支持[扩展](/graph/extensibility-overview)，您可以使用`POST`操作并创建它时将使用您自己的数据的自定义属性添加到用户实例。</span><span class="sxs-lookup"><span data-stu-id="ee3f4-152">Since the **user** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the user instance while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="ee3f4-153">响应</span><span class="sxs-lookup"><span data-stu-id="ee3f4-153">Response</span></span>

<span data-ttu-id="ee3f4-154">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [user](../resources/user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ee3f4-154">If successful, this method returns `201 Created` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee3f4-155">示例</span><span class="sxs-lookup"><span data-stu-id="ee3f4-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ee3f4-156">请求</span><span class="sxs-lookup"><span data-stu-id="ee3f4-156">Request</span></span>
<span data-ttu-id="ee3f4-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ee3f4-157">Here is an example of the request.</span></span>
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
<span data-ttu-id="ee3f4-158">在请求正文中，提供 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ee3f4-158">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="ee3f4-159">响应</span><span class="sxs-lookup"><span data-stu-id="ee3f4-159">Response</span></span>
<span data-ttu-id="ee3f4-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ee3f4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="ee3f4-163">另请参阅</span><span class="sxs-lookup"><span data-stu-id="ee3f4-163">See also</span></span>

- [<span data-ttu-id="ee3f4-164">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="ee3f4-164">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="ee3f4-165">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="ee3f4-165">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="ee3f4-166">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="ee3f4-166">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
    "Error: /api-reference/beta/api/user-post-users.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
