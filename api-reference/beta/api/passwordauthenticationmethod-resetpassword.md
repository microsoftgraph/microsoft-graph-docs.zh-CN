---
title: passwordAuthenticationMethod：resetPassword
description: 重置用户密码
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 71f144592ec2d0d99eccbfa2d0627f74982a5fa3
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761421"
---
# <a name="passwordauthenticationmethod-resetpassword"></a><span data-ttu-id="1a80b-103">passwordAuthenticationMethod：resetPassword</span><span class="sxs-lookup"><span data-stu-id="1a80b-103">passwordAuthenticationMethod: resetPassword</span></span>

<span data-ttu-id="1a80b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a80b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a80b-105">为与密码身份验证方法对象关联的 [密码启动重置](../resources/passwordauthenticationmethod.md) 。</span><span class="sxs-lookup"><span data-stu-id="1a80b-105">Initiate a reset for the password associated with a [password authentication method](../resources/passwordauthenticationmethod.md) object.</span></span> <span data-ttu-id="1a80b-106">这只能由具有适当权限的管理员完成，并且不能对用户自己的帐户执行。</span><span class="sxs-lookup"><span data-stu-id="1a80b-106">This can only be done by an administrator with appropriate permissions and cannot be performed on a user's own account.</span></span>

<span data-ttu-id="1a80b-107">此流会将新密码写入 Azure Active Directory，如果已使用密码写回进行配置，则推送到本地 Active Directory。</span><span class="sxs-lookup"><span data-stu-id="1a80b-107">This flow writes the new password to Azure Active Directory and pushes it to on-premises Active Directory if configured using password writeback.</span></span> <span data-ttu-id="1a80b-108">管理员可以提供新密码或使系统生成一个密码。</span><span class="sxs-lookup"><span data-stu-id="1a80b-108">The admin can either provide a new password or have the system generate one.</span></span> <span data-ttu-id="1a80b-109">系统将提示用户在下次登录时更改其密码。</span><span class="sxs-lookup"><span data-stu-id="1a80b-109">The user is prompted to change their password on their next sign in.</span></span>

<span data-ttu-id="1a80b-110">此重置是一项长时间运行的操作，它将在标头中返回一个链接，调用方可在其中定期检查 `Location` 重置的状态。</span><span class="sxs-lookup"><span data-stu-id="1a80b-110">This reset is a long-running operation and will return a link in the `Location` header where the caller can periodically check for the status of the reset.</span></span>

## <a name="permissions"></a><span data-ttu-id="1a80b-111">权限</span><span class="sxs-lookup"><span data-stu-id="1a80b-111">Permissions</span></span>

<span data-ttu-id="1a80b-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1a80b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1a80b-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="1a80b-114">Permission type</span></span>                        | <span data-ttu-id="1a80b-115">自行操作的权限 (权限从最低权限级别) </span><span class="sxs-lookup"><span data-stu-id="1a80b-115">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="1a80b-116">对他人操作的权限 (权限从最低到最多特权) </span><span class="sxs-lookup"><span data-stu-id="1a80b-116">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="1a80b-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1a80b-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="1a80b-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a80b-118">Not supported.</span></span> | <span data-ttu-id="1a80b-119">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a80b-119">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="1a80b-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1a80b-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a80b-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a80b-121">Not supported.</span></span> | <span data-ttu-id="1a80b-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a80b-122">Not supported.</span></span> |
| <span data-ttu-id="1a80b-123">应用程序</span><span class="sxs-lookup"><span data-stu-id="1a80b-123">Application</span></span>                            | <span data-ttu-id="1a80b-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a80b-124">Not supported.</span></span> | <span data-ttu-id="1a80b-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a80b-125">Not supported.</span></span> |

