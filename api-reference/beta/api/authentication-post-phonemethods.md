---
title: 创建 phoneAuthenticationMethod
description: 添加新的电话身份验证方法。
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 48133bff3dc0532c2669a608697e1fca1a10d9ca
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/10/2020
ms.locfileid: "48417772"
---
# <a name="create-phoneauthenticationmethod"></a><span data-ttu-id="7bbbf-103">创建 phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="7bbbf-103">Create phoneAuthenticationMethod</span></span>

<span data-ttu-id="7bbbf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7bbbf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7bbbf-105">添加新的 [电话身份验证方法](../resources/phoneauthenticationmethod.md)。</span><span class="sxs-lookup"><span data-stu-id="7bbbf-105">Add a new [phone authentication method](../resources/phoneauthenticationmethod.md).</span></span> <span data-ttu-id="7bbbf-106">用户的每种类型只能有一个电话，在 **phoneType** 属性中捕获。</span><span class="sxs-lookup"><span data-stu-id="7bbbf-106">A user may only have one phone of each type, captured in the **phoneType** property.</span></span> <span data-ttu-id="7bbbf-107">这意味着， `mobile` 向具有预先存在的手机的用户添加电话将会 `mobile` 失败。</span><span class="sxs-lookup"><span data-stu-id="7bbbf-107">This means, for example, adding a `mobile` phone to a user with a preexisting `mobile` phone will fail.</span></span> <span data-ttu-id="7bbbf-108">此外，在添加电话之前，用户必须始终具有 `mobile` 电话 `alternateMobile` 。</span><span class="sxs-lookup"><span data-stu-id="7bbbf-108">Additionally, a user must always have a `mobile` phone before adding an `alternateMobile` phone.</span></span>

<span data-ttu-id="7bbbf-109">通过添加电话号码，可以在 Azure 多重身份验证 (MFA) 和自助服务密码重置 (SSPR) （如果已启用）中使用。</span><span class="sxs-lookup"><span data-stu-id="7bbbf-109">Adding a phone number makes it available for use in both Azure multi-factor authentication (MFA) and self-service password reset (SSPR), if enabled.</span></span>

<span data-ttu-id="7bbbf-110">此外，如果用户启用了策略以使用 SMS 登录并添加了一个 `mobile` 号码，则系统会尝试注册该号码以在该系统中使用。</span><span class="sxs-lookup"><span data-stu-id="7bbbf-110">Additionally, if a user is enabled by policy to use SMS sign-in and a `mobile` number is added, the system will attempt to register the number for use in that system.</span></span>

## <a name="permissions"></a><span data-ttu-id="7bbbf-111">权限</span><span class="sxs-lookup"><span data-stu-id="7bbbf-111">Permissions</span></span>

<span data-ttu-id="7bbbf-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7bbbf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7bbbf-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="7bbbf-114">Permission type</span></span>                        | <span data-ttu-id="7bbbf-115">从最高特权到最高特权) 对自己 (的权限</span><span class="sxs-lookup"><span data-stu-id="7bbbf-115">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="7bbbf-116">对其他人进行操作的权限 (从至少到最高特权) </span><span class="sxs-lookup"><span data-stu-id="7bbbf-116">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="7bbbf-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7bbbf-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="7bbbf-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="7bbbf-118">Not supported.</span></span> | <span data-ttu-id="7bbbf-119">UserAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="7bbbf-119">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="7bbbf-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7bbbf-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7bbbf-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="7bbbf-121">Not supported.</span></span> | <span data-ttu-id="7bbbf-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="7bbbf-122">Not supported.</span></span> |
| <span data-ttu-id="7bbbf-123">应用程序</span><span class="sxs-lookup"><span data-stu-id="7bbbf-123">Application</span></span>                            | <span data-ttu-id="7bbbf-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="7bbbf-124">Not supported.</span></span> | <span data-ttu-id="7bbbf-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="7bbbf-125">Not supported.</span></span> |

