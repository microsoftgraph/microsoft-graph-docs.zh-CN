---
title: 创建用户
description: 使用此 API 新建用户。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e81ecd9b31ab5f2836e40e3b461a4974e161eb60
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34981459"
---
# <a name="create-user"></a><span data-ttu-id="d4679-103">创建用户</span><span class="sxs-lookup"><span data-stu-id="d4679-103">Create User</span></span>

<span data-ttu-id="d4679-p101">创建新[用户](../resources/user.md)。请求正文包含要创建的用户。至少要为该用户指定必需的属性。可以选择指定其他任意可写属性。</span><span class="sxs-lookup"><span data-stu-id="d4679-p101">Use this API to create a new User. The request body contains the user to create. At a minimum, you must specify the required properties for the user. You can optionally specify any other writable properties.</span></span>

>[!NOTE]
><span data-ttu-id="d4679-108">若要创建外部用户，请使用[邀请 API](invitation-post.md)。</span><span class="sxs-lookup"><span data-stu-id="d4679-108">To create external users, use the [invitation API](invitation-post.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d4679-109">权限</span><span class="sxs-lookup"><span data-stu-id="d4679-109">Permissions</span></span>

<span data-ttu-id="d4679-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d4679-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4679-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="d4679-112">Permission type</span></span>      | <span data-ttu-id="d4679-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d4679-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d4679-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d4679-114">Delegated (work or school account)</span></span> | <span data-ttu-id="d4679-115">User.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d4679-115">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d4679-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d4679-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4679-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d4679-117">Not supported.</span></span>    |
|<span data-ttu-id="d4679-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="d4679-118">Application</span></span> | <span data-ttu-id="d4679-119">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4679-119">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d4679-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d4679-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="d4679-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="d4679-121">Request headers</span></span>

| <span data-ttu-id="d4679-122">标头</span><span class="sxs-lookup"><span data-stu-id="d4679-122">Header</span></span>       | <span data-ttu-id="d4679-123">值</span><span class="sxs-lookup"><span data-stu-id="d4679-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d4679-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4679-124">Authorization</span></span>  | <span data-ttu-id="d4679-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d4679-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d4679-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d4679-127">Content-Type</span></span>  | <span data-ttu-id="d4679-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d4679-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d4679-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="d4679-129">Request body</span></span>

<span data-ttu-id="d4679-130">在请求正文中，提供 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d4679-130">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

<span data-ttu-id="d4679-131">下表显示创建用户时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d4679-131">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="d4679-132">参数</span><span class="sxs-lookup"><span data-stu-id="d4679-132">Parameter</span></span> | <span data-ttu-id="d4679-133">类型</span><span class="sxs-lookup"><span data-stu-id="d4679-133">Type</span></span> | <span data-ttu-id="d4679-134">说明</span><span class="sxs-lookup"><span data-stu-id="d4679-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d4679-135">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="d4679-135">accountEnabled</span></span> |<span data-ttu-id="d4679-136">boolean</span><span class="sxs-lookup"><span data-stu-id="d4679-136">boolean</span></span> |<span data-ttu-id="d4679-137">启用此帐户时为 true，否则为 false。</span><span class="sxs-lookup"><span data-stu-id="d4679-137">true if the account is enabled; otherwise, false.</span></span>|
|<span data-ttu-id="d4679-138">displayName</span><span class="sxs-lookup"><span data-stu-id="d4679-138">displayName</span></span> |<span data-ttu-id="d4679-139">string</span><span class="sxs-lookup"><span data-stu-id="d4679-139">string</span></span> |<span data-ttu-id="d4679-140">要在用户的通讯簿中显示的名称。</span><span class="sxs-lookup"><span data-stu-id="d4679-140">The name to display in the address book for the user.</span></span>|
|<span data-ttu-id="d4679-141">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="d4679-141">onPremisesImmutableId</span></span> |<span data-ttu-id="d4679-142">string</span><span class="sxs-lookup"><span data-stu-id="d4679-142">string</span></span> |<span data-ttu-id="d4679-143">如果你对用户的 userPrincipalName (UPN) 属性使用联盟域，只需在创建新用户帐户时指定。</span><span class="sxs-lookup"><span data-stu-id="d4679-143">Only needs to be specified when creating a new user account if you are using a federated domain for the user's userPrincipalName (UPN) property.</span></span>|
|<span data-ttu-id="d4679-144">mailNickname</span><span class="sxs-lookup"><span data-stu-id="d4679-144">mailNickname</span></span> |<span data-ttu-id="d4679-145">string</span><span class="sxs-lookup"><span data-stu-id="d4679-145">string</span></span> |<span data-ttu-id="d4679-146">用户的邮件别名。</span><span class="sxs-lookup"><span data-stu-id="d4679-146">The mail alias for the user.</span></span>|
|<span data-ttu-id="d4679-147">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="d4679-147">passwordProfile</span></span>|[<span data-ttu-id="d4679-148">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="d4679-148">PasswordProfile</span></span>](../resources/passwordprofile.md) |<span data-ttu-id="d4679-149">用户的密码配置文件。</span><span class="sxs-lookup"><span data-stu-id="d4679-149">The password profile for the user.</span></span>|
|<span data-ttu-id="d4679-150">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d4679-150">userPrincipalName</span></span> |<span data-ttu-id="d4679-151">string</span><span class="sxs-lookup"><span data-stu-id="d4679-151">string</span></span> |<span data-ttu-id="d4679-152">用户主体名称 (someuser@contoso.com)。</span><span class="sxs-lookup"><span data-stu-id="d4679-152">The user principal name (someuser@contoso.com).</span></span>|

<span data-ttu-id="d4679-153">由于**用户**资源支持[扩展](/graph/extensibility-overview)，因此可以使用 `POST` 操作，并在创建用户实例时向其添加含有自己的数据的自定义属性。</span><span class="sxs-lookup"><span data-stu-id="d4679-153">Since the **event** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the event while creating it.</span></span>

>[!NOTE]
><span data-ttu-id="d4679-154">默认情况下，使用此 API 创建的联合用户将被强制每 12 小时登录一次。</span><span class="sxs-lookup"><span data-stu-id="d4679-154">Federated users created using this API will be forced to sign-in every 12 hours by default.</span></span>  <span data-ttu-id="d4679-155">有关如何对其进行更改的详细信息，请参阅[令牌生存期的例外](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions)。</span><span class="sxs-lookup"><span data-stu-id="d4679-155">For more information on how to change this, see [Exceptions for token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions).</span></span>

## <a name="response"></a><span data-ttu-id="d4679-156">响应</span><span class="sxs-lookup"><span data-stu-id="d4679-156">Response</span></span>

<span data-ttu-id="d4679-157">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [user](../resources/user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d4679-157">If successful, this method returns `201 Created` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4679-158">示例</span><span class="sxs-lookup"><span data-stu-id="d4679-158">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d4679-159">请求</span><span class="sxs-lookup"><span data-stu-id="d4679-159">Request</span></span>

<span data-ttu-id="d4679-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d4679-160">Here is an example of the request.</span></span>
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

<span data-ttu-id="d4679-161">在请求正文中，提供 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d4679-161">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="d4679-162">响应</span><span class="sxs-lookup"><span data-stu-id="d4679-162">Response</span></span>

<span data-ttu-id="d4679-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d4679-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

#### <a name="sdk-sample-code"></a><span data-ttu-id="d4679-166">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="d4679-166">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d4679-167">C#</span><span class="sxs-lookup"><span data-stu-id="d4679-167">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_user_from_users-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d4679-168">Javascript</span><span class="sxs-lookup"><span data-stu-id="d4679-168">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_user_from_users-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create User",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/user-post-users.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/user-post-users.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