<span data-ttu-id="1a80b-126">对于管理员正在操作其他用户的委派方案，管理员需要下列 [角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="1a80b-126">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="1a80b-127">全局管理员</span><span class="sxs-lookup"><span data-stu-id="1a80b-127">Global admin</span></span>
* <span data-ttu-id="1a80b-128">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="1a80b-128">Privileged authentication admin</span></span>
* <span data-ttu-id="1a80b-129">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="1a80b-129">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="1a80b-130">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1a80b-130">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/authentication/passwordMethods/{id}/resetPassword
```

## <a name="request-headers"></a><span data-ttu-id="1a80b-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="1a80b-131">Request headers</span></span>

| <span data-ttu-id="1a80b-132">名称</span><span class="sxs-lookup"><span data-stu-id="1a80b-132">Name</span></span>          | <span data-ttu-id="1a80b-133">说明</span><span class="sxs-lookup"><span data-stu-id="1a80b-133">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="1a80b-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a80b-134">Authorization</span></span> | <span data-ttu-id="1a80b-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1a80b-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1a80b-137">Content-type</span><span class="sxs-lookup"><span data-stu-id="1a80b-137">Content-type</span></span>  | <span data-ttu-id="1a80b-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="1a80b-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1a80b-140">请求正文</span><span class="sxs-lookup"><span data-stu-id="1a80b-140">Request body</span></span>

<span data-ttu-id="1a80b-141">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="1a80b-141">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1a80b-142">参数</span><span class="sxs-lookup"><span data-stu-id="1a80b-142">Parameter</span></span>    | <span data-ttu-id="1a80b-143">类型</span><span class="sxs-lookup"><span data-stu-id="1a80b-143">Type</span></span>        | <span data-ttu-id="1a80b-144">说明</span><span class="sxs-lookup"><span data-stu-id="1a80b-144">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1a80b-145">newPassword</span><span class="sxs-lookup"><span data-stu-id="1a80b-145">newPassword</span></span>|<span data-ttu-id="1a80b-146">String</span><span class="sxs-lookup"><span data-stu-id="1a80b-146">String</span></span>|<span data-ttu-id="1a80b-147">管理员输入的新密码。对于具有混合密码方案的租户，此为必需项。</span><span class="sxs-lookup"><span data-stu-id="1a80b-147">The new password entered by the admin. Required for tenants with hybrid password scenarios.</span></span> <span data-ttu-id="1a80b-148">如果省略仅云密码，系统将返回系统生成的密码。</span><span class="sxs-lookup"><span data-stu-id="1a80b-148">If omitted for a cloud-only password, the system returns a system-generated password.</span></span> <span data-ttu-id="1a80b-149">这是一个没有其他编码的 unicode 字符串。</span><span class="sxs-lookup"><span data-stu-id="1a80b-149">This is a unicode string with no other encoding.</span></span> <span data-ttu-id="1a80b-150">在验收之前，将针对租户的禁止密码系统验证它，并且必须遵守租户的云和/或本地密码要求。</span><span class="sxs-lookup"><span data-stu-id="1a80b-150">It is validated against the tenant's banned password system before acceptance, and must adhere to the tenant's cloud and/or on-premises password requirements.</span></span>|

## <a name="response"></a><span data-ttu-id="1a80b-151">响应</span><span class="sxs-lookup"><span data-stu-id="1a80b-151">Response</span></span>

<span data-ttu-id="1a80b-152">如果成功，此方法在 标头 `202 ACCEPTED` 中返回 响应代码和 `Location` URL。</span><span class="sxs-lookup"><span data-stu-id="1a80b-152">If successful, this method returns a `202 ACCEPTED` response code and a URL in the `Location` header.</span></span>

<span data-ttu-id="1a80b-153">如果调用方未提交密码，则响应正文中的 JSON 对象中会提供 Microsoft 生成的密码。</span><span class="sxs-lookup"><span data-stu-id="1a80b-153">If the caller did not submit a password, a Microsoft-generated password is provided in a JSON object in the response body.</span></span>

### <a name="response-headers"></a><span data-ttu-id="1a80b-154">响应标头</span><span class="sxs-lookup"><span data-stu-id="1a80b-154">Response headers</span></span>

| <span data-ttu-id="1a80b-155">名称</span><span class="sxs-lookup"><span data-stu-id="1a80b-155">Name</span></span>        | <span data-ttu-id="1a80b-156">说明</span><span class="sxs-lookup"><span data-stu-id="1a80b-156">Description</span></span>     |
|:------------|:----------------|
|<span data-ttu-id="1a80b-157">Location</span><span class="sxs-lookup"><span data-stu-id="1a80b-157">Location</span></span>     | <span data-ttu-id="1a80b-158">要调用以检查操作状态的 URL。</span><span class="sxs-lookup"><span data-stu-id="1a80b-158">URL to call to check the status of the operation.</span></span>|
|<span data-ttu-id="1a80b-159">重试后</span><span class="sxs-lookup"><span data-stu-id="1a80b-159">Retry-after</span></span>  | <span data-ttu-id="1a80b-160">持续时间（以秒表示）。</span><span class="sxs-lookup"><span data-stu-id="1a80b-160">Duration in seconds.</span></span>|

## <a name="examples"></a><span data-ttu-id="1a80b-161">示例</span><span class="sxs-lookup"><span data-stu-id="1a80b-161">Examples</span></span>

### <a name="example-1-user-submitted-password"></a><span data-ttu-id="1a80b-162">示例 1：用户提交的密码</span><span class="sxs-lookup"><span data-stu-id="1a80b-162">Example 1: User-submitted password</span></span>

<span data-ttu-id="1a80b-163">以下示例显示当调用方提交密码时如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="1a80b-163">The following example shows how to call this API when the caller submits a password.</span></span>

#### <a name="request"></a><span data-ttu-id="1a80b-164">请求</span><span class="sxs-lookup"><span data-stu-id="1a80b-164">Request</span></span>

<span data-ttu-id="1a80b-165">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1a80b-165">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1a80b-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="1a80b-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "passwordauthenticationmethod_resetpassword_adminprovided"
}-->

```http
POST https://graph.microsoft.com/beta/users/{id | userPrincipalName}/authentication/passwordMethods/{id}/resetPassword
Content-type: application/json

{
  "newPassword": "newPassword-value",
}
```
# <a name="c"></a>[<span data-ttu-id="1a80b-167">C#</span><span class="sxs-lookup"><span data-stu-id="1a80b-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/passwordauthenticationmethod-resetpassword-adminprovided-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1a80b-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1a80b-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/passwordauthenticationmethod-resetpassword-adminprovided-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1a80b-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1a80b-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/passwordauthenticationmethod-resetpassword-adminprovided-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1a80b-170">Java</span><span class="sxs-lookup"><span data-stu-id="1a80b-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/passwordauthenticationmethod-resetpassword-adminprovided-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1a80b-171">响应</span><span class="sxs-lookup"><span data-stu-id="1a80b-171">Response</span></span>

<span data-ttu-id="1a80b-172">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1a80b-172">The following is an example of the response.</span></span>

> <span data-ttu-id="1a80b-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1a80b-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 202 ACCEPTED
Content-type: application/json
Location: https://graph.microsoft.com/beta/users/{id | userPrincipalName}/authentication/operations/{id}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordAuthenticationMethod: resetPassword",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

### <a name="example-2-system-generated-password"></a><span data-ttu-id="1a80b-175">示例 2：系统生成的密码</span><span class="sxs-lookup"><span data-stu-id="1a80b-175">Example 2: System-generated password</span></span>

<span data-ttu-id="1a80b-176">以下示例演示当调用方不提交密码时如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="1a80b-176">The following example shows how to call this API when the caller does not submit a password.</span></span>

#### <a name="request"></a><span data-ttu-id="1a80b-177">请求</span><span class="sxs-lookup"><span data-stu-id="1a80b-177">Request</span></span>

<span data-ttu-id="1a80b-178">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1a80b-178">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1a80b-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="1a80b-179">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "passwordauthenticationmethod_resetpassword_systemgenerated"
}-->

```http
POST https://graph.microsoft.com/beta/users/{id | userPrincipalName}/authentication/passwordMethods/{id}/resetPassword
```
# <a name="c"></a>[<span data-ttu-id="1a80b-180">C#</span><span class="sxs-lookup"><span data-stu-id="1a80b-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/passwordauthenticationmethod-resetpassword-systemgenerated-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1a80b-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1a80b-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/passwordauthenticationmethod-resetpassword-systemgenerated-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1a80b-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1a80b-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/passwordauthenticationmethod-resetpassword-systemgenerated-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1a80b-183">Java</span><span class="sxs-lookup"><span data-stu-id="1a80b-183">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/passwordauthenticationmethod-resetpassword-systemgenerated-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1a80b-184">响应</span><span class="sxs-lookup"><span data-stu-id="1a80b-184">Response</span></span>

<span data-ttu-id="1a80b-185">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1a80b-185">The following is an example of the response.</span></span>

> <span data-ttu-id="1a80b-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1a80b-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.entity"
} -->

```http
HTTP/1.1 202 ACCEPTED
Location: https://graph.microsoft.com/beta/users/{id | userPrincipalName}/authentication/operations/{id}
Content-type: application/json

{
  "password": "new system generated password"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordAuthenticationMethod: resetPassword",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