<span data-ttu-id="7bbbf-126">对于在其他用户上执行管理的委派方案，管理员需要 [以下角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="7bbbf-126">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="7bbbf-127">全局管理员</span><span class="sxs-lookup"><span data-stu-id="7bbbf-127">Global admin</span></span>
* <span data-ttu-id="7bbbf-128">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="7bbbf-128">Privileged authentication admin</span></span>
* <span data-ttu-id="7bbbf-129">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="7bbbf-129">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="7bbbf-130">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7bbbf-130">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/authentication/phoneMethods
POST /users/{id | userPrincipalName}/authentication/phoneMethods
```

## <a name="request-headers"></a><span data-ttu-id="7bbbf-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="7bbbf-131">Request headers</span></span>

| <span data-ttu-id="7bbbf-132">名称</span><span class="sxs-lookup"><span data-stu-id="7bbbf-132">Name</span></span>          | <span data-ttu-id="7bbbf-133">说明</span><span class="sxs-lookup"><span data-stu-id="7bbbf-133">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="7bbbf-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="7bbbf-134">Authorization</span></span> | <span data-ttu-id="7bbbf-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7bbbf-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7bbbf-137">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7bbbf-137">Content-Type</span></span>  | <span data-ttu-id="7bbbf-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="7bbbf-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7bbbf-140">请求正文</span><span class="sxs-lookup"><span data-stu-id="7bbbf-140">Request body</span></span>

<span data-ttu-id="7bbbf-141">在请求正文中，提供 [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7bbbf-141">In the request body, supply a JSON representation of a [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object.</span></span> <span data-ttu-id="7bbbf-142">JSON 必须包括 `phoneNumber` 和 `phoneType` ，但不 `smsSignInState` 是只读) 的 (。</span><span class="sxs-lookup"><span data-stu-id="7bbbf-142">The JSON must include `phoneNumber` and `phoneType`, but not `smsSignInState` (which is read-only).</span></span>

| <span data-ttu-id="7bbbf-143">属性</span><span class="sxs-lookup"><span data-stu-id="7bbbf-143">Property</span></span>     | <span data-ttu-id="7bbbf-144">类型</span><span class="sxs-lookup"><span data-stu-id="7bbbf-144">Type</span></span>        | <span data-ttu-id="7bbbf-145">说明</span><span class="sxs-lookup"><span data-stu-id="7bbbf-145">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7bbbf-146">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="7bbbf-146">phoneNumber</span></span>|<span data-ttu-id="7bbbf-147">String</span><span class="sxs-lookup"><span data-stu-id="7bbbf-147">String</span></span>|<span data-ttu-id="7bbbf-148">将电话号码设为文本或呼叫以进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="7bbbf-148">The phone number to text or call for authentication.</span></span> <span data-ttu-id="7bbbf-149">电话号码使用格式 "+ \<country code\> \<number\> x \<extension\> "，扩展名为可选。</span><span class="sxs-lookup"><span data-stu-id="7bbbf-149">Phone numbers use the format "+\<country code\> \<number\>x\<extension\>", with extension optional.</span></span> <span data-ttu-id="7bbbf-150">例如，+ 1 5555551234 或 + 1 5555551234x123 是有效的。</span><span class="sxs-lookup"><span data-stu-id="7bbbf-150">For example, +1 5555551234 or +1 5555551234x123 are valid.</span></span> <span data-ttu-id="7bbbf-151">如果创建/更新时编号不符合要求的格式，则会拒绝编号。</span><span class="sxs-lookup"><span data-stu-id="7bbbf-151">Numbers are rejected when creating/updating if they do not match the required format.</span></span>|
|<span data-ttu-id="7bbbf-152">phoneType</span><span class="sxs-lookup"><span data-stu-id="7bbbf-152">phoneType</span></span>|<span data-ttu-id="7bbbf-153">字符串</span><span class="sxs-lookup"><span data-stu-id="7bbbf-153">String</span></span>|<span data-ttu-id="7bbbf-154">可能的值为： `mobile` 、 `alternateMobile` 和 `office` 。</span><span class="sxs-lookup"><span data-stu-id="7bbbf-154">Possible values are: `mobile`, `alternateMobile`, and `office`.</span></span>|

## <a name="response"></a><span data-ttu-id="7bbbf-155">响应</span><span class="sxs-lookup"><span data-stu-id="7bbbf-155">Response</span></span>

<span data-ttu-id="7bbbf-156">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和新的 [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7bbbf-156">If successful, this method returns a `201 Created` response code and a new [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7bbbf-157">示例</span><span class="sxs-lookup"><span data-stu-id="7bbbf-157">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7bbbf-158">请求</span><span class="sxs-lookup"><span data-stu-id="7bbbf-158">Request</span></span>

<span data-ttu-id="7bbbf-159">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7bbbf-159">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7bbbf-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="7bbbf-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_phoneauthenticationmethod_from_authentication"
}-->

```http
POST https://graph.microsoft.com/beta/me/authentication/phoneMethods
Content-type: application/json

{
  "phoneNumber": "+1 2065555555",
  "phoneType": "mobile"
}
```
# <a name="c"></a>[<span data-ttu-id="7bbbf-161">C#</span><span class="sxs-lookup"><span data-stu-id="7bbbf-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-phoneauthenticationmethod-from-authentication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7bbbf-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7bbbf-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-phoneauthenticationmethod-from-authentication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7bbbf-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7bbbf-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-phoneauthenticationmethod-from-authentication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7bbbf-164">响应</span><span class="sxs-lookup"><span data-stu-id="7bbbf-164">Response</span></span>

<span data-ttu-id="7bbbf-165">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7bbbf-165">The following is an example of the response.</span></span>

> <span data-ttu-id="7bbbf-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7bbbf-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.phoneAuthenticationMethod"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "phoneNumber": "+1 2065555555",
  "phoneType": "phoneType-value",
  "smsSignInState": "ready",
  "id": "3179e48a-750b-4051-897c-87b9720928f7"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create phoneAuthenticationMethod",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
